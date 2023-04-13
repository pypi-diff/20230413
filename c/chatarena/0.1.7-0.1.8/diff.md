# Comparing `tmp/chatarena-0.1.7.tar.gz` & `tmp/chatarena-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatarena-0.1.7.tar", last modified: Thu Apr  6 00:37:07 2023, max compression
+gzip compressed data, was "chatarena-0.1.8.tar", last modified: Thu Apr 13 16:45:14 2023, max compression
```

## Comparing `chatarena-0.1.7.tar` & `chatarena-0.1.8.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-06 00:37:07.440980 chatarena-0.1.7/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    11404 2023-04-03 15:56:48.000000 chatarena-0.1.7/LICENSE
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     8577 2023-04-06 00:37:07.440343 chatarena-0.1.7/PKG-INFO
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     7984 2023-04-05 23:21:36.000000 chatarena-0.1.7/README.md
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-06 00:37:07.431563 chatarena-0.1.7/chatarena/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)        0 2023-04-03 15:56:48.000000 chatarena-0.1.7/chatarena/__init__.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4769 2023-04-04 12:55:00.000000 chatarena-0.1.7/chatarena/agent.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     6681 2023-04-06 00:36:02.000000 chatarena-0.1.7/chatarena/arena.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-06 00:37:07.437459 chatarena-0.1.7/chatarena/backends/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      706 2023-04-03 15:56:48.000000 chatarena-0.1.7/chatarena/backends/__init__.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1334 2023-04-05 14:34:27.000000 chatarena-0.1.7/chatarena/backends/base.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4117 2023-04-05 14:34:27.000000 chatarena-0.1.7/chatarena/backends/cohere.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3534 2023-04-05 14:34:27.000000 chatarena-0.1.7/chatarena/backends/hf_transformers.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      669 2023-04-04 12:55:00.000000 chatarena-0.1.7/chatarena/backends/human.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3723 2023-04-05 23:06:33.000000 chatarena-0.1.7/chatarena/backends/openai.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4839 2023-04-05 14:34:27.000000 chatarena-0.1.7/chatarena/config.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4671 2023-04-05 14:34:27.000000 chatarena-0.1.7/chatarena/database.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-06 00:37:07.439908 chatarena-0.1.7/chatarena/environments/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      700 2023-04-06 00:36:02.000000 chatarena-0.1.7/chatarena/environments/__init__.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2647 2023-04-05 14:34:27.000000 chatarena-0.1.7/chatarena/environments/base.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    11463 2023-04-05 14:34:27.000000 chatarena-0.1.7/chatarena/environments/chameleon.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     6153 2023-04-05 14:34:27.000000 chatarena-0.1.7/chatarena/environments/conversation.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4757 2023-04-05 14:34:27.000000 chatarena-0.1.7/chatarena/environments/pettingzoo_chess.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2772 2023-04-03 15:56:48.000000 chatarena-0.1.7/chatarena/message.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      827 2023-04-03 15:56:48.000000 chatarena-0.1.7/chatarena/utils.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-06 00:37:07.433917 chatarena-0.1.7/chatarena.egg-info/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     8577 2023-04-06 00:37:07.000000 chatarena-0.1.7/chatarena.egg-info/PKG-INFO
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      713 2023-04-06 00:37:07.000000 chatarena-0.1.7/chatarena.egg-info/SOURCES.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)        1 2023-04-06 00:37:07.000000 chatarena-0.1.7/chatarena.egg-info/dependency_links.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      111 2023-04-06 00:37:07.000000 chatarena-0.1.7/chatarena.egg-info/requires.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)       10 2023-04-06 00:37:07.000000 chatarena-0.1.7/chatarena.egg-info/top_level.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      603 2023-04-06 00:33:12.000000 chatarena-0.1.7/pyproject.toml
--rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2023-04-06 00:37:07.441069 chatarena-0.1.7/setup.cfg
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      866 2023-04-06 00:33:02.000000 chatarena-0.1.7/setup.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-13 16:45:14.663982 chatarena-0.1.8/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    11404 2023-04-03 15:56:48.000000 chatarena-0.1.8/LICENSE
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    12250 2023-04-13 16:45:14.663591 chatarena-0.1.8/PKG-INFO
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    11657 2023-04-12 19:45:36.000000 chatarena-0.1.8/README.md
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-13 16:45:14.654802 chatarena-0.1.8/chatarena/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)        0 2023-04-03 15:56:48.000000 chatarena-0.1.8/chatarena/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4899 2023-04-12 22:43:42.000000 chatarena-0.1.8/chatarena/agent.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     6681 2023-04-06 00:43:37.000000 chatarena-0.1.8/chatarena/arena.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-13 16:45:14.660732 chatarena-0.1.8/chatarena/backends/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      749 2023-04-12 22:35:18.000000 chatarena-0.1.8/chatarena/backends/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3859 2023-04-12 23:12:18.000000 chatarena-0.1.8/chatarena/backends/anthropic.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1337 2023-04-12 22:43:42.000000 chatarena-0.1.8/chatarena/backends/base.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4088 2023-04-12 22:43:42.000000 chatarena-0.1.8/chatarena/backends/cohere.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3613 2023-04-12 22:42:35.000000 chatarena-0.1.8/chatarena/backends/hf_transformers.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      669 2023-04-04 12:55:00.000000 chatarena-0.1.8/chatarena/backends/human.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3646 2023-04-12 22:43:42.000000 chatarena-0.1.8/chatarena/backends/openai.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4839 2023-04-05 14:34:27.000000 chatarena-0.1.8/chatarena/config.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4671 2023-04-05 14:34:27.000000 chatarena-0.1.8/chatarena/database.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-13 16:45:14.663104 chatarena-0.1.8/chatarena/environments/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      700 2023-04-06 00:43:37.000000 chatarena-0.1.8/chatarena/environments/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2647 2023-04-05 14:34:27.000000 chatarena-0.1.8/chatarena/environments/base.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    11463 2023-04-05 14:34:27.000000 chatarena-0.1.8/chatarena/environments/chameleon.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     6153 2023-04-05 14:34:27.000000 chatarena-0.1.8/chatarena/environments/conversation.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4757 2023-04-05 14:34:27.000000 chatarena-0.1.8/chatarena/environments/pettingzoo_chess.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2794 2023-04-12 22:12:06.000000 chatarena-0.1.8/chatarena/message.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      827 2023-04-03 15:56:48.000000 chatarena-0.1.8/chatarena/utils.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-13 16:45:14.656742 chatarena-0.1.8/chatarena.egg-info/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    12250 2023-04-13 16:45:14.000000 chatarena-0.1.8/chatarena.egg-info/PKG-INFO
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      745 2023-04-13 16:45:14.000000 chatarena-0.1.8/chatarena.egg-info/SOURCES.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)        1 2023-04-13 16:45:14.000000 chatarena-0.1.8/chatarena.egg-info/dependency_links.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      111 2023-04-13 16:45:14.000000 chatarena-0.1.8/chatarena.egg-info/requires.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)       10 2023-04-13 16:45:14.000000 chatarena-0.1.8/chatarena.egg-info/top_level.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      603 2023-04-13 12:35:26.000000 chatarena-0.1.8/pyproject.toml
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2023-04-13 16:45:14.664063 chatarena-0.1.8/setup.cfg
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      866 2023-04-13 12:35:26.000000 chatarena-0.1.8/setup.py
```

### Comparing `chatarena-0.1.7/LICENSE` & `chatarena-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.7/PKG-INFO` & `chatarena-0.1.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,20 @@
-Metadata-Version: 2.1
-Name: chatarena
-Version: 0.1.7
-Summary: Multi-Agent Language Game Environments for LLMs
-Home-page: https://github.com/chatarena/chatarena
-Author: Yuxiang Wu
-Author-email: Yuxiang Wu <yuxiang.cs@gmail.com>
-Project-URL: Homepage, https://github.com/chatarena/chatarena
-Project-URL: Bug Tracker, https://github.com/chatarena/chatarena/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center"> 🏟 <span style="color:orange">ChatArena</span> </h1>
 
 <h3 align="center">
     <p>Multi-Agent Language Game Environments for LLMs</p>
 </h3>
 
 
-[![License: Apache2](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://github.com/chatarena/chatarena/blob/main/LICENSE) [![PyPI](https://img.shields.io/pypi/v/chatarena)](https://pypi.org/project/chatarena/) [![Python 3.9+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![License: Apache2](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://github.com/chatarena/chatarena/blob/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/chatarena)](https://pypi.org/project/chatarena/)
+[![Python 3.9+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![twitter](https://img.shields.io/twitter/follow/_chatarena?style=social&label=Follow%20ChatArena)](https://twitter.com/_chatarena)
+[![slack](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
+
 ---
 
 ChatArena is a Python library designed to facilitate communication and collaboration between multiple large language
 models (LLMs).
 It provides the following features:
 
 - **Language Game Environments**: it provides a framework for creating multi-agent language game environments, and a set
@@ -35,15 +24,17 @@
 - **User-friendly Interfaces**: it provides both Web browser UI and command line interface (CLI) to develop (prompt
   engineer) your LLM players to succeed in the environment.
 
 ![ChatArena Architecture](docs/images/chatarena_architecture.png)
 
 ## Getting Started
 
-[![Demo button](docs/images/demo_button.svg)](https://chatarena-chatarena-demo.hf.space)
+**Try our online demo:**
+[![demo](https://img.shields.io/badge/Demo-Huggingface%F0%9F%A4%97%20Space-orange?style=flat)](https://chatarena-chatarena-demo.hf.space)
+[![Demo video](https://img.shields.io/badge/Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816979419)
 
 ### Installation
 
 Requirements:
 
 - Python >= 3. 7
 - OpenAI API key (optional, for using GPT-3.5-turbo or GPT-4 as an LLM agent)
@@ -74,36 +65,36 @@
 To launch the demo on your local machine, you first need to git clone the repository and install it from source
 (see above instruction). Then run the following command in the root directory of the repository:
 
 ```shell
 gradio app.py
 ```
 
-This will launch a demo server for ChatArena and you can access it via http://127.0.0.1:7860/ in your browser.
+This will launch a demo server for ChatArena and you can access it in your browser.
+
+[//]: # (The interface looks like this:)
 
-[//]: # (TODO: put a gif here)
+[//]: # (![webui screenshot]&#40;docs/images/webui.png&#41;)
+
+Check out this video to learn how to use Web
+UI: [![Webui demo video](https://img.shields.io/badge/WebUI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816979419)
 
 ## Basic Usage
 
 ### Key Concepts
 
-- **Player**: a player is an agent that can interact with other players in a game environment. A player can be a human
-  or
-  a large language model (LLM). A player is defined by its name, its backend, and its role.
-    - **Backend**: a backend is a Python class that defines how a player interacts with other players. A backend can be
-      a
-      human, a LLM, or a combination of them. A backend is defined by its name, its type, and its parameters.
-- **Environment**: an environment is a Python class that defines the rules of a game. An environment is defined by its
-  name, its type, and its parameters.
-    - **Moderator**: a moderator is a Python class that defines how the game is played. A moderator is defined by its
-      name,
-      its type, and its parameters.
-- **Arena**: an arena is a Python class that defines the overall game. An arena is defined by its name, its type, and
-  its
-  parameters.
+- **Player**: a player is an agent that can interact with other players in a game environment. A player is defined by
+  its name, its backend, and its role description.
+    - **Backend**: a backend is a class that actually processes queries and generates responses in a conversation. A
+      backend can be a human, a remote or local LLM, or any program you create.
+- **Environment**: an environment is a class that defines the rules of a game and the game state transition.
+    - **Moderator**: a moderator is a special type of player that can control the game environment. It allows you to
+      define game environments using an LLM.
+- **Arena**: an arena is a utility class that contains the game environment and the players. It enables you to easily
+  run the game and save the game history, as well as interacting with the game via Web UI or CLI.
 
 ### Step 1: Define Multiple Players with LLM Backend
 
 ```python
 from chatarena.agent import Player
 from chatarena.backends import OpenAIChat
 
@@ -175,15 +166,16 @@
 
 Run the game in an interactive CLI interface
 
 ```python
 arena.launch_cli()
 ```
 
-[//]: # (TODO: put a CLI gif here)
+Check out this video to learn how to use
+CLI: [![cli demo video](https://img.shields.io/badge/CLI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816989884)
 
 ## Advanced Usage
 
 ### `ModeratedConversation`: a LLM-driven Environment
 
 We support a more advanced environment called `ModeratedConversation` that allows you to **control the game dynamics
 using an LLM**.
@@ -214,31 +206,95 @@
 5. Develop role description prompts (and global prompt if necessary) for players using CLI or Web UI and save them to a
    config file.
 
 We provide [a detailed tutorial](docs/tutorials/create_your_environment.md) to demonstrate how to define a custom
 environment,
 using the [`Chameleon` environment](chatarena/environments/chameleon.py) as example.
 
-If you want to port an existing library's environment to ChatArena, check out [`PettingzooChess` environment](chatarena/environments/pettingzoo_chess.py) as an example.
+If you want to port an existing library's environment to ChatArena, check
+out [`PettingzooChess` environment](chatarena/environments/pettingzoo_chess.py) as an example.
+
+## List of Games and Environments
+
+### [Conversation](chatarena/environments/conversation.py)
+
+A multi-player language game environment that simulates a
+conversation.
+
+* [NLP Classroom](examples/nlp-classroom-3players.json): a 3-player language game environment that simulates a
+  classroom
+  setting. The game is played in turns, and each turn a player can either ask a question or answer a question.
+  The game ends when all players have asked and answered all questions.
+
+### [Moderator Conversation](chatarena/environments/conversation.py)
+
+Based on converstion, but with a moderator that controls the game dynamics.
+
+* [Rock-paper-scissors](examples/rock-paper-scissors.json): a 2-player language game environment that simulates a
+  rock-paper-scissors game with moderator conversation.
+  Both player will act in parallel, and the game ends when one player wins 2 rounds.
+* [Tic-tac-toe](examples/tic-tac-toe.json): a 2-player language game environment that simulates a tic-tac-toe
+  game with moderator conversation.
+  The game is played in turns, and each turn a player can either ask for a move or make a move. The game ends when
+  one
+  player wins or the board is full.
+
+### [Chameleon](chatarena/environments/chameleon.py)
+
+A multi-player social deduction game. There are two roles in the game, chameleon and non-chameleon.
+The topic of the secret word will be first revealed to all the players.
+Then the secret word will be revealed to non-chameleons.
+The chameleon does not know the secret word.
+The objective in the game depends on the role of the player:
+
+- If you are not a chameleon, your goal is to reveal the chameleon without exposing the secret word.
+- If you are a chameleon, your aim is to blend in with other players, avoid being caught, and figure out the secret
+  word.
+  There are three stages in the game:
+
+1. The giving clues stage: each player will describe the clues about the secret word.
+2. The accusation stage: In this stage, each player will vote for another player who is most likely the chameleon. The
+   chameleon should vote for other players.
+3. The guess stage: If the accusation is correct, the chameleon should guess the secret word given the clues revealed by
+   other players.
+
+### [PettingZooChess](chatarena/environments/pettingzoo_chess.py)
+
+A two-player chess game environment that uses the PettingZoo Chess environment.
 
 ## Contributing
 
 We welcome contributions to improve and extend ChatArena. Please follow these steps to contribute:
 
 1. Fork the repository.
 2. Create a new branch for your feature or bugfix.
 3. Commit your changes to the new branch.
 4. Create a pull request describing your changes.
 5. We will review your pull request and provide feedback or merge your changes.
 
 Please ensure your code follows the existing style and structure.
 
+## Citation
+
+If you find ChatArena useful for your research, please cite our repository (our arxiv paper is coming soon):
+
+```bibtex
+@misc{ChatArena,
+  author = {Yuxiang Wu, Zhengyao Jiang, Akbir Khan, Yao Fu, Laura Ruis, Edward Grefenstette, and Tim Rocktäschel},
+  title = {ChatArena: Multi-Agent Language Game Environments for Large Language Models},
+  year = {2023},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/chatarena/chatarena}},
+}
+```
+
 ## Contact
 
 If you have any questions or suggestions, feel free to open an issue or submit a pull request.
-You can also follow the lead
-developer [![Twitter](https://img.shields.io/twitter/follow/mindjimmy?style=social)](https://twitter.com/mindjimmy) to
-get the latest updates.
+You can also follow us on [Twitter](https://twitter.com/_chatarena) or
+join [our Slack channel](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
+to get the latest updates.
 
 Happy chatting!
```

### Comparing `chatarena-0.1.7/README.md` & `chatarena-0.1.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,36 @@
+Metadata-Version: 2.1
+Name: chatarena
+Version: 0.1.8
+Summary: Multi-Agent Language Game Environments for LLMs
+Home-page: https://github.com/chatarena/chatarena
+Author: Yuxiang Wu
+Author-email: Yuxiang Wu <yuxiang.cs@gmail.com>
+Project-URL: Homepage, https://github.com/chatarena/chatarena
+Project-URL: Bug Tracker, https://github.com/chatarena/chatarena/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 align="center"> 🏟 <span style="color:orange">ChatArena</span> </h1>
 
 <h3 align="center">
     <p>Multi-Agent Language Game Environments for LLMs</p>
 </h3>
 
 
-[![License: Apache2](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://github.com/chatarena/chatarena/blob/main/LICENSE) [![PyPI](https://img.shields.io/pypi/v/chatarena)](https://pypi.org/project/chatarena/) [![Python 3.9+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![License: Apache2](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://github.com/chatarena/chatarena/blob/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/chatarena)](https://pypi.org/project/chatarena/)
+[![Python 3.9+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![twitter](https://img.shields.io/twitter/follow/_chatarena?style=social&label=Follow%20ChatArena)](https://twitter.com/_chatarena)
+[![slack](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
+
 ---
 
 ChatArena is a Python library designed to facilitate communication and collaboration between multiple large language
 models (LLMs).
 It provides the following features:
 
 - **Language Game Environments**: it provides a framework for creating multi-agent language game environments, and a set
@@ -19,15 +40,17 @@
 - **User-friendly Interfaces**: it provides both Web browser UI and command line interface (CLI) to develop (prompt
   engineer) your LLM players to succeed in the environment.
 
 ![ChatArena Architecture](docs/images/chatarena_architecture.png)
 
 ## Getting Started
 
-[![Demo button](docs/images/demo_button.svg)](https://chatarena-chatarena-demo.hf.space)
+**Try our online demo:**
+[![demo](https://img.shields.io/badge/Demo-Huggingface%F0%9F%A4%97%20Space-orange?style=flat)](https://chatarena-chatarena-demo.hf.space)
+[![Demo video](https://img.shields.io/badge/Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816979419)
 
 ### Installation
 
 Requirements:
 
 - Python >= 3. 7
 - OpenAI API key (optional, for using GPT-3.5-turbo or GPT-4 as an LLM agent)
@@ -58,36 +81,36 @@
 To launch the demo on your local machine, you first need to git clone the repository and install it from source
 (see above instruction). Then run the following command in the root directory of the repository:
 
 ```shell
 gradio app.py
 ```
 
-This will launch a demo server for ChatArena and you can access it via http://127.0.0.1:7860/ in your browser.
+This will launch a demo server for ChatArena and you can access it in your browser.
+
+[//]: # (The interface looks like this:)
 
-[//]: # (TODO: put a gif here)
+[//]: # (![webui screenshot]&#40;docs/images/webui.png&#41;)
+
+Check out this video to learn how to use Web
+UI: [![Webui demo video](https://img.shields.io/badge/WebUI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816979419)
 
 ## Basic Usage
 
 ### Key Concepts
 
-- **Player**: a player is an agent that can interact with other players in a game environment. A player can be a human
-  or
-  a large language model (LLM). A player is defined by its name, its backend, and its role.
-    - **Backend**: a backend is a Python class that defines how a player interacts with other players. A backend can be
-      a
-      human, a LLM, or a combination of them. A backend is defined by its name, its type, and its parameters.
-- **Environment**: an environment is a Python class that defines the rules of a game. An environment is defined by its
-  name, its type, and its parameters.
-    - **Moderator**: a moderator is a Python class that defines how the game is played. A moderator is defined by its
-      name,
-      its type, and its parameters.
-- **Arena**: an arena is a Python class that defines the overall game. An arena is defined by its name, its type, and
-  its
-  parameters.
+- **Player**: a player is an agent that can interact with other players in a game environment. A player is defined by
+  its name, its backend, and its role description.
+    - **Backend**: a backend is a class that actually processes queries and generates responses in a conversation. A
+      backend can be a human, a remote or local LLM, or any program you create.
+- **Environment**: an environment is a class that defines the rules of a game and the game state transition.
+    - **Moderator**: a moderator is a special type of player that can control the game environment. It allows you to
+      define game environments using an LLM.
+- **Arena**: an arena is a utility class that contains the game environment and the players. It enables you to easily
+  run the game and save the game history, as well as interacting with the game via Web UI or CLI.
 
 ### Step 1: Define Multiple Players with LLM Backend
 
 ```python
 from chatarena.agent import Player
 from chatarena.backends import OpenAIChat
 
@@ -159,15 +182,16 @@
 
 Run the game in an interactive CLI interface
 
 ```python
 arena.launch_cli()
 ```
 
-[//]: # (TODO: put a CLI gif here)
+Check out this video to learn how to use
+CLI: [![cli demo video](https://img.shields.io/badge/CLI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816989884)
 
 ## Advanced Usage
 
 ### `ModeratedConversation`: a LLM-driven Environment
 
 We support a more advanced environment called `ModeratedConversation` that allows you to **control the game dynamics
 using an LLM**.
@@ -198,31 +222,95 @@
 5. Develop role description prompts (and global prompt if necessary) for players using CLI or Web UI and save them to a
    config file.
 
 We provide [a detailed tutorial](docs/tutorials/create_your_environment.md) to demonstrate how to define a custom
 environment,
 using the [`Chameleon` environment](chatarena/environments/chameleon.py) as example.
 
-If you want to port an existing library's environment to ChatArena, check out [`PettingzooChess` environment](chatarena/environments/pettingzoo_chess.py) as an example.
+If you want to port an existing library's environment to ChatArena, check
+out [`PettingzooChess` environment](chatarena/environments/pettingzoo_chess.py) as an example.
+
+## List of Games and Environments
+
+### [Conversation](chatarena/environments/conversation.py)
+
+A multi-player language game environment that simulates a
+conversation.
+
+* [NLP Classroom](examples/nlp-classroom-3players.json): a 3-player language game environment that simulates a
+  classroom
+  setting. The game is played in turns, and each turn a player can either ask a question or answer a question.
+  The game ends when all players have asked and answered all questions.
+
+### [Moderator Conversation](chatarena/environments/conversation.py)
+
+Based on converstion, but with a moderator that controls the game dynamics.
+
+* [Rock-paper-scissors](examples/rock-paper-scissors.json): a 2-player language game environment that simulates a
+  rock-paper-scissors game with moderator conversation.
+  Both player will act in parallel, and the game ends when one player wins 2 rounds.
+* [Tic-tac-toe](examples/tic-tac-toe.json): a 2-player language game environment that simulates a tic-tac-toe
+  game with moderator conversation.
+  The game is played in turns, and each turn a player can either ask for a move or make a move. The game ends when
+  one
+  player wins or the board is full.
+
+### [Chameleon](chatarena/environments/chameleon.py)
+
+A multi-player social deduction game. There are two roles in the game, chameleon and non-chameleon.
+The topic of the secret word will be first revealed to all the players.
+Then the secret word will be revealed to non-chameleons.
+The chameleon does not know the secret word.
+The objective in the game depends on the role of the player:
+
+- If you are not a chameleon, your goal is to reveal the chameleon without exposing the secret word.
+- If you are a chameleon, your aim is to blend in with other players, avoid being caught, and figure out the secret
+  word.
+  There are three stages in the game:
+
+1. The giving clues stage: each player will describe the clues about the secret word.
+2. The accusation stage: In this stage, each player will vote for another player who is most likely the chameleon. The
+   chameleon should vote for other players.
+3. The guess stage: If the accusation is correct, the chameleon should guess the secret word given the clues revealed by
+   other players.
+
+### [PettingZooChess](chatarena/environments/pettingzoo_chess.py)
+
+A two-player chess game environment that uses the PettingZoo Chess environment.
 
 ## Contributing
 
 We welcome contributions to improve and extend ChatArena. Please follow these steps to contribute:
 
 1. Fork the repository.
 2. Create a new branch for your feature or bugfix.
 3. Commit your changes to the new branch.
 4. Create a pull request describing your changes.
 5. We will review your pull request and provide feedback or merge your changes.
 
 Please ensure your code follows the existing style and structure.
 
+## Citation
+
+If you find ChatArena useful for your research, please cite our repository (our arxiv paper is coming soon):
+
+```bibtex
+@misc{ChatArena,
+  author = {Yuxiang Wu, Zhengyao Jiang, Akbir Khan, Yao Fu, Laura Ruis, Edward Grefenstette, and Tim Rocktäschel},
+  title = {ChatArena: Multi-Agent Language Game Environments for Large Language Models},
+  year = {2023},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/chatarena/chatarena}},
+}
+```
+
 ## Contact
 
 If you have any questions or suggestions, feel free to open an issue or submit a pull request.
-You can also follow the lead
-developer [![Twitter](https://img.shields.io/twitter/follow/mindjimmy?style=social)](https://twitter.com/mindjimmy) to
-get the latest updates.
+You can also follow us on [Twitter](https://twitter.com/_chatarena) or
+join [our Slack channel](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
+to get the latest updates.
 
 Happy chatting!
```

### Comparing `chatarena-0.1.7/chatarena/agent.py` & `chatarena-0.1.8/chatarena/agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from tenacity import RetryError
 import logging
 import uuid
 from abc import abstractmethod
 
 from .backends import IntelligenceBackend, load_backend
-from .message import Message
+from .message import Message, SYSTEM_NAME
 from .config import AgentConfig, Configurable, BackendConfig
 
 # A special signal sent by the player to indicate that it is not possible to continue the conversation, and it requests to end the conversation.
 # It contains a random UUID string to avoid being exploited by any of the players.
 SIGNAL_END_OF_CONVERSATION = f"<<<<<<END_OF_CONVERSATION>>>>>>{uuid.uuid4()}"
 
 
@@ -36,14 +36,16 @@
             backend_config = backend
             backend = load_backend(backend_config)
         elif isinstance(backend, IntelligenceBackend):
             backend_config = backend.to_config()
         else:
             raise ValueError(f"backend must be a BackendConfig or an IntelligenceBackend, but got {type(backend)}")
 
+        assert name != SYSTEM_NAME, f"Player name cannot be {SYSTEM_NAME}, which is reserved for the system."
+
         # Register the fields in the _config
         super().__init__(name=name, role_desc=role_desc, backend=backend_config,
                          global_prompt=global_prompt, **kwargs)
 
         self.backend = backend
 
     def to_config(self) -> AgentConfig:
@@ -55,15 +57,15 @@
         )
 
     def __call__(self, observation: List[Message]) -> str:
         """
         Call the agents to generate a response (equivalent to taking an action).
         """
         try:
-            response = self.backend.query(agent_name=self.name, prompt=self.role_desc,
+            response = self.backend.query(agent_name=self.name, role_desc=self.role_desc,
                                           history_messages=observation, global_prompt=self.global_prompt,
                                           request_msg=None)
         except RetryError as e:
             logging.warning(f"Agent {self.name} failed to generate a response. "
                             f"Error: {e.last_attempt.exception()}. "
                             f"Sending signal to end the conversation.")
             response = SIGNAL_END_OF_CONVERSATION
@@ -101,15 +103,15 @@
         """
         # If the last message is the signal, then the conversation is over
         if history[-1].content == SIGNAL_END_OF_CONVERSATION:
             return True
 
         try:
             request_msg = Message(agent_name=self.name, content=self.terminal_condition, turn=-1)
-            response = self.backend.query(agent_name=self.name, prompt=self.role_desc, history_messages=history,
+            response = self.backend.query(agent_name=self.name, role_desc=self.role_desc, history_messages=history,
                                           global_prompt=self.global_prompt, request_msg=request_msg, *args, **kwargs)
         except RetryError as e:
             logging.warning(f"Agent {self.name} failed to generate a response. "
                             f"Error: {e.last_attempt.exception()}.")
             return True
 
         if re.match(r"yes|y|yea|yeah|yep|yup|sure|ok|okay|alright", response, re.IGNORECASE):
```

### Comparing `chatarena-0.1.7/chatarena/arena.py` & `chatarena-0.1.8/chatarena/arena.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.7/chatarena/backends/__init__.py` & `chatarena-0.1.8/chatarena/backends/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from ..config import BackendConfig
 
 from .base import IntelligenceBackend
 from .openai import OpenAIChat
 from .cohere import CohereAIChat
 from .human import Human
 from .hf_transformers import TransformersConversational
+from .anthropic import Claude
 
 ALL_BACKENDS = [
     Human,
     OpenAIChat,
     CohereAIChat,
-    TransformersConversational
+    TransformersConversational,
+    Claude,
 ]
 
 BACKEND_REGISTRY = {backend.type_name: backend for backend in ALL_BACKENDS}
 
 
 # Load a backend from a config dictionary
 def load_backend(config: BackendConfig):
```

### Comparing `chatarena-0.1.7/chatarena/backends/base.py` & `chatarena-0.1.8/chatarena/backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         return super().__init_subclass__(**kwargs)
 
     def to_config(self) -> BackendConfig:
         self._config_dict["backend_type"] = self.type_name
         return BackendConfig(**self._config_dict)
 
     @abstractmethod
-    def query(self, agent_name: str, prompt: str, history_messages: List[Message], global_prompt: str = None,
+    def query(self, agent_name: str, role_desc: str, history_messages: List[Message], global_prompt: str = None,
               request_msg: Message = None, *args, **kwargs) -> str:
         raise NotImplementedError
 
     # reset the state of the backend
     def reset(self):
         if self.stateful:
             raise NotImplementedError
```

### Comparing `chatarena-0.1.7/chatarena/backends/cohere.py` & `chatarena-0.1.8/chatarena/backends/cohere.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import List
 import os
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 
 from .base import IntelligenceBackend
-from ..config import BackendConfig
 from ..message import Message
 
 # Try to import the cohere package and check whether the API key is set
 try:
     import cohere
 except ImportError:
     is_cohere_available = False
@@ -58,15 +57,15 @@
             max_tokens=self.max_tokens,
             session_id=self.session_id
         )
 
         self.session_id = response.session_id  # Update the session id
         return response.reply
 
-    def query(self, agent_name: str, prompt: str, history_messages: List[Message], global_prompt: str = None,
+    def query(self, agent_name: str, role_desc: str, history_messages: List[Message], global_prompt: str = None,
               request_msg: Message = None, *args, **kwargs) -> str:
         """
         format the input and call the Cohere API
         args:
             agent_name: the name of the agent
             role_desc: the description of the role of the agent
             env_desc: the description of the environment
@@ -91,15 +90,15 @@
                 new_conversations.append(f"[{message.agent_name}]: {message.content}")
 
         if request_msg:
             new_conversations.append(f"[{request_msg.agent_name}]: {request_msg.content}")
 
         # Concatenate all new messages into one message because the Cohere API only accepts one message
         new_message = "\n".join(new_conversations)
-        persona_prompt = f"Environment:\n{global_prompt}\n\nYour role:\n{prompt}"
+        persona_prompt = f"Environment:\n{global_prompt}\n\nYour role:\n{role_desc}"
 
         response = self._get_response(new_message, persona_prompt)
 
         # Only update the last message hash if the API call is successful
         self.last_msg_hash = new_messages[-1].msg_hash
 
         return response
```

### Comparing `chatarena-0.1.7/chatarena/backends/hf_transformers.py` & `chatarena-0.1.8/chatarena/backends/hf_transformers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import List
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 
 from .base import IntelligenceBackend
-from ..config import BackendConfig
-from ..message import Message
+from ..message import Message, SYSTEM_NAME as SYSTEM
 
 # Try to import the transformers package
 try:
     import transformers
     from transformers import pipeline
     from transformers.pipelines.conversational import Conversation, ConversationalPipeline
 except ImportError:
@@ -37,41 +36,41 @@
         response = conversation.generated_responses[-1]
         return response
 
     @staticmethod
     def _msg_template(agent_name, content):
         return f"[{agent_name}]: {content}"
 
-    def query(self, agent_name: str, prompt: str, history_messages: List[Message], global_prompt: str = None,
+    def query(self, agent_name: str, role_desc: str, history_messages: List[Message], global_prompt: str = None,
               request_msg: Message = None, *args, **kwargs) -> str:
         user_inputs, generated_responses = [], []
+        all_messages = [(SYSTEM, global_prompt), (SYSTEM, role_desc)] if global_prompt else [(SYSTEM, role_desc)]
 
-        all_messages = [("System", global_prompt), ("System", prompt)]
         for msg in history_messages:
             all_messages.append((msg.agent_name, msg.content))
         if request_msg:
-            all_messages.append(("System", request_msg.content))
+            all_messages.append((SYSTEM, request_msg.content))
 
-        last_is_user = False
+        prev_is_user = False  # Whether the previous message is from the user
         for i, message in enumerate(all_messages):
             if i == 0:
-                assert message[0] == "System"  # The first message should be from the system
+                assert message[0] == SYSTEM  # The first message should be from the system
 
             if message[0] != agent_name:
-                if not last_is_user:
+                if not prev_is_user:
                     user_inputs.append(self._msg_template(message[0], message[1]))
                 else:
                     user_inputs[-1] += "\n" + self._msg_template(message[0], message[1])
-                last_is_user = True
+                prev_is_user = True
             else:
-                if last_is_user:
+                if prev_is_user:
                     generated_responses.append(message[1])
                 else:
                     generated_responses[-1] += "\n" + message[1]
-                last_is_user = False
+                prev_is_user = False
 
         assert len(user_inputs) == len(generated_responses) + 1
         past_user_inputs = user_inputs[:-1]
         new_user_input = user_inputs[-1]
 
         # Recreate a conversation object from the history messages
         conversation = Conversation(text=new_user_input, past_user_inputs=past_user_inputs,
```

### Comparing `chatarena-0.1.7/chatarena/backends/human.py` & `chatarena-0.1.8/chatarena/backends/human.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.7/chatarena/backends/openai.py` & `chatarena-0.1.8/chatarena/backends/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import List
 import os
+import re
 import logging
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 
 from .base import IntelligenceBackend
 from ..message import Message
-from ..config import BackendConfig
 
 try:
     import openai
 except ImportError:
     is_openai_available = False
-    logging.warning("OpenAI package is not installed")
+    logging.warning("openai package is not installed")
 else:
     openai.api_key = os.environ.get("OPENAI_API_KEY")
     if openai.api_key is None:
         logging.warning("OpenAI API key is not set. Please set the environment variable OPENAI_API_KEY")
         is_openai_available = False
     else:
         is_openai_available = True
@@ -33,15 +33,15 @@
     Interface to the ChatGPT style model with system, user, assistant roles separation
     """
     stateful = False
     type_name = "openai-chat"
 
     def __init__(self, temperature: float = DEFAULT_TEMPERATURE, max_tokens: int = DEFAULT_MAX_TOKENS,
                  model: str = DEFAULT_MODEL, **kwargs):
-        assert is_openai_available, "OpenAI package is not installed or the API key is not set"
+        assert is_openai_available, "openai package is not installed or the API key is not set"
         super().__init__(temperature=temperature, max_tokens=max_tokens, model=model, **kwargs)
 
         self.temperature = temperature
         self.max_tokens = max_tokens
         self.model = model
 
     @retry(stop=stop_after_attempt(6), wait=wait_random_exponential(min=1, max=60))
@@ -54,15 +54,15 @@
             stop=STOP
         )
 
         response = completion.choices[0]['message']['content']
         response = response.strip()
         return response
 
-    def query(self, agent_name: str, prompt: str, history_messages: List[Message], global_prompt: str = None,
+    def query(self, agent_name: str, role_desc: str, history_messages: List[Message], global_prompt: str = None,
               request_msg: Message = None, *args, **kwargs) -> str:
         """
         format the input and call the ChatGPT/GPT-4 API
         args:
             agent_name: the name of the agent
             role_desc: the description of the role of the agent
             env_desc: the description of the environment
@@ -74,25 +74,23 @@
             if message.agent_name == agent_name:
                 conversations.append({"role": "assistant", "content": message.content})
             else:
                 # Since there are more than one player, we need to distinguish between the players
                 conversations.append({"role": "user", "content": f"[{message.agent_name}]: {message.content}"})
 
         if global_prompt:  # Prepend the global prompt if it exists
-            system_prompt_str = f"{global_prompt.strip()}\n{prompt}"
+            system_prompt_str = f"{global_prompt.strip()}\n{role_desc}"
         else:
-            system_prompt_str = prompt
+            system_prompt_str = role_desc
         system_prompt = {"role": "system", "content": system_prompt_str}
 
         if request_msg:
             request_prompt = [{"role": "user", "content": request_msg.content}]
         else:
             request_prompt = []
 
         response = self._get_response([system_prompt] + conversations + request_prompt, *args, **kwargs)
 
-        # Remove the prefix if the response starts with it
-        prefix = f"[{agent_name}]:"
-        if response.startswith(prefix):
-            response = response[len(prefix):].strip()
+        # Remove the agent name if the response starts with it
+        response = re.sub(rf"^\s*\[{agent_name}]", "", response)
 
         return response
```

### Comparing `chatarena-0.1.7/chatarena/config.py` & `chatarena-0.1.8/chatarena/config.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.7/chatarena/database.py` & `chatarena-0.1.8/chatarena/database.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.7/chatarena/environments/__init__.py` & `chatarena-0.1.8/chatarena/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.7/chatarena/environments/base.py` & `chatarena-0.1.8/chatarena/environments/base.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.7/chatarena/environments/chameleon.py` & `chatarena-0.1.8/chatarena/environments/chameleon.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.7/chatarena/environments/conversation.py` & `chatarena-0.1.8/chatarena/environments/conversation.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.7/chatarena/environments/pettingzoo_chess.py` & `chatarena-0.1.8/chatarena/environments/pettingzoo_chess.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.7/chatarena/message.py` & `chatarena-0.1.8/chatarena/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import List, Union
 from dataclasses import dataclass
 import time
 from uuid import uuid1
 import hashlib
 
 
+SYSTEM_NAME="System"
+
 def _hash(input: str):
     hex_dig = hashlib.sha256(input.encode()).hexdigest()
     return hex_dig
 
 
 @dataclass
 class Message:
```

### Comparing `chatarena-0.1.7/chatarena/utils.py` & `chatarena-0.1.8/chatarena/utils.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.7/chatarena.egg-info/PKG-INFO` & `chatarena-0.1.8/chatarena.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatarena
-Version: 0.1.7
+Version: 0.1.8
 Summary: Multi-Agent Language Game Environments for LLMs
 Home-page: https://github.com/chatarena/chatarena
 Author: Yuxiang Wu
 Author-email: Yuxiang Wu <yuxiang.cs@gmail.com>
 Project-URL: Homepage, https://github.com/chatarena/chatarena
 Project-URL: Bug Tracker, https://github.com/chatarena/chatarena/issues
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,20 @@
 <h1 align="center"> 🏟 <span style="color:orange">ChatArena</span> </h1>
 
 <h3 align="center">
     <p>Multi-Agent Language Game Environments for LLMs</p>
 </h3>
 
 
-[![License: Apache2](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://github.com/chatarena/chatarena/blob/main/LICENSE) [![PyPI](https://img.shields.io/pypi/v/chatarena)](https://pypi.org/project/chatarena/) [![Python 3.9+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![License: Apache2](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://github.com/chatarena/chatarena/blob/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/chatarena)](https://pypi.org/project/chatarena/)
+[![Python 3.9+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![twitter](https://img.shields.io/twitter/follow/_chatarena?style=social&label=Follow%20ChatArena)](https://twitter.com/_chatarena)
+[![slack](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
+
 ---
 
 ChatArena is a Python library designed to facilitate communication and collaboration between multiple large language
 models (LLMs).
 It provides the following features:
 
 - **Language Game Environments**: it provides a framework for creating multi-agent language game environments, and a set
@@ -35,15 +40,17 @@
 - **User-friendly Interfaces**: it provides both Web browser UI and command line interface (CLI) to develop (prompt
   engineer) your LLM players to succeed in the environment.
 
 ![ChatArena Architecture](docs/images/chatarena_architecture.png)
 
 ## Getting Started
 
-[![Demo button](docs/images/demo_button.svg)](https://chatarena-chatarena-demo.hf.space)
+**Try our online demo:**
+[![demo](https://img.shields.io/badge/Demo-Huggingface%F0%9F%A4%97%20Space-orange?style=flat)](https://chatarena-chatarena-demo.hf.space)
+[![Demo video](https://img.shields.io/badge/Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816979419)
 
 ### Installation
 
 Requirements:
 
 - Python >= 3. 7
 - OpenAI API key (optional, for using GPT-3.5-turbo or GPT-4 as an LLM agent)
@@ -74,36 +81,36 @@
 To launch the demo on your local machine, you first need to git clone the repository and install it from source
 (see above instruction). Then run the following command in the root directory of the repository:
 
 ```shell
 gradio app.py
 ```
 
-This will launch a demo server for ChatArena and you can access it via http://127.0.0.1:7860/ in your browser.
+This will launch a demo server for ChatArena and you can access it in your browser.
+
+[//]: # (The interface looks like this:)
+
+[//]: # (![webui screenshot]&#40;docs/images/webui.png&#41;)
 
-[//]: # (TODO: put a gif here)
+Check out this video to learn how to use Web
+UI: [![Webui demo video](https://img.shields.io/badge/WebUI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816979419)
 
 ## Basic Usage
 
 ### Key Concepts
 
-- **Player**: a player is an agent that can interact with other players in a game environment. A player can be a human
-  or
-  a large language model (LLM). A player is defined by its name, its backend, and its role.
-    - **Backend**: a backend is a Python class that defines how a player interacts with other players. A backend can be
-      a
-      human, a LLM, or a combination of them. A backend is defined by its name, its type, and its parameters.
-- **Environment**: an environment is a Python class that defines the rules of a game. An environment is defined by its
-  name, its type, and its parameters.
-    - **Moderator**: a moderator is a Python class that defines how the game is played. A moderator is defined by its
-      name,
-      its type, and its parameters.
-- **Arena**: an arena is a Python class that defines the overall game. An arena is defined by its name, its type, and
-  its
-  parameters.
+- **Player**: a player is an agent that can interact with other players in a game environment. A player is defined by
+  its name, its backend, and its role description.
+    - **Backend**: a backend is a class that actually processes queries and generates responses in a conversation. A
+      backend can be a human, a remote or local LLM, or any program you create.
+- **Environment**: an environment is a class that defines the rules of a game and the game state transition.
+    - **Moderator**: a moderator is a special type of player that can control the game environment. It allows you to
+      define game environments using an LLM.
+- **Arena**: an arena is a utility class that contains the game environment and the players. It enables you to easily
+  run the game and save the game history, as well as interacting with the game via Web UI or CLI.
 
 ### Step 1: Define Multiple Players with LLM Backend
 
 ```python
 from chatarena.agent import Player
 from chatarena.backends import OpenAIChat
 
@@ -175,15 +182,16 @@
 
 Run the game in an interactive CLI interface
 
 ```python
 arena.launch_cli()
 ```
 
-[//]: # (TODO: put a CLI gif here)
+Check out this video to learn how to use
+CLI: [![cli demo video](https://img.shields.io/badge/CLI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816989884)
 
 ## Advanced Usage
 
 ### `ModeratedConversation`: a LLM-driven Environment
 
 We support a more advanced environment called `ModeratedConversation` that allows you to **control the game dynamics
 using an LLM**.
@@ -214,31 +222,95 @@
 5. Develop role description prompts (and global prompt if necessary) for players using CLI or Web UI and save them to a
    config file.
 
 We provide [a detailed tutorial](docs/tutorials/create_your_environment.md) to demonstrate how to define a custom
 environment,
 using the [`Chameleon` environment](chatarena/environments/chameleon.py) as example.
 
-If you want to port an existing library's environment to ChatArena, check out [`PettingzooChess` environment](chatarena/environments/pettingzoo_chess.py) as an example.
+If you want to port an existing library's environment to ChatArena, check
+out [`PettingzooChess` environment](chatarena/environments/pettingzoo_chess.py) as an example.
+
+## List of Games and Environments
+
+### [Conversation](chatarena/environments/conversation.py)
+
+A multi-player language game environment that simulates a
+conversation.
+
+* [NLP Classroom](examples/nlp-classroom-3players.json): a 3-player language game environment that simulates a
+  classroom
+  setting. The game is played in turns, and each turn a player can either ask a question or answer a question.
+  The game ends when all players have asked and answered all questions.
+
+### [Moderator Conversation](chatarena/environments/conversation.py)
+
+Based on converstion, but with a moderator that controls the game dynamics.
+
+* [Rock-paper-scissors](examples/rock-paper-scissors.json): a 2-player language game environment that simulates a
+  rock-paper-scissors game with moderator conversation.
+  Both player will act in parallel, and the game ends when one player wins 2 rounds.
+* [Tic-tac-toe](examples/tic-tac-toe.json): a 2-player language game environment that simulates a tic-tac-toe
+  game with moderator conversation.
+  The game is played in turns, and each turn a player can either ask for a move or make a move. The game ends when
+  one
+  player wins or the board is full.
+
+### [Chameleon](chatarena/environments/chameleon.py)
+
+A multi-player social deduction game. There are two roles in the game, chameleon and non-chameleon.
+The topic of the secret word will be first revealed to all the players.
+Then the secret word will be revealed to non-chameleons.
+The chameleon does not know the secret word.
+The objective in the game depends on the role of the player:
+
+- If you are not a chameleon, your goal is to reveal the chameleon without exposing the secret word.
+- If you are a chameleon, your aim is to blend in with other players, avoid being caught, and figure out the secret
+  word.
+  There are three stages in the game:
+
+1. The giving clues stage: each player will describe the clues about the secret word.
+2. The accusation stage: In this stage, each player will vote for another player who is most likely the chameleon. The
+   chameleon should vote for other players.
+3. The guess stage: If the accusation is correct, the chameleon should guess the secret word given the clues revealed by
+   other players.
+
+### [PettingZooChess](chatarena/environments/pettingzoo_chess.py)
+
+A two-player chess game environment that uses the PettingZoo Chess environment.
 
 ## Contributing
 
 We welcome contributions to improve and extend ChatArena. Please follow these steps to contribute:
 
 1. Fork the repository.
 2. Create a new branch for your feature or bugfix.
 3. Commit your changes to the new branch.
 4. Create a pull request describing your changes.
 5. We will review your pull request and provide feedback or merge your changes.
 
 Please ensure your code follows the existing style and structure.
 
+## Citation
+
+If you find ChatArena useful for your research, please cite our repository (our arxiv paper is coming soon):
+
+```bibtex
+@misc{ChatArena,
+  author = {Yuxiang Wu, Zhengyao Jiang, Akbir Khan, Yao Fu, Laura Ruis, Edward Grefenstette, and Tim Rocktäschel},
+  title = {ChatArena: Multi-Agent Language Game Environments for Large Language Models},
+  year = {2023},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/chatarena/chatarena}},
+}
+```
+
 ## Contact
 
 If you have any questions or suggestions, feel free to open an issue or submit a pull request.
-You can also follow the lead
-developer [![Twitter](https://img.shields.io/twitter/follow/mindjimmy?style=social)](https://twitter.com/mindjimmy) to
-get the latest updates.
+You can also follow us on [Twitter](https://twitter.com/_chatarena) or
+join [our Slack channel](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
+to get the latest updates.
 
 Happy chatting!
```

### Comparing `chatarena-0.1.7/chatarena.egg-info/SOURCES.txt` & `chatarena-0.1.8/chatarena.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 chatarena/utils.py
 chatarena.egg-info/PKG-INFO
 chatarena.egg-info/SOURCES.txt
 chatarena.egg-info/dependency_links.txt
 chatarena.egg-info/requires.txt
 chatarena.egg-info/top_level.txt
 chatarena/backends/__init__.py
+chatarena/backends/anthropic.py
 chatarena/backends/base.py
 chatarena/backends/cohere.py
 chatarena/backends/hf_transformers.py
 chatarena/backends/human.py
 chatarena/backends/openai.py
 chatarena/environments/__init__.py
 chatarena/environments/base.py
```

### Comparing `chatarena-0.1.7/pyproject.toml` & `chatarena-0.1.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatarena"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
     { name = "Yuxiang Wu", email = "yuxiang.cs@gmail.com" },
 ]
 description = "Multi-Agent Language Game Environments for LLMs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `chatarena-0.1.7/setup.py` & `chatarena-0.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 requirements = _deps
 
 setup(
     name="chatarena",
-    version="0.1.7",
+    version="0.1.8",
     author="Yuxiang Wu",
     author_email="yuxiang.cs@gmail.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/chatarena/chatarena",
     packages=find_packages(),
```

