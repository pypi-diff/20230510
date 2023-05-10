# Comparing `tmp/airoboros-0.0.6.tar.gz` & `tmp/airoboros-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airoboros-0.0.6.tar", last modified: Thu May  4 10:18:11 2023, max compression
+gzip compressed data, was "airoboros-0.1.0.tar", last modified: Wed May 10 11:17:26 2023, max compression
```

## Comparing `airoboros-0.0.6.tar` & `airoboros-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:18:11.906221 airoboros-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 10:17:56.000000 airoboros-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-04 10:18:11.906221 airoboros-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-04 10:17:56.000000 airoboros-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:18:11.902221 airoboros-0.0.6/airoboros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:17:56.000000 airoboros-0.0.6/airoboros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-04 10:17:56.000000 airoboros-0.0.6/airoboros/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 10:17:56.000000 airoboros-0.0.6/airoboros/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-05-04 10:17:56.000000 airoboros-0.0.6/airoboros/self_instruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:18:11.906221 airoboros-0.0.6/airoboros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-04 10:18:11.000000 airoboros-0.0.6/airoboros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-04 10:18:11.000000 airoboros-0.0.6/airoboros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:18:11.000000 airoboros-0.0.6/airoboros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-04 10:18:11.000000 airoboros-0.0.6/airoboros.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-04 10:18:11.000000 airoboros-0.0.6/airoboros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 10:18:11.000000 airoboros-0.0.6/airoboros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 10:18:11.906221 airoboros-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-04 10:17:56.000000 airoboros-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:26.109802 airoboros-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 11:17:15.000000 airoboros-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-05-10 11:17:26.109802 airoboros-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-10 11:17:15.000000 airoboros-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:26.109802 airoboros-0.1.0/airoboros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:15.000000 airoboros-0.1.0/airoboros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-10 11:17:15.000000 airoboros-0.1.0/airoboros/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-10 11:17:15.000000 airoboros-0.1.0/airoboros/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29687 2023-05-10 11:17:15.000000 airoboros-0.1.0/airoboros/self_instruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:26.109802 airoboros-0.1.0/airoboros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-05-10 11:17:26.000000 airoboros-0.1.0/airoboros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-10 11:17:26.000000 airoboros-0.1.0/airoboros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:17:26.000000 airoboros-0.1.0/airoboros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 11:17:26.000000 airoboros-0.1.0/airoboros.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 11:17:26.000000 airoboros-0.1.0/airoboros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 11:17:26.000000 airoboros-0.1.0/airoboros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:17:26.109802 airoboros-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-10 11:17:15.000000 airoboros-0.1.0/setup.py
```

### Comparing `airoboros-0.0.6/LICENSE` & `airoboros-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airoboros-0.0.6/PKG-INFO` & `airoboros-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,101 +1,108 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 0.0.6
+Version: 0.1.0
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # airoboros: using large language models to fine-tune large language models
 
-This is my take on implementing the [Self-Instruct paper](https://arxiv.org/abs/2212.10560).  The approach is quite heavily modified, and uses the human generated seeds provided by [Databricks Dolly Project](https://huggingface.co/datasets/databricks/databricks-dolly-15k)
+This is my take on implementing the [Self-Instruct paper](https://arxiv.org/abs/2212.10560).  The approach is quite heavily modified, and does not use any human-generated seeds.
 
 This updated implementation supports either the /v1/completions endpoint or /v1/chat/completions, which is particularly useful in that it supports gpt-4 and gpt-3.5-turbo (which is 1/10 the cost of text-davinci-003).
 
 
 ## Key differences
 
-* Sample instructions in prompts by default use the human-generated seeds from Dolly.
-* Machine-generated instructions are not sampled for prompt examples, to avoid degredation.
-* Support for either /v1/completions or /v1/chat/completions APIs (which allows gpt-3.5-turbo instead of text-davinci-003, as well as gpt-4 if you have access).
-* In memory vector db (Chroma) for similarity comparison, which is much faster than calculating rouge score for each generated instruction.
-* (Seemingly) better prompt, which includes injection of random topics to relate the instructions to, which creates much more diverse prompts.
-* Multi-threaded producers/consumer implementation for significantly faster runtimes (generally 150+ unique prompts per minute, more initially since there are fewer duplicates, decreasing over time).
-* Tries to ensure the context, if provided, is relevant to the topic and contains all the information that would be necessary to respond to the instruction, and nost just a link to article/etc.
-* Generally speaking, this implementation tries to reduce some of the [noise](https://github.com/tloen/alpaca-lora/issues/65)
-
-
-## Initial datasets
-
-Be sure to look over the openai terms of service before using the datasets, specifically the section about using the outputs to generate competing models...
-
-### 100k synthetic instructions, gpt-3.5-turbo
-
-* [instructions.jsonl](https://storage.googleapis.com/airoboros-dump/gpt-3.5-turbo-100k/instructions.jsonl)
-* [topics.txt](https://storage.googleapis.com/airoboros-dump/gpt-3.5-turbo-100k/topics.txt)
+* support for either /v1/completions or /v1/chat/completions APIs (which allows gpt-3.5-turbo instead of text-davinci-003, as well as gpt-4 if you have access)
+* support for custom topics list, custom topic generation prompt, or completely random topics
+* sn memory vector db (Chroma) for similarity comparison, which is much faster than calculating rouge score for each generated instruction
+* (seemingly) better prompts, which includes injection of random topics to relate the instructions to, which creates much more diverse synthetic instructions
+* multi-threaded producer/consumer implementation for significantly faster runtimes (generally 150+ unique prompts per minute, more initially since there are fewer duplicates, decreasing over time).
+* tries to ensure the context, if provided, is relevant to the topic and contains all the information that would be necessary to respond to the instruction, and nost just a link to article/etc.
+* generally speaking, this implementation tries to reduce some of the [noise](https://github.com/tloen/alpaca-lora/issues/65)
 
 
 ## Generating instructions
 
 See available options via:
 ```
 airoboros generate-instructions --help
 ```
 
-Example output:
+Help as of 2023-05-10:
 ```
-usage: self_instruct.py [-h] [--model MODEL] [--organization-id ORGANIZATION_ID] [--openai-api-key OPENAI_API_KEY] [--instruction-count INSTRUCTION_COUNT] [--seed-tasks-path SEED_TASKS_PATH] [--output-path OUTPUT_PATH] [--overwrite] [--append] [--prompt PROMPT] [--skip-instruction-re SKIP_INSTRUCTION_RE] [--code-gen-re CODE_GEN_RE]
-                        [--samples-per-request SAMPLES_PER_REQUEST] [--min-instruction-length MIN_INSTRUCTION_LENGTH] [--max-instruction-length MAX_INSTRUCTION_LENGTH] [--temperature TEMPERATURE] [--top-p TOP_P] [--frequency-penalty FREQUENCY_PENALTY] [--presence-penalty PRESENCE_PENALTY] [--max-usage-tokens MAX_USAGE_TOKENS]
-                        [--prompt-generation-concurrency PROMPT_GENERATION_CONCURRENCY] [--min-docsearch-score MIN_DOCSEARCH_SCORE]
+usage: self_instruct.py [-h] [--model MODEL] [--organization-id ORGANIZATION_ID] [--openai-api-key OPENAI_API_KEY] [--instruction-count INSTRUCTION_COUNT] [--batch-size BATCH_SIZE] [--output-path OUTPUT_PATH] [--topics-path TOPICS_PATH] [--overwrite] [--append] [--prompt PROMPT] [--contextual-prompt CONTEXTUAL_PROMPT]
+                        [--topic-generation-prompt TOPIC_GENERATION_PROMPT] [--topic-request-count TOPIC_REQUEST_COUNT] [--contextual-prompt-ratio CONTEXTUAL_PROMPT_RATIO] [--skip-instruction-re SKIP_INSTRUCTION_RE] [--temperature TEMPERATURE] [--top-p TOP_P] [--frequency-penalty FREQUENCY_PENALTY] [--presence-penalty PRESENCE_PENALTY]
+                        [--max-usage-tokens MAX_USAGE_TOKENS] [--concurrency CONCURRENCY] [--min-docsearch-score MIN_DOCSEARCH_SCORE]
 
 options:
   -h, --help            show this help message and exit
   --model MODEL         OpenAI model/engine to use for prompt generation, which can be either part of the /v1/completions or /v1/chat/completions endpoints
   --organization-id ORGANIZATION_ID
                         organization ID to include in the request to OpenAI, defaults to organization ID tied to the API key
   --openai-api-key OPENAI_API_KEY
                         OpenAI API key to use, defaults to the OPENAI_API_KEY environment variable
   --instruction-count INSTRUCTION_COUNT
                         number of instructions to generate, not including the seed instructions
-  --seed-tasks-path SEED_TASKS_PATH
-                        path to an input seed instructions JSONL file
+  --batch-size BATCH_SIZE
+                        number of candidate instructions to (attempt to) generate per request
   --output-path OUTPUT_PATH
                         path to store all generated instructions in
+  --topics-path TOPICS_PATH
+                        path to a newline separated list of topics
   --overwrite           overwrite output path if it exists
   --append              append to output path if it exists
-  --prompt PROMPT       prompt prefix to use for generating tasks
+  --prompt PROMPT       prompt prefix to use for generating non-contextual instructions
+  --contextual-prompt CONTEXTUAL_PROMPT
+                        prompt to use for generating contextual prompts
+  --topic-generation-prompt TOPIC_GENERATION_PROMPT
+                        prompt to use in generating random topics
+  --topic-request-count TOPIC_REQUEST_COUNT
+                        number of requests to perform in random topic generation
+  --contextual-prompt-ratio CONTEXTUAL_PROMPT_RATIO
+                        ratio of prompts that should be contextual, e.g. summarization of an article
   --skip-instruction-re SKIP_INSTRUCTION_RE
                         regular expression used to filter low-quality/unusable instructions
-  --code-gen-re CODE_GEN_RE
-                        regular expression used to filter coding/programming tasks
-  --samples-per-request SAMPLES_PER_REQUEST
-                        number of random sample instructions to include in prompts
-  --min-instruction-length MIN_INSTRUCTION_LENGTH
-                        minimum instruction length
-  --max-instruction-length MAX_INSTRUCTION_LENGTH
-                        maximum instruction length
   --temperature TEMPERATURE
                         temperature parameter to use in OpenAI requests
   --top-p TOP_P         top-p parameter to use in OpenAI requests
   --frequency-penalty FREQUENCY_PENALTY
                         frequency penalty to use in OpenAI requests
   --presence-penalty PRESENCE_PENALTY
                         presence penalty to use in OpenAI requests
   --max-usage-tokens MAX_USAGE_TOKENS
                         Maximum token usage, calculated as sum of total_tokens from responses
-  --prompt-generation-concurrency PROMPT_GENERATION_CONCURRENCY
-                        Number of concurrent prompt generation threads/requests to use
+  --concurrency CONCURRENCY
+                        Number of concurrent threads/requests to use
   --min-docsearch-score MIN_DOCSEARCH_SCORE
+                        Minimum similarity score when querying vector DB to consider a prompt unique
+```
+
+### Using custom topics:
+
+If you want to use a specific set of topics for prompt generation, add `--topics-path /path/to/topics.txt` to the command.  This file must be plain text, one topic per line.
+
+### Using a custom topic generator:
+
+If you want to use random topics, but want those topics to be somewhat related to a specific category or idea, try playing with `--topic-generation-prompt` (and probablyl `--topic-request-count`).  By default, the topic generation prompt is just random, but you can try things like:
+
 ```
+... --topic-generation-prompt "Give me a list of 100 significant historical battles." --topic-request-count 10
+```
+
+Since the returned topics may include duplicates, it is not guaranteed that your topic list will contain 100 * 10 topics.
+
 
 ## Coming soon
 
 Scripts for fine-tuning various models using the self-instruct (and human-generated) prompts.
```

### Comparing `airoboros-0.0.6/README.md` & `airoboros-0.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,85 +1,92 @@
 # airoboros: using large language models to fine-tune large language models
 
-This is my take on implementing the [Self-Instruct paper](https://arxiv.org/abs/2212.10560).  The approach is quite heavily modified, and uses the human generated seeds provided by [Databricks Dolly Project](https://huggingface.co/datasets/databricks/databricks-dolly-15k)
+This is my take on implementing the [Self-Instruct paper](https://arxiv.org/abs/2212.10560).  The approach is quite heavily modified, and does not use any human-generated seeds.
 
 This updated implementation supports either the /v1/completions endpoint or /v1/chat/completions, which is particularly useful in that it supports gpt-4 and gpt-3.5-turbo (which is 1/10 the cost of text-davinci-003).
 
 
 ## Key differences
 
-* Sample instructions in prompts by default use the human-generated seeds from Dolly.
-* Machine-generated instructions are not sampled for prompt examples, to avoid degredation.
-* Support for either /v1/completions or /v1/chat/completions APIs (which allows gpt-3.5-turbo instead of text-davinci-003, as well as gpt-4 if you have access).
-* In memory vector db (Chroma) for similarity comparison, which is much faster than calculating rouge score for each generated instruction.
-* (Seemingly) better prompt, which includes injection of random topics to relate the instructions to, which creates much more diverse prompts.
-* Multi-threaded producers/consumer implementation for significantly faster runtimes (generally 150+ unique prompts per minute, more initially since there are fewer duplicates, decreasing over time).
-* Tries to ensure the context, if provided, is relevant to the topic and contains all the information that would be necessary to respond to the instruction, and nost just a link to article/etc.
-* Generally speaking, this implementation tries to reduce some of the [noise](https://github.com/tloen/alpaca-lora/issues/65)
-
-
-## Initial datasets
-
-Be sure to look over the openai terms of service before using the datasets, specifically the section about using the outputs to generate competing models...
-
-### 100k synthetic instructions, gpt-3.5-turbo
-
-* [instructions.jsonl](https://storage.googleapis.com/airoboros-dump/gpt-3.5-turbo-100k/instructions.jsonl)
-* [topics.txt](https://storage.googleapis.com/airoboros-dump/gpt-3.5-turbo-100k/topics.txt)
+* support for either /v1/completions or /v1/chat/completions APIs (which allows gpt-3.5-turbo instead of text-davinci-003, as well as gpt-4 if you have access)
+* support for custom topics list, custom topic generation prompt, or completely random topics
+* sn memory vector db (Chroma) for similarity comparison, which is much faster than calculating rouge score for each generated instruction
+* (seemingly) better prompts, which includes injection of random topics to relate the instructions to, which creates much more diverse synthetic instructions
+* multi-threaded producer/consumer implementation for significantly faster runtimes (generally 150+ unique prompts per minute, more initially since there are fewer duplicates, decreasing over time).
+* tries to ensure the context, if provided, is relevant to the topic and contains all the information that would be necessary to respond to the instruction, and nost just a link to article/etc.
+* generally speaking, this implementation tries to reduce some of the [noise](https://github.com/tloen/alpaca-lora/issues/65)
 
 
 ## Generating instructions
 
 See available options via:
 ```
 airoboros generate-instructions --help
 ```
 
-Example output:
+Help as of 2023-05-10:
 ```
-usage: self_instruct.py [-h] [--model MODEL] [--organization-id ORGANIZATION_ID] [--openai-api-key OPENAI_API_KEY] [--instruction-count INSTRUCTION_COUNT] [--seed-tasks-path SEED_TASKS_PATH] [--output-path OUTPUT_PATH] [--overwrite] [--append] [--prompt PROMPT] [--skip-instruction-re SKIP_INSTRUCTION_RE] [--code-gen-re CODE_GEN_RE]
-                        [--samples-per-request SAMPLES_PER_REQUEST] [--min-instruction-length MIN_INSTRUCTION_LENGTH] [--max-instruction-length MAX_INSTRUCTION_LENGTH] [--temperature TEMPERATURE] [--top-p TOP_P] [--frequency-penalty FREQUENCY_PENALTY] [--presence-penalty PRESENCE_PENALTY] [--max-usage-tokens MAX_USAGE_TOKENS]
-                        [--prompt-generation-concurrency PROMPT_GENERATION_CONCURRENCY] [--min-docsearch-score MIN_DOCSEARCH_SCORE]
+usage: self_instruct.py [-h] [--model MODEL] [--organization-id ORGANIZATION_ID] [--openai-api-key OPENAI_API_KEY] [--instruction-count INSTRUCTION_COUNT] [--batch-size BATCH_SIZE] [--output-path OUTPUT_PATH] [--topics-path TOPICS_PATH] [--overwrite] [--append] [--prompt PROMPT] [--contextual-prompt CONTEXTUAL_PROMPT]
+                        [--topic-generation-prompt TOPIC_GENERATION_PROMPT] [--topic-request-count TOPIC_REQUEST_COUNT] [--contextual-prompt-ratio CONTEXTUAL_PROMPT_RATIO] [--skip-instruction-re SKIP_INSTRUCTION_RE] [--temperature TEMPERATURE] [--top-p TOP_P] [--frequency-penalty FREQUENCY_PENALTY] [--presence-penalty PRESENCE_PENALTY]
+                        [--max-usage-tokens MAX_USAGE_TOKENS] [--concurrency CONCURRENCY] [--min-docsearch-score MIN_DOCSEARCH_SCORE]
 
 options:
   -h, --help            show this help message and exit
   --model MODEL         OpenAI model/engine to use for prompt generation, which can be either part of the /v1/completions or /v1/chat/completions endpoints
   --organization-id ORGANIZATION_ID
                         organization ID to include in the request to OpenAI, defaults to organization ID tied to the API key
   --openai-api-key OPENAI_API_KEY
                         OpenAI API key to use, defaults to the OPENAI_API_KEY environment variable
   --instruction-count INSTRUCTION_COUNT
                         number of instructions to generate, not including the seed instructions
-  --seed-tasks-path SEED_TASKS_PATH
-                        path to an input seed instructions JSONL file
+  --batch-size BATCH_SIZE
+                        number of candidate instructions to (attempt to) generate per request
   --output-path OUTPUT_PATH
                         path to store all generated instructions in
+  --topics-path TOPICS_PATH
+                        path to a newline separated list of topics
   --overwrite           overwrite output path if it exists
   --append              append to output path if it exists
-  --prompt PROMPT       prompt prefix to use for generating tasks
+  --prompt PROMPT       prompt prefix to use for generating non-contextual instructions
+  --contextual-prompt CONTEXTUAL_PROMPT
+                        prompt to use for generating contextual prompts
+  --topic-generation-prompt TOPIC_GENERATION_PROMPT
+                        prompt to use in generating random topics
+  --topic-request-count TOPIC_REQUEST_COUNT
+                        number of requests to perform in random topic generation
+  --contextual-prompt-ratio CONTEXTUAL_PROMPT_RATIO
+                        ratio of prompts that should be contextual, e.g. summarization of an article
   --skip-instruction-re SKIP_INSTRUCTION_RE
                         regular expression used to filter low-quality/unusable instructions
-  --code-gen-re CODE_GEN_RE
-                        regular expression used to filter coding/programming tasks
-  --samples-per-request SAMPLES_PER_REQUEST
-                        number of random sample instructions to include in prompts
-  --min-instruction-length MIN_INSTRUCTION_LENGTH
-                        minimum instruction length
-  --max-instruction-length MAX_INSTRUCTION_LENGTH
-                        maximum instruction length
   --temperature TEMPERATURE
                         temperature parameter to use in OpenAI requests
   --top-p TOP_P         top-p parameter to use in OpenAI requests
   --frequency-penalty FREQUENCY_PENALTY
                         frequency penalty to use in OpenAI requests
   --presence-penalty PRESENCE_PENALTY
                         presence penalty to use in OpenAI requests
   --max-usage-tokens MAX_USAGE_TOKENS
                         Maximum token usage, calculated as sum of total_tokens from responses
-  --prompt-generation-concurrency PROMPT_GENERATION_CONCURRENCY
-                        Number of concurrent prompt generation threads/requests to use
+  --concurrency CONCURRENCY
+                        Number of concurrent threads/requests to use
   --min-docsearch-score MIN_DOCSEARCH_SCORE
+                        Minimum similarity score when querying vector DB to consider a prompt unique
+```
+
+### Using custom topics:
+
+If you want to use a specific set of topics for prompt generation, add `--topics-path /path/to/topics.txt` to the command.  This file must be plain text, one topic per line.
+
+### Using a custom topic generator:
+
+If you want to use random topics, but want those topics to be somewhat related to a specific category or idea, try playing with `--topic-generation-prompt` (and probablyl `--topic-request-count`).  By default, the topic generation prompt is just random, but you can try things like:
+
 ```
+... --topic-generation-prompt "Give me a list of 100 significant historical battles." --topic-request-count 10
+```
+
+Since the returned topics may include duplicates, it is not guaranteed that your topic list will contain 100 * 10 topics.
+
 
 ## Coming soon
 
 Scripts for fine-tuning various models using the self-instruct (and human-generated) prompts.
```

### Comparing `airoboros-0.0.6/airoboros/self_instruct.py` & `airoboros-0.1.0/airoboros/self_instruct.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import argparse
 import backoff
 import os
 import json
+import hashlib
 import random
 import re
 import requests
 import secrets
 import signal
 import string
 import sys
 import threading
 import concurrent.futures
 from functools import partial
 from loguru import logger
-from queue import Queue
-from rouge_score import rouge_scorer
+from queue import Queue, Empty
 from typing import List, Dict, Any
 from uuid import uuid4
 from .exceptions import (
     RateLimitError,
     TooManyRequestsError,
     TokensExhaustedError,
     ServerOverloadedError,
@@ -26,38 +26,48 @@
     ContextLengthExceededError,
     BadResponseError,
 )
 from langchain.vectorstores import Chroma
 from langchain.embeddings import HuggingFaceEmbeddings
 
 # Defaults and constants.
-BATCH_SIZE = 13
-DEFAULT_PROMPT = f"""You are asked to generate a set of {BATCH_SIZE} diverse prompts.  These prompts will be given to a GPT model and we will evaluate the GPT model for completing the prompts.
+BATCH_SIZE = 20
+TOPIC_GENERATION_PROMPT = "Give me a list of 200 completely random topics."
+CONTEXTUAL_PROMPT = """Create a few instructions that can be provided to a GPT system to create text and a task related to the text.  Use diverse verbs, subject matters, and writing styles, and don't use any placeholders.
+
+Examples:
+ * Generate a few paragraphs about the process of making damascus steel.
+ * Write a short story about a goat/bird chimera that enjoys sailing.
+ * Compose a news article about a breakthrough in tire technology.
+ * Give me a detailed description of the Battle of Rennell Island during World War II, along with key dates, locations, and people involved.
 
-Here are the requirements:
- * Try not to repeat the verb for each __instruction__ to maximize diversity.
+Ensure each instruction is related to one of the following topics:
+{topics}
+
+Numbered list of {batch_size} instructions:
+"""
+CONTEXT_TASK_INJECTION = """After generating your response, add a line with "=:=:=", then generate a unique and interesting instruction or question that could be answered using only the generated text.  Examples include summarization, questions about specific details found within the text, or information extraction."""
+DEFAULT_PROMPT = """Create a set of {batch_size} diverse instructions.
+
+Requirements for the instructions:
+ * Do not repeat the verb for each instruction to maximize diversity.
  * Try to avoid controversial and politically charged subjects.
- * The __instruction__ should include a variety of types of prompts, such as open-ended generation, brainstorming, classification, closed question-answering, summarization, editing, information extraction, etc.
- * The __instruction__ should be something a large language model can complete with a text response, for example do not create a task asking to create visual/audio output, setting an alarm, scheduling something on the calendar, etc. because the language model cannot perform those tasks.
- * The __instruction__ should be in English.
- * The __instruction__ should be between 1 and 3 sentences long.
- * For prompts that require extracting information from __passage__, e.g. question-answering, summarization, information extraction, etc., include a passage of text with 2-8 sentences in __passage__ providing all relevant data, including more information than necessary to generate __response__. __passage__ must not be simple placeholders or links to external resources.  Be sure to include all words, phrases, dates, or lists of items in __passage__ if those are part of __response__.
- * Not all prompts require __passage__. For example, when a task asks about some general information, e.g. "what is the highest peak in the world?", it is not necssary to provide a specific __passage__. In this case, we simply put "__no_context__" in the __passage__ field.
- * The __response__ should be an appropriate response to the __instruction__ and __passage__
- * Be sure to include {BATCH_SIZE} prompts in the response.
-REPLACE_TOPICS
+ * The list of instructions should include a variety of types of prompts, such as open-ended text generation, creative writing, brainstorming, classification, editing, logical reasoning, etc.
+ * Each instruction must be something a large language model can complete with a text response, for example do not create a task asking to create visual/audio output, setting an alarm, scheduling something on the calendar, etc. because the language model cannot perform those tasks.
+ * Each instruction should be in English, and be between 1 and 3 sentences long.
+ * Do not include any prompts that would require additional information, for example instructions to summarize or extract information from a passage of text.
+ * Any instruction referencing a list of objects, such as classifying a list of items, should include the list of items.
 
-List of {BATCH_SIZE} prompts:
+Ensure each instruction is related to one of the following topics:
+{topics}
+
+Numbered list of {batch_size} prompts:
 """
 SKIP_WORDS = ["image", "graph", "picture", "file", "map", "draw", "plot", "go to"]
 SKIP_SEARCH_RE = re.compile(r"\b{'|'.join(SKIP_WORDS)}s?\b", re.I)
-CODE_GEN_RE = re.compile(
-    r"^(?:write|generate|create)(?:a )?(?:\w+ )?(?:script|program|code)\W", re.I
-)
-DOLLY_SEED_URL = "https://storage.googleapis.com/airoboros-dump/databricks-dolly-15k.jsonl"
 OPENAI_API_BASE_URL = "https://api.openai.com"
 MODEL_ENDPOINTS = {
     "completions": [
         "text-davinci-003",
         "text-davinci-002",
         "text-curie-001",
         "text-babbage-001",
@@ -92,63 +102,69 @@
             "help": "OpenAI API key to use, defaults to the OPENAI_API_KEY environment variable",
         },
         "--instruction-count": {
             "type": int,
             "default": 100000,
             "help": "number of instructions to generate, not including the seed instructions",
         },
-        "--seed-tasks-path": {
-            "type": str,
-            "help": "path to an input seed instructions JSONL file",
+        "--batch-size": {
+            "type": int,
+            "default": BATCH_SIZE,
+            "help": "number of candidate instructions to (attempt to) generate per request",
         },
         "--output-path": {
             "type": str,
             "help": "path to store all generated instructions in",
+            "default": "instructions.jsonl",
+        },
+        "--topics-path": {
+            "type": str,
+            "help": "path to a newline separated list of topics",
         },
         "--overwrite": {
             "action": "store_true",
             "help": "overwrite output path if it exists",
         },
         "--append": {
             "action": "store_true",
             "help": "append to output path if it exists",
         },
         "--prompt": {
             "type": str,
             "default": DEFAULT_PROMPT,
-            "help": "prompt prefix to use for generating tasks",
+            "help": "prompt prefix to use for generating non-contextual instructions",
         },
-        "--skip-instruction-re": {
+        "--contextual-prompt": {
             "type": str,
-            "default": SKIP_SEARCH_RE.pattern,
-            "help": "regular expression used to filter low-quality/unusable instructions",
+            "default": CONTEXTUAL_PROMPT,
+            "help": "prompt to use for generating contextual prompts",
         },
-        "--code-gen-re": {
+        "--topic-generation-prompt": {
             "type": str,
-            "default": CODE_GEN_RE.pattern,
-            "help": "regular expression used to filter coding/programming tasks",
+            "default": TOPIC_GENERATION_PROMPT,
+            "help": "prompt to use in generating random topics",
         },
-        "--samples-per-request": {
-            "type": str,
-            "default": 3,
-            "help": "number of random sample instructions to include in prompts",
-        },
-        "--min-instruction-length": {
+        "--topic-request-count": {
             "type": int,
-            "default": 2,
-            "help": "minimum instruction length",
+            "default": 4000,
+            "help": "number of requests to perform in random topic generation",
         },
-        "--max-instruction-length": {
-            "type": int,
-            "default": 150,
-            "help": "maximum instruction length",
+        "--contextual-prompt-ratio": {
+            "type": float,
+            "default": 0.1,
+            "help": "ratio of prompts that should be contextual, e.g. summarization of an article",
+        },
+        "--skip-instruction-re": {
+            "type": str,
+            "default": SKIP_SEARCH_RE.pattern,
+            "help": "regular expression used to filter low-quality/unusable instructions",
         },
         "--temperature": {
             "type": float,
-            "default": 0.7,
+            "default": 0.9,
             "help": "temperature parameter to use in OpenAI requests",
         },
         "--top-p": {
             "type": float,
             "default": 0.5,
             "help": "top-p parameter to use in OpenAI requests",
         },
@@ -162,17 +178,17 @@
             "default": 2,
             "help": "presence penalty to use in OpenAI requests",
         },
         "--max-usage-tokens": {
             "type": int,
             "help": "Maximum token usage, calculated as sum of total_tokens from responses",
         },
-        "--prompt-generation-concurrency": {
+        "--concurrency": {
             "type": int,
-            "help": "Number of concurrent prompt generation threads/requests to use",
+            "help": "Number of concurrent threads/requests to use",
             "default": 50,
         },
         "--min-docsearch-score": {
             "type": float,
             "help": "Minimum similarity score when querying vector DB to consider a prompt unique",
             "default": "0.35",
         },
@@ -181,138 +197,96 @@
     def __init__(
         self,
         *,
         model: str = "gpt-3.5-turbo",
         organization_id: str = None,
         openai_api_key: str = None,
         instruction_count: int = 100000,
-        seed_tasks: List[Dict[str, str]] = None,
-        seed_tasks_path: str = None,
-        output_path: str = None,
+        batch_size: int = BATCH_SIZE,
+        output_path: str = "instructions.jsonl",
+        topics_path: str = None,
         overwrite: bool = False,
         append: bool = True,
-        use_dolly_seed: bool = True,
         prompt: str = DEFAULT_PROMPT,
+        contextual_prompt: str = CONTEXTUAL_PROMPT,
+        topic_generation_prompt: str = TOPIC_GENERATION_PROMPT,
+        topic_request_count: int = 4000,
+        contextual_prompt_ratio: float = 0.15,
         skip_instruction_re: re.Pattern = SKIP_SEARCH_RE,
-        code_gen_re: re.Pattern = CODE_GEN_RE,
-        min_instruction_length: int = 3,
-        max_instruction_length: int = 150,
-        samples_per_request: int = 3,
         temperature: float = 0.7,
         top_p: float = 0.5,
         frequency_penalty: int = 0,
         presence_penalty: int = 2,
         max_usage_tokens: int | None = None,
-        prompt_generation_concurrency: int = 50,
+        concurrency: int = 50,
         min_docsearch_score: float = 0.35,
     ):
         """Constructor."""
         self.model = model
         self.organization_id = organization_id
         self.openai_api_key = openai_api_key or os.environ.get("OPENAI_API_KEY")
         if not self.openai_api_key:
             raise ValueError(
                 "OPENAI_API_KEY environment variable or openai_api_key must be provided"
             )
         self.instruction_count = instruction_count
-        if not output_path:
-            output_path = os.path.join(
-                os.path.dirname(os.path.abspath(__file__)),
-                "output",
-                "instructions.jsonl",
-            )
-        self.output_path = output_path
+        self.batch_size = batch_size
+        self.output_path = os.path.abspath(output_path)
+        self.topics_path = topics_path
         self.overwrite = overwrite
         self.append = append
-        output_dir = os.path.dirname(os.path.abspath(output_path))
-        if not os.path.exists(output_dir):
-            os.makedirs(output_dir)
         self.prompt = prompt
+        self.contextual_prompt = contextual_prompt
+        self.topic_generation_prompt = topic_generation_prompt
+        self.topic_request_count = topic_request_count
+        self.contextual_prompt_ratio = contextual_prompt_ratio
         self.skip_instruction_re = skip_instruction_re
         if isinstance(skip_instruction_re, str):
             self.skip_instruction_re = re.compile(skip_instruction_re, re.I)
-        self.code_gen_re = code_gen_re
-        if isinstance(code_gen_re, str):
-            self.code_gen_re = re.compile(code_gen_re, re.I)
-        self.min_instruction_length = min_instruction_length
-        self.max_instruction_length = max_instruction_length
         self.temperature = temperature
         self.top_p = top_p
         self.frequency_penalty = frequency_penalty
         self.presence_penalty = presence_penalty
-        self.samples_per_request = samples_per_request
         self.max_usage_tokens = max_usage_tokens
-        self._validate_model()
-        self.machine_tasks = []
-        self._initialize_seed_tasks(seed_tasks, seed_tasks_path, use_dolly_seed)
+        self.validate_model()
         self.used_tokens = 0
-        self.random_topics = set([])
         self.stop_producing = False
-        self.prompt_generation_concurrency = prompt_generation_concurrency
+        self.concurrency = concurrency
         self.min_docsearch_score = min_docsearch_score
-        self._initialize_docstore()
-
-    def _initialize_docstore(self):
-        """Initialize the in-memory vector database used to check prompt uniqueness."""
-        logger.info(
-            "Initializing in-memory document store for similarity comparison..."
-        )
-        texts = [
-            prompt["instruction"] for prompt in self.seed_tasks + self.machine_tasks
-        ]
-        self.docstore = Chroma.from_texts(texts, HuggingFaceEmbeddings())
+        self.initialize_docstores()
 
-    def _initialize_seed_tasks(
-        self,
-        seed_tasks: List[Dict[str, str]],
-        seed_tasks_path: str,
-        use_dolly_seed: bool,
-    ):
-        """Helper method to construct the seed tasks, either as input dict, from
-        user-provided seed path, or using the dolly 15k seeds (default).
-        """
-        if seed_tasks:
-            self.seed_tasks = seed_tasks
-            return
-        if seed_tasks_path:
-            seed_tasks = []
-            with open(seed_tasks_path) as infile:
-                for line in infile.readlines():
-                    seed_tasks.append(json.loads(line))
-        elif use_dolly_seed:
-            dolly_seed_path = os.path.join(
-                os.path.dirname(os.path.abspath(__file__)), ".seed", "dolly_seeds.jsonl"
-            )
-            if not os.path.exists(os.path.dirname(dolly_seed_path)):
-                os.mkdir(os.path.dirname(dolly_seed_path))
-            if not os.path.isfile(dolly_seed_path):
-                result = requests.get(DOLLY_SEED_URL)
-                with open(dolly_seed_path, "w") as outfile:
-                    outfile.write(result.text)
-            with open(dolly_seed_path, "r") as infile:
-                seed_tasks = [json.loads(line) for line in infile.readlines()]
-            self.seed_tasks = seed_tasks
-        logger.info(f"Found {len(self.seed_tasks)} human seed tasks to use...")
+    def initialize_docstores(self):
+        """Initialize the in-memory vector databases used to check prompt uniqueness."""
+        self.machine_task_count = 0
+        docs = []
         if os.path.exists(self.output_path):
             if self.overwrite:
                 os.remove(self.output_path)
             elif self.append:
                 with open(self.output_path, "r") as infile:
-                    self.machine_tasks = [
-                        json.loads(line) for line in infile.readlines()
-                    ]
+                    for line in infile.readlines():
+                        task = json.loads(line)
+                        self.machine_task_count += 1
+                        docs.append(task["instruction"])
                 logger.info(
-                    f"Found {len(self.machine_tasks)} pre-existing machine seed tasks to use..."
+                    f"Found {self.machine_task_count} existing machine-generated instructions."
                 )
             else:
                 raise RuntimeError(
                     f"{self.output_path} already exists, but overwrite and append are false!"
                 )
+        logger.info(
+            "Initializing in-memory document store for similarity comparison..."
+        )
+        if not docs:
+            docs = ["__initialize__"]
+        embeddings = HuggingFaceEmbeddings()
+        self.docstore = Chroma.from_texts(docs, embeddings)
 
-    def _validate_model(self):
+    def validate_model(self):
         """Ensure the specified model is available, and configure the endpoint
         to use accordingly (chat completions or completions).
         """
         if self.model in MODEL_ENDPOINTS["completions"]:
             self._completions = True
         elif self.model in MODEL_ENDPOINTS["chat_completions"]:
             self._completions = False
@@ -328,194 +302,110 @@
                 f"Invalid openai API key [{result.status_code}: {result.text}]"
             )
         available = {item["id"] for item in result.json()["data"]}
         if self.model not in available:
             raise ValueError(f"Model is not available to your API key: {self.model}")
         logger.success(f"Successfully validated model: {self.model}")
 
-    @staticmethod
-    def clean_instruction_text(instruction: str) -> str:
-        """Remove extra/trailing whitespace from instruction prompts.
-
-        :param instruction: The prompt text to clean.
-        :type instruction: str
-
-        :return: The cleaned prompt text.
-        :rtype: str
-        """
-        return re.sub(
-            r"\s+", " ", " ".join(instruction.splitlines()).strip().rstrip(":")
-        )
-
-    def initialize_random_topics(self):
-        path = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), ".seed", "topics.txt"
-        )
-        if os.path.exists(path):
-            with open(path, "r") as infile:
-                self.random_topics = {
-                    line.strip().lower() for line in infile.readlines() if line.strip()
+    def initialize_topics(self) -> None:
+        """Read existing cached topics, or generate a new list."""
+        if self.topics_path:
+            if not os.path.exists(self.topics_path):
+                raise ValueError(f"Topics file: {self.topics_path} does not exis!")
+        if not self.topics_path:
+            self.topics_path = f"topics-{hashlib.md5((self.topic_generation_prompt + str(self.topic_request_count)).encode()).hexdigest()}.txt"
+        if os.path.exists(self.topics_path):
+            with open(self.topics_path, "r") as infile:
+                self.topics = {
+                    line.strip() for line in infile.readlines() if line.strip()
                 }
-                logger.info(f"Using {len(self.random_topics)} cached random topics...")
-            return
+                logger.info(
+                    f"Using {len(self.topics)} topics from {self.topics_path}..."
+                )
+                return
+        self.topics = set([])
         logger.info("Generating random topics to use in prompts...")
-        with concurrent.futures.ThreadPoolExecutor(20) as pool:
-            responses = pool.map(
-                partial(self._post_no_exc, "/v1/completions"),
-                [
+        topic_prompts = [
+            {
+                "model": "gpt-3.5-turbo",
+                "messages": [
                     {
-                        "model": "text-davinci-003",
-                        "prompt": ["Give me a list of 200 completely random topics."]
-                        * 20,
-                        "temperature": 1.0,
-                        "max_tokens": 800,
+                        "role": "user",
+                        "content": self.topic_generation_prompt,
                     }
-                ]
-                * 20,
+                ],
+                "temperature": 1.0,
+            }
+            for _ in range(self.topic_request_count)
+        ]
+        with concurrent.futures.ThreadPoolExecutor(self.concurrency) as pool:
+            responses = pool.map(
+                partial(self._post_no_exc, "/v1/chat/completions"), topic_prompts
             )
-        with open(path, "w") as outfile:
+        seen = set([])
+        with open(self.topics_path, "w") as outfile:
             for response in responses:
                 if not response:
                     continue
                 for choice in response["choices"]:
-                    for line in choice["text"].splitlines():
-                        if match := re.search(r"\s*\d+\s*\.\s*(.+)", line):
-                            topic = match.group(1).lower()
-                            self.random_topics.add(topic)
-                            outfile.write(topic + "\n")
+                    for line in choice["message"]["content"].splitlines():
+                        topic = re.sub(r"(\s*\d+\s*\.\s+)+", "", line).strip()
+                        if not topic or topic.lower() in seen:
+                            continue
+                        seen.add(topic.lower())
+                        self.topics.add(topic)
+                        outfile.write(topic + "\n")
         logger.success(
-            f"Successfully generated {len(self.random_topics)} random topics..."
+            f"Successfully generated {len(self.topics)} topics, stored in {self.topics_path}..."
         )
 
-    def generate_prompt_from_instructions(
-        self, instructions: List[Dict[str, any]]
-    ) -> str:
-        """Generate a single prompt string with multiple instructions.
+    def generate_prompt(self, template: str):
+        """Generate a single prompt, inserting random topics.
 
-        :param instructions: A list of instructions to encode.
-        :type instructions: List[str]
+        :param template: The prompt template to use.
+        :type template: str
 
-        :return: The encoded prompt.
+        :return: The prompt, including a list of random topics.
         :rtype: str
         """
-        topic_prompt = (
-            "* Ensure each generated prompt is related to one of the following topics: "
+        topics = "\n".join(
+            [
+                f" * {topic}"
+                for topic in random.sample(list(self.topics), min(self.batch_size, 10))
+            ]
         )
-        topic_texts = random.sample(list(self.random_topics), min(BATCH_SIZE, 6))
-        topic_prompt += ", ".join(topic_texts)
-        prompt = [self.prompt.replace("REPLACE_TOPICS", topic_prompt)]
-        for idx, instruction in enumerate(instructions):
-            text = self.clean_instruction_text(instruction["instruction"])
-            prompt.append(f"{idx + 1}. __instruction__: {text}")
-            context = (
-                "__no_context__"
-                if not instruction["context"].strip()
-                else instruction["context"].strip()
-            )
-            prompt.append(f"{idx + 1}. __passage__: {context}")
-            prompt.append(f"{idx + 1}. __response__: {instruction['response']}")
-        return "\n".join(prompt)
-
-    def extract_instructions_from_response(
-        self, response: Dict[str, Any]
-    ) -> List[Dict[str, Any]]:
+        return template.format(topics=topics, batch_size=self.batch_size)
+
+    def extract_instructions_from_response(self, text: str) -> List[str]:
         """Extract the list of instructions from the OpenAI response.
 
-        :param response: The response from the OpenAI request.
-        :type re: Dict[str, Any]
+        :param text: The OpenAI response text.
+        :type text: str
 
         :return: List of instructions.
         :rtype: List[str]
         """
-        if (
-            not response
-            or not response.get("choices")
-            or response["choices"][0]["finish_reason"] == "length"
-        ):
+        if not text:
             return []
-
-        text = None
-        if self._completions:
-            text = response["choices"][0]["text"]
-        else:
-            text = response["choices"][0]["message"]["content"]
-
-        tasks = []
-        for instruction in re.findall(
-            r"(\d+\s*\.\s*__instruction__:[\s\r\n]*.*?)(?=\d+\s*\.\s*__|$)",
-            text,
-            re.DOTALL,
-        ):
-            idx = instruction.split(".")[0].strip()
-            instruction_text = instruction.split("__instruction__:")[-1].strip()
-            if not instruction_text:
-                continue
-            if (
-                not self.min_instruction_length
-                < len(instruction_text.split())
-                < self.max_instruction_length
-            ):
-                logger.warning(
-                    f"Skipping instruction: {instruction_text} [instruction length]"
-                )
+        instructions = []
+        for instruction in re.findall(r"\s*\d+\s*\.\s(.*)\s*", text):
             # Skip various prompts that have been deemed unsuitable for language models
             # by the self-instruct team.
             if (
-                self.skip_instruction_re.search(instruction_text)
-                or self.code_gen_re.search(instruction_text)
-                or instruction_text[0] in string.punctuation
-                or not instruction_text[0].isascii()
+                self.skip_instruction_re.search(instruction)
+                or instruction[0] in string.punctuation
+                or not instruction[0].isascii()
             ):
                 logger.warning(
-                    f"Skipping instruction: {instruction_text} [code, ascii, other unsuitable]"
+                    f"Skipping instruction: {instruction} [unsuitable prompt]"
                 )
                 continue
-            context = re.search(
-                f"(?<!\\d){idx}\\s*\\.\\s*__passage__:[\\r\\n\\s]*(.*?)(?=\\d+\\s*\\.\\s*__|$)",
-                text,
-                re.DOTALL,
-            )
-            if not context:
-                logger.warning(
-                    f"Skipping instruction: {instruction_text} [context not provided]"
-                )
-                continue
-            context = context.group(1).strip()
-            if context == "__no_context__":
-                context = ""
-            response = re.search(
-                f"(?<!\\d){idx}\\s*\\.\\s*__response__:[\\r\\n\\s]*(.*?)(?=\\d+\\s*\\.\\s*__|$)",
-                text,
-                re.DOTALL,
-            )
-            if not response or not response.group(1).strip():
-                logger.warning(
-                    f"Skipping instruction: {instruction_text} [response not provided]"
-                )
-                continue
-            response = response.group(1).strip()
-            if len(response) > len(context):
-                logger.warning("Ignoring context, shorter than response.")
-                context = ""
-            else:
-                scorer = rouge_scorer.RougeScorer(["rougeL"], use_stemmer=False)
-                if scorer.score(context, response)["rougeL"].fmeasure >= 0.7:
-                    logger.warning("Ignoring context, too similar to response.")
-                    context = ""
-            tasks.append(
-                {
-                    "instruction": instruction_text,
-                    "context": context,
-                    "response": response,
-                }
-            )
-            logger.info(
-                f"Generated candidate task [has context: {context != ''}]: {instruction_text}"
-            )
-        return tasks
+            instructions.append(instruction)
+            logger.info(f"Generated candidate task: {instruction}")
+        return instructions
 
     @backoff.on_exception(
         backoff.expo,
         (
             requests.exceptions.ConnectionError,
             requests.exceptions.Timeout,
             ServerError,
@@ -541,15 +431,15 @@
             headers["OpenAI-Organization"] = self.organization_id
         request_id = str(uuid4())
         logger.debug(f"POST [{request_id}] with payload {json.dumps(payload)}")
         result = requests.post(
             f"{OPENAI_API_BASE_URL}{path}",
             headers=headers,
             json=payload,
-            timeout=240.0,
+            timeout=600.0,
         )
         if result.status_code != 200:
             text = result.text
             if "too many requests" in text.lower():
                 raise TooManyRequestsError(text)
             if "rate limit reached" in text.lower():
                 raise RateLimitError(text)
@@ -573,47 +463,85 @@
         """Post, ignoring all exceptions."""
         try:
             return self._post(*a, **k)
         except Exception as ex:
             logger.error(f"Error performing post: {ex}")
         return None
 
-    def generate_instruction_batch(self, queue: Queue) -> None:
-        """Generate an set of instructions.
+    def generate_response(self, instruction: str) -> str:
+        """Call OpenAI with the specified instruction and return the text response.
 
-        :param queue: Queue to pass generated outputs to.
-        :type queue: Queue
+        :param instruction: The instruction to respond to.
+        :type instruction: str
+
+        :return: Response text.
+        :rtype: str
         """
-        instructions = random.sample(self.seed_tasks, self.samples_per_request)
-        prompt = self.generate_prompt_from_instructions(instructions)
-        estimated_tokens = int(len(prompt) / 4)
-        if estimated_tokens > 2700:
-            logger.warning("Skipping prompt, too long")
-            return
         path = "/v1/completions" if self._completions else "/v1/chat/completions"
         payload = {
             "model": self.model,
             "temperature": self.temperature,
             "top_p": self.top_p,
             "frequency_penalty": self.frequency_penalty,
             "presence_penalty": self.presence_penalty,
-            "stop": [f"{BATCH_SIZE+1}."],
-            "max_tokens": 4000 - estimated_tokens if self._completions else None,
         }
         if self._completions:
-            payload["prompt"] = prompt
+            payload["prompt"] = instruction
+            payload["max_tokens"] = 4000
         else:
-            payload["messages"] = [{"role": "user", "content": prompt}]
-        try:
-            for new_instruction in self.extract_instructions_from_response(
-                self._post(path, payload)
-            ):
-                queue.put(new_instruction)
-        except ContextLengthExceededError:
-            ...
+            payload["messages"] = [{"role": "user", "content": instruction}]
+        response = self._post_no_exc(path, payload)
+        if (
+            not response
+            or not response.get("choices")
+            or response["choices"][0]["finish_reason"] == "length"
+        ):
+            return None
+        text = None
+        if self._completions:
+            text = response["choices"][0]["text"]
+        else:
+            text = response["choices"][0]["message"]["content"]
+        return text
+
+    def generate_instruction_batch(self, queue: Queue) -> None:
+        """Generate an set of instructions.
+
+        :param queue: Queue to pass generated outputs to.
+        :type queue: Queue
+        """
+        contextual = random.random() <= self.contextual_prompt_ratio
+        prompt = self.generate_prompt(
+            self.prompt if not contextual else self.contextual_prompt
+        )
+        for new_instruction in self.extract_instructions_from_response(
+            self.generate_response(prompt)
+        ):
+            prompt = new_instruction
+            if contextual:
+                new_instruction += f"\n{CONTEXT_TASK_INJECTION}"
+                prompt = self.generate_response(
+                    "  ".join([new_instruction, CONTEXT_TASK_INJECTION])
+                )
+                if not prompt or "=:=:=" not in prompt:
+                    logger.error(
+                        f"Error generating contextual prompt: {new_instruction}"
+                    )
+                parts = [part.strip() for part in prompt.split("=:=:=")]
+                flip = random.random()
+                if flip <= 0.7:
+                    prompt = f"Using the provided text, respond to the instruction: {parts[1]}\n\n{parts[0]}"
+                elif flip <= 0.85:
+                    prompt = (
+                        parts[0]
+                        + f"\n\nUsing the text above, respond to the instruction: {parts[1]}"
+                    )
+                else:
+                    prompt = parts[1] + f"\n\nContext:\n{parts[0]}"
+            queue.put({"instruction": prompt})
 
     def generate_instruction_batches(self, queue: Queue) -> None:
         """Generate batches of instructions, storing new instructions in queue.
 
         :param queue: Queue to store new instructions in for post-processing.
         :type queue: Queue
         """
@@ -628,24 +556,22 @@
             except Exception as exc:
                 logger.error(f"Unhandled exception generating batch: {exc}")
                 consecutive_errors += 1
                 if consecutive_errors > 3:
                     logger.error("Too many consecutive errors, shutting down!")
                     os.kill(os.getpid(), signal.SIGKILL)
 
-    def validate_and_store_results(
-        self, queue: Queue, consume_remaining: bool = False
-    ) -> None:
+    def validate_and_store_results(self, queue: Queue) -> None:
         """Dedupe based on rouge score for each new instruction and save results.
 
         :param queue: Queue to consume messages from.
         :type queue: Queue
         """
         with open(self.output_path, "a+") as outfile:
-            while len(self.machine_tasks) < self.instruction_count or consume_remaining:
+            while True:
                 instruction = queue.get()
                 if not instruction:
                     break
                 similar = self.docstore.similarity_search_with_score(
                     instruction["instruction"], k=1
                 )
                 similarity_score = 1.0
@@ -654,50 +580,156 @@
                 if similarity_score <= self.min_docsearch_score:
                     logger.warning(
                         f"Skipping instruction, too similar [{score}]: {instruction['instruction']}"
                     )
                     continue
                 outfile.write(json.dumps(instruction) + "\n")
                 outfile.flush()
-                self.machine_tasks.append(instruction)
+                self.machine_task_count += 1
+                if self.machine_task_count >= self.instruction_count:
+                    self.stop_producing = True
                 self.docstore.add_texts([instruction["instruction"]])
                 logger.success(
-                    f"Generated unique [score={similarity_score}] instruction [total={len(self.machine_tasks)}]: {instruction['instruction']}"
+                    f"Generated unique [score={similarity_score}] instruction [total={self.machine_task_count}]: {instruction['instruction']}"
                 )
-        self.stop_producing = True
 
-    def run(self):
-        """Run the self-instruct, instruction generation task to completion."""
-        self.initialize_random_topics()
-        if len(self.machine_tasks) >= self.instruction_count:
-            logger.error(
-                f"Already have {len(self.machine_tasks)} machine-generated tasks!"
+    def inject_response(self, instruction):
+        """Update the input instruction with the response from OpenAI."""
+        if instruction.get("response"):
+            return instruction
+        result = self.generate_response(instruction["instruction"])
+        if result:
+            return {"instruction": instruction["instruction"], "response": result}
+        return None
+
+    def run_prompt_generation_phase(self):
+        """Run the self-instruct, instruction generation (without responses)."""
+        self.initialize_topics()
+        if self.machine_task_count >= self.instruction_count:
+            logger.warning(
+                f"Already have {self.machine_task_count} machine-generated tasks, skipping generation..."
             )
             return
-        queue = Queue(maxsize=100)
+        queue = Queue(maxsize=self.concurrency * BATCH_SIZE)
         producers = [
             threading.Thread(target=self.generate_instruction_batches, args=(queue,))
-            for _ in range(self.prompt_generation_concurrency)
+            for _ in range(self.concurrency)
         ]
         for producer in producers:
             producer.start()
         consumer = threading.Thread(
             target=self.validate_and_store_results, args=(queue,)
         )
         consumer.start()
-        consumer.join()
         for producer in producers:
             producer.join()
-
-        # Consume any tasks generated after the consumer stopped.
         queue.put(None)
-        self.validate_and_store_results(queue, consume_remaining=True)
+        consumer.join()
 
+    def generate_responses(self, input_queue: Queue, output_queue: Queue):
+        """Generate responses to machine-generated prompts."""
+        while True:
+            try:
+                instruction = input_queue.get(block=True, timeout=10.0)
+                if instruction is None:
+                    output_queue.put(None)
+                    break
+            except Empty:
+                continue
+            if result := self.inject_response(instruction):
+                output_queue.put(result)
+
+    def store_completed_results(self, tmp_path: str, queue: Queue) -> None:
+        """Store all completed instructions."""
+        finished_count = 0
+        with open(tmp_path, "a+") as outfile:
+            while True:
+                try:
+                    instruction = queue.get(block=True, timeout=10.0)
+                except Empty:
+                    continue
+                if instruction is None:
+                    finished_count += 1
+                    if finished_count == self.concurrency:
+                        break
+                else:
+                    outfile.write(json.dumps(instruction) + "\n")
+                    logger.success(
+                        f"Generated response [{instruction['instruction'][0:100]}]\n{instruction['response']}"
+                    )
+
+    def run_response_generation_phase(self):
+        """Generate the responses for each of the generated prompts."""
+        input_queue = Queue(maxsize=self.concurrency * 4)
+        output_queue = Queue()
+        producers = [
+            threading.Thread(
+                target=self.generate_responses, args=(input_queue, output_queue)
+            )
+            for _ in range(self.concurrency)
+        ]
+        for producer in producers:
+            producer.start()
+
+        # Skip over any responses that have already been generated.
+        tmp_path = f"{self.output_path}.with_results.tmp"
+        already_responded = set([])
+        if os.path.exists(tmp_path):
+            with open(f"{tmp_path}.filtered", "w") as outfile:
+                with open(tmp_path, "r") as infile:
+                    for line in infile:
+                        instruction = json.loads(line)
+                        if "response" in instruction:
+                            already_responded.add(
+                                hashlib.md5(
+                                    instruction["instruction"].encode()
+                                ).hexdigest()
+                            )
+                            outfile.write(line)
+            os.rename(f"{tmp_path}.filtered", tmp_path)
+            logger.info(
+                f"Found {len(already_responded)} prompts that have already been responded to..."
+            )
+
+        # Start consumer.
+        consumer = threading.Thread(
+            target=self.store_completed_results, args=(tmp_path, output_queue)
+        )
+        consumer.start()
+
+        # Queue up the instructions to be answered.
+        with open(self.output_path, "r") as infile:
+            for line in infile:
+                instruction = json.loads(line)
+                if (
+                    hashlib.md5(instruction["instruction"].encode()).hexdigest()
+                    in already_responded
+                ):
+                    continue
+                input_queue.put(instruction)
+
+        # Send termination queue messages to each producer.
+        for _ in range(self.concurrency):
+            input_queue.put(None)
+
+        # Join all threads.
+        for producer in producers:
+            producer.join()
+        consumer.join()
+        os.rename(tmp_path, self.output_path)
+
+    def run(self):
+        """Run prompt generation and answer to completion."""
+        self.run_prompt_generation_phase()
+        logger.success(
+            f"Finished generating instructions [asked for {self.instruction_count}, created {self.machine_task_count}], generating responses..."
+        )
+        self.run_response_generation_phase()
         logger.success(
-            f"Finished generating {len(self.machine_tasks)} instructions and responses."
+            f"Finished self-instruct task, total instructions: {self.machine_task_count}"
         )
 
 
 def main(args):
     random.seed(secrets.randbelow(1000000000))
     parser = argparse.ArgumentParser()
     for arg, kwargs in SelfInstructor.CLI_ARGS.items():
```

### Comparing `airoboros-0.0.6/airoboros.egg-info/PKG-INFO` & `airoboros-0.1.0/airoboros.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,101 +1,108 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 0.0.6
+Version: 0.1.0
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # airoboros: using large language models to fine-tune large language models
 
-This is my take on implementing the [Self-Instruct paper](https://arxiv.org/abs/2212.10560).  The approach is quite heavily modified, and uses the human generated seeds provided by [Databricks Dolly Project](https://huggingface.co/datasets/databricks/databricks-dolly-15k)
+This is my take on implementing the [Self-Instruct paper](https://arxiv.org/abs/2212.10560).  The approach is quite heavily modified, and does not use any human-generated seeds.
 
 This updated implementation supports either the /v1/completions endpoint or /v1/chat/completions, which is particularly useful in that it supports gpt-4 and gpt-3.5-turbo (which is 1/10 the cost of text-davinci-003).
 
 
 ## Key differences
 
-* Sample instructions in prompts by default use the human-generated seeds from Dolly.
-* Machine-generated instructions are not sampled for prompt examples, to avoid degredation.
-* Support for either /v1/completions or /v1/chat/completions APIs (which allows gpt-3.5-turbo instead of text-davinci-003, as well as gpt-4 if you have access).
-* In memory vector db (Chroma) for similarity comparison, which is much faster than calculating rouge score for each generated instruction.
-* (Seemingly) better prompt, which includes injection of random topics to relate the instructions to, which creates much more diverse prompts.
-* Multi-threaded producers/consumer implementation for significantly faster runtimes (generally 150+ unique prompts per minute, more initially since there are fewer duplicates, decreasing over time).
-* Tries to ensure the context, if provided, is relevant to the topic and contains all the information that would be necessary to respond to the instruction, and nost just a link to article/etc.
-* Generally speaking, this implementation tries to reduce some of the [noise](https://github.com/tloen/alpaca-lora/issues/65)
-
-
-## Initial datasets
-
-Be sure to look over the openai terms of service before using the datasets, specifically the section about using the outputs to generate competing models...
-
-### 100k synthetic instructions, gpt-3.5-turbo
-
-* [instructions.jsonl](https://storage.googleapis.com/airoboros-dump/gpt-3.5-turbo-100k/instructions.jsonl)
-* [topics.txt](https://storage.googleapis.com/airoboros-dump/gpt-3.5-turbo-100k/topics.txt)
+* support for either /v1/completions or /v1/chat/completions APIs (which allows gpt-3.5-turbo instead of text-davinci-003, as well as gpt-4 if you have access)
+* support for custom topics list, custom topic generation prompt, or completely random topics
+* sn memory vector db (Chroma) for similarity comparison, which is much faster than calculating rouge score for each generated instruction
+* (seemingly) better prompts, which includes injection of random topics to relate the instructions to, which creates much more diverse synthetic instructions
+* multi-threaded producer/consumer implementation for significantly faster runtimes (generally 150+ unique prompts per minute, more initially since there are fewer duplicates, decreasing over time).
+* tries to ensure the context, if provided, is relevant to the topic and contains all the information that would be necessary to respond to the instruction, and nost just a link to article/etc.
+* generally speaking, this implementation tries to reduce some of the [noise](https://github.com/tloen/alpaca-lora/issues/65)
 
 
 ## Generating instructions
 
 See available options via:
 ```
 airoboros generate-instructions --help
 ```
 
-Example output:
+Help as of 2023-05-10:
 ```
-usage: self_instruct.py [-h] [--model MODEL] [--organization-id ORGANIZATION_ID] [--openai-api-key OPENAI_API_KEY] [--instruction-count INSTRUCTION_COUNT] [--seed-tasks-path SEED_TASKS_PATH] [--output-path OUTPUT_PATH] [--overwrite] [--append] [--prompt PROMPT] [--skip-instruction-re SKIP_INSTRUCTION_RE] [--code-gen-re CODE_GEN_RE]
-                        [--samples-per-request SAMPLES_PER_REQUEST] [--min-instruction-length MIN_INSTRUCTION_LENGTH] [--max-instruction-length MAX_INSTRUCTION_LENGTH] [--temperature TEMPERATURE] [--top-p TOP_P] [--frequency-penalty FREQUENCY_PENALTY] [--presence-penalty PRESENCE_PENALTY] [--max-usage-tokens MAX_USAGE_TOKENS]
-                        [--prompt-generation-concurrency PROMPT_GENERATION_CONCURRENCY] [--min-docsearch-score MIN_DOCSEARCH_SCORE]
+usage: self_instruct.py [-h] [--model MODEL] [--organization-id ORGANIZATION_ID] [--openai-api-key OPENAI_API_KEY] [--instruction-count INSTRUCTION_COUNT] [--batch-size BATCH_SIZE] [--output-path OUTPUT_PATH] [--topics-path TOPICS_PATH] [--overwrite] [--append] [--prompt PROMPT] [--contextual-prompt CONTEXTUAL_PROMPT]
+                        [--topic-generation-prompt TOPIC_GENERATION_PROMPT] [--topic-request-count TOPIC_REQUEST_COUNT] [--contextual-prompt-ratio CONTEXTUAL_PROMPT_RATIO] [--skip-instruction-re SKIP_INSTRUCTION_RE] [--temperature TEMPERATURE] [--top-p TOP_P] [--frequency-penalty FREQUENCY_PENALTY] [--presence-penalty PRESENCE_PENALTY]
+                        [--max-usage-tokens MAX_USAGE_TOKENS] [--concurrency CONCURRENCY] [--min-docsearch-score MIN_DOCSEARCH_SCORE]
 
 options:
   -h, --help            show this help message and exit
   --model MODEL         OpenAI model/engine to use for prompt generation, which can be either part of the /v1/completions or /v1/chat/completions endpoints
   --organization-id ORGANIZATION_ID
                         organization ID to include in the request to OpenAI, defaults to organization ID tied to the API key
   --openai-api-key OPENAI_API_KEY
                         OpenAI API key to use, defaults to the OPENAI_API_KEY environment variable
   --instruction-count INSTRUCTION_COUNT
                         number of instructions to generate, not including the seed instructions
-  --seed-tasks-path SEED_TASKS_PATH
-                        path to an input seed instructions JSONL file
+  --batch-size BATCH_SIZE
+                        number of candidate instructions to (attempt to) generate per request
   --output-path OUTPUT_PATH
                         path to store all generated instructions in
+  --topics-path TOPICS_PATH
+                        path to a newline separated list of topics
   --overwrite           overwrite output path if it exists
   --append              append to output path if it exists
-  --prompt PROMPT       prompt prefix to use for generating tasks
+  --prompt PROMPT       prompt prefix to use for generating non-contextual instructions
+  --contextual-prompt CONTEXTUAL_PROMPT
+                        prompt to use for generating contextual prompts
+  --topic-generation-prompt TOPIC_GENERATION_PROMPT
+                        prompt to use in generating random topics
+  --topic-request-count TOPIC_REQUEST_COUNT
+                        number of requests to perform in random topic generation
+  --contextual-prompt-ratio CONTEXTUAL_PROMPT_RATIO
+                        ratio of prompts that should be contextual, e.g. summarization of an article
   --skip-instruction-re SKIP_INSTRUCTION_RE
                         regular expression used to filter low-quality/unusable instructions
-  --code-gen-re CODE_GEN_RE
-                        regular expression used to filter coding/programming tasks
-  --samples-per-request SAMPLES_PER_REQUEST
-                        number of random sample instructions to include in prompts
-  --min-instruction-length MIN_INSTRUCTION_LENGTH
-                        minimum instruction length
-  --max-instruction-length MAX_INSTRUCTION_LENGTH
-                        maximum instruction length
   --temperature TEMPERATURE
                         temperature parameter to use in OpenAI requests
   --top-p TOP_P         top-p parameter to use in OpenAI requests
   --frequency-penalty FREQUENCY_PENALTY
                         frequency penalty to use in OpenAI requests
   --presence-penalty PRESENCE_PENALTY
                         presence penalty to use in OpenAI requests
   --max-usage-tokens MAX_USAGE_TOKENS
                         Maximum token usage, calculated as sum of total_tokens from responses
-  --prompt-generation-concurrency PROMPT_GENERATION_CONCURRENCY
-                        Number of concurrent prompt generation threads/requests to use
+  --concurrency CONCURRENCY
+                        Number of concurrent threads/requests to use
   --min-docsearch-score MIN_DOCSEARCH_SCORE
+                        Minimum similarity score when querying vector DB to consider a prompt unique
+```
+
+### Using custom topics:
+
+If you want to use a specific set of topics for prompt generation, add `--topics-path /path/to/topics.txt` to the command.  This file must be plain text, one topic per line.
+
+### Using a custom topic generator:
+
+If you want to use random topics, but want those topics to be somewhat related to a specific category or idea, try playing with `--topic-generation-prompt` (and probablyl `--topic-request-count`).  By default, the topic generation prompt is just random, but you can try things like:
+
 ```
+... --topic-generation-prompt "Give me a list of 100 significant historical battles." --topic-request-count 10
+```
+
+Since the returned topics may include duplicates, it is not guaranteed that your topic list will contain 100 * 10 topics.
+
 
 ## Coming soon
 
 Scripts for fine-tuning various models using the self-instruct (and human-generated) prompts.
```

### Comparing `airoboros-0.0.6/setup.py` & `airoboros-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,40 +2,39 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md")) as infile:
     long_description = infile.read()
 
 setup(
     name="airoboros",
-    version="0.0.6",
+    version="0.1.0",
     description="Updated and improved implementation of the self-instruct system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jondurbin/airoboros",
     author="Jon Durbin",
     license="Apache 2.0",
     packages=["airoboros"],
     install_requires=[
-        "rouge-score>=0.1.2",
         "aiohttp>=3.8",
         "backoff>=2.2",
         "requests>=2.28",
         "loguru>=0.7",
         "chromadb>=0.3.21",
-        "langchain>=0.0.155",
+        "langchain>=0.0.162",
         "sentence-transformers>=2.2.2",
     ],
     extras_require={
         "dev": [
             "black",
             "flake8",
         ],
     },
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3.10",
     ],
     entry_points={
         "console_scripts": [
```

