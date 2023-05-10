# Comparing `tmp/obgraph-0.0.8.tar.gz` & `tmp/obgraph-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obgraph-0.0.8.tar", last modified: Wed Dec 15 22:04:40 2021, max compression
+gzip compressed data, was "obgraph-0.0.9.tar", last modified: Thu Mar 17 13:36:30 2022, max compression
```

## Comparing `obgraph-0.0.8.tar` & `obgraph-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-15 22:04:40.981369 obgraph-0.0.8/
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      255 2021-12-15 22:04:40.981369 obgraph-0.0.8/PKG-INFO
-drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-15 22:04:40.981369 obgraph-0.0.8/obgraph/
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      210 2021-02-09 13:18:00.000000 obgraph-0.0.8/obgraph/__init__.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)    20692 2021-12-06 20:23:58.000000 obgraph-0.0.8/obgraph/command_line_interface.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     1151 2021-04-01 21:43:50.000000 obgraph-0.0.8/obgraph/coordinate_converter.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     7764 2021-10-29 08:25:52.000000 obgraph-0.0.8/obgraph/dummy_node_adder.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)    20195 2021-12-06 20:23:58.000000 obgraph-0.0.8/obgraph/genotype_matrix.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)    38821 2021-11-03 10:18:44.000000 obgraph-0.0.8/obgraph/graph.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     8515 2021-10-29 08:25:52.000000 obgraph-0.0.8/obgraph/graph_construction.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     3194 2021-01-25 11:42:43.000000 obgraph-0.0.8/obgraph/graph_merger.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     3578 2021-12-06 20:23:58.000000 obgraph-0.0.8/obgraph/haplotype_matrix.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)    15681 2021-12-06 20:23:58.000000 obgraph-0.0.8/obgraph/haplotype_nodes.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     4215 2021-01-27 16:16:56.000000 obgraph-0.0.8/obgraph/mutable_graph.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      258 2021-04-23 13:45:15.000000 obgraph-0.0.8/obgraph/neighbour_haplotype_nodes.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     2699 2021-12-15 17:51:26.000000 obgraph-0.0.8/obgraph/numpy_variants.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     2321 2021-01-26 14:14:09.000000 obgraph-0.0.8/obgraph/traversing.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     7920 2021-08-23 20:31:20.000000 obgraph-0.0.8/obgraph/util.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     2887 2021-11-03 14:06:17.000000 obgraph-0.0.8/obgraph/variant_to_nodes.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)    23017 2021-11-30 13:42:10.000000 obgraph-0.0.8/obgraph/variants.py
-drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-15 22:04:40.981369 obgraph-0.0.8/obgraph.egg-info/
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      255 2021-12-15 22:04:40.000000 obgraph-0.0.8/obgraph.egg-info/PKG-INFO
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      667 2021-12-15 22:04:40.000000 obgraph-0.0.8/obgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)        1 2021-12-15 22:04:40.000000 obgraph-0.0.8/obgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       65 2021-12-15 22:04:40.000000 obgraph-0.0.8/obgraph.egg-info/entry_points.txt
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)        1 2020-12-09 14:37:07.000000 obgraph-0.0.8/obgraph.egg-info/not-zip-safe
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       65 2021-12-15 22:04:40.000000 obgraph-0.0.8/obgraph.egg-info/requires.txt
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)        8 2021-12-15 22:04:40.000000 obgraph-0.0.8/obgraph.egg-info/top_level.txt
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       38 2021-12-15 22:04:40.981369 obgraph-0.0.8/setup.cfg
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      682 2021-12-15 22:04:27.000000 obgraph-0.0.8/setup.py
+drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2022-03-17 13:36:30.169914 obgraph-0.0.9/
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      255 2022-03-17 13:36:30.169914 obgraph-0.0.9/PKG-INFO
+drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2022-03-17 13:36:30.169914 obgraph-0.0.9/obgraph/
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      210 2021-02-09 13:18:00.000000 obgraph-0.0.9/obgraph/__init__.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)    20126 2022-03-16 20:43:37.000000 obgraph-0.0.9/obgraph/command_line_interface.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     1151 2021-04-01 21:43:50.000000 obgraph-0.0.9/obgraph/coordinate_converter.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)   894480 2022-03-14 13:02:35.000000 obgraph-0.0.9/obgraph/cython_traversing.c
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     7904 2022-03-04 12:03:25.000000 obgraph-0.0.9/obgraph/dummy_node_adder.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)    20195 2021-12-06 20:23:58.000000 obgraph-0.0.9/obgraph/genotype_matrix.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)    39565 2022-03-17 12:39:19.000000 obgraph-0.0.9/obgraph/graph.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     8956 2022-03-07 12:58:30.000000 obgraph-0.0.9/obgraph/graph_construction.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     2373 2022-03-16 20:31:12.000000 obgraph-0.0.9/obgraph/graph_merger.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     3578 2021-12-06 20:23:58.000000 obgraph-0.0.9/obgraph/haplotype_matrix.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)    15827 2022-03-14 17:23:39.000000 obgraph-0.0.9/obgraph/haplotype_nodes.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     4215 2021-01-27 16:16:56.000000 obgraph-0.0.9/obgraph/mutable_graph.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      258 2021-04-23 13:45:15.000000 obgraph-0.0.9/obgraph/neighbour_haplotype_nodes.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     2699 2021-12-15 17:51:26.000000 obgraph-0.0.9/obgraph/numpy_variants.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      489 2022-01-21 14:08:48.000000 obgraph-0.0.9/obgraph/position_id.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     2321 2022-03-14 10:58:44.000000 obgraph-0.0.9/obgraph/traversing.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     7920 2021-08-23 20:31:20.000000 obgraph-0.0.9/obgraph/util.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     2887 2021-11-03 14:06:17.000000 obgraph-0.0.9/obgraph/variant_to_nodes.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)    23868 2022-03-14 17:09:03.000000 obgraph-0.0.9/obgraph/variants.py
+drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2022-03-17 13:36:30.169914 obgraph-0.0.9/obgraph.egg-info/
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      255 2022-03-17 13:36:30.000000 obgraph-0.0.9/obgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      718 2022-03-17 13:36:30.000000 obgraph-0.0.9/obgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)        1 2022-03-17 13:36:30.000000 obgraph-0.0.9/obgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       65 2022-03-17 13:36:30.000000 obgraph-0.0.9/obgraph.egg-info/entry_points.txt
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)        1 2020-12-09 14:37:07.000000 obgraph-0.0.9/obgraph.egg-info/not-zip-safe
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       80 2022-03-17 13:36:30.000000 obgraph-0.0.9/obgraph.egg-info/requires.txt
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)        8 2022-03-17 13:36:30.000000 obgraph-0.0.9/obgraph.egg-info/top_level.txt
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       38 2022-03-17 13:36:30.169914 obgraph-0.0.9/setup.cfg
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      796 2022-03-17 13:34:23.000000 obgraph-0.0.9/setup.py
```

### Comparing `obgraph-0.0.8/obgraph/command_line_interface.py` & `obgraph-0.0.9/obgraph/command_line_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
 logging.basicConfig(level=logging.INFO, format='%(module)s %(asctime)s %(levelname)s: %(message)s')
+from obgraph.cython_traversing import traverse_graph_by_following_nodes
 import pyximport; pyximport.install()
 import sys
 import argparse
 from . import Graph
 from .util import add_indel_dummy_nodes
 from .variants import VcfVariants
 from .haplotype_nodes import HaplotypeToNodes, NodeToHaplotypes
 from .dummy_node_adder import DummyNodeAdder
 from .haplotype_nodes import NodeToHaplotypes
 from .genotype_matrix import GenotypeMatrix, GenotypeMatrixAnalyser, GenotypeFrequencies
 from pyfaidx import Fasta
 from .graph_construction import GraphConstructor
 from .graph_merger import merge_graphs
 import numpy as np
-from shared_memory_wrapper.shared_memory import from_shared_memory, to_shared_memory, SingleSharedArray, remove_shared_memory_in_session
+from shared_memory_wrapper.shared_memory import from_shared_memory, to_shared_memory, SingleSharedArray, remove_shared_memory_in_session, to_file, from_file
 from multiprocessing import Pool
 import time
 from itertools import repeat
 from graph_kmer_index.flat_kmers import letter_sequence_to_numeric
 
 
 def np_letter_sequence_to_numeric(letter_sequence):
@@ -87,16 +88,17 @@
     graph.set_allele_frequencies_from_variants(variants, use_chromosome=1)  # Use chromosome 1 because we always assume this is a single-chromosome graph
     graph.to_file(args.graph_file_name)
     logging.info("Wrote modified graph to the same file %s" % args.graph_file_name)
 
 
 def make_haplotype_to_nodes(args):
     graph = Graph.from_file(args.graph_file_name)
-    variants = VcfVariants.from_vcf(args.vcf_file_name)
-    haplotype_to_nodes = HaplotypeToNodes.from_graph_and_variants(graph, variants, args.n_haplotypes)
+    variants = VcfVariants.from_vcf(args.vcf_file_name, make_generator=True, skip_index=True)
+    haplotype_to_nodes = HaplotypeToNodes.from_graph_and_variants(graph, variants, args.n_haplotypes, n_threads=args.n_threads)
+    #haplotype_to_nodes = haplotype_to_nodes.get_new_by_traversing_graph(graph, args.n_haplotypes)
     logging.info("Saving to file")
     haplotype_to_nodes.to_file(args.out_file_name)
     logging.info("Wrote to file %s" % args.out_file_name)
 
 
 def main():
     run_argument_parser(sys.argv[1:])
@@ -130,14 +132,15 @@
     subparser.set_defaults(func=add_allele_frequencies)
 
     subparser = subparsers.add_parser("make_haplotype_to_nodes")
     subparser.add_argument("-g", "--graph-file-name", required=True)
     subparser.add_argument("-v", "--vcf-file-name", required=True)
     subparser.add_argument("-n", "--n-haplotypes", type=int, required=True)
     subparser.add_argument("-o", "--out_file_name", required=True)
+    subparser.add_argument("-t", "--n-threads", type=int, default=8, required=False)
     subparser.set_defaults(func=make_haplotype_to_nodes)
 
     def make_node_to_haplotypes_lookup(args):
         haplotype_nodes = HaplotypeNodes.from_file(args.haplotype_nodes)
         n = NodeToHaplotypes.from_haplotype_nodes(haplotype_nodes)
         n.to_file(args.out_file_name)
         logging.info("Saved to %s" % args.out_file_name)
@@ -244,17 +247,19 @@
 
     def traverse(args):
         g = Graph.from_file(args.graph)
         haplotype_to_nodes = HaplotypeToNodes.from_file(args.haplotype_nodes)
         #from .traversing import traverse_graph_by_following_nodes
 
         for haplotype in range(0, args.n_haplotypes):
-            nodes_to_follow = set(haplotype_to_nodes.get_nodes(haplotype))
+
+            nodes_to_follow = np.zeros(len(g.nodes), dtype=np.uint8)
+            nodes_to_follow[haplotype_to_nodes.get_nodes(haplotype)] = 1
             start_time = time.time()
-            new_nodes = cython_traversing.traverse_graph_by_following_nodes(g, nodes_to_follow)
+            new_nodes = traverse_graph_by_following_nodes(g, nodes_to_follow)
             logging.info("Got %d nodes" % len(new_nodes))
             end_time = time.time()
             logging.info("Time spent on haplotype %d: %.5f" % (haplotype, end_time - start_time))
 
     subparser = subparsers.add_parser("traverse")
     subparser.add_argument("-g", "--graph", required=True)
     subparser.add_argument("-T", "--type", required=False, default="correct_haplotype_nodes")
@@ -342,41 +347,14 @@
         node_to_variants.to_file(args.out_file_name)
 
     subparser = subparsers.add_parser("make_node_to_variants")
     subparser.add_argument("-v", "--variant_to_nodes", required=True)
     subparser.add_argument("-o", "--out_file_name", required=True)
     subparser.set_defaults(func=make_node_to_variants)
 
-    def set_numeric_node_sequences(args):
-        graph = Graph.from_file(args.graph)
-        to_shared_memory(graph, "graph_shared")
-        pool = Pool(args.n_threads)
-
-        numeric_node_sequences = SingleSharedArray(np.zeros(len(graph.node_sequences), dtype=np.uint8))
-        to_shared_memory(numeric_node_sequences, "numeric_node_sequences")
-
-
-        intervals = list([int(i) for i in np.linspace(0, len(graph.node_sequences), args.n_threads+1)])
-        intervals = [(from_pos, to_pos) for from_pos, to_pos in zip(intervals[0:-1], intervals[1:])]
-        logging.info("Intervals: %s" % intervals)
-
-        for from_pos, to_pos in pool.imap(get_numeric_node_sequence_single_thread, intervals):
-            logging.info("Done processing interval %d-%d. Inserting into full array" % (from_pos, to_pos))
-
-        logging.info("Done with all intervals. Saving new graph")
-        numeric_node_sequences = from_shared_memory(SingleSharedArray, "numeric_node_sequences")
-        graph.numeric_node_sequences = numeric_node_sequences.array
-        graph.to_file(args.graph)
-        logging.info("Saved to the same file %s" % args.graph)
-
-    subparser = subparsers.add_parser("set_numeric_node_sequences")
-    subparser.add_argument("-g", "--graph", required=True)
-    subparser.add_argument("-t", "--n-threads", required=False, default=10, type=int)
-    subparser.set_defaults(func=set_numeric_node_sequences)
-
     def create_coordinate_converter(args):
         from .coordinate_converter import CoordinateConverter
         converter = CoordinateConverter.from_graph(Graph.from_file(args.graph))
         converter.to_file(args.out_file_name)
         logging.info("Wrote to file %s" % args.out_file_name)
 
     subparser = subparsers.add_parser("create_coordinate_converter")
@@ -405,14 +383,27 @@
 
     subparser = subparsers.add_parser("make_numpy_variants")
     subparser.add_argument("-v", "--vcf", required=True)
     subparser.add_argument("-o", "--out-file-name", required=True)
     subparser.set_defaults(func=make_numpy_variants)
 
 
+    def make_position_id(args):
+        from .position_id import PositionId
+        graph = Graph.from_file(args.graph)
+        position_id = PositionId.from_graph(graph)
+        to_file(position_id, args.out_file_name)
+
+
+    subparser = subparsers.add_parser("make_position_id")
+    subparser.add_argument("-g", "--graph", required=True)
+    subparser.add_argument("-o", "--out-file-name", required=True)
+    subparser.set_defaults(func=make_position_id)
+
+
     if len(args) == 0:
         parser.print_help()
         sys.exit(1)
 
     args = parser.parse_args(args)
     args.func(args)
     remove_shared_memory_in_session()
```

### Comparing `obgraph-0.0.8/obgraph/coordinate_converter.py` & `obgraph-0.0.9/obgraph/coordinate_converter.py`

 * *Files identical despite different names*

### Comparing `obgraph-0.0.8/obgraph/dummy_node_adder.py` & `obgraph-0.0.9/obgraph/dummy_node_adder.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             self.mutable_graph = use_mutable_graph
 
         logging.info("Adding dummy nodes")
         for i, variant in enumerate(self.variants):
             if i % 10000 == 0:
                 logging.info("%d variants processed" % i)
 
-            if variant.type == "SNP":
+            if variant.type == "SNP" or variant.type == "SUBSTITUTION":
                 continue
 
             try:
                 self._add_dummy_edges_around_indel(variant)
             except VariantNotFoundException as e:
                 logging.error("Could not find variant: %s" % str(e))
                 self._n_variants_failed += 1
@@ -53,14 +53,16 @@
         return inserted_nodes
 
     def _add_dummy_edges_around_indel(self, variant):
         if variant.type == "DELETION":
             inserted_sequence = variant.ref_sequence[1:]
         elif variant.type == "INSERTION":
             inserted_sequence = variant.variant_sequence[1:]
+        elif variant.type == "SUBSTITUTION":
+            inserted_sequence = variant.variant_sequence[1:]
         else:
             raise Exception("Unsupported variant")
 
         _, possible_inserted_node_paths = self.get_nodes_for_inserted_sequence_at_ref_pos(inserted_sequence, variant.position, variant.type)
 
         #logging.info("===========")
         #logging.info("Variant %s. Inserted nodes: %s" % (variant, possible_inserted_node_paths))
```

### Comparing `obgraph-0.0.8/obgraph/genotype_matrix.py` & `obgraph-0.0.9/obgraph/genotype_matrix.py`

 * *Files identical despite different names*

### Comparing `obgraph-0.0.8/obgraph/graph.py` & `obgraph-0.0.9/obgraph/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,33 +2,49 @@
 import json
 import logging
 import re
 import numpy as np
 from .variants import VcfVariants
 from collections import defaultdict
 from .mutable_graph import MutableGraph
+from dataclasses import dataclass
+from npstructures import RaggedArray, HashTable
+from shared_memory_wrapper import to_file, from_file
+from graph_kmer_index.nplist import NpList
+
 
 class VariantNotFoundException(Exception):
     pass
 
-class Graph:
-    properties = {
-        "nodes", "node_to_sequence_index", "node_sequences", "node_to_edge_index", "node_to_n_edges", "edges",
-        "node_to_ref_offset", "ref_offset_to_node", "chromosome_start_nodes", "linear_ref_nodes_index", "allele_frequencies", "numeric_node_sequences"
-    }
+def remap_array(array, from_values, to_values):
+    index = np.digitize(array.ravel(), from_values, right=True)
+    return to_values[index].reshape(array.shape)
+
+
+def convert_sequence_array_to_numeric(sequence):
+    assert type(sequence) == np.ndarray
+    sequences_as_byte_values = sequence.astype("|S1").view(np.int8)
+    # from byte values
+    from_values = np.array([65, 67, 71, 84, 97, 99, 103, 116], dtype=np.uint64)  # NB: Must be increasing
+    # to internal base values for a, c, t, g
+    to_values = np.array([0, 1, 3, 2, 0, 1, 3, 2], dtype=np.uint64)
+    return remap_array(sequences_as_byte_values, from_values, to_values).astype(np.uint8)
+
+numeric_to_letter_sequence = np.array(["A", "C", "T", "G"])
 
-    def __init__(self, nodes=None, node_to_sequence_index=None, node_sequences=None, node_to_edge_index=None, node_to_n_edges=None, edges=None,
+class Graph:
+    def __init__(self, nodes,
+                 sequences: RaggedArray,
+                 edges: RaggedArray,
                  node_to_ref_offset=None, ref_offset_to_node=None, chromosome_start_nodes=None, allele_frequencies=None, linear_ref_nodes_index=None,
                  numeric_node_sequences=None, linear_ref_nodes_and_dummy_nodes_index=None):
         self.nodes = nodes
-        self.node_to_sequence_index = node_to_sequence_index
-        self.node_sequences = node_sequences
-        self.node_to_edge_index = node_to_edge_index
-        self.node_to_n_edges = node_to_n_edges
         self.edges = edges
+        self.sequences = sequences
+
         self.node_to_ref_offset = node_to_ref_offset
         self.ref_offset_to_node = ref_offset_to_node
         self._linear_ref_nodes_cache = None
         self.chromosome_start_nodes = chromosome_start_nodes
         self.allele_frequencies = allele_frequencies
         self.numeric_node_sequences = numeric_node_sequences
 
@@ -54,22 +70,27 @@
 
         for edge in edges:
             if edge not in edges:
                 return False
 
         return True
 
+    def set_numeric_node_sequences(self):
+        raise Exception("Unsupported")
+
     def get_all_nodes(self):
-        return np.union1d(np.where(self.nodes != 0)[0], np.where(self.node_to_n_edges > 0)[0])
+        node_to_n_edges = self.edges.shape.lengths   # a bit hacky, accessing length of RaggedShape in npstructures
+        return np.union1d(np.where(self.nodes != 0)[0], np.where(node_to_n_edges > 0)[0])
         # This does not return nodes of size 0
         #return np.where(self.nodes != 0)[0]
 
     def __str__(self):
-        mutable_graph = self.to_mutable_graph()
-        return str(mutable_graph)
+        #mutable_graph = self.to_mutable_graph()
+        #return str(mutable_graph)
+        return "Obgraph"
 
     def __repr__(self):
         return self.__str__()
 
     def to_mutable_graph(self):
         all_nodes = self.get_all_nodes()
         nodes = {node: self.get_node_size(node) for node in all_nodes}
@@ -80,69 +101,60 @@
     @classmethod
     def from_mutable_graph(cls, mutable_graph):
         return cls.from_dicts(mutable_graph.node_sequences, mutable_graph.edges, mutable_graph.linear_ref_nodes)
 
     def get_node_size(self, node):
         return self.nodes[node]
 
+    def get_node_allele_frequencies(self, nodes):
+        if self.allele_frequencies is None:
+            return np.ones(len(nodes))
+        return self.allele_frequencies[nodes]
+
     def get_node_allele_frequency(self, node):
         if self.allele_frequencies is None:
             return 1.0
         return self.allele_frequencies[node]
 
     def get_node_subsequence(self, node, start, end):
-        index_position = self.node_to_sequence_index[node]
-        return ''.join(self.node_sequences[int(index_position+start):int(index_position+end)])
+        return self.get_node_sequence(node)[int(start):int(end)]
 
     def get_node_sequence(self, node):
-        index_position = self.node_to_sequence_index[node]
-        return ''.join(self.node_sequences[index_position:index_position+self.nodes[node]])
-
-    def get_nodes_sequence_index_positions(self, nodes):
-        # First find the number of indexes we ned
-        sequence_length = np.sum(self.nodes[nodes])
-        indexes = np.zeros(sequence_length, dtype=np.uint64)
-        i = 0
-        for node in nodes:
-            node_size = self.nodes[node]
-            index_position = self.node_to_sequence_index[node]
-            indexes[i:i+node_size] = np.arange(index_position, index_position+node_size)
-            i += self.nodes[node]
-
-        return indexes
+        return ''.join(numeric_to_letter_sequence[self.sequences[node]])
 
     def max_node_id(self):
         return len(self.nodes)-1
 
-    def get_numeric_node_sequences(self, nodes):
-        logging.info("Getting sequence length")
-        sequence_length = np.sum(self.nodes[nodes])
-        numeric_sequence = np.zeros(sequence_length, dtype=np.uint8)
+    def get_numeric_node_sequence(self, node):
+        return self.sequences[node]
 
-        i = 0
-        for node in nodes:
-            node_size = self.nodes[node]
-            index_position = self.node_to_sequence_index[node]
-            numeric_sequence[i:i + node_size] = self.numeric_node_sequences[index_position:index_position+node_size]
-            i += self.nodes[node]
+        if self.get_node_size(node) == 0:
+            return np.array([-1])
+
+        index_pos = self.node_to_sequence_index[node]
+        return self.numeric_node_sequences[index_pos:index_pos+self.get_node_size(node)]
 
-        return numeric_sequence
+    def get_numeric_base_sequence(self, node, offset):
+        if self.get_node_size(node) == 0:
+            return -1
+
+        return self.get_numeric_node_sequence(int(node))[int(offset)]
+
+    def get_numeric_node_sequences(self, nodes):
+        return self.sequences[nodes].ravel()
 
     def get_nodes_sequences2(self, nodes):
-        return ''.join(self.node_sequences[self.get_nodes_sequence_index_positions(nodes)])
+        raise NotImplementedError("Use get_nodes_sequences instead")
 
     def get_nodes_sequence(self, nodes):
         sequences = []
 
         for node in nodes:
-            index_position = self.node_to_sequence_index[node]
-            sequences.extend(self.node_sequences[index_position:index_position+self.nodes[node]])
+            sequences.extend(self.get_node_sequence(node))
 
-        #for node in nodes:
-        #    sequences.append(self.get_node_sequence(node))
         return ''.join(sequences)
 
     def get_node_offset_at_chromosome_and_chromosome_offset(self, chromosome, offset):
         chromosome_position = chromosome - 1
         chromosome_start_node = self.chromosome_start_nodes[chromosome_position]
         chromosome_offset = self.get_ref_offset_at_node(chromosome_start_node)
         real_offset = int(chromosome_offset + offset)
@@ -161,24 +173,18 @@
 
         # Shift offset with chromosome start offset
         chromosome_offset = self.get_ref_offset_at_node(chromosome_start_node)
         real_offset = int(chromosome_offset + offset)
         return self.get_node_at_ref_offset(real_offset)
 
     def get_edges(self, node):
-        if node >= len(self.node_to_edge_index):
+        if node >= len(self.edges):
             return []
 
-        index = self.node_to_edge_index[node]
-        n_edges = self.node_to_n_edges[node]
-
-        if n_edges == 0:
-            return []
-
-        return self.edges[index:index+n_edges]
+        return self.edges[node]
 
     def linear_ref_nodes(self):
         if self._linear_ref_nodes_cache is not None:
             return self._linear_ref_nodes_cache
         else:
             nodes = set(np.unique(self.ref_offset_to_node))
             self._linear_ref_nodes_cache = nodes
@@ -232,78 +238,19 @@
 
     def get_node_offset_at_ref_offset(self, ref_offset):
         node = self.get_node_at_ref_offset(ref_offset)
         offset_at_node = self.get_ref_offset_at_node(node)
         return ref_offset - offset_at_node
 
     def to_file(self, file_name):
-        allele_frequencies = self.allele_frequencies
-        if allele_frequencies is None:
-            allele_frequencies = np.zeros(0)
-
-        numeric_node_sequences = self.numeric_node_sequences
-        if numeric_node_sequences is None:
-            numeric_node_sequences = np.zeros(0)
-
-        np.savez(file_name,
-                 nodes=self.nodes,
-                 node_to_sequence_index=self.node_to_sequence_index,
-                 node_sequences=self.node_sequences,
-                 node_to_edge_index=self.node_to_edge_index,
-                 node_to_n_edges=self.node_to_n_edges,
-                 edges=self.edges,
-                 node_to_ref_offset=self.node_to_ref_offset,
-                 ref_offset_to_node=self.ref_offset_to_node,
-                 chromosome_start_nodes=self.chromosome_start_nodes,
-                 allele_frequencies=allele_frequencies,
-                 linear_ref_nodes_index=self.linear_ref_nodes_index,
-                 numeric_node_sequences=numeric_node_sequences,
-                 linear_ref_nodes_and_dummy_nodes_index=self.linear_ref_nodes_and_dummy_nodes_index
-                 )
-
-        logging.info("Saved to file %s" % file_name)
+        return to_file(self, file_name)
 
     @classmethod
     def from_file(cls, file_name):
-        logging.info("Reading file from %s" % file_name)
-        try:
-            data = np.load(file_name)
-        except FileNotFoundError:
-            data = np.load(file_name + ".npz")
-
-        allele_frequencies = None
-        if "allele_frequencies" in data:
-            allele_frequencies = data["allele_frequencies"]
-
-        linear_ref_nodes_index = None
-        if "linear_ref_nodes_index" in data:
-            linear_ref_nodes_index = data["linear_ref_nodes_index"]
-
-        linear_ref_nodes_and_dummy_nodes_index = None
-        if "linear_ref_nodes_and_dummy_nodes_index" in data:
-            linear_ref_nodes_and_dummy_nodes_index = data["linear_ref_nodes_and_dummy_nodes_index"]
-
-        numeric_node_sequences = None
-        if "numeric_node_sequences" in data:
-            numeric_node_sequences = data["numeric_node_sequences"]
-
-        return cls(data["nodes"],
-                   data["node_to_sequence_index"],
-                   data["node_sequences"],
-                   data["node_to_edge_index"],
-                   data["node_to_n_edges"],
-                   data["edges"],
-                   data["node_to_ref_offset"],
-                   data["ref_offset_to_node"],
-                   data["chromosome_start_nodes"],
-                   allele_frequencies,
-                   linear_ref_nodes_index,
-                   numeric_node_sequences,
-                   linear_ref_nodes_and_dummy_nodes_index)
-
+        return from_file(file_name)
 
     def get_flat_graph(self):
         node_ids = list(np.where(self.nodes > 0)[0])
         node_sizes = list(self.nodes[node_ids])
         node_sequences = []
         for node in node_ids:
             node_sequences.append(list(self.get_node_sequence(node)))
@@ -318,87 +265,121 @@
 
         return node_ids, node_sequences, node_sizes, from_nodes, to_nodes, linear_ref_nodes, self.chromosome_start_nodes
 
     @classmethod
     def from_dicts(cls, node_sequences, edges, linear_ref_nodes):
         assert linear_ref_nodes is not None
         logging.info("Making graph from dicts")
-        nodes = list(node_sequences.keys())
+        nodes = np.sort(list(node_sequences.keys())).astype(np.uint32)
+        node_ids = nodes
+        max_node = nodes[-1]
+        logging.info("Max node id is %d" % max_node)
+
         logging.info("Making sequences")
-        node_sequences = [list(node_sequences[node]) for node in nodes]
+        node_sequences = np.array([node_sequences[node] for node in nodes])
         node_sizes = [len(seq) for seq in node_sequences]
-        from_nodes = []
+        node_sizes_array = np.zeros(nodes[-1]+1, dtype=np.uint32)
+        node_sizes_array[nodes] = node_sizes
+        nodes = node_sizes_array
+        logging.info("Node sizes array: %s" % node_sizes_array)
+
+        #from_nodes = []
+
         to_nodes = []
-        i = 0
-        for from_node, to_nodes_edges in edges.items():
-            if i % 100000 == 0:
-                logging.info("%d nodes processed" % i)
-            for to_node in to_nodes_edges:
-                from_nodes.append(from_node)
-                to_nodes.append(to_node)
+        n_edges = []
 
-            i += 1
+        to_nodes = np.concatenate([edges[n] for n in range(max_node+1) if n in edges]).astype(np.uint32)
+        n_edges = np.array([len(edges[n]) if n in edges else 0 for n in range(max_node+1)], dtype=np.uint8)
 
         to_nodes_set = set(to_nodes)
         logging.info("Done preparing data from dicts")
         logging.info("There are %d node sequences" % len(node_sequences))
-        return Graph.from_flat_nodes_and_edges(nodes, node_sequences, node_sizes, np.array(from_nodes), np.array(to_nodes), np.array(linear_ref_nodes), [node for node in nodes if node not in to_nodes_set])
+
+        # sequences
+        sequence = np.array(list(''.join(node_sequences)))
+        numeric_sequence = convert_sequence_array_to_numeric(sequence)
+        sequences = RaggedArray(numeric_sequence, nodes, dtype=np.uint8)
+
+        # linear ref index
+        node_to_ref_offset = np.zeros(max_node + 1, np.uint64)
+        ref_node_sizes = nodes[linear_ref_nodes]
+
+        # print("Ref node sizes: %s"  % ref_node_sizes)
+        ref_offsets = np.cumsum(ref_node_sizes)
+        node_to_ref_offset[linear_ref_nodes[1:]] = ref_offsets[:-1]
+
+
+        # Find last node to add to linear ref size
+        last_node_in_graph = np.argmax(node_to_ref_offset)
+        last_node_size = nodes[last_node_in_graph]
+        logging.info("Last node in graph is %d with size %d" % (last_node_in_graph, last_node_size))
+
+        ref_offset_to_node = np.zeros(int(np.max(node_to_ref_offset)) + last_node_size)
+        index_positions = np.cumsum(ref_node_sizes)[:-1]
+        # logging.info("INdex positions: %s" % index_positions)
+        # logging.info("Linear ref nodes: %s" % linear_ref_nodes)
+        # logging.info("Diff linear ref nodes: %s" % np.diff(linear_ref_nodes))
+        ref_offset_to_node[index_positions] = np.diff(linear_ref_nodes)
+        ref_offset_to_node[0] = linear_ref_nodes[0]
+        # logging.info("Ref offset to node 1: %s" % ref_offset_to_node)
+        ref_offset_to_node = np.cumsum(ref_offset_to_node, dtype=np.uint32)
+
+        chromosome_start_nodes = [node for node in node_ids if node not in to_nodes_set]
+        logging.info("Chromosome start nodes are %s" % chromosome_start_nodes)
+        print("Ref offset to node: %s" % ref_offset_to_node)
+
+        return Graph(node_sizes_array, sequences, RaggedArray(to_nodes, n_edges, dtype=np.uint32), node_to_ref_offset, ref_offset_to_node, chromosome_start_nodes)
+        #return Graph.from_flat_nodes_and_edges(nodes, node_sequences, node_sizes, to_nodes, n_edges, np.array(linear_ref_nodes))
 
     @classmethod
-    def from_flat_nodes_and_edges(cls, node_ids, node_sequences, node_sizes, from_nodes, to_nodes, linear_ref_nodes, chromosome_start_nodes):
-        logging.info("Chromosome start nodes are: %s" % chromosome_start_nodes)
+    def from_flat_nodes_and_edges(cls, node_ids, node_sequences, node_sizes, to_nodes, n_edges, linear_ref_nodes, chromosome_start_nodes):
+        raise Exception("This method has been removed.")
 
-        """
-        logging.info("Asserting linear ref nodes are not empty")
-        for i, node in enumerate(node_ids):
-            size = node_sizes[i]
-            if size == 0 and node in linear_ref_nodes:
-                raise Exception("Placeholder nodes (for insertions) cannot be marked as linear ref nodes, since that breaks ref position to node lookup. Best solution is to not put these in linear ref nodes")
-        """
+        logging.info("Chromosome start nodes are: %s" % chromosome_start_nodes)
 
+        #assert node_ids[0] == 1, "Nodes must start with id 1. First id now is %d" % node_ids[0]
 
         max_node = np.max(node_ids)
         nodes = np.zeros(max_node+1, dtype=np.uint32)
         nodes[node_ids] = node_sizes
 
         # Node sequences
+        node_sorting = np.argsort(node_ids)
+
+        sequences_sorted = node_sequences[node_sorting]
         logging.info("Making node sequences")
-        new_node_positions = np.cumsum(node_sizes)
-        node_sequence_index = np.zeros(max_node+1, dtype=np.uint64)
-        node_sequence_index[node_ids[0]] = 0
-        node_sequence_index[node_ids[1:]] = new_node_positions[:-1]
-        logging.info("Merging sequences into one string, chaining them first")
-        node_sequences = list(itertools.chain.from_iterable(node_sequences))
-        logging.info("Total length of graph sequences: %d" % len(node_sequences))
-        logging.info("Done chaining sequences")
-        node_sequences_array = np.array(node_sequences).astype("<U1")
-        logging.info("Done merging sequences")
-
-
-        #node_sequences_array = np.zeros(max_node+0, dtype=object)
-        #logging.info("Allocating empty sequence array for node sequences")
-        #node_sequences_array = np.array([np.zeros(size, dtype="<U1") for size in nodes])  # Must allocate space
-        #node_sequences_array[node_ids] = node_sequences
+        sequence = np.array(list(''.join(sequences_sorted)))
+        numeric_sequence = convert_sequence_array_to_numeric(sequence)
+        sequences = RaggedArray(numeric_sequence, nodes, dtype=np.uint8)
+
+
+
+
 
         logging.info("Sorting nodes")
-        sorting = np.argsort(from_nodes)
-        from_nodes = from_nodes[sorting]
-        to_nodes = to_nodes[sorting]
+        #sorting = np.argsort(from_nodes)
+        #from_nodes = from_nodes[sorting]
+        #to_nodes = to_nodes[sorting]
+
+        edges = RaggedArray(to_nodes, n_edges, dtype=np.uint32)
+        print(edges)
 
+        """
         logging.info("Making node index")
         diffs = np.ediff1d(from_nodes, to_begin=1)
         positions_of_unique_nodes = np.nonzero(diffs)[0]
         unique_nodes = from_nodes[positions_of_unique_nodes]
 
         logging.info("Making node to edge index")
         node_to_edge_index = np.zeros(max_node+1, dtype=np.uint32)
         node_to_n_edges = np.zeros(max_node+1, dtype=np.uint8)
         node_to_edge_index[unique_nodes] = positions_of_unique_nodes
         n_edges_numbers = np.ediff1d(positions_of_unique_nodes, to_end=len(from_nodes)-positions_of_unique_nodes[-1])
         node_to_n_edges[unique_nodes] = n_edges_numbers
+        """
 
         #logging.info("Finding ref offsets")
         node_to_ref_offset = np.zeros(max_node+1, np.uint64)
         try:
             ref_node_sizes = nodes[linear_ref_nodes]
         except IndexError:
             logging.error("Problem with linear ref nodes, which are %s" % linear_ref_nodes)
@@ -420,16 +401,15 @@
         #logging.info("Linear ref nodes: %s" % linear_ref_nodes)
         #logging.info("Diff linear ref nodes: %s" % np.diff(linear_ref_nodes))
         ref_offset_to_node[index_positions] = np.diff(linear_ref_nodes)
         ref_offset_to_node[0] = linear_ref_nodes[0]
         #logging.info("Ref offset to node 1: %s" % ref_offset_to_node)
         ref_offset_to_node = np.cumsum(ref_offset_to_node, dtype=np.uint32)
 
-        return cls(nodes, node_sequence_index, node_sequences_array, node_to_edge_index,
-                   node_to_n_edges, to_nodes, node_to_ref_offset, ref_offset_to_node, chromosome_start_nodes)
+        return cls(nodes, sequences, edges, node_to_ref_offset, ref_offset_to_node, chromosome_start_nodes)
 
     @classmethod
     def from_vg_json_files(cls, file_names):
 
         node_sequences = []
         node_ids = []
         node_sizes = []
@@ -487,36 +467,65 @@
         linear_ref_nodes = np.array(linear_ref_nodes, dtype=np.uint32)
         chromosome_start_nodes = np.array(chromosome_start_nodes, dtype=np.uint32)
         logging.info("Chromosome start nodes are: %s" % chromosome_start_nodes)
 
         return cls.from_flat_nodes_and_edges(node_ids, node_sequences, node_sizes, edges_from, edges_to, linear_ref_nodes, chromosome_start_nodes)
 
 
-    def get_snp_nodes(self, ref_offset, variant_bases, chromosome=1):
+    def get_snp_nodes(self, ref_offset, reference_bases, variant_bases, chromosome=1):
         node = self.get_node_at_chromosome_and_chromosome_offset(chromosome, ref_offset)
         node_offset = self.get_node_offset_at_chromosome_and_chromosome_offset(chromosome, ref_offset)
-        assert node_offset == 0, "Node offset is 0 at ref_offset %d. Variant bases: %s. Chromosome %d" % (ref_offset, variant_bases, chromosome)
+        assert node_offset == 0, "Node offset is %d at ref_offset %d. Variant bases: %s. Chromosome %d" % (node_offset, ref_offset, variant_bases, chromosome)
         prev_node = self.get_node_at_chromosome_and_chromosome_offset(chromosome, ref_offset - 1)
 
         _, possible_snp_nodes = self.find_nodes_from_node_that_matches_sequence(prev_node, variant_bases, [], [])
         assert len(possible_snp_nodes) > 0, "Did not find any possible snp nodes for variant at ref offset %s with variant sequence %s" % (ref_offset, variant_bases)
 
+        next_ref_pos = ref_offset + len(reference_bases)
+        next_ref_node = self.get_node_at_chromosome_and_chromosome_offset(chromosome, next_ref_pos)
+
+        # attempt at simpler approach. Should only be one non-linear-ref-node that matches sequence?
+        """
+        possible_snp_nodes = [n[-1] for n in possible_snp_nodes if not self.is_linear_ref_node_or_linear_ref_dummy_node(n[-1])]
+        # only keep nodes 
+
+        if len(possible_snp_nodes) != 1:
+            logging.info("Multiple or no nodes (%s) nodes with sequence %s from node %d" % (possible_snp_nodes, variant_bases, prev_node))
+            logging.info(str([(node, self.get_node_sequence(node)) for node in possible_snp_nodes]))
+            logging.info("ref node is %d" % node)
+            logging.info("Ref offset is %d" % ref_offset)
+            raise Exception("Error")
+
+        return node, possible_snp_nodes[0]
+        """
+
         for possible_snp_node in possible_snp_nodes:
             # Not true if deletion before snp
             #assert len(possible_snp_node) == 1, "SNP nodes should only be one node"
             assert len([n for n in possible_snp_node if self.get_node_size(n) > 0]) == 1, "There should only be one non-empty SNP node"
             potential_next = possible_snp_node[-1]  # Get last node, this will be the snp node if there are more nodes
             assert self.get_node_size(potential_next) > 0
             # Also require that this node shares next node with our ref snp node, if not this could be a false match against an indel node
+            # this assumption does not work for subsitutions
+            # why does this not work for substitutions??
             next_from_snp_node = self.get_edges(node)
             if len([n for n in next_from_snp_node if n in self.get_edges(potential_next)]) > 0:
                 return node, potential_next
 
-        logging.error("Could not parse substitution at offset %d with bases %s" % (ref_offset, variant_bases))
-        logging.error("Next nodes from snp node: %d" % next_from_snp_node)
+            # logging.info("Node after deletion: %d" % next_ref_node)
+            if self.get_node_offset_at_chromosome_and_chromosome_offset(chromosome, next_ref_pos) != 0:
+                raise Exception("Could not find next ref node")
+
+            #logging.info("Next ref node: %d. Edges from potential: %s" % (next_ref_node, str(self.get_edges(potential_next))))
+            if next_ref_node in self.get_edges(potential_next):
+                return node, potential_next
+
+        logging.error("Could not parse substitution at offset %d with bases %s. Next ref pos is %d. Next ref node is %d" % (ref_offset, variant_bases, next_ref_pos, next_ref_node))
+        logging.info("Reference node for snp/subsitution is %d" % node)
+        logging.error("Possible nodes are: %s" % possible_snp_nodes)
         raise Exception("Parseerrror")
 
     def get_deletion_nodes(self, ref_offset, deletion_length, deleted_sequence, chromosome=1):
         ref_offset += 1
         # Node is the reference node that is deleted (the first one if there are multiple)
         node = self.get_node_at_chromosome_and_chromosome_offset(chromosome, ref_offset)
         node_offset = self.get_node_offset_at_chromosome_and_chromosome_offset(chromosome, ref_offset)
@@ -630,15 +639,17 @@
         insertion_node = dummy_nodes[0]
         assert next_ref_node in self.get_edges(insertion_node), "Failed parsing insertion %s. Found %d as next ref node after dummy node, but there is no edge from dumy node %d to %d" % (variant, next_ref_node, insertion_node, next_ref_node)
 
         return (insertion_node, variant_node)
 
     def get_variant_nodes(self, variant):
         if variant.type == "SNP":
-            return self.get_snp_nodes(variant.position-1, variant.variant_sequence, variant.chromosome)
+            return self.get_snp_nodes(variant.position-1, variant.get_reference_sequence(), variant.variant_sequence, variant.chromosome)
+        elif variant.type == "SUBSTITUTION":
+            return self.get_snp_nodes(variant.position, variant.get_reference_sequence(), variant.get_variant_sequence(), variant.chromosome)
         elif variant.type == "DELETION":
             return self.get_deletion_nodes(variant.position-1, len(variant.ref_sequence)-1, variant.get_deleted_sequence(), variant.chromosome)
         elif variant.type == "INSERTION":
             return self.get_insertion_nodes(variant, variant.chromosome)
 
         raise Exception("Invalid variant %s. Has no type set." % variant)
 
@@ -664,14 +675,17 @@
         self.allele_frequencies = frequencies
 
     def get_variant_nodes_in_region(self, chromosome, linear_ref_start, linear_ref_end):
         nodes = set(self.get_node_at_chromosome_and_chromosome_offset(chromosome, pos) for pos in range(linear_ref_start, linear_ref_end))
         return [self.get_edges(node) for node in nodes if len(self.get_edges(node)) == 2]
 
     def get_first_node(self):
+        # chromosome start nodes should always be set
+        #return self.chromosome_start_nodes[0]
+
         for candidate in [0, 1]:
             if len(self.get_edges(candidate)) > 0:
                 return candidate
 
         raise Exception("Couldn't find first graph node")
 
     def get_haplotype_node_paths_for_haplotypes(self, variants, limit_to_n_haplotypes=10):
@@ -720,14 +734,25 @@
                 current_node = next_node
                 i += 1
 
             nodes[haplotype, i] = current_node
 
         return nodes
 
+    def get_reverse_edges_hashtable(self):
+        from_nodes = NpList(dtype=np.uint32)
+        to_nodes = NpList(dtype=np.uint32)
+
+        for node in self.get_all_nodes():
+            for edge in self.get_edges(node):
+                from_nodes.append(edge)
+                to_nodes.append(node)
+
+        return HashTable(from_nodes.get_nparray(), to_nodes.get_nparray())
+
     def get_reverse_edges_dict(self):
         reverse_edges = defaultdict(list)
         for node in self.get_all_nodes():
             for edge in self.get_edges(node):
                 reverse_edges[edge].append(node)
 
         return reverse_edges
```

### Comparing `obgraph-0.0.8/obgraph/graph_construction.py` & `obgraph-0.0.9/obgraph/graph_construction.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import logging
 from collections import defaultdict
 from .mutable_graph import MutableGraph
 from .graph import Graph
 from .dummy_node_adder import DummyNodeAdder
 import numpy as np
 
+class EmptyNodeException(Exception):
+    pass
+
 class GraphConstructor:
     def __init__(self, reference_sequence, variants: VcfVariants):
         self.reference_sequence = reference_sequence
         self.variants = variants
         self.breakpoints = []
         self.make_sorted_breakpoints()
 
@@ -79,15 +82,18 @@
         for next_ref_pos in self._deletions[ref_pos_before_to_node+1]:
             for node_after_deletion in self._ref_pos_to_node_after[next_ref_pos - 1]:
                 #logging.info("    Adding deletion edge from %d to %d" % (from_node, node_after_deletion))
                 self._make_edge(from_node, node_after_deletion, next_ref_pos-1)
 
 
     def _make_node(self, ref_position_before_node, ref_position_after_node, sequence, is_ref_node=False, is_deletion=False):
-        assert sequence != "", "Empty sequence for node"
+        if sequence == "":
+            logging.error("Ref pos before node: %d" % ref_position_before_node)
+            raise EmptyNodeException("Empty sequence for node")
+
         #size = len(sequence)
         #self._node_ids.append(self._current_node_id)
         #self._node_sequences.append(np.array(list(sequence)))
         #self._node_sizes.append(size)
 
         #if is_ref_node and len(sequence) > 0:  # We never want empty dummy nodes as reference node (by definition)
         #    self._reference_nodes.append(self._current_node_id)
@@ -115,15 +121,21 @@
                 logging.info("%d/%d breakpoints processed" % (i, len(self.breakpoints)))
 
             #logging.info("At breakpoint %s, %s" % (breakpoint_position, variant))
             # Always make a ref variant from prev_ref_node_end to this breakpoints
             if breakpoint_position > prev_ref_node_end:
                 #logging.info("   Making a reference node %d. Pos before/after: %d/%d." % (
                 #self._current_node_id, prev_ref_node_end, breakpoint_position + 1))
-                prev_ref_node_id = self._make_node(prev_ref_node_end, breakpoint_position+1, self.reference_sequence[prev_ref_node_end+1:breakpoint_position+1], is_ref_node=True)
+                try:
+                    prev_ref_node_id = self._make_node(prev_ref_node_end, breakpoint_position+1, self.reference_sequence[prev_ref_node_end+1:breakpoint_position+1], is_ref_node=True)
+                except EmptyNodeException:
+                    logging.error("Tried making a node between pos %d and %d" % (prev_ref_node_end, breakpoint_position+1))
+                    logging.info("Variant is %s" % variant)
+                    raise
+
                 prev_ref_node_end = breakpoint_position
                 #logging.info("    Setting prev ref node end to %d" % prev_ref_node_end)
 
             # If breakpoint is a new variant, make a variant node
             if variant is not None:
                 if variant.type != "DELETION":
                     #logging.info("   Making a variant node %d. Pos before/after: %d/%d. Variant node sequence: %s" % (
```

### Comparing `obgraph-0.0.8/obgraph/graph_merger.py` & `obgraph-0.0.9/obgraph/graph_merger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import logging
 import numpy as np
 from .graph import Graph
 
 
 def merge_graphs(graphs):
 
-
     # Makes list of all data, then concatenates those in the end into numpy arrays that can be used to create a new graph
     new_nodes = []
-    new_nodes_to_sequence_index = []
     new_node_sequences = []
-    new_node_to_edge_index = []
-    new_node_to_n_edges = []
     new_edges = []
     new_node_to_ref_offset = []
     new_ref_offset_to_node = []
     new_chromosome_start_nodes = []
     new_allele_frequencies = []
 
     node_offset = 0
@@ -28,54 +24,44 @@
         logging.info("Node offset is now %d" % node_offset)
 
         # Add nodes, these are simply just appended
         new_nodes.append(graph.nodes)
 
         # All node ids should be increased by node_offset
 
-        # Node to sequence index can just be appended and index positions should increase by the length
-        # of the index up to now (new indexes needs to point this offset further in the sequence array)
-        new_nodes_to_sequence_index.append(graph.node_to_sequence_index+node_sequence_offset)
-
-        new_node_sequences.append(graph.node_sequences)
-        new_node_to_edge_index.append(graph.node_to_edge_index+edge_index_offset)
-        new_edges.append(graph.edges+node_offset)
-        new_node_to_n_edges.append(graph.node_to_n_edges)
+        # RaggedArrays can be concatenated
+        new_node_sequences.append(graph.sequences)
+        new_edges.append(graph.edges)
 
         new_node_to_ref_offset.append(graph.node_to_ref_offset+ref_offset)
         new_ref_offset_to_node.append(graph.ref_offset_to_node+node_offset)
 
         new_chromosome_start_nodes.append(graph.get_first_node() + node_offset)
 
         if graph.allele_frequencies is not None:
             new_allele_frequencies.append(graph.allele_frequencies)
 
         # Increase offsets
         node_offset += len(graph.nodes)
-        node_sequence_offset += len(graph.node_sequences)
+        node_sequence_offset += len(graph.sequences)
         edge_index_offset += len(graph.edges)
 
         # increase the length of the linear reference genome
         ref_offset += len(graph.ref_offset_to_node)
 
         logging.info("Ref offset is now %d" % ref_offset)
 
     logging.info("Concatenating all data")
     new_nodes = np.concatenate(new_nodes)
-    new_nodes_to_sequence_index = np.concatenate(new_nodes_to_sequence_index)
     new_node_sequences = np.concatenate(new_node_sequences)
-    new_node_to_edge_index = np.concatenate(new_node_to_edge_index)
-    new_node_to_n_edges = np.concatenate(new_node_to_n_edges)
     new_edges = np.concatenate(new_edges)
     new_node_to_ref_offset = np.concatenate(new_node_to_ref_offset)
     new_ref_offset_to_node = np.concatenate(new_ref_offset_to_node)
     new_chromosome_start_nodes = np.array(new_chromosome_start_nodes)
     if len(new_allele_frequencies) > 0:
         new_allele_frequencies = np.concatenate(new_allele_frequencies)
     else:
         new_allele_frequencies = None
 
-
-    return Graph(new_nodes, new_nodes_to_sequence_index, new_node_sequences,
-                 new_node_to_edge_index, new_node_to_n_edges, new_edges,
+    return Graph(new_nodes, new_node_sequences, new_edges,
                  new_node_to_ref_offset, new_ref_offset_to_node, new_chromosome_start_nodes,
                  new_allele_frequencies)
```

### Comparing `obgraph-0.0.8/obgraph/haplotype_matrix.py` & `obgraph-0.0.9/obgraph/haplotype_matrix.py`

 * *Files identical despite different names*

### Comparing `obgraph-0.0.8/obgraph/haplotype_nodes.py` & `obgraph-0.0.9/obgraph/haplotype_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
         self._haplotype_to_index = haplotype_to_index
         self._haplotype_to_n_nodes = haplotype_to_n_nodes
         self._nodes = nodes
 
     def to_file(self, file_name):
         np.savez(file_name, index=self._haplotype_to_index, n=self._haplotype_to_n_nodes, haplotypes=self._nodes)
 
+    def n_haplotypes(self):
+        return len(self._haplotype_to_index)
+
     def get_nodes(self, haplotype):
         assert type(haplotype) == int
         index = self._haplotype_to_index[haplotype]
         n = self._haplotype_to_n_nodes[haplotype]
 
         if n == 0:
             return np.array([])
@@ -201,17 +204,19 @@
 
     @classmethod
     def from_graph_and_variants(cls, graph, variants, limit_to_n_haplotypes=10, n_threads=10):
         # Flat structures used to make the index later
         flat_nodes = []
         flat_haplotypes = []
 
+        logging.info("Making pool")
         pool = Pool(n_threads)
-        shared_memory_graph_name = "graph_shared"
-        to_shared_memory(graph, shared_memory_graph_name)
+        logging.info("Made pool")
+        shared_memory_graph_name = to_shared_memory(graph)
+        logging.info("Put graph in shared memory")
 
         for haplotypes, nodes in pool.starmap(HaplotypeToNodes._multiprocess_wrapper, zip(repeat(shared_memory_graph_name), variants.get_chunks(chunk_size=1000), repeat(limit_to_n_haplotypes))):
             logging.info("Done with 1 iteration")
             flat_haplotypes.extend(haplotypes)
             flat_nodes.extend(nodes)
             logging.info("Added nodes and haplotypes")
```

### Comparing `obgraph-0.0.8/obgraph/mutable_graph.py` & `obgraph-0.0.9/obgraph/mutable_graph.py`

 * *Files identical despite different names*

### Comparing `obgraph-0.0.8/obgraph/numpy_variants.py` & `obgraph-0.0.9/obgraph/numpy_variants.py`

 * *Files identical despite different names*

### Comparing `obgraph-0.0.8/obgraph/traversing.py` & `obgraph-0.0.9/obgraph/traversing.py`

 * *Files identical despite different names*

### Comparing `obgraph-0.0.8/obgraph/util.py` & `obgraph-0.0.9/obgraph/util.py`

 * *Files identical despite different names*

### Comparing `obgraph-0.0.8/obgraph/variant_to_nodes.py` & `obgraph-0.0.9/obgraph/variant_to_nodes.py`

 * *Files identical despite different names*

### Comparing `obgraph-0.0.8/obgraph/variants.py` & `obgraph-0.0.9/obgraph/variants.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 def get_variant_type(vcf_line):
 
     l = vcf_line.split()
     if len(l[3]) == len(l[4]):
         return "SNP"
     elif "VT=SNP" in vcf_line:
         return "SNP"
-    elif len(l[3]) > len(l[4]):
+    elif len(l[3]) > 1 and len(l[4]) > 1:
+        return "SUBSTITUTION"
+    elif len(l[3]) > len(l[4]) and len(l[4]) == 1:
         return "DELETION"
-    elif len(l[3]) < len(l[4]):
+    elif len(l[3]) < len(l[4]) and len(l[3]) == 1:
         return "INSERTION"
     elif "VT=INDEL" in vcf_line:
         if len(l[3]) > len(l[4]):
             return "DELETION"
         else:
             return "INSERTION"
     else:
@@ -117,16 +119,18 @@
         return "chr%d:%d %s/%s %s %s" % (self.chromosome, self.position, self.ref_sequence, self.variant_sequence, self.genotype, self.type)
 
     def length(self):
         if self.type == "SNP":
             return 1
         elif self.type == "DELETION":
             return len(self.get_deleted_sequence())
-        elif self.type == "INSERTION":
+        elif self.type == "INSERTION" or self.type == "SUBSTITUTION":
             return len(self.variant_sequence) - 1
+        else:
+            raise Exception("Variant type %s not implemented" % self.type)
 
     def __repr__(self):
         return self.__str__()
 
     def __eq__(self, other):
         if self.id() == other.id():
             if self.genotype == other.genotype:
@@ -141,19 +145,26 @@
             return self.ref_sequence[1:]
 
         raise Exception("Variant %s is not a deletion" % self)
 
     def get_variant_sequence(self):
         if self.type == "DELETION":
             return ""
-        elif self.type == "INSERTION":
+        elif self.type == "INSERTION" or self.type == "SUBSTITUTION":
             return self.variant_sequence[1:]
         else:
             return self.variant_sequence
 
+    def get_reference_sequence(self):
+        if self.type == "INSERTION":
+            return ""
+        elif self.type == "INSERTION" or self.type == "SUBSTITUTION":
+            return self.ref_sequence[1:]
+        else:
+            return self.ref_sequence
 
     def get_variant_allele_frequency(self):
         try:
             info_field = self.vcf_line.split("\t")[7]
             af = float(info_field.split("AF=")[1].split(";")[0])
         except IndexError:
             logging.error("Could not get allele frequency from vcf line. VCF needs to contain an info column with AF= some allele frequency")
@@ -199,14 +210,16 @@
         numeric = 4
         if genotype_string == "0|0":
             numeric = 0
         elif genotype_string == "1|1":
             numeric = 2
         elif genotype_string == "0|1" or genotype_string == "1|0":
             numeric = 1
+        elif genotype_string == ".":
+            numberic = 4
         else:
             logging.error("Could not parse genotype string %s" % genotype_string)
             raise Exception("Unknown genotype")
 
         return numeric
 
     def _numeric_genotype3(self, genotype_string):
@@ -276,14 +289,18 @@
         start = self.get_reference_position_before_variant()
         if self.type == "SNP":
             return start + 2
         elif self.type == "INSERTION":
             return start + 1
         elif self.type == "DELETION":
             return start + len(self.ref_sequence) - 1 + 1
+        elif self.type == "SUBSTITUTION":
+            return start + len(self.ref_sequence)
+        else:
+            raise Exception("Not able to get ref pos after variant of type %s" % self.type)
 
 
 class VcfVariants:
     def __init__(self, variant_genotypes=[], skip_index=False, header_lines=""):
         self._header_lines = header_lines
         self.variant_genotypes = variant_genotypes
         self._index = {}
@@ -304,14 +321,15 @@
     def get_variant_by_line_number(self, line_number):
         return self.variant_genotypes[line_number]
 
     def add_variants(self, variant_list):
         self.variant_genotypes.extend(variant_list)
 
     def get_chunks(self, chunk_size=5000, add_variants_to_list=None):
+        logging.info("Getting variant chunks of size %d" % chunk_size)
         out = []
         prev_time = time.time()
         i = 0
         for variant_number, variant in enumerate(self.variant_genotypes):
             if variant_number % 100000 == 0:
                 logging.info("%d variants read" % variant_number)
             out.append(variant)
```

### Comparing `obgraph-0.0.8/obgraph.egg-info/SOURCES.txt` & `obgraph-0.0.9/obgraph.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 setup.py
 obgraph/__init__.py
 obgraph/command_line_interface.py
 obgraph/coordinate_converter.py
+obgraph/cython_traversing.c
 obgraph/dummy_node_adder.py
 obgraph/genotype_matrix.py
 obgraph/graph.py
 obgraph/graph_construction.py
 obgraph/graph_merger.py
 obgraph/haplotype_matrix.py
 obgraph/haplotype_nodes.py
 obgraph/mutable_graph.py
 obgraph/neighbour_haplotype_nodes.py
 obgraph/numpy_variants.py
+obgraph/position_id.py
 obgraph/traversing.py
 obgraph/util.py
 obgraph/variant_to_nodes.py
 obgraph/variants.py
 obgraph.egg-info/PKG-INFO
 obgraph.egg-info/SOURCES.txt
 obgraph.egg-info/dependency_links.txt
```

### Comparing `obgraph-0.0.8/setup.py` & `obgraph-0.0.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from setuptools import setup
 from distutils.core import setup
+from Cython.Build import cythonize
 
 setup(name='obgraph',
-      version='0.0.8',
+      version='0.0.9',
       description='obgraph',
       url='http://github.com/ivargr/obgraph',
       author='Ivar Grytten',
       author_email='',
       license='MIT',
       packages=["obgraph"],
       zip_safe=False,
-      install_requires=['numpy==1.20.3', 'tqdm', 'pathos', 'graph_kmer_index', 'shared_memory_wrapper'],
+      install_requires=['numpy==1.20.3', 'tqdm', 'pathos', 'graph_kmer_index>=0.0.15', 'shared_memory_wrapper>=0.0.7'],
       classifiers=[
             'Programming Language :: Python :: 3'
       ],
       entry_points={
             'console_scripts': ['obgraph=obgraph.command_line_interface:main']
       },
+      ext_modules = cythonize("obgraph/cython_traversing.pyx"),
 )
 
 """
 
 rm -rf dist
 python3 setup.py sdist
 twine upload --skip-existing dist/*
```

