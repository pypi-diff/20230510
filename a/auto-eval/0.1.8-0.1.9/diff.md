# Comparing `tmp/auto-eval-0.1.8.tar.gz` & `tmp/auto-eval-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.1.8.tar", last modified: Mon May  8 13:28:27 2023, max compression
+gzip compressed data, was "auto-eval-0.1.9.tar", last modified: Wed May 10 10:56:57 2023, max compression
```

## Comparing `auto-eval-0.1.8.tar` & `auto-eval-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:28:27.824972 auto-eval-0.1.8/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.8/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    11522 2023-05-08 13:28:27.824711 auto-eval-0.1.8/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    11096 2023-05-08 02:17:16.000000 auto-eval-0.1.8/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:28:27.821655 auto-eval-0.1.8/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    11522 2023-05-08 13:28:27.000000 auto-eval-0.1.8/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      480 2023-05-08 13:28:27.000000 auto-eval-0.1.8/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-08 13:28:27.000000 auto-eval-0.1.8/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-05-08 13:28:27.000000 auto-eval-0.1.8/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-08 13:28:27.000000 auto-eval-0.1.8/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-05-08 13:28:27.000000 auto-eval-0.1.8/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:28:27.822258 auto-eval-0.1.8/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.1.8/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     7011 2023-05-08 13:00:48.000000 auto-eval-0.1.8/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:28:27.822755 auto-eval-0.1.8/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.8/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3928 2023-05-08 07:55:11.000000 auto-eval-0.1.8/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:28:27.823827 auto-eval-0.1.8/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)       44 2023-05-05 07:40:16.000000 auto-eval-0.1.8/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)      775 2023-05-06 02:34:00.000000 auto-eval-0.1.8/eval/prompt_template/eval_prompt_template.json
--rw-r--r--   0 zhangchong   (501) staff       (20)     3092 2023-05-08 13:10:10.000000 auto-eval-0.1.8/eval/prompt_template/prompter.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:28:27.824425 auto-eval-0.1.8/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.8/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3108 2023-05-08 13:22:30.000000 auto-eval-0.1.8/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-08 13:28:27.825025 auto-eval-0.1.8/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      950 2023-05-08 13:28:24.000000 auto-eval-0.1.8/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-10 10:56:57.588708 auto-eval-0.1.9/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.9/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    13658 2023-05-10 10:56:57.588509 auto-eval-0.1.9/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    13232 2023-05-09 07:43:05.000000 auto-eval-0.1.9/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-10 10:56:57.585940 auto-eval-0.1.9/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    13658 2023-05-10 10:56:57.000000 auto-eval-0.1.9/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      480 2023-05-10 10:56:57.000000 auto-eval-0.1.9/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-10 10:56:57.000000 auto-eval-0.1.9/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-05-10 10:56:57.000000 auto-eval-0.1.9/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-10 10:56:57.000000 auto-eval-0.1.9/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-05-10 10:56:57.000000 auto-eval-0.1.9/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-10 10:56:57.586349 auto-eval-0.1.9/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.1.9/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7022 2023-05-10 10:54:05.000000 auto-eval-0.1.9/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-10 10:56:57.586742 auto-eval-0.1.9/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.9/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3928 2023-05-08 07:55:11.000000 auto-eval-0.1.9/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-10 10:56:57.587553 auto-eval-0.1.9/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       44 2023-05-05 07:40:16.000000 auto-eval-0.1.9/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)      775 2023-05-06 02:34:00.000000 auto-eval-0.1.9/eval/prompt_template/eval_prompt_template.json
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3092 2023-05-08 13:10:10.000000 auto-eval-0.1.9/eval/prompt_template/prompter.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-10 10:56:57.588137 auto-eval-0.1.9/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.9/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3108 2023-05-08 13:22:30.000000 auto-eval-0.1.9/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-10 10:56:57.588756 auto-eval-0.1.9/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      950 2023-05-10 10:54:54.000000 auto-eval-0.1.9/setup.py
```

### Comparing `auto-eval-0.1.8/LICENSE` & `auto-eval-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.8/PKG-INFO` & `auto-eval-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.8
+Version: 0.1.9
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -54,15 +54,15 @@
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 
 ### 2. Usage with command lines
-#### Evaluate one sample
+#### Evaluate single sample
 ```sh
 auto-eval line --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "Janet’s ducks lay 16 eggs per day. She eats three for breakfast every morning and bakes muffins for her friends every day with four. She sells the remainder at the farmers' market daily for $2 per fresh duck egg. How much in dollars does she make every day at the farmers' market?" \
 --answers 20 100 21 18 \
 --target "Janet sells 16 - 3 - 4 = <<16-3-4=9>>9 duck eggs a day. She makes 9 * 2 = $<<9*2=18>>18 every day at the farmer’s market. #### 18"
 ```
@@ -135,18 +135,47 @@
 auto-eval file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --eval_data_path model_a_pred.json model_b_pred.json model_c_pred.json \
 --output_path eval_result_path.xlsx \
 --model gpt-4 
 ```
 
 **Input file format:**<br>
-The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The headers(column names) of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
+
+- The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions.<br>
+
+- To score multiple files for comparison, use the argument `-eval_data_path` followed by the file names separated by spaces. For example: `-eval_data_path file1.json file2.json ... fileN.json`. Files can have different formats as long as they adhere to one of the mentioned formats below.<br>To simplify comparison of scores across various models, it is recommended to add a "model" column that distinguishes between the names of different models and enables easy outputting of statistics on scores from multiple models.
+
+- To view more detailed arguments, Please use the command `auto-eval file -h` after installing this repository or refer to the full documentation below.<br>
+
+- The headers(column names) of the file can be one of the following types: 
+    - `{"instruction", "input", "output"}`
+    -  `{"prompt", "output"}`
+    -  `{"question", "answer"}`
+    -  `{"question", "output"}` <br>
+
+    The "question," "prompt," and "instruction" + "input" refer to the original inquiry, such as "Please calculate carefully: 1+1=?" or "Explain landing on the moon like I am five." The  "answer" and "output" represent the predicted answer of the model for a given question. If the format is in an {"instruction", "input"} form, we will concatenate both elements to create a complete question. <br>
+
+
+To get an idea of what eval input file looks like.
+here is an example of test data in JSON format with model's pseudo prediction.<br>
+```json
+[
+    {"category":"Mathematics","instruction":"'I want to repair a fence for my garden. Help me estimate how much fence length I need to prepare. My garden is 10 meters wide, 5 meters long, and one side is against a wall.'", "input":"","output":"The answer is 15 meters", "model": "model_a"},
+    {"category":"Mathematics","instruction":"Sort this list of numbers in ascending order", "input": "[230, 1, 4, 7000, 20, 300]","output":"[1, 4, 230, 7000, 20, 300]", "model": "model_a"},
+    {"category":"Mathematics","instruction":"Sort this list of numbers in descending order", "input":"[230，1，4，7000，20 ，300]","output":"[7000, 300, 230, 20, 4, 1]", "model": "model_a"}
+]
+```
+
 
 **Output File format:**<br>
-The output file can be specified as a .json, .jsonl, .csv or.xlsx extension. If it contains a field called "model", scores and statistics will be grouped based on this field. If it also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
+
+- The output file can be specified as a .json, .jsonl, .csv or.xlsx extension.<br> 
+- If the input file contains a field called "model", scores and statistics will be grouped based on this field. 
+- If the input file also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. 
+- Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
 
 <details open> <summary>log output example:</summary>
 
 <br>
 prompts and responses detail...
 
 -------------------- Scores by Model --------------------
@@ -219,7 +248,12 @@
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
 
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
+
+
+## ToDo
+- [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
+- [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.1.8/README.md` & `auto-eval-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 
 ### 2. Usage with command lines
-#### Evaluate one sample
+#### Evaluate single sample
 ```sh
 auto-eval line --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "Janet’s ducks lay 16 eggs per day. She eats three for breakfast every morning and bakes muffins for her friends every day with four. She sells the remainder at the farmers' market daily for $2 per fresh duck egg. How much in dollars does she make every day at the farmers' market?" \
 --answers 20 100 21 18 \
 --target "Janet sells 16 - 3 - 4 = <<16-3-4=9>>9 duck eggs a day. She makes 9 * 2 = $<<9*2=18>>18 every day at the farmer’s market. #### 18"
 ```
@@ -123,18 +123,47 @@
 auto-eval file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --eval_data_path model_a_pred.json model_b_pred.json model_c_pred.json \
 --output_path eval_result_path.xlsx \
 --model gpt-4 
 ```
 
 **Input file format:**<br>
-The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The headers(column names) of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
+
+- The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions.<br>
+
+- To score multiple files for comparison, use the argument `-eval_data_path` followed by the file names separated by spaces. For example: `-eval_data_path file1.json file2.json ... fileN.json`. Files can have different formats as long as they adhere to one of the mentioned formats below.<br>To simplify comparison of scores across various models, it is recommended to add a "model" column that distinguishes between the names of different models and enables easy outputting of statistics on scores from multiple models.
+
+- To view more detailed arguments, Please use the command `auto-eval file -h` after installing this repository or refer to the full documentation below.<br>
+
+- The headers(column names) of the file can be one of the following types: 
+    - `{"instruction", "input", "output"}`
+    -  `{"prompt", "output"}`
+    -  `{"question", "answer"}`
+    -  `{"question", "output"}` <br>
+
+    The "question," "prompt," and "instruction" + "input" refer to the original inquiry, such as "Please calculate carefully: 1+1=?" or "Explain landing on the moon like I am five." The  "answer" and "output" represent the predicted answer of the model for a given question. If the format is in an {"instruction", "input"} form, we will concatenate both elements to create a complete question. <br>
+
+
+To get an idea of what eval input file looks like.
+here is an example of test data in JSON format with model's pseudo prediction.<br>
+```json
+[
+    {"category":"Mathematics","instruction":"'I want to repair a fence for my garden. Help me estimate how much fence length I need to prepare. My garden is 10 meters wide, 5 meters long, and one side is against a wall.'", "input":"","output":"The answer is 15 meters", "model": "model_a"},
+    {"category":"Mathematics","instruction":"Sort this list of numbers in ascending order", "input": "[230, 1, 4, 7000, 20, 300]","output":"[1, 4, 230, 7000, 20, 300]", "model": "model_a"},
+    {"category":"Mathematics","instruction":"Sort this list of numbers in descending order", "input":"[230，1，4，7000，20 ，300]","output":"[7000, 300, 230, 20, 4, 1]", "model": "model_a"}
+]
+```
+
 
 **Output File format:**<br>
-The output file can be specified as a .json, .jsonl, .csv or.xlsx extension. If it contains a field called "model", scores and statistics will be grouped based on this field. If it also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
+
+- The output file can be specified as a .json, .jsonl, .csv or.xlsx extension.<br> 
+- If the input file contains a field called "model", scores and statistics will be grouped based on this field. 
+- If the input file also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. 
+- Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
 
 <details open> <summary>log output example:</summary>
 
 <br>
 prompts and responses detail...
 
 -------------------- Scores by Model --------------------
@@ -206,8 +235,13 @@
 
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
 
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
-`--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
+`--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
+
+
+## ToDo
+- [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
+- [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.1.8/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.1.9/auto_eval.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.8
+Version: 0.1.9
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -54,15 +54,15 @@
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 
 ### 2. Usage with command lines
-#### Evaluate one sample
+#### Evaluate single sample
 ```sh
 auto-eval line --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "Janet’s ducks lay 16 eggs per day. She eats three for breakfast every morning and bakes muffins for her friends every day with four. She sells the remainder at the farmers' market daily for $2 per fresh duck egg. How much in dollars does she make every day at the farmers' market?" \
 --answers 20 100 21 18 \
 --target "Janet sells 16 - 3 - 4 = <<16-3-4=9>>9 duck eggs a day. She makes 9 * 2 = $<<9*2=18>>18 every day at the farmer’s market. #### 18"
 ```
@@ -135,18 +135,47 @@
 auto-eval file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --eval_data_path model_a_pred.json model_b_pred.json model_c_pred.json \
 --output_path eval_result_path.xlsx \
 --model gpt-4 
 ```
 
 **Input file format:**<br>
-The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The headers(column names) of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
+
+- The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions.<br>
+
+- To score multiple files for comparison, use the argument `-eval_data_path` followed by the file names separated by spaces. For example: `-eval_data_path file1.json file2.json ... fileN.json`. Files can have different formats as long as they adhere to one of the mentioned formats below.<br>To simplify comparison of scores across various models, it is recommended to add a "model" column that distinguishes between the names of different models and enables easy outputting of statistics on scores from multiple models.
+
+- To view more detailed arguments, Please use the command `auto-eval file -h` after installing this repository or refer to the full documentation below.<br>
+
+- The headers(column names) of the file can be one of the following types: 
+    - `{"instruction", "input", "output"}`
+    -  `{"prompt", "output"}`
+    -  `{"question", "answer"}`
+    -  `{"question", "output"}` <br>
+
+    The "question," "prompt," and "instruction" + "input" refer to the original inquiry, such as "Please calculate carefully: 1+1=?" or "Explain landing on the moon like I am five." The  "answer" and "output" represent the predicted answer of the model for a given question. If the format is in an {"instruction", "input"} form, we will concatenate both elements to create a complete question. <br>
+
+
+To get an idea of what eval input file looks like.
+here is an example of test data in JSON format with model's pseudo prediction.<br>
+```json
+[
+    {"category":"Mathematics","instruction":"'I want to repair a fence for my garden. Help me estimate how much fence length I need to prepare. My garden is 10 meters wide, 5 meters long, and one side is against a wall.'", "input":"","output":"The answer is 15 meters", "model": "model_a"},
+    {"category":"Mathematics","instruction":"Sort this list of numbers in ascending order", "input": "[230, 1, 4, 7000, 20, 300]","output":"[1, 4, 230, 7000, 20, 300]", "model": "model_a"},
+    {"category":"Mathematics","instruction":"Sort this list of numbers in descending order", "input":"[230，1，4，7000，20 ，300]","output":"[7000, 300, 230, 20, 4, 1]", "model": "model_a"}
+]
+```
+
 
 **Output File format:**<br>
-The output file can be specified as a .json, .jsonl, .csv or.xlsx extension. If it contains a field called "model", scores and statistics will be grouped based on this field. If it also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
+
+- The output file can be specified as a .json, .jsonl, .csv or.xlsx extension.<br> 
+- If the input file contains a field called "model", scores and statistics will be grouped based on this field. 
+- If the input file also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. 
+- Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
 
 <details open> <summary>log output example:</summary>
 
 <br>
 prompts and responses detail...
 
 -------------------- Scores by Model --------------------
@@ -219,7 +248,12 @@
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
 
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
+
+
+## ToDo
+- [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
+- [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.1.8/eval/auto_llms_eval.py` & `auto-eval-0.1.9/eval/auto_llms_eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     if 'model' in eval_results_df.keys():
         print( eval_results_df.groupby('model')['score'])
         score_models = eval_results_df.groupby('model')['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}')
         print(f'{"-"*20} Scores by Model {"-"*20}\n{score_models.to_markdown()}')
         if 'category' in eval_results_df.keys():
             score_category = eval_results_df.groupby([
                 'model', 'category'
-            ])['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}').reset_index().sort_values(by='category')
+            ])['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}').reset_index().sort_values(by=['category', 'model'])
             print(
                 f'\n{"-"*20} Scores by Model and Task Category {"-"*20}\n{score_category.to_markdown(index=False)}'
             )
 
 def save_results(eval_results_df: pd.DataFrame, output_path: str):
     print(f'Saving evaluation results: {output_path}')
     df_saver(eval_results_df, output_path)
```

### Comparing `auto-eval-0.1.8/eval/commands/auto_eval.py` & `auto-eval-0.1.9/eval/commands/auto_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.8/eval/prompt_template/eval_prompt_template.json` & `auto-eval-0.1.9/eval/prompt_template/eval_prompt_template.json`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.8/eval/prompt_template/prompter.py` & `auto-eval-0.1.9/eval/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.8/eval/utils/data_utils.py` & `auto-eval-0.1.9/eval/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.8/setup.py` & `auto-eval-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     package_data={
       "eval":["prompt_template/eval_prompt_template.json"]  
     },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

