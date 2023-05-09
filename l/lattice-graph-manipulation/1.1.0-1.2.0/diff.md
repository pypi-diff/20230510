# Comparing `tmp/Lattice-Graph-Manipulation-1.1.0.tar.gz` & `tmp/Lattice-Graph-Manipulation-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lattice-Graph-Manipulation-1.1.0.tar", last modified: Tue May  9 00:16:10 2023, max compression
+gzip compressed data, was "Lattice-Graph-Manipulation-1.2.0.tar", last modified: Tue May  9 23:38:40 2023, max compression
```

## Comparing `Lattice-Graph-Manipulation-1.1.0.tar` & `Lattice-Graph-Manipulation-1.2.0.tar`

### file list

```diff
@@ -1,69 +1,75 @@
--rw-r--r--   0        0        0     1070 2023-04-30 13:12:10.136468 Lattice-Graph-Manipulation-1.1.0/LICENSE
--rw-r--r--   0        0        0      541 2023-05-09 00:00:20.318358 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv
--rw-r--r--   0        0        0     6152 2023-05-09 00:00:20.345023 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv.pdf
--rw-r--r--   0        0        0        0 2023-05-09 00:13:53.962236 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/40861fca-41e9-4582-8ebf-fb5f53177aa2
--rw-r--r--   0        0        0        0 2023-05-09 00:13:53.958902 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/420099d8-e96d-4900-9fe7-b952495b28c0
--rw-r--r--   0        0        0      541 2023-05-09 00:00:25.531313 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv
--rw-r--r--   0        0        0     6118 2023-05-09 00:00:25.551312 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv.pdf
--rw-r--r--   0        0        0      541 2023-05-09 00:00:07.779270 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv
--rw-r--r--   0        0        0     6118 2023-05-09 00:00:07.805935 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv.pdf
--rw-r--r--   0        0        0      541 2023-05-09 00:00:23.294809 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv
--rw-r--r--   0        0        0     6152 2023-05-09 00:00:23.314807 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv.pdf
--rw-r--r--   0        0        0        0 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/__init__.py
--rw-r--r--   0        0        0      639 2023-05-07 00:22:21.936580 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/bb_tree.py
--rw-r--r--   0        0        0     1368 2023-05-05 22:09:45.090958 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv
--rw-r--r--   0        0        0     5573 2023-05-05 22:09:45.107624 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv.pdf
--rw-r--r--   0        0        0     4236 2023-05-05 22:01:27.915042 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv
--rw-r--r--   0        0        0     7654 2023-05-05 22:01:27.935042 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv.pdf
--rw-r--r--   0        0        0     1368 2023-05-05 21:59:43.450219 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv
--rw-r--r--   0        0        0     5567 2023-05-05 21:59:43.470219 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv.pdf
--rw-r--r--   0        0        0     4236 2023-05-05 22:02:54.341480 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv
--rw-r--r--   0        0        0     7750 2023-05-05 22:02:54.361480 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv.pdf
--rw-r--r--   0        0        0     4236 2023-05-05 22:04:13.795053 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv
--rw-r--r--   0        0        0     7593 2023-05-05 22:04:13.815054 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv.pdf
--rw-r--r--   0        0        0     7905 2023-05-07 00:23:54.513172 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv
--rw-r--r--   0        0        0     9268 2023-05-07 00:23:54.536505 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv.pdf
--rw-r--r--   0        0        0     7905 2023-05-07 00:19:22.396730 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv
--rw-r--r--   0        0        0     9201 2023-05-07 00:19:22.426730 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv.pdf
--rw-r--r--   0        0        0     4236 2023-05-05 22:02:27.888198 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv
--rw-r--r--   0        0        0     7617 2023-05-05 22:02:27.911531 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv.pdf
--rw-r--r--   0        0        0     7905 2023-05-07 00:36:00.902560 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv
--rw-r--r--   0        0        0     9214 2023-05-07 00:36:00.925894 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv.pdf
--rw-r--r--   0        0        0     5352 2023-05-05 22:10:28.170815 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv
--rw-r--r--   0        0        0     7753 2023-05-05 22:10:28.194148 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv.pdf
--rw-r--r--   0        0        0     7905 2023-05-05 22:10:58.647394 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv
--rw-r--r--   0        0        0     9267 2023-05-05 22:10:58.670728 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv.pdf
--rw-r--r--   0        0        0     2304 2023-05-07 00:23:41.253183 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv
--rw-r--r--   0        0        0     6086 2023-05-07 00:23:41.273183 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv.pdf
--rw-r--r--   0        0        0      451 2023-05-05 16:12:08.031549 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv
--rw-r--r--   0        0        0     6700 2023-05-05 16:12:08.054882 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv.pdf
--rw-r--r--   0        0        0     7905 2023-05-07 00:34:13.555984 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv
--rw-r--r--   0        0        0     9276 2023-05-07 00:34:13.579317 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv.pdf
--rw-r--r--   0        0        0      451 2023-05-07 00:20:50.539988 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv
--rw-r--r--   0        0        0     6728 2023-05-07 00:20:50.559988 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv.pdf
--rw-r--r--   0        0        0     2364 2023-05-05 22:01:03.491857 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv
--rw-r--r--   0        0        0     6142 2023-05-05 22:01:03.511857 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv.pdf
--rw-r--r--   0        0        0     1368 2023-05-05 21:58:56.455608 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv
--rw-r--r--   0        0        0     5809 2023-05-05 21:58:56.478942 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv.pdf
--rw-r--r--   0        0        0      541 2023-05-07 00:36:08.819221 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv
--rw-r--r--   0        0        0     6146 2023-05-07 00:36:08.852554 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv.pdf
--rw-r--r--   0        0        0      541 2023-05-09 00:00:23.338139 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv
--rw-r--r--   0        0        0     6152 2023-05-09 00:00:23.368137 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv.pdf
--rw-r--r--   0        0        0        0 2023-05-09 00:13:53.962236 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/ff81f168-34cc-4770-8535-2befc371ab12
--rw-r--r--   0        0        0     1045 2023-05-05 22:10:58.580728 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/grid_example.py
--rw-r--r--   0        0        0      648 2023-05-01 21:34:44.057078 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/simple_examples.py
--rw-r--r--   0        0        0      433 2023-05-08 23:43:22.403128 Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/simple_graph.py
--rw-r--r--   0        0        0        9 2023-04-30 13:12:10.136468 Lattice-Graph-Manipulation-1.1.0/README.md
--rw-r--r--   0        0        0       61 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.1.0/lattice/__init__.py
--rw-r--r--   0        0        0      148 2023-05-04 09:15:27.080595 Lattice-Graph-Manipulation-1.1.0/lattice/edge/__init__.py
--rw-r--r--   0        0        0      584 2023-05-01 21:31:00.683002 Lattice-Graph-Manipulation-1.1.0/lattice/edge/edge.py
--rw-r--r--   0        0        0      440 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.1.0/lattice/edge/traversaledge.py
--rw-r--r--   0        0        0      358 2023-05-04 09:11:10.130523 Lattice-Graph-Manipulation-1.1.0/lattice/edge/visualedge.py
--rw-r--r--   0        0        0      114 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.1.0/lattice/graph/__init__.py
--rw-r--r--   0        0        0     1558 2023-05-01 21:00:58.830421 Lattice-Graph-Manipulation-1.1.0/lattice/graph/bbtree.py
--rw-r--r--   0        0        0     4120 2023-05-09 00:15:47.432576 Lattice-Graph-Manipulation-1.1.0/lattice/graph/graph.py
--rw-r--r--   0        0        0      829 2023-05-05 12:55:46.790589 Lattice-Graph-Manipulation-1.1.0/lattice/graph/tree.py
--rw-r--r--   0        0        0       43 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.1.0/lattice/node/__init__.py
--rw-r--r--   0        0        0     1151 2023-05-05 21:58:39.058953 Lattice-Graph-Manipulation-1.1.0/lattice/node/node.py
--rw-r--r--   0        0        0      368 2023-05-09 00:16:03.968323 Lattice-Graph-Manipulation-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      196 1970-01-01 00:00:00.000000 Lattice-Graph-Manipulation-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-30 13:12:10.136468 Lattice-Graph-Manipulation-1.2.0/LICENSE
+-rw-r--r--   0        0        0      541 2023-05-09 00:00:20.318358 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv
+-rw-r--r--   0        0        0     6152 2023-05-09 00:00:20.345023 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv.pdf
+-rw-r--r--   0        0        0        0 2023-05-09 00:13:53.962236 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/40861fca-41e9-4582-8ebf-fb5f53177aa2
+-rw-r--r--   0        0        0        0 2023-05-09 00:13:53.958902 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/420099d8-e96d-4900-9fe7-b952495b28c0
+-rw-r--r--   0        0        0      541 2023-05-09 15:26:45.205033 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/5ee8c02a-4299-4464-9406-c91d7596a3df.gv
+-rw-r--r--   0        0        0     6152 2023-05-09 15:26:45.228366 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/5ee8c02a-4299-4464-9406-c91d7596a3df.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-09 00:00:25.531313 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv
+-rw-r--r--   0        0        0     6118 2023-05-09 00:00:25.551312 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-09 00:00:07.779270 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv
+-rw-r--r--   0        0        0     6118 2023-05-09 00:00:07.805935 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-09 00:00:23.294809 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv
+-rw-r--r--   0        0        0     6152 2023-05-09 00:00:23.314807 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-09 15:26:37.261708 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/9d8f8c6d-22ed-4a7e-af45-8ac72691f52c.gv
+-rw-r--r--   0        0        0     6142 2023-05-09 15:26:37.285041 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/9d8f8c6d-22ed-4a7e-af45-8ac72691f52c.gv.pdf
+-rw-r--r--   0        0        0        0 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/__init__.py
+-rw-r--r--   0        0        0      639 2023-05-07 00:22:21.936580 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/bb_tree.py
+-rw-r--r--   0        0        0     1368 2023-05-05 22:09:45.090958 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv
+-rw-r--r--   0        0        0     5573 2023-05-05 22:09:45.107624 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv.pdf
+-rw-r--r--   0        0        0     4236 2023-05-05 22:01:27.915042 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv
+-rw-r--r--   0        0        0     7654 2023-05-05 22:01:27.935042 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv.pdf
+-rw-r--r--   0        0        0     1368 2023-05-05 21:59:43.450219 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv
+-rw-r--r--   0        0        0     5567 2023-05-05 21:59:43.470219 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv.pdf
+-rw-r--r--   0        0        0     4236 2023-05-05 22:02:54.341480 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv
+-rw-r--r--   0        0        0     7750 2023-05-05 22:02:54.361480 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv.pdf
+-rw-r--r--   0        0        0     4236 2023-05-05 22:04:13.795053 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv
+-rw-r--r--   0        0        0     7593 2023-05-05 22:04:13.815054 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-07 00:23:54.513172 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv
+-rw-r--r--   0        0        0     9268 2023-05-07 00:23:54.536505 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-07 00:19:22.396730 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv
+-rw-r--r--   0        0        0     9201 2023-05-07 00:19:22.426730 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv.pdf
+-rw-r--r--   0        0        0     4236 2023-05-05 22:02:27.888198 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv
+-rw-r--r--   0        0        0     7617 2023-05-05 22:02:27.911531 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-07 00:36:00.902560 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv
+-rw-r--r--   0        0        0     9214 2023-05-07 00:36:00.925894 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv.pdf
+-rw-r--r--   0        0        0     5352 2023-05-05 22:10:28.170815 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv
+-rw-r--r--   0        0        0     7753 2023-05-05 22:10:28.194148 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-05 22:10:58.647394 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv
+-rw-r--r--   0        0        0     9267 2023-05-05 22:10:58.670728 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv.pdf
+-rw-r--r--   0        0        0     2304 2023-05-07 00:23:41.253183 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv
+-rw-r--r--   0        0        0     6086 2023-05-07 00:23:41.273183 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv.pdf
+-rw-r--r--   0        0        0      451 2023-05-05 16:12:08.031549 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv
+-rw-r--r--   0        0        0     6700 2023-05-05 16:12:08.054882 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-07 00:34:13.555984 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv
+-rw-r--r--   0        0        0     9276 2023-05-07 00:34:13.579317 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv.pdf
+-rw-r--r--   0        0        0      451 2023-05-07 00:20:50.539988 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv
+-rw-r--r--   0        0        0     6728 2023-05-07 00:20:50.559988 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv.pdf
+-rw-r--r--   0        0        0     2364 2023-05-05 22:01:03.491857 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv
+-rw-r--r--   0        0        0     6142 2023-05-05 22:01:03.511857 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv.pdf
+-rw-r--r--   0        0        0     1368 2023-05-05 21:58:56.455608 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv
+-rw-r--r--   0        0        0     5809 2023-05-05 21:58:56.478942 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-07 00:36:08.819221 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv
+-rw-r--r--   0        0        0     6146 2023-05-07 00:36:08.852554 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-09 00:00:23.338139 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv
+-rw-r--r--   0        0        0     6152 2023-05-09 00:00:23.368137 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv.pdf
+-rw-r--r--   0        0        0      470 2023-05-09 15:29:25.438125 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/f99dc209-e23f-406f-8d61-5e0943af8836.gv
+-rw-r--r--   0        0        0     7583 2023-05-09 15:29:25.458125 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/f99dc209-e23f-406f-8d61-5e0943af8836.gv.pdf
+-rw-r--r--   0        0        0        0 2023-05-09 00:13:53.962236 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/ff81f168-34cc-4770-8535-2befc371ab12
+-rw-r--r--   0        0        0     1045 2023-05-05 22:10:58.580728 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/grid_example.py
+-rw-r--r--   0        0        0      648 2023-05-01 21:34:44.057078 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/simple_examples.py
+-rw-r--r--   0        0        0      366 2023-05-09 23:37:35.585078 Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/simple_graph.py
+-rw-r--r--   0        0        0        9 2023-04-30 13:12:10.136468 Lattice-Graph-Manipulation-1.2.0/README.md
+-rw-r--r--   0        0        0       61 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.2.0/lattice/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-04 09:15:27.080595 Lattice-Graph-Manipulation-1.2.0/lattice/edge/__init__.py
+-rw-r--r--   0        0        0      584 2023-05-01 21:31:00.683002 Lattice-Graph-Manipulation-1.2.0/lattice/edge/edge.py
+-rw-r--r--   0        0        0      440 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.2.0/lattice/edge/traversaledge.py
+-rw-r--r--   0        0        0      358 2023-05-04 09:11:10.130523 Lattice-Graph-Manipulation-1.2.0/lattice/edge/visualedge.py
+-rw-r--r--   0        0        0      114 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.2.0/lattice/graph/__init__.py
+-rw-r--r--   0        0        0     1558 2023-05-01 21:00:58.830421 Lattice-Graph-Manipulation-1.2.0/lattice/graph/bbtree.py
+-rw-r--r--   0        0        0     4160 2023-05-09 15:39:15.649734 Lattice-Graph-Manipulation-1.2.0/lattice/graph/graph.py
+-rw-r--r--   0        0        0      829 2023-05-05 12:55:46.790589 Lattice-Graph-Manipulation-1.2.0/lattice/graph/tree.py
+-rw-r--r--   0        0        0       43 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.2.0/lattice/node/__init__.py
+-rw-r--r--   0        0        0     1279 2023-05-09 23:36:53.491816 Lattice-Graph-Manipulation-1.2.0/lattice/node/node.py
+-rw-r--r--   0        0        0      368 2023-05-09 23:38:36.348309 Lattice-Graph-Manipulation-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      196 1970-01-01 00:00:00.000000 Lattice-Graph-Manipulation-1.2.0/PKG-INFO
```

### Comparing `Lattice-Graph-Manipulation-1.1.0/LICENSE` & `Lattice-Graph-Manipulation-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/bb_tree.py` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/bb_tree.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv.pdf` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/grid_example.py` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/grid_example.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/Lattice_Scripts/simple_examples.py` & `Lattice-Graph-Manipulation-1.2.0/Lattice_Scripts/simple_examples.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/lattice/edge/edge.py` & `Lattice-Graph-Manipulation-1.2.0/lattice/edge/edge.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/lattice/graph/bbtree.py` & `Lattice-Graph-Manipulation-1.2.0/lattice/graph/bbtree.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/lattice/graph/graph.py` & `Lattice-Graph-Manipulation-1.2.0/lattice/graph/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,8 +103,9 @@
 
         return explored
 
     def __repr__(self):
         graphoutput = self.visualise()
         dotoutput = graphoutput.pipe(format='dot', encoding='utf-8')
         os.system('echo \'' + dotoutput + '\' | graph-easy --from=dot --as_ascii')
+        # graphoutput.render(view=True)
         return "​"
```

### Comparing `Lattice-Graph-Manipulation-1.1.0/lattice/graph/tree.py` & `Lattice-Graph-Manipulation-1.2.0/lattice/graph/tree.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.1.0/lattice/node/node.py` & `Lattice-Graph-Manipulation-1.2.0/lattice/node/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 class Node:
     _successors: set
     _predecessors: set
     _label: str
     _fingerprint: uuid.UUID
 
     def __init__(self, pointer, label=None):
+        """instantiate the node, if no label is given, then it is just the string representation of the data"""
         self.pointer = pointer
         self._predecessors = set()
         self._successors = set()
-        self._label = label
+        self._label = label or str(pointer)
         self._fingerprint = uuid.uuid4()
 
     def copy(self, label=None):
         return Node(self.pointer, label)
 
     @property
     def data(self):
```

