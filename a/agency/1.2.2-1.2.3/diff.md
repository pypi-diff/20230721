# Comparing `tmp/agency-1.2.2.tar.gz` & `tmp/agency-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-1.2.2.tar", max compression
+gzip compressed data, was "agency-1.2.3.tar", max compression
```

## Comparing `agency-1.2.2.tar` & `agency-1.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35148 2023-07-16 09:53:16.905806 agency-1.2.2/LICENSE
--rw-r--r--   0        0        0     9675 2023-07-16 09:53:16.905806 agency-1.2.2/README.md
--rw-r--r--   0        0        0        0 2023-07-16 09:53:16.905806 agency-1.2.2/agency/__init__.py
--rw-r--r--   0        0        0     9502 2023-07-16 09:53:16.905806 agency-1.2.2/agency/agent.py
--rw-r--r--   0        0        0     7953 2023-07-16 09:53:16.905806 agency-1.2.2/agency/amqp_space.py
--rw-r--r--   0        0        0     2770 2023-07-16 09:53:16.905806 agency-1.2.2/agency/native_space.py
--rw-r--r--   0        0        0      802 2023-07-16 09:53:16.905806 agency-1.2.2/agency/schema.py
--rwxr-xr-x   0        0        0      754 2023-07-16 09:53:16.905806 agency-1.2.2/agency/space.py
--rw-r--r--   0        0        0     3824 2023-07-16 09:53:16.905806 agency-1.2.2/agency/util.py
--rw-r--r--   0        0        0      568 2023-07-16 09:53:18.641885 agency-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    10350 1970-01-01 00:00:00.000000 agency-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-21 03:42:25.783268 agency-1.2.3/LICENSE
+-rw-r--r--   0        0        0    10342 2023-07-21 03:42:25.783268 agency-1.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 03:42:25.783268 agency-1.2.3/agency/__init__.py
+-rw-r--r--   0        0        0     9541 2023-07-21 03:42:25.783268 agency-1.2.3/agency/agent.py
+-rw-r--r--   0        0        0     7953 2023-07-21 03:42:25.783268 agency-1.2.3/agency/amqp_space.py
+-rw-r--r--   0        0        0     2770 2023-07-21 03:42:25.783268 agency-1.2.3/agency/native_space.py
+-rw-r--r--   0        0        0      802 2023-07-21 03:42:25.783268 agency-1.2.3/agency/schema.py
+-rwxr-xr-x   0        0        0      754 2023-07-21 03:42:25.783268 agency-1.2.3/agency/space.py
+-rw-r--r--   0        0        0     3824 2023-07-21 03:42:25.787268 agency-1.2.3/agency/util.py
+-rw-r--r--   0        0        0      556 2023-07-21 03:42:27.663282 agency-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    11005 1970-01-01 00:00:00.000000 agency-1.2.3/PKG-INFO
```

### Comparing `agency-1.2.2/LICENSE` & `agency-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-1.2.2/README.md` & `agency-1.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Summary
 
-`agency` is a python library that provides a communication and action framework
-for creating AI agent-integrated systems.
+`agency` is a python library that provides a minimal framework for creating
+agent-integrated systems.
 
-The library provides a foundation for connecting agents, software systems, and
-human users by defining actions, callbacks, and access policies that you can use
-to connect, monitor, control, and interact with your agents.
+The library provides a simple foundation for connecting agents, software systems,
+and human users by defining actions, callbacks, and access policies that you can
+use to connect, monitor, and interact with your agents.
 
 `agency` handles the communication details and allows discovering and invoking
 actions across parties, automatically handling things such as reporting
 exceptions, enforcing access restrictions, and more.
 
 
 ## Features
@@ -19,31 +19,33 @@
 * Supports defining single process applications or networked agent systems
 using AMQP
 
 ### Observability and Control
 * Before/after action and lifecycle callbacks for observability or other needs
 * Access policies and permission callbacks for access control
 
-### Performance
+### Performance and Scalability
 * Multithreaded (though python's GIL is a bottleneck for single process apps)
 * AMQP support for multiprocess and networked systems (avoids GIL)
 * [_Python multiprocess support is planned for better scalability on
   single-host systems_](https://github.com/operand/agency/issues/33)
+* [_Decentralized networking support planned_](https://github.com/operand/agency/issues/83)
 
 ### Multimodal support
 * [_In development_](https://github.com/operand/agency/issues/26), though a
 timeline of features is not yet determined.
 
 ### Full demo available at [`examples/demo`](./examples/demo/)
 * Two OpenAI agent examples
 * HuggingFace transformers agent example
 * Simple Flask/React web interface included
 * Operating system access for agents
 * Docker configuration for reference and development
 
+(_Please note that [a Gradio UI is being developed](https://github.com/operand/agency/issues/82) to replace the Flask/React app above_)
 
 # API Overview
 
 `agency` is an implementation of the [Actor
 model](https://en.wikipedia.org/wiki/Actor_model) for building AI agent
 integrated systems.
 
@@ -135,14 +137,15 @@
 or
 ```sh
 poetry add agency
 ```
 
 
 # Running the Demo Application
+_(Note: [a Gradio app is being developed](https://github.com/operand/agency/issues/82) to replace the following UI soon.)_
 
 To run the demo, please follow the directions at
 [examples/demo](./examples/demo/). After a short boot time you can visit the
 web app at `http://localhost:8080` and you should see a simple chat interface.
 
 The following is a screenshot of the web UI that demonstrates multiple demo
 agents interacting and following orders.
@@ -161,58 +164,59 @@
 
 # FAQ
 
 ## How does `agency` compare to other agent libraries?
 
 Though you could entirely create a simple agent using only the primitives in
 `agency` (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
-intended to be an agent toolset like other libraries.
+intended to be an agent toolset like other libraries. For example, you won't
+find much support for building prompts or working with vector databases, etc.
+Implementation of agent behavior is left up to you.
+
+`agency` is concerned with providing a minimal communication and control
+foundation on which to define and integrate agent systems in a performant
+and flexible way, allowing developers to create custom agent solutions as
+they see fit.
 
-`agency` is a framework for defining and integrating agent-driven systems. It
-strives to provide a practical yet minimal foundation, allowing developers the
-freedom to create custom agent-integrated solutions as they see fit.
-
-So while you might use other libraries for implementing agent behavior, you can
-use `agency` for providing the foundation on which to define, connect, and
-control your agents.
+So if you're looking for a library with just enough structure to build from
+but not so much that it gets in your way, then `agency` might be for you.
 
 ## What are some known limitations or issues?
 
 * `agency` is still in early development. Like many projects in the AI agent
   space it is somewhat experimental at this time, with the goal of finding and
-  providing a minimal yet useful foundation for building AI agent systems.
+  providing a minimal yet useful foundation for building agent systems.
 
-  Expect changes to the API over time as features are added or changed. Stay up
-  to date on changes by following the
-  [issues](https://github.com/operand/agency/issues) or
-  [discussions](https://github.com/operand/agency/discussions) pages and please
-  reach out regarding bugs, features, ideas, or any feedback you'd like to
-  share.
+  Expect changes to the API over time as features are added or changed. The
+  library follows semver versioning starting at 1.x.x. Minor version updates
+  may contain breaking API changes. Patch versions should not.
 
 * This library makes use of threads for each individual agent. Multithreading
   is limited by [python's
   GIL](https://wiki.python.org/moin/GlobalInterpreterLock), meaning that if you
   run a local model or other heavy computation in the same process as other
   agents, they may have to wait for their "turn". Note that I/O does not block,
   so networked backends or services will execute in parallel.
 
   For blocking processes, it's recommended to use the `AMQPSpace` class and run
-  heavy computations in isolation to avoid blocking other agents.
+  heavy computations in isolation to avoid blocking other agents. [Multiprocessing
+  support](https://github.com/operand/agency/issues/33) is also planned as
+  another option for avoiding the GIL.
 
 * This API does not assume or enforce predefined roles like "user", "system",
   "assistant", etc. This is an intentional decision and is not likely to change.
 
   `agency` is intended to allow potentially large numbers of agents, systems,
   and people to come together. A small predefined set of roles gets in the way
   of representing many things generally. This is a core design feature of
-  `agency`: that all entities are treated similarly and may be interacted with
-  through common means.
+  `agency`: that all entities are represented similarly and may be interacted
+  with through common means.
 
-  The lack of roles may require extra translation code when integrating with
-  role based APIs. See the implementation of
+  The lack of roles may require extra work when integrating with role based
+  APIs. See the implementation of
   [`OpenAIFunctionAgent`](./examples/demo/agents/openai_function_agent.py) for
   an example.
 
 * There is currently not much by way of storage support. That is mostly left up
   to you and I'd suggest looking at the many technologies that focus on that.
   The `Agent` class implements a simple `_message_log` array which you can make
   use of or overwrite to back it with longer term storage. More direct support
@@ -255,29 +259,34 @@
 ```bash
 poetry run pytest
 ```
 
 
 # Roadmap
 
-- **Multiprocess Support**:
-An additional space type utilizing python multiprocessing, as another
-parallelism option for single-host systems.
-
 - **Multimodal Support**:
 Multimedia transfer for use with multimodal models or other multimedia services.
 
+- **Multiprocess Support**:
+An additional `Space` type utilizing python multiprocessing, as another
+parallelism option for single-host systems.
+
 - **Storage Support**
 Durable session support will be included. Other forms of storage will be
 considered though it's not clear yet what that may look like.
 
-- **Starter Application**
-The current demo application is proof-of-concept quality. A more modern and
-higher quality application will be developed to replace the main demo and serve
-as a reference example that can be extended or modified.
+- **Gradio Application**
+The current demo application uses a proof-of-concept quality Flask/React
+web app. A Gradio application will be developed to replace the Flask app
+and serve as a reference example that can be extended or modified.
+
+- **Decentralized Networking**
+An additional `Space` type using decentralized protocols, enabling the
+highest levels of scalability and opening the door for peer-to-peer
+agent networks.
 
 - **More Examples**:
 More examples of integrations with popular AI libraries and services will be
 added.
 
 
 ## Planned Work
```

### Comparing `agency-1.2.2/agency/agent.py` & `agency-1.2.3/agency/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
                 'args': get_arguments(method),
               }
               for name, method in methods.items()
               if method.access_policy != ACCESS_DENIED \
                 and re.search(r'^_action__(help|return|error)$', name) is None
             ]
         if action_name:
-            return self.__cached__help[action_name]
+            return [item for item in self.__cached__help if item["action"] == action_name]
         else:
             return self.__cached__help
 
     # Override any of the following methods as needed to implement your agent
 
     @access_policy(ACCESS_PERMITTED)
     def _action__help(self, action_name: str = None) -> list:
```

### Comparing `agency-1.2.2/agency/amqp_space.py` & `agency-1.2.3/agency/amqp_space.py`

 * *Files identical despite different names*

### Comparing `agency-1.2.2/agency/native_space.py` & `agency-1.2.3/agency/native_space.py`

 * *Files identical despite different names*

### Comparing `agency-1.2.2/agency/schema.py` & `agency-1.2.3/agency/schema.py`

 * *Files identical despite different names*

### Comparing `agency-1.2.2/agency/space.py` & `agency-1.2.3/agency/space.py`

 * *Files identical despite different names*

### Comparing `agency-1.2.2/agency/util.py` & `agency-1.2.3/agency/util.py`

 * *Files identical despite different names*

### Comparing `agency-1.2.2/PKG-INFO` & `agency-1.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: agency
-Version: 1.2.2
-Summary: A fast and minimal actor model framework for building agent-integrated systems
+Version: 1.2.3
+Summary: A fast and minimal framework for building agent-integrated systems
 License: GPL-3.0
 Author: Daniel Rodriguez
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,20 +14,20 @@
 Requires-Dist: colorama (>=0.4,<0.5)
 Requires-Dist: kombu (>=5.3.1,<6.0.0)
 Requires-Dist: pydantic (>=1.8,<2.0)
 Description-Content-Type: text/markdown
 
 # Summary
 
-`agency` is a python library that provides a communication and action framework
-for creating AI agent-integrated systems.
+`agency` is a python library that provides a minimal framework for creating
+agent-integrated systems.
 
-The library provides a foundation for connecting agents, software systems, and
-human users by defining actions, callbacks, and access policies that you can use
-to connect, monitor, control, and interact with your agents.
+The library provides a simple foundation for connecting agents, software systems,
+and human users by defining actions, callbacks, and access policies that you can
+use to connect, monitor, and interact with your agents.
 
 `agency` handles the communication details and allows discovering and invoking
 actions across parties, automatically handling things such as reporting
 exceptions, enforcing access restrictions, and more.
 
 
 ## Features
@@ -37,31 +37,33 @@
 * Supports defining single process applications or networked agent systems
 using AMQP
 
 ### Observability and Control
 * Before/after action and lifecycle callbacks for observability or other needs
 * Access policies and permission callbacks for access control
 
-### Performance
+### Performance and Scalability
 * Multithreaded (though python's GIL is a bottleneck for single process apps)
 * AMQP support for multiprocess and networked systems (avoids GIL)
 * [_Python multiprocess support is planned for better scalability on
   single-host systems_](https://github.com/operand/agency/issues/33)
+* [_Decentralized networking support planned_](https://github.com/operand/agency/issues/83)
 
 ### Multimodal support
 * [_In development_](https://github.com/operand/agency/issues/26), though a
 timeline of features is not yet determined.
 
 ### Full demo available at [`examples/demo`](./examples/demo/)
 * Two OpenAI agent examples
 * HuggingFace transformers agent example
 * Simple Flask/React web interface included
 * Operating system access for agents
 * Docker configuration for reference and development
 
+(_Please note that [a Gradio UI is being developed](https://github.com/operand/agency/issues/82) to replace the Flask/React app above_)
 
 # API Overview
 
 `agency` is an implementation of the [Actor
 model](https://en.wikipedia.org/wiki/Actor_model) for building AI agent
 integrated systems.
 
@@ -153,14 +155,15 @@
 or
 ```sh
 poetry add agency
 ```
 
 
 # Running the Demo Application
+_(Note: [a Gradio app is being developed](https://github.com/operand/agency/issues/82) to replace the following UI soon.)_
 
 To run the demo, please follow the directions at
 [examples/demo](./examples/demo/). After a short boot time you can visit the
 web app at `http://localhost:8080` and you should see a simple chat interface.
 
 The following is a screenshot of the web UI that demonstrates multiple demo
 agents interacting and following orders.
@@ -179,58 +182,59 @@
 
 # FAQ
 
 ## How does `agency` compare to other agent libraries?
 
 Though you could entirely create a simple agent using only the primitives in
 `agency` (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
-intended to be an agent toolset like other libraries.
+intended to be an agent toolset like other libraries. For example, you won't
+find much support for building prompts or working with vector databases, etc.
+Implementation of agent behavior is left up to you.
+
+`agency` is concerned with providing a minimal communication and control
+foundation on which to define and integrate agent systems in a performant
+and flexible way, allowing developers to create custom agent solutions as
+they see fit.
 
-`agency` is a framework for defining and integrating agent-driven systems. It
-strives to provide a practical yet minimal foundation, allowing developers the
-freedom to create custom agent-integrated solutions as they see fit.
-
-So while you might use other libraries for implementing agent behavior, you can
-use `agency` for providing the foundation on which to define, connect, and
-control your agents.
+So if you're looking for a library with just enough structure to build from
+but not so much that it gets in your way, then `agency` might be for you.
 
 ## What are some known limitations or issues?
 
 * `agency` is still in early development. Like many projects in the AI agent
   space it is somewhat experimental at this time, with the goal of finding and
-  providing a minimal yet useful foundation for building AI agent systems.
+  providing a minimal yet useful foundation for building agent systems.
 
-  Expect changes to the API over time as features are added or changed. Stay up
-  to date on changes by following the
-  [issues](https://github.com/operand/agency/issues) or
-  [discussions](https://github.com/operand/agency/discussions) pages and please
-  reach out regarding bugs, features, ideas, or any feedback you'd like to
-  share.
+  Expect changes to the API over time as features are added or changed. The
+  library follows semver versioning starting at 1.x.x. Minor version updates
+  may contain breaking API changes. Patch versions should not.
 
 * This library makes use of threads for each individual agent. Multithreading
   is limited by [python's
   GIL](https://wiki.python.org/moin/GlobalInterpreterLock), meaning that if you
   run a local model or other heavy computation in the same process as other
   agents, they may have to wait for their "turn". Note that I/O does not block,
   so networked backends or services will execute in parallel.
 
   For blocking processes, it's recommended to use the `AMQPSpace` class and run
-  heavy computations in isolation to avoid blocking other agents.
+  heavy computations in isolation to avoid blocking other agents. [Multiprocessing
+  support](https://github.com/operand/agency/issues/33) is also planned as
+  another option for avoiding the GIL.
 
 * This API does not assume or enforce predefined roles like "user", "system",
   "assistant", etc. This is an intentional decision and is not likely to change.
 
   `agency` is intended to allow potentially large numbers of agents, systems,
   and people to come together. A small predefined set of roles gets in the way
   of representing many things generally. This is a core design feature of
-  `agency`: that all entities are treated similarly and may be interacted with
-  through common means.
+  `agency`: that all entities are represented similarly and may be interacted
+  with through common means.
 
-  The lack of roles may require extra translation code when integrating with
-  role based APIs. See the implementation of
+  The lack of roles may require extra work when integrating with role based
+  APIs. See the implementation of
   [`OpenAIFunctionAgent`](./examples/demo/agents/openai_function_agent.py) for
   an example.
 
 * There is currently not much by way of storage support. That is mostly left up
   to you and I'd suggest looking at the many technologies that focus on that.
   The `Agent` class implements a simple `_message_log` array which you can make
   use of or overwrite to back it with longer term storage. More direct support
@@ -273,29 +277,34 @@
 ```bash
 poetry run pytest
 ```
 
 
 # Roadmap
 
-- **Multiprocess Support**:
-An additional space type utilizing python multiprocessing, as another
-parallelism option for single-host systems.
-
 - **Multimodal Support**:
 Multimedia transfer for use with multimodal models or other multimedia services.
 
+- **Multiprocess Support**:
+An additional `Space` type utilizing python multiprocessing, as another
+parallelism option for single-host systems.
+
 - **Storage Support**
 Durable session support will be included. Other forms of storage will be
 considered though it's not clear yet what that may look like.
 
-- **Starter Application**
-The current demo application is proof-of-concept quality. A more modern and
-higher quality application will be developed to replace the main demo and serve
-as a reference example that can be extended or modified.
+- **Gradio Application**
+The current demo application uses a proof-of-concept quality Flask/React
+web app. A Gradio application will be developed to replace the Flask app
+and serve as a reference example that can be extended or modified.
+
+- **Decentralized Networking**
+An additional `Space` type using decentralized protocols, enabling the
+highest levels of scalability and opening the door for peer-to-peer
+agent networks.
 
 - **More Examples**:
 More examples of integrations with popular AI libraries and services will be
 added.
 
 
 ## Planned Work
```

