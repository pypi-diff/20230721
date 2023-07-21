# Comparing `tmp/multimcts-0.2.1.tar.gz` & `tmp/multimcts-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimcts-0.2.1.tar", last modified: Thu Jul 20 01:22:42 2023, max compression
+gzip compressed data, was "multimcts-0.2.2.tar", last modified: Fri Jul 21 00:56:22 2023, max compression
```

## Comparing `multimcts-0.2.1.tar` & `multimcts-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-20 01:22:42.894697 multimcts-0.2.1/
--rw-r--r--   0 taylorvance   (501) staff       (20)       24 2023-07-17 19:47:43.000000 multimcts-0.2.1/MANIFEST.in
--rw-r--r--   0 taylorvance   (501) staff       (20)     2005 2023-07-20 01:22:42.894581 multimcts-0.2.1/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)     1711 2023-07-19 19:51:18.000000 multimcts-0.2.1/README.md
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-20 01:22:42.893422 multimcts-0.2.1/multimcts/
--rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.2.1/multimcts/__init__.py
--rw-r--r--   0 taylorvance   (501) staff       (20)   470686 2023-07-20 01:22:42.000000 multimcts-0.2.1/multimcts/mcts.c
--rw-r--r--   0 taylorvance   (501) staff       (20)     8517 2023-07-20 01:21:14.000000 multimcts-0.2.1/multimcts/mcts.pyx
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-20 01:22:42.894408 multimcts-0.2.1/multimcts.egg-info/
--rw-r--r--   0 taylorvance   (501) staff       (20)     2005 2023-07-20 01:22:42.000000 multimcts-0.2.1/multimcts.egg-info/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)      257 2023-07-17 23:05:38.000000 multimcts-0.2.1/multimcts.egg-info/SOURCES 2.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)      300 2023-07-20 01:22:42.000000 multimcts-0.2.1/multimcts.egg-info/SOURCES.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-20 01:22:42.000000 multimcts-0.2.1/multimcts.egg-info/dependency_links.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 19:12:04.000000 multimcts-0.2.1/multimcts.egg-info/not-zip-safe
--rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-20 01:22:42.000000 multimcts-0.2.1/multimcts.egg-info/top_level.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-17 18:23:36.000000 multimcts-0.2.1/pyproject.toml
--rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-20 01:22:42.894737 multimcts-0.2.1/setup.cfg
--rw-r--r--   0 taylorvance   (501) staff       (20)      520 2023-07-20 01:17:04.000000 multimcts-0.2.1/setup.py
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-21 00:56:22.477183 multimcts-0.2.2/
+-rw-r--r--   0 taylorvance   (501) staff       (20)       24 2023-07-17 19:47:43.000000 multimcts-0.2.2/MANIFEST.in
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2005 2023-07-21 00:56:22.477046 multimcts-0.2.2/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)     1711 2023-07-19 19:51:18.000000 multimcts-0.2.2/README.md
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-21 00:56:22.475889 multimcts-0.2.2/multimcts/
+-rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.2.2/multimcts/__init__.py
+-rw-r--r--   0 taylorvance   (501) staff       (20)   412842 2023-07-21 00:56:22.000000 multimcts-0.2.2/multimcts/mcts.c
+-rw-r--r--   0 taylorvance   (501) staff       (20)     8809 2023-07-20 17:20:51.000000 multimcts-0.2.2/multimcts/mcts.pyx
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-21 00:56:22.476843 multimcts-0.2.2/multimcts.egg-info/
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2005 2023-07-21 00:56:22.000000 multimcts-0.2.2/multimcts.egg-info/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)      257 2023-07-17 23:05:38.000000 multimcts-0.2.2/multimcts.egg-info/SOURCES 2.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)      300 2023-07-21 00:56:22.000000 multimcts-0.2.2/multimcts.egg-info/SOURCES.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-21 00:56:22.000000 multimcts-0.2.2/multimcts.egg-info/dependency_links.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 19:12:04.000000 multimcts-0.2.2/multimcts.egg-info/not-zip-safe
+-rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-21 00:56:22.000000 multimcts-0.2.2/multimcts.egg-info/top_level.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-17 18:23:36.000000 multimcts-0.2.2/pyproject.toml
+-rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-21 00:56:22.477229 multimcts-0.2.2/setup.cfg
+-rw-r--r--   0 taylorvance   (501) staff       (20)      520 2023-07-20 01:24:59.000000 multimcts-0.2.2/setup.py
```

### Comparing `multimcts-0.2.1/PKG-INFO` & `multimcts-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimcts
-Version: 0.2.1
+Version: 0.2.2
 Summary: Monte Carlo Tree Search for multiple teams
 Home-page: https://github.com/taylorvance/multimcts
 Author: Taylor Vance
 Author-email: mirrors.cities0w@icloud.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `multimcts-0.2.1/README.md` & `multimcts-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `multimcts-0.2.1/multimcts/mcts.c` & `multimcts-0.2.2/multimcts/mcts.c`

 * *Files 4% similar despite different names*

```diff
@@ -970,46 +970,14 @@
 
 
 static const char *__pyx_f[] = {
   "multimcts/mcts.pyx",
 };
 
 /*--- Type declarations ---*/
-struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child;
-struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr;
-
-/* "multimcts/mcts.pyx":193
- *             node = node.parent
- * 
- *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         cur_team = node.state.get_current_team()
- * 
- */
-struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child {
-  PyObject_HEAD
-  PyObject *__pyx_v_child;
-};
-
-
-/* "multimcts/mcts.pyx":207
- *         for child in node.children:
- *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())             # <<<<<<<<<<<<<<
- *             visits = child.num_visits
- * 
- */
-struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr {
-  PyObject_HEAD
-  struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *__pyx_outer_scope;
-  PyObject *__pyx_v_x;
-  PyObject *__pyx_t_0;
-  Py_ssize_t __pyx_t_1;
-  PyObject *(*__pyx_t_2)(PyObject *);
-};
-
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
@@ -1447,27 +1415,14 @@
     (likely(PyDict_CheckExact(obj)) ?\
      __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
 #else
 #define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
 #define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
 #endif
 
-/* None.proto */
-static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname);
-
-/* IncludeStringH.proto */
-#include <string.h>
-
-/* PyObject_GenericGetAttrNoDict.proto */
-#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
-#else
-#define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
-#endif
-
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* FetchCommonType.proto */
@@ -1602,181 +1557,91 @@
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
-/* SwapException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#else
-static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
-#endif
-
-/* CoroutineBase.proto */
-typedef PyObject *(*__pyx_coroutine_body_t)(PyObject *, PyThreadState *, PyObject *);
-#if CYTHON_USE_EXC_INFO_STACK
-#define __Pyx_ExcInfoStruct  _PyErr_StackItem
-#else
-typedef struct {
-    PyObject *exc_type;
-    PyObject *exc_value;
-    PyObject *exc_traceback;
-} __Pyx_ExcInfoStruct;
-#endif
-typedef struct {
-    PyObject_HEAD
-    __pyx_coroutine_body_t body;
-    PyObject *closure;
-    __Pyx_ExcInfoStruct gi_exc_state;
-    PyObject *gi_weakreflist;
-    PyObject *classobj;
-    PyObject *yieldfrom;
-    PyObject *gi_name;
-    PyObject *gi_qualname;
-    PyObject *gi_modulename;
-    PyObject *gi_code;
-    PyObject *gi_frame;
-    int resume_label;
-    char is_running;
-} __pyx_CoroutineObject;
-static __pyx_CoroutineObject *__Pyx__Coroutine_New(
-    PyTypeObject *type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
-    PyObject *name, PyObject *qualname, PyObject *module_name);
-static __pyx_CoroutineObject *__Pyx__Coroutine_NewInit(
-            __pyx_CoroutineObject *gen, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
-            PyObject *name, PyObject *qualname, PyObject *module_name);
-static CYTHON_INLINE void __Pyx_Coroutine_ExceptionClear(__Pyx_ExcInfoStruct *self);
-static int __Pyx_Coroutine_clear(PyObject *self);
-static PyObject *__Pyx_Coroutine_Send(PyObject *self, PyObject *value);
-static PyObject *__Pyx_Coroutine_Close(PyObject *self);
-static PyObject *__Pyx_Coroutine_Throw(PyObject *gen, PyObject *args);
-#if CYTHON_USE_EXC_INFO_STACK
-#define __Pyx_Coroutine_SwapException(self)
-#define __Pyx_Coroutine_ResetAndClearException(self)  __Pyx_Coroutine_ExceptionClear(&(self)->gi_exc_state)
-#else
-#define __Pyx_Coroutine_SwapException(self) {\
-    __Pyx_ExceptionSwap(&(self)->gi_exc_state.exc_type, &(self)->gi_exc_state.exc_value, &(self)->gi_exc_state.exc_traceback);\
-    __Pyx_Coroutine_ResetFrameBackpointer(&(self)->gi_exc_state);\
-    }
-#define __Pyx_Coroutine_ResetAndClearException(self) {\
-    __Pyx_ExceptionReset((self)->gi_exc_state.exc_type, (self)->gi_exc_state.exc_value, (self)->gi_exc_state.exc_traceback);\
-    (self)->gi_exc_state.exc_type = (self)->gi_exc_state.exc_value = (self)->gi_exc_state.exc_traceback = NULL;\
-    }
-#endif
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyGen_FetchStopIterationValue(pvalue)\
-    __Pyx_PyGen__FetchStopIterationValue(__pyx_tstate, pvalue)
-#else
-#define __Pyx_PyGen_FetchStopIterationValue(pvalue)\
-    __Pyx_PyGen__FetchStopIterationValue(__Pyx_PyThreadState_Current, pvalue)
-#endif
-static int __Pyx_PyGen__FetchStopIterationValue(PyThreadState *tstate, PyObject **pvalue);
-static CYTHON_INLINE void __Pyx_Coroutine_ResetFrameBackpointer(__Pyx_ExcInfoStruct *exc_state);
-
-/* PatchModuleWithCoroutine.proto */
-static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code);
-
-/* PatchGeneratorABC.proto */
-static int __Pyx_patch_abc(void);
-
-/* Generator.proto */
-#define __Pyx_Generator_USED
-static PyTypeObject *__pyx_GeneratorType = 0;
-#define __Pyx_Generator_CheckExact(obj) (Py_TYPE(obj) == __pyx_GeneratorType)
-#define __Pyx_Generator_New(body, code, closure, name, qualname, module_name)\
-    __Pyx__Coroutine_New(__pyx_GeneratorType, body, code, closure, name, qualname, module_name)
-static PyObject *__Pyx_Generator_Next(PyObject *self);
-static int __pyx_Generator_init(void);
-
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
+/* Module declarations from 'cython' */
+
 /* Module declarations from 'libc.math' */
 
 /* Module declarations from 'multimcts.mcts' */
-static PyTypeObject *__pyx_ptype_9multimcts_4mcts___pyx_scope_struct__get_best_child = 0;
-static PyTypeObject *__pyx_ptype_9multimcts_4mcts___pyx_scope_struct_1_genexpr = 0;
 #define __Pyx_MODULE_NAME "multimcts.mcts"
 extern int __pyx_module_is_main_multimcts__mcts;
 int __pyx_module_is_main_multimcts__mcts = 0;
 
 /* Implementation of 'multimcts.mcts' */
 static PyObject *__pyx_builtin_staticmethod;
 static PyObject *__pyx_builtin_NotImplementedError;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_IndexError;
-static PyObject *__pyx_builtin_sum;
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_k[] = "k";
 static const char __pyx_k_v[] = "v";
 static const char __pyx_k_Any[] = "Any";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_pop[] = "pop";
-static const char __pyx_k_sum[] = "sum";
+static const char __pyx_k_ucb[] = "ucb";
 static const char __pyx_k_MCTS[] = "MCTS";
 static const char __pyx_k_Node[] = "Node";
-static const char __pyx_k_args[] = "args";
-static const char __pyx_k_best[] = "best";
 static const char __pyx_k_dict[] = "dict";
 static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_move[] = "move";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_node[] = "node";
 static const char __pyx_k_self[] = "self";
-static const char __pyx_k_send[] = "send";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_time[] = "time";
 static const char __pyx_k_Union[] = "Union";
 static const char __pyx_k_child[] = "child";
-static const char __pyx_k_close[] = "close";
 static const char __pyx_k_float[] = "float";
 static const char __pyx_k_items[] = "items";
-static const char __pyx_k_score[] = "score";
 static const char __pyx_k_state[] = "state";
-static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_append[] = "append";
 static const char __pyx_k_choice[] = "choice";
 static const char __pyx_k_expand[] = "expand";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_parent[] = "parent";
 static const char __pyx_k_random[] = "random";
 static const char __pyx_k_return[] = "return";
 static const char __pyx_k_reward[] = "reward";
 static const char __pyx_k_search[] = "search";
 static const char __pyx_k_select[] = "select";
 static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_values[] = "values";
 static const char __pyx_k_visits[] = "visits";
-static const char __pyx_k_genexpr[] = "genexpr";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_shuffle[] = "shuffle";
 static const char __pyx_k_children[] = "children";
 static const char __pyx_k_cur_team[] = "cur_team";
 static const char __pyx_k_end_time[] = "end_time";
 static const char __pyx_k_max_time[] = "max_time";
 static const char __pyx_k_qualname[] = "__qualname__";
 static const char __pyx_k_simulate[] = "simulate";
 static const char __pyx_k_GameState[] = "GameState";
 static const char __pyx_k_heuristic[] = "heuristic";
 static const char __pyx_k_make_move[] = "make_move";
-static const char __pyx_k_max_score[] = "max_score";
 static const char __pyx_k_metaclass[] = "__metaclass__";
+static const char __pyx_k_subreward[] = "subreward";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
+static const char __pyx_k_best_child[] = "best_child";
+static const char __pyx_k_best_score[] = "best_score";
 static const char __pyx_k_get_reward[] = "get_reward";
 static const char __pyx_k_num_visits[] = "num_visits";
 static const char __pyx_k_MCTS___init[] = "MCTS.__init__";
 static const char __pyx_k_MCTS_expand[] = "MCTS.expand";
 static const char __pyx_k_MCTS_search[] = "MCTS.search";
 static const char __pyx_k_MCTS_select[] = "MCTS.select";
 static const char __pyx_k_Node___init[] = "Node.__init__";
@@ -1809,15 +1674,14 @@
 static const char __pyx_k_GameState_get_current_team[] = "GameState.get_current_team";
 static const char __pyx_k_Represents_a_game_state_node_in[] = "Represents a game state node in the MCTS search tree.\n\n    Args:\n        state (GameState): The game state at the current node.\n        parent (Node): The parent of the current node in the search tree.\n\n    Attributes:\n        children (list): The child nodes of the current node. These represent legal moves that have been visited.\n        num_visits (int): The number of times the node has been visited.\n        total_reward (dict): The total reward obtained from simulations through the node. Keys are teams; values are rewards.\n        is_terminal (bool): Whether the node represents a terminal state.\n        is_fully_expanded (bool): Whether all children of the node have been visited.\n        remaining_moves (list): A list of moves that have not yet been tried.\n    ";
 static const char __pyx_k_GameState_must_implement_get_cur[] = "GameState must implement get_current_team.";
 static const char __pyx_k_GameState_must_implement_get_leg[] = "GameState must implement get_legal_moves.";
 static const char __pyx_k_GameState_must_implement_get_rew[] = "GameState must implement get_reward.";
 static const char __pyx_k_GameState_must_implement_is_term[] = "GameState must implement is_terminal.";
 static const char __pyx_k_GameState_must_implement_make_mo[] = "GameState must implement make_move.";
-static const char __pyx_k_MCTS_get_best_child_locals_genex[] = "MCTS.get_best_child.<locals>.genexpr";
 static const char __pyx_k_One_or_more_of_max_time_max_iter[] = "One or more of max_time/max_iterations is required.";
 static const char __pyx_k_Tried_to_expand_a_node_with_no_r[] = "Tried to expand a node with no remaining moves.";
 static PyObject *__pyx_n_s_Any;
 static PyObject *__pyx_n_s_GameState;
 static PyObject *__pyx_n_s_GameState_get_current_team;
 static PyObject *__pyx_n_s_GameState_get_legal_moves;
 static PyObject *__pyx_n_s_GameState_get_reward;
@@ -1830,45 +1694,42 @@
 static PyObject *__pyx_kp_s_GameState_must_implement_make_mo;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_n_s_MCTS;
 static PyObject *__pyx_n_s_MCTS___init;
 static PyObject *__pyx_n_s_MCTS_backpropagate;
 static PyObject *__pyx_n_s_MCTS_expand;
 static PyObject *__pyx_n_s_MCTS_get_best_child;
-static PyObject *__pyx_n_s_MCTS_get_best_child_locals_genex;
 static PyObject *__pyx_n_s_MCTS_search;
 static PyObject *__pyx_n_s_MCTS_select;
 static PyObject *__pyx_n_s_MCTS_simulate;
 static PyObject *__pyx_n_s_Node;
 static PyObject *__pyx_n_s_Node___init;
 static PyObject *__pyx_n_s_NotImplementedError;
 static PyObject *__pyx_kp_s_One_or_more_of_max_time_max_iter;
 static PyObject *__pyx_kp_s_Represents_a_game_state_node_in;
 static PyObject *__pyx_kp_s_Tried_to_expand_a_node_with_no_r;
 static PyObject *__pyx_n_s_Union;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_append;
-static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_backpropagate;
-static PyObject *__pyx_n_s_best;
+static PyObject *__pyx_n_s_best_child;
+static PyObject *__pyx_n_s_best_score;
 static PyObject *__pyx_n_s_child;
 static PyObject *__pyx_n_s_children;
 static PyObject *__pyx_n_s_choice;
 static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_close;
 static PyObject *__pyx_n_s_collections;
 static PyObject *__pyx_n_s_cur_team;
 static PyObject *__pyx_n_s_defaultdict;
 static PyObject *__pyx_n_u_dict;
 static PyObject *__pyx_n_s_doc;
 static PyObject *__pyx_n_s_end_time;
 static PyObject *__pyx_n_s_expand;
 static PyObject *__pyx_n_s_exploration_bias;
 static PyObject *__pyx_n_u_float;
-static PyObject *__pyx_n_s_genexpr;
 static PyObject *__pyx_n_s_get_best_child;
 static PyObject *__pyx_n_s_get_current_team;
 static PyObject *__pyx_n_s_get_legal_moves;
 static PyObject *__pyx_n_s_get_reward;
 static PyObject *__pyx_n_s_heuristic;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_import;
@@ -1879,15 +1740,14 @@
 static PyObject *__pyx_n_s_items;
 static PyObject *__pyx_n_s_k;
 static PyObject *__pyx_n_s_key;
 static PyObject *__pyx_n_s_ln_parent_visits;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_make_move;
 static PyObject *__pyx_n_s_max_iterations;
-static PyObject *__pyx_n_s_max_score;
 static PyObject *__pyx_n_s_max_time;
 static PyObject *__pyx_n_s_metaclass;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_move;
 static PyObject *__pyx_n_s_multimcts_mcts;
 static PyObject *__pyx_kp_s_multimcts_mcts_pyx;
 static PyObject *__pyx_n_s_name;
@@ -1897,30 +1757,28 @@
 static PyObject *__pyx_n_s_pop;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_random;
 static PyObject *__pyx_n_s_remaining_moves;
 static PyObject *__pyx_n_s_return;
 static PyObject *__pyx_n_s_reward;
-static PyObject *__pyx_n_s_score;
 static PyObject *__pyx_n_s_search;
 static PyObject *__pyx_n_s_select;
 static PyObject *__pyx_n_s_self;
-static PyObject *__pyx_n_s_send;
 static PyObject *__pyx_n_s_shuffle;
 static PyObject *__pyx_n_s_simulate;
 static PyObject *__pyx_n_s_state;
 static PyObject *__pyx_n_s_staticmethod;
-static PyObject *__pyx_n_s_sum;
+static PyObject *__pyx_n_s_subreward;
 static PyObject *__pyx_n_s_terminal_team;
 static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_throw;
 static PyObject *__pyx_n_s_time;
 static PyObject *__pyx_n_s_total_reward;
 static PyObject *__pyx_n_s_typing;
+static PyObject *__pyx_n_s_ucb;
 static PyObject *__pyx_n_s_v;
 static PyObject *__pyx_n_s_values;
 static PyObject *__pyx_n_s_visits;
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_get_current_team(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_2get_legal_moves(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_4make_move(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_move); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_6is_terminal(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
@@ -1928,18 +1786,15 @@
 static PyObject *__pyx_pf_9multimcts_4mcts_4Node___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_parent); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_exploration_bias); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_2search(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_max_time, PyObject *__pyx_v_max_iterations, PyObject *__pyx_v_heuristic); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_4select(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_node); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_6expand(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_8simulate(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_node, PyObject *__pyx_v_heuristic); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node, PyObject *__pyx_v_reward); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_14get_best_child_genexpr(PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_node); /* proto */
-static PyObject *__pyx_tp_new_9multimcts_4mcts___pyx_scope_struct__get_best_child(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_9multimcts_4mcts___pyx_scope_struct_1_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_items = {0, &__pyx_n_s_items, 0, 0, 0};
 static __Pyx_CachedCFunction __pyx_umethod_PyList_Type_pop = {0, &__pyx_n_s_pop, 0, 0, 0};
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_2;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
@@ -1973,17 +1828,17 @@
 static PyObject *__pyx_codeobj__26;
 static PyObject *__pyx_codeobj__28;
 static PyObject *__pyx_codeobj__30;
 static PyObject *__pyx_codeobj__32;
 static PyObject *__pyx_codeobj__34;
 /* Late includes */
 
-/* "multimcts/mcts.pyx":10
+/* "multimcts/mcts.pyx":12
  * 
- * class GameState():
+ * class GameState:
  *     def get_current_team(self) -> Union[int,str]:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_1get_current_team(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
@@ -2005,30 +1860,30 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_current_team", 0);
 
-  /* "multimcts/mcts.pyx":12
+  /* "multimcts/mcts.pyx":14
  *     def get_current_team(self) -> Union[int,str]:
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")             # <<<<<<<<<<<<<<
  * 
  *     def get_legal_moves(self) -> list[Any]:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 12, __pyx_L1_error)
+  __PYX_ERR(0, 14, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":10
+  /* "multimcts/mcts.pyx":12
  * 
- * class GameState():
+ * class GameState:
  *     def get_current_team(self) -> Union[int,str]:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")
  */
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2036,15 +1891,15 @@
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_current_team", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":14
+/* "multimcts/mcts.pyx":16
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> list[Any]:             # <<<<<<<<<<<<<<
  *         """Returns a list of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
 
@@ -2068,28 +1923,28 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_legal_moves", 0);
 
-  /* "multimcts/mcts.pyx":16
+  /* "multimcts/mcts.pyx":18
  *     def get_legal_moves(self) -> list[Any]:
  *         """Returns a list of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")             # <<<<<<<<<<<<<<
  * 
  *     def make_move(self, move:Any) -> 'GameState':
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 16, __pyx_L1_error)
+  __PYX_ERR(0, 18, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":14
+  /* "multimcts/mcts.pyx":16
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> list[Any]:             # <<<<<<<<<<<<<<
  *         """Returns a list of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
 
@@ -2099,15 +1954,15 @@
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_legal_moves", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":18
+/* "multimcts/mcts.pyx":20
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Any) -> 'GameState':             # <<<<<<<<<<<<<<
  *         """Returns a new GameState, which is the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
 
@@ -2143,32 +1998,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_move)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("make_move", 1, 2, 2, 1); __PYX_ERR(0, 18, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("make_move", 1, 2, 2, 1); __PYX_ERR(0, 20, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "make_move") < 0)) __PYX_ERR(0, 18, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "make_move") < 0)) __PYX_ERR(0, 20, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_move = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("make_move", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 18, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("make_move", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 20, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.GameState.make_move", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_4make_move(__pyx_self, __pyx_v_self, __pyx_v_move);
 
@@ -2182,28 +2037,28 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("make_move", 0);
 
-  /* "multimcts/mcts.pyx":22
+  /* "multimcts/mcts.pyx":24
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  *         """
  *         raise NotImplementedError("GameState must implement make_move.")             # <<<<<<<<<<<<<<
  * 
  *     def is_terminal(self) -> bool:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 22, __pyx_L1_error)
+  __PYX_ERR(0, 24, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":18
+  /* "multimcts/mcts.pyx":20
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Any) -> 'GameState':             # <<<<<<<<<<<<<<
  *         """Returns a new GameState, which is the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
 
@@ -2213,15 +2068,15 @@
   __Pyx_AddTraceback("multimcts.mcts.GameState.make_move", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":24
+/* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
 
@@ -2245,28 +2100,28 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_terminal", 0);
 
-  /* "multimcts/mcts.pyx":26
+  /* "multimcts/mcts.pyx":28
  *     def is_terminal(self) -> bool:
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
  * 
  *     def get_reward(self) -> Union[float, dict[Union[int,str], float]]:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 26, __pyx_L1_error)
+  __PYX_ERR(0, 28, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":24
+  /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
 
@@ -2276,15 +2131,15 @@
   __Pyx_AddTraceback("multimcts.mcts.GameState.is_terminal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":28
+/* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float, dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
  *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
 
@@ -2308,28 +2163,28 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_reward", 0);
 
-  /* "multimcts/mcts.pyx":34
+  /* "multimcts/mcts.pyx":36
  *         Note: This method is only called on terminal states.
  *         """
  *         raise NotImplementedError("GameState must implement get_reward.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 34, __pyx_L1_error)
+  __PYX_ERR(0, 36, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":28
+  /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float, dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
  *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
 
@@ -2339,15 +2194,15 @@
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_reward", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":52
+/* "multimcts/mcts.pyx":54
  *         remaining_moves (list): A list of moves that have not yet been tried.
  *     """
  *     def __init__(self, state:GameState, parent:'Node'=None):             # <<<<<<<<<<<<<<
  *         self.state = state
  *         self.parent = parent
  */
 
@@ -2386,25 +2241,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_state)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 52, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 54, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parent);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 52, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 54, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -2414,15 +2269,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_state = values[1];
     __pyx_v_parent = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 52, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 54, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.Node.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4Node___init__(__pyx_self, __pyx_v_self, __pyx_v_state, __pyx_v_parent);
 
@@ -2440,220 +2295,220 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "multimcts/mcts.pyx":53
+  /* "multimcts/mcts.pyx":55
  *     """
  *     def __init__(self, state:GameState, parent:'Node'=None):
  *         self.state = state             # <<<<<<<<<<<<<<
  *         self.parent = parent
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_state, __pyx_v_state) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_state, __pyx_v_state) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":54
+  /* "multimcts/mcts.pyx":56
  *     def __init__(self, state:GameState, parent:'Node'=None):
  *         self.state = state
  *         self.parent = parent             # <<<<<<<<<<<<<<
  * 
  *         self.children:list['Node'] = []
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_parent, __pyx_v_parent) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_parent, __pyx_v_parent) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":56
+  /* "multimcts/mcts.pyx":58
  *         self.parent = parent
  * 
  *         self.children:list['Node'] = []             # <<<<<<<<<<<<<<
- *         self.num_visits:int = 0
+ *         self.num_visits = 0
  *         self.total_reward = defaultdict(float)
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_children, __pyx_t_1) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_children, __pyx_t_1) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":57
+  /* "multimcts/mcts.pyx":59
  * 
  *         self.children:list['Node'] = []
- *         self.num_visits:int = 0             # <<<<<<<<<<<<<<
+ *         self.num_visits = 0             # <<<<<<<<<<<<<<
  *         self.total_reward = defaultdict(float)
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_num_visits, __pyx_int_0) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_num_visits, __pyx_int_0) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":58
+  /* "multimcts/mcts.pyx":60
  *         self.children:list['Node'] = []
- *         self.num_visits:int = 0
+ *         self.num_visits = 0
  *         self.total_reward = defaultdict(float)             # <<<<<<<<<<<<<<
  * 
  *         self.is_terminal:bool = self.state.is_terminal()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)(&PyFloat_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)(&PyFloat_Type)));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_total_reward, __pyx_t_1) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_total_reward, __pyx_t_1) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":60
+  /* "multimcts/mcts.pyx":62
  *         self.total_reward = defaultdict(float)
  * 
  *         self.is_terminal:bool = self.state.is_terminal()             # <<<<<<<<<<<<<<
  *         self.is_fully_expanded:bool = self.is_terminal
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_is_terminal, __pyx_t_1) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_is_terminal, __pyx_t_1) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":61
+  /* "multimcts/mcts.pyx":63
  * 
  *         self.is_terminal:bool = self.state.is_terminal()
  *         self.is_fully_expanded:bool = self.is_terminal             # <<<<<<<<<<<<<<
  * 
  *         if self.is_fully_expanded:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_is_fully_expanded, __pyx_t_1) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_is_fully_expanded, __pyx_t_1) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":63
+  /* "multimcts/mcts.pyx":65
  *         self.is_fully_expanded:bool = self.is_terminal
  * 
  *         if self.is_fully_expanded:             # <<<<<<<<<<<<<<
  *             self.remaining_moves = []
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_4) {
 
-    /* "multimcts/mcts.pyx":64
+    /* "multimcts/mcts.pyx":66
  * 
  *         if self.is_fully_expanded:
  *             self.remaining_moves = []             # <<<<<<<<<<<<<<
  *         else:
  *             self.remaining_moves = self.state.get_legal_moves()
  */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_remaining_moves, __pyx_t_1) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_remaining_moves, __pyx_t_1) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":63
+    /* "multimcts/mcts.pyx":65
  *         self.is_fully_expanded:bool = self.is_terminal
  * 
  *         if self.is_fully_expanded:             # <<<<<<<<<<<<<<
  *             self.remaining_moves = []
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "multimcts/mcts.pyx":66
+  /* "multimcts/mcts.pyx":68
  *             self.remaining_moves = []
  *         else:
  *             self.remaining_moves = self.state.get_legal_moves()             # <<<<<<<<<<<<<<
  *             shuffle(self.remaining_moves)
  * 
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_state); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_state); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_remaining_moves, __pyx_t_1) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_remaining_moves, __pyx_t_1) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":67
+    /* "multimcts/mcts.pyx":69
  *         else:
  *             self.remaining_moves = self.state.get_legal_moves()
  *             shuffle(self.remaining_moves)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "multimcts/mcts.pyx":52
+  /* "multimcts/mcts.pyx":54
  *         remaining_moves (list): A list of moves that have not yet been tried.
  *     """
  *     def __init__(self, state:GameState, parent:'Node'=None):             # <<<<<<<<<<<<<<
  *         self.state = state
  *         self.parent = parent
  */
 
@@ -2669,17 +2524,17 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":71
+/* "multimcts/mcts.pyx":73
  * 
- * class MCTS():
+ * class MCTS:
  *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
@@ -2717,35 +2572,35 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exploration_bias);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 71, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 73, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_self = values[0];
     if (values[1]) {
-      __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 71, __pyx_L3_error)
+      __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L3_error)
     } else {
       __pyx_v_exploration_bias = ((double)((double)1.414));
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 71, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 73, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS___init__(__pyx_self, __pyx_v_self, __pyx_v_exploration_bias);
 
@@ -2759,29 +2614,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "multimcts/mcts.pyx":79
+  /* "multimcts/mcts.pyx":81
  *                 Default is 1.414, which is sqrt(2) and often used in practice.
  *         """
  *         self.exploration_bias = exploration_bias             # <<<<<<<<<<<<<<
  * 
  *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None) -> GameState:
  */
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_exploration_bias, __pyx_t_1) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_exploration_bias, __pyx_t_1) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":71
+  /* "multimcts/mcts.pyx":73
  * 
- * class MCTS():
+ * class MCTS:
  *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
@@ -2792,15 +2647,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":81
+/* "multimcts/mcts.pyx":83
  *         self.exploration_bias = exploration_bias
  * 
  *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None) -> GameState:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
  * 
  */
 
@@ -2842,26 +2697,26 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_state)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("search", 1, 2, 2, 1); __PYX_ERR(0, 81, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("search", 1, 2, 2, 1); __PYX_ERR(0, 83, __pyx_L3_error)
         }
       }
       if (kw_args > 0 && likely(kw_args <= 3)) {
         Py_ssize_t index;
         for (index = 2; index < 5 && kw_args > 0; index++) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search") < 0)) __PYX_ERR(0, 81, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search") < 0)) __PYX_ERR(0, 83, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
@@ -2869,15 +2724,15 @@
     __pyx_v_state = values[1];
     __pyx_v_max_time = values[2];
     __pyx_v_max_iterations = values[3];
     __pyx_v_heuristic = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("search", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 81, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("search", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 83, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_2search(__pyx_self, __pyx_v_self, __pyx_v_state, __pyx_v_max_time, __pyx_v_max_iterations, __pyx_v_heuristic);
 
@@ -2904,15 +2759,15 @@
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("search", 0);
 
-  /* "multimcts/mcts.pyx":92
+  /* "multimcts/mcts.pyx":94
  *             GameState: A new game state which is the result of applying the best move to the given state.
  *         """
  *         if max_time is None and max_iterations is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  */
   __pyx_t_2 = (__pyx_v_max_time == Py_None);
@@ -2924,213 +2779,213 @@
   }
   __pyx_t_3 = (__pyx_v_max_iterations == Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "multimcts/mcts.pyx":93
+    /* "multimcts/mcts.pyx":95
  *         """
  *         if max_time is None and max_iterations is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         node = Node(state)
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 93, __pyx_L1_error)
+    __PYX_ERR(0, 95, __pyx_L1_error)
 
-    /* "multimcts/mcts.pyx":92
+    /* "multimcts/mcts.pyx":94
  *             GameState: A new game state which is the result of applying the best move to the given state.
  *         """
  *         if max_time is None and max_iterations is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":95
+  /* "multimcts/mcts.pyx":97
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  *         node = Node(state)             # <<<<<<<<<<<<<<
  * 
  *         cdef double end_time
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Node); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Node); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_state) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_state);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_node = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":99
+  /* "multimcts/mcts.pyx":101
  *         cdef double end_time
  *         cdef int i
  *         if max_time is not None:             # <<<<<<<<<<<<<<
  *             end_time = time() + max_time
  *         if max_iterations is not None:
  */
   __pyx_t_1 = (__pyx_v_max_time != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "multimcts/mcts.pyx":100
+    /* "multimcts/mcts.pyx":102
  *         cdef int i
  *         if max_time is not None:
  *             end_time = time() + max_time             # <<<<<<<<<<<<<<
  *         if max_iterations is not None:
  *             i = max_iterations
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_time); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_time); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_v_max_time); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+    __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_v_max_time); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_7 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_7 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 100, __pyx_L1_error)
+    __pyx_t_7 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_7 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_end_time = __pyx_t_7;
 
-    /* "multimcts/mcts.pyx":99
+    /* "multimcts/mcts.pyx":101
  *         cdef double end_time
  *         cdef int i
  *         if max_time is not None:             # <<<<<<<<<<<<<<
  *             end_time = time() + max_time
  *         if max_iterations is not None:
  */
   }
 
-  /* "multimcts/mcts.pyx":101
+  /* "multimcts/mcts.pyx":103
  *         if max_time is not None:
  *             end_time = time() + max_time
  *         if max_iterations is not None:             # <<<<<<<<<<<<<<
  *             i = max_iterations
  * 
  */
   __pyx_t_2 = (__pyx_v_max_iterations != Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "multimcts/mcts.pyx":102
+    /* "multimcts/mcts.pyx":104
  *             end_time = time() + max_time
  *         if max_iterations is not None:
  *             i = max_iterations             # <<<<<<<<<<<<<<
  * 
  *         while True:
  */
-    __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_v_max_iterations); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 102, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_v_max_iterations); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 104, __pyx_L1_error)
     __pyx_v_i = __pyx_t_8;
 
-    /* "multimcts/mcts.pyx":101
+    /* "multimcts/mcts.pyx":103
  *         if max_time is not None:
  *             end_time = time() + max_time
  *         if max_iterations is not None:             # <<<<<<<<<<<<<<
  *             i = max_iterations
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":104
+  /* "multimcts/mcts.pyx":106
  *             i = max_iterations
  * 
  *         while True:             # <<<<<<<<<<<<<<
  *             child = self.select(node)
  *             reward = self.simulate(child, heuristic=heuristic)
  */
   while (1) {
 
-    /* "multimcts/mcts.pyx":105
+    /* "multimcts/mcts.pyx":107
  * 
  *         while True:
  *             child = self.select(node)             # <<<<<<<<<<<<<<
  *             reward = self.simulate(child, heuristic=heuristic)
  *             self.backpropagate(child, reward)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_select); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_select); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 107, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_6, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_node);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF_SET(__pyx_v_child, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "multimcts/mcts.pyx":106
+    /* "multimcts/mcts.pyx":108
  *         while True:
  *             child = self.select(node)
  *             reward = self.simulate(child, heuristic=heuristic)             # <<<<<<<<<<<<<<
  *             self.backpropagate(child, reward)
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_simulate); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 106, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_simulate); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_child);
     __Pyx_GIVEREF(__pyx_v_child);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_child);
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 106, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_heuristic, __pyx_v_heuristic) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 106, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_heuristic, __pyx_v_heuristic) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF_SET(__pyx_v_reward, __pyx_t_9);
     __pyx_t_9 = 0;
 
-    /* "multimcts/mcts.pyx":107
+    /* "multimcts/mcts.pyx":109
  *             child = self.select(node)
  *             reward = self.simulate(child, heuristic=heuristic)
  *             self.backpropagate(child, reward)             # <<<<<<<<<<<<<<
  * 
  *             if max_time is not None and time() >= end_time:
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_4 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -3139,198 +2994,198 @@
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_child, __pyx_v_reward};
-      __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 109, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_9);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_child, __pyx_v_reward};
-      __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 109, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_9);
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_4) {
         __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_INCREF(__pyx_v_child);
       __Pyx_GIVEREF(__pyx_v_child);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_8, __pyx_v_child);
       __Pyx_INCREF(__pyx_v_reward);
       __Pyx_GIVEREF(__pyx_v_reward);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_8, __pyx_v_reward);
-      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 109, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "multimcts/mcts.pyx":109
+    /* "multimcts/mcts.pyx":111
  *             self.backpropagate(child, reward)
  * 
  *             if max_time is not None and time() >= end_time:             # <<<<<<<<<<<<<<
  *                 break
  *             if max_iterations is not None:
  */
     __pyx_t_2 = (__pyx_v_max_time != Py_None);
     __pyx_t_3 = (__pyx_t_2 != 0);
     if (__pyx_t_3) {
     } else {
       __pyx_t_1 = __pyx_t_3;
       goto __pyx_L11_bool_binop_done;
     }
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_time); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_time); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_9 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 109, __pyx_L1_error)
+    if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyFloat_FromDouble(__pyx_v_end_time); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+    __pyx_t_6 = PyFloat_FromDouble(__pyx_v_end_time); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PyObject_RichCompare(__pyx_t_9, __pyx_t_6, Py_GE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
+    __pyx_t_5 = PyObject_RichCompare(__pyx_t_9, __pyx_t_6, Py_GE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 109, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_1 = __pyx_t_3;
     __pyx_L11_bool_binop_done:;
     if (__pyx_t_1) {
 
-      /* "multimcts/mcts.pyx":110
+      /* "multimcts/mcts.pyx":112
  * 
  *             if max_time is not None and time() >= end_time:
  *                 break             # <<<<<<<<<<<<<<
  *             if max_iterations is not None:
  *                 i -= 1
  */
       goto __pyx_L9_break;
 
-      /* "multimcts/mcts.pyx":109
+      /* "multimcts/mcts.pyx":111
  *             self.backpropagate(child, reward)
  * 
  *             if max_time is not None and time() >= end_time:             # <<<<<<<<<<<<<<
  *                 break
  *             if max_iterations is not None:
  */
     }
 
-    /* "multimcts/mcts.pyx":111
+    /* "multimcts/mcts.pyx":113
  *             if max_time is not None and time() >= end_time:
  *                 break
  *             if max_iterations is not None:             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 if i <= 0:
  */
     __pyx_t_1 = (__pyx_v_max_iterations != Py_None);
     __pyx_t_3 = (__pyx_t_1 != 0);
     if (__pyx_t_3) {
 
-      /* "multimcts/mcts.pyx":112
+      /* "multimcts/mcts.pyx":114
  *                 break
  *             if max_iterations is not None:
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 if i <= 0:
  *                     break
  */
       __pyx_v_i = (__pyx_v_i - 1);
 
-      /* "multimcts/mcts.pyx":113
+      /* "multimcts/mcts.pyx":115
  *             if max_iterations is not None:
  *                 i -= 1
  *                 if i <= 0:             # <<<<<<<<<<<<<<
  *                     break
  * 
  */
       __pyx_t_3 = ((__pyx_v_i <= 0) != 0);
       if (__pyx_t_3) {
 
-        /* "multimcts/mcts.pyx":114
+        /* "multimcts/mcts.pyx":116
  *                 i -= 1
  *                 if i <= 0:
  *                     break             # <<<<<<<<<<<<<<
  * 
  *         return self.get_best_child(node).state
  */
         goto __pyx_L9_break;
 
-        /* "multimcts/mcts.pyx":113
+        /* "multimcts/mcts.pyx":115
  *             if max_iterations is not None:
  *                 i -= 1
  *                 if i <= 0:             # <<<<<<<<<<<<<<
  *                     break
  * 
  */
       }
 
-      /* "multimcts/mcts.pyx":111
+      /* "multimcts/mcts.pyx":113
  *             if max_time is not None and time() >= end_time:
  *                 break
  *             if max_iterations is not None:             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 if i <= 0:
  */
     }
   }
   __pyx_L9_break:;
 
-  /* "multimcts/mcts.pyx":116
+  /* "multimcts/mcts.pyx":118
  *                     break
  * 
  *         return self.get_best_child(node).state             # <<<<<<<<<<<<<<
  * 
  *     def select(self, node:Node) -> Node:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_9, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_node);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_state); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_state); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":81
+  /* "multimcts/mcts.pyx":83
  *         self.exploration_bias = exploration_bias
  * 
  *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None) -> GameState:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
  * 
  */
 
@@ -3347,15 +3202,15 @@
   __Pyx_XDECREF(__pyx_v_child);
   __Pyx_XDECREF(__pyx_v_reward);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":118
+/* "multimcts/mcts.pyx":120
  *         return self.get_best_child(node).state
  * 
  *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
@@ -3391,32 +3246,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, 1); __PYX_ERR(0, 118, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, 1); __PYX_ERR(0, 120, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "select") < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "select") < 0)) __PYX_ERR(0, 120, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_node = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 118, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 120, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.select", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_4select(__pyx_self, __pyx_v_self, __pyx_v_node);
 
@@ -3435,124 +3290,124 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("select", 0);
   __Pyx_INCREF(__pyx_v_node);
 
-  /* "multimcts/mcts.pyx":123
+  /* "multimcts/mcts.pyx":125
  *         Looks for an unexplored child of this node's best child's best child's...best child.
  *         """
  *         while not node.is_terminal:             # <<<<<<<<<<<<<<
  *             if not node.is_fully_expanded:
  *                 return self.expand(node)
  */
   while (1) {
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_3 = ((!__pyx_t_2) != 0);
     if (!__pyx_t_3) break;
 
-    /* "multimcts/mcts.pyx":124
+    /* "multimcts/mcts.pyx":126
  *         """
  *         while not node.is_terminal:
  *             if not node.is_fully_expanded:             # <<<<<<<<<<<<<<
  *                 return self.expand(node)
  *             else:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_2 = ((!__pyx_t_3) != 0);
     if (__pyx_t_2) {
 
-      /* "multimcts/mcts.pyx":125
+      /* "multimcts/mcts.pyx":127
  *         while not node.is_terminal:
  *             if not node.is_fully_expanded:
  *                 return self.expand(node)             # <<<<<<<<<<<<<<
  *             else:
  *                 node = self.get_best_child(node)
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_expand); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_expand); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_node);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_1;
       __pyx_t_1 = 0;
       goto __pyx_L0;
 
-      /* "multimcts/mcts.pyx":124
+      /* "multimcts/mcts.pyx":126
  *         """
  *         while not node.is_terminal:
  *             if not node.is_fully_expanded:             # <<<<<<<<<<<<<<
  *                 return self.expand(node)
  *             else:
  */
     }
 
-    /* "multimcts/mcts.pyx":127
+    /* "multimcts/mcts.pyx":129
  *                 return self.expand(node)
  *             else:
  *                 node = self.get_best_child(node)             # <<<<<<<<<<<<<<
  * 
  *         return node
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_node);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF_SET(__pyx_v_node, __pyx_t_1);
       __pyx_t_1 = 0;
     }
   }
 
-  /* "multimcts/mcts.pyx":129
+  /* "multimcts/mcts.pyx":131
  *                 node = self.get_best_child(node)
  * 
  *         return node             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_node);
   __pyx_r = __pyx_v_node;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":118
+  /* "multimcts/mcts.pyx":120
  *         return self.get_best_child(node).state
  * 
  *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
@@ -3566,15 +3421,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_node);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":132
+/* "multimcts/mcts.pyx":134
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
 
@@ -3611,15 +3466,15 @@
   Py_ssize_t __pyx_t_11;
   int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expand", 0);
 
-  /* "multimcts/mcts.pyx":136
+  /* "multimcts/mcts.pyx":138
  *         Add a new child to this node.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             move = node.remaining_moves.pop()
  *         except IndexError:
  */
   {
@@ -3627,30 +3482,30 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "multimcts/mcts.pyx":137
+      /* "multimcts/mcts.pyx":139
  *         """
  *         try:
  *             move = node.remaining_moves.pop()             # <<<<<<<<<<<<<<
  *         except IndexError:
  *             raise IndexError("Tried to expand a node with no remaining moves.")
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 137, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_Pop(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 137, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_Pop(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 139, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v_move = __pyx_t_5;
       __pyx_t_5 = 0;
 
-      /* "multimcts/mcts.pyx":136
+      /* "multimcts/mcts.pyx":138
  *         Add a new child to this node.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             move = node.remaining_moves.pop()
  *         except IndexError:
  */
     }
@@ -3658,87 +3513,87 @@
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "multimcts/mcts.pyx":138
+    /* "multimcts/mcts.pyx":140
  *         try:
  *             move = node.remaining_moves.pop()
  *         except IndexError:             # <<<<<<<<<<<<<<
  *             raise IndexError("Tried to expand a node with no remaining moves.")
  * 
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError);
     if (__pyx_t_6) {
       __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 138, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 140, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "multimcts/mcts.pyx":139
+      /* "multimcts/mcts.pyx":141
  *             move = node.remaining_moves.pop()
  *         except IndexError:
  *             raise IndexError("Tried to expand a node with no remaining moves.")             # <<<<<<<<<<<<<<
  * 
  *         child = Node(node.state.make_move(move), node)
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 139, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 141, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(0, 139, __pyx_L5_except_error)
+      __PYX_ERR(0, 141, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "multimcts/mcts.pyx":136
+    /* "multimcts/mcts.pyx":138
  *         Add a new child to this node.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             move = node.remaining_moves.pop()
  *         except IndexError:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "multimcts/mcts.pyx":141
+  /* "multimcts/mcts.pyx":143
  *             raise IndexError("Tried to expand a node with no remaining moves.")
  * 
  *         child = Node(node.state.make_move(move), node)             # <<<<<<<<<<<<<<
  *         node.children.append(child)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_make_move); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_make_move); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_9, function);
     }
   }
   __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_8, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_move);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_t_9 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_9)) {
@@ -3748,106 +3603,106 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_5, __pyx_v_node};
-    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 141, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_5, __pyx_v_node};
-    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 141, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 141, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_9) {
       __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_9); __pyx_t_9 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_v_node);
     __Pyx_GIVEREF(__pyx_v_node);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_6, __pyx_v_node);
     __pyx_t_5 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 141, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_child = __pyx_t_7;
   __pyx_t_7 = 0;
 
-  /* "multimcts/mcts.pyx":142
+  /* "multimcts/mcts.pyx":144
  * 
  *         child = Node(node.state.make_move(move), node)
  *         node.children.append(child)             # <<<<<<<<<<<<<<
  * 
  *         if len(node.remaining_moves) == 0:
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_10 = __Pyx_PyObject_Append(__pyx_t_7, __pyx_v_child); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_Append(__pyx_t_7, __pyx_v_child); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "multimcts/mcts.pyx":144
+  /* "multimcts/mcts.pyx":146
  *         node.children.append(child)
  * 
  *         if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
  *             node.is_fully_expanded = True
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_11 = PyObject_Length(__pyx_t_7); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_11 = PyObject_Length(__pyx_t_7); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_12 = ((__pyx_t_11 == 0) != 0);
   if (__pyx_t_12) {
 
-    /* "multimcts/mcts.pyx":145
+    /* "multimcts/mcts.pyx":147
  * 
  *         if len(node.remaining_moves) == 0:
  *             node.is_fully_expanded = True             # <<<<<<<<<<<<<<
  * 
  *         return child
  */
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded, Py_True) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded, Py_True) < 0) __PYX_ERR(0, 147, __pyx_L1_error)
 
-    /* "multimcts/mcts.pyx":144
+    /* "multimcts/mcts.pyx":146
  *         node.children.append(child)
  * 
  *         if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
  *             node.is_fully_expanded = True
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":147
+  /* "multimcts/mcts.pyx":149
  *             node.is_fully_expanded = True
  * 
  *         return child             # <<<<<<<<<<<<<<
  * 
  *     def simulate(self, node:Node, *, heuristic=None) -> dict[Union[int,str], float]:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_child);
   __pyx_r = __pyx_v_child;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":132
+  /* "multimcts/mcts.pyx":134
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
 
@@ -3864,15 +3719,15 @@
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF(__pyx_v_child);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":149
+/* "multimcts/mcts.pyx":151
  *         return child
  * 
  *     def simulate(self, node:Node, *, heuristic=None) -> dict[Union[int,str], float]:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout/rollout)
  *         Play out a game, from the given node to termination, and return the final reward.
  */
 
@@ -3910,38 +3765,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, 1); __PYX_ERR(0, 149, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, 1); __PYX_ERR(0, 151, __pyx_L3_error)
         }
       }
       if (kw_args == 1) {
         const Py_ssize_t index = 2;
         PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
         if (value) { values[index] = value; kw_args--; }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulate") < 0)) __PYX_ERR(0, 149, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulate") < 0)) __PYX_ERR(0, 151, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_node = values[1];
     __pyx_v_heuristic = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 149, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 151, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_8simulate(__pyx_self, __pyx_v_self, __pyx_v_node, __pyx_v_heuristic);
 
@@ -3965,152 +3820,152 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("simulate", 0);
 
-  /* "multimcts/mcts.pyx":158
+  /* "multimcts/mcts.pyx":160
  *             heuristic (callable): A function that takes a state and returns a move.
  *         """
  *         state = node.state             # <<<<<<<<<<<<<<
  * 
  *         if node.is_terminal:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_state = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":160
+  /* "multimcts/mcts.pyx":162
  *         state = node.state
  * 
  *         if node.is_terminal:             # <<<<<<<<<<<<<<
  *             terminal_team = node.parent.state.get_current_team()
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "multimcts/mcts.pyx":161
+    /* "multimcts/mcts.pyx":163
  * 
  *         if node.is_terminal:
  *             terminal_team = node.parent.state.get_current_team()             # <<<<<<<<<<<<<<
  *         else:
  *             while not state.is_terminal():
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_state); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_state); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_terminal_team = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":160
+    /* "multimcts/mcts.pyx":162
  *         state = node.state
  * 
  *         if node.is_terminal:             # <<<<<<<<<<<<<<
  *             terminal_team = node.parent.state.get_current_team()
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "multimcts/mcts.pyx":163
+  /* "multimcts/mcts.pyx":165
  *             terminal_team = node.parent.state.get_current_team()
  *         else:
  *             while not state.is_terminal():             # <<<<<<<<<<<<<<
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:
  */
   /*else*/ {
     while (1) {
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 165, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_5 = ((!__pyx_t_2) != 0);
       if (!__pyx_t_5) break;
 
-      /* "multimcts/mcts.pyx":164
+      /* "multimcts/mcts.pyx":166
  *         else:
  *             while not state.is_terminal():
  *                 terminal_team = state.get_current_team()             # <<<<<<<<<<<<<<
  *                 if heuristic is not None:
  *                     move = heuristic(state)
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_terminal_team, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "multimcts/mcts.pyx":165
+      /* "multimcts/mcts.pyx":167
  *             while not state.is_terminal():
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:             # <<<<<<<<<<<<<<
  *                     move = heuristic(state)
  *                 else:
  */
       __pyx_t_5 = (__pyx_v_heuristic != Py_None);
       __pyx_t_2 = (__pyx_t_5 != 0);
       if (__pyx_t_2) {
 
-        /* "multimcts/mcts.pyx":166
+        /* "multimcts/mcts.pyx":168
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:
  *                     move = heuristic(state)             # <<<<<<<<<<<<<<
  *                 else:
  *                     move = choice(state.get_legal_moves())
  */
         __Pyx_INCREF(__pyx_v_heuristic);
@@ -4122,55 +3977,55 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_state) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_state);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF_SET(__pyx_v_move, __pyx_t_1);
         __pyx_t_1 = 0;
 
-        /* "multimcts/mcts.pyx":165
+        /* "multimcts/mcts.pyx":167
  *             while not state.is_terminal():
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:             # <<<<<<<<<<<<<<
  *                     move = heuristic(state)
  *                 else:
  */
         goto __pyx_L6;
       }
 
-      /* "multimcts/mcts.pyx":168
+      /* "multimcts/mcts.pyx":170
  *                     move = heuristic(state)
  *                 else:
  *                     move = choice(state.get_legal_moves())             # <<<<<<<<<<<<<<
  *                 state = state.make_move(move)
  * 
  */
       /*else*/ {
-        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_choice); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_choice); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 170, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 168, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 170, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_7 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
             __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_6, function);
           }
         }
         __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 168, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 170, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_t_6 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_6)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -4178,126 +4033,126 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF_SET(__pyx_v_move, __pyx_t_1);
         __pyx_t_1 = 0;
       }
       __pyx_L6:;
 
-      /* "multimcts/mcts.pyx":169
+      /* "multimcts/mcts.pyx":171
  *                 else:
  *                     move = choice(state.get_legal_moves())
  *                 state = state.make_move(move)             # <<<<<<<<<<<<<<
  * 
  *         reward = state.get_reward()
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 171, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_move);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF_SET(__pyx_v_state, __pyx_t_1);
       __pyx_t_1 = 0;
     }
   }
   __pyx_L3:;
 
-  /* "multimcts/mcts.pyx":171
+  /* "multimcts/mcts.pyx":173
  *                 state = state.make_move(move)
  * 
  *         reward = state.get_reward()             # <<<<<<<<<<<<<<
  *         if not isinstance(reward, dict):
  *             reward = {terminal_team: reward}
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_reward = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":172
+  /* "multimcts/mcts.pyx":174
  * 
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):             # <<<<<<<<<<<<<<
  *             reward = {terminal_team: reward}
  * 
  */
   __pyx_t_2 = PyDict_Check(__pyx_v_reward); 
   __pyx_t_5 = ((!(__pyx_t_2 != 0)) != 0);
   if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":173
+    /* "multimcts/mcts.pyx":175
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):
  *             reward = {terminal_team: reward}             # <<<<<<<<<<<<<<
  * 
  *         return reward
  */
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(!__pyx_v_terminal_team)) { __Pyx_RaiseUnboundLocalError("terminal_team"); __PYX_ERR(0, 173, __pyx_L1_error) }
-    if (PyDict_SetItem(__pyx_t_1, __pyx_v_terminal_team, __pyx_v_reward) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
+    if (unlikely(!__pyx_v_terminal_team)) { __Pyx_RaiseUnboundLocalError("terminal_team"); __PYX_ERR(0, 175, __pyx_L1_error) }
+    if (PyDict_SetItem(__pyx_t_1, __pyx_v_terminal_team, __pyx_v_reward) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_reward, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":172
+    /* "multimcts/mcts.pyx":174
  * 
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):             # <<<<<<<<<<<<<<
  *             reward = {terminal_team: reward}
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":175
+  /* "multimcts/mcts.pyx":177
  *             reward = {terminal_team: reward}
  * 
  *         return reward             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_reward);
   __pyx_r = __pyx_v_reward;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":149
+  /* "multimcts/mcts.pyx":151
  *         return child
  * 
  *     def simulate(self, node:Node, *, heuristic=None) -> dict[Union[int,str], float]:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout/rollout)
  *         Play out a game, from the given node to termination, and return the final reward.
  */
 
@@ -4316,15 +4171,15 @@
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF(__pyx_v_reward);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":178
+/* "multimcts/mcts.pyx":180
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:dict):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
@@ -4360,38 +4215,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reward)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, 1); __PYX_ERR(0, 178, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, 1); __PYX_ERR(0, 180, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "backpropagate") < 0)) __PYX_ERR(0, 178, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "backpropagate") < 0)) __PYX_ERR(0, 180, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_node = values[0];
     __pyx_v_reward = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 178, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 180, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.backpropagate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_reward), (&PyDict_Type), 1, "reward", 1))) __PYX_ERR(0, 178, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_reward), (&PyDict_Type), 1, "reward", 1))) __PYX_ERR(0, 180, __pyx_L1_error)
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(__pyx_self, __pyx_v_node, __pyx_v_reward);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4422,126 +4277,126 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("backpropagate", 0);
   __Pyx_INCREF(__pyx_v_node);
   __Pyx_INCREF(__pyx_v_reward);
 
-  /* "multimcts/mcts.pyx":183
+  /* "multimcts/mcts.pyx":185
  *         """
  *         # Remove 0-values for efficiency
  *         reward = {k:v for k,v in reward.items() if v!=0}             # <<<<<<<<<<<<<<
  * 
  *         while node is not None:
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L5_error)
+    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(__pyx_v_reward == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 183, __pyx_L5_error)
+      __PYX_ERR(0, 185, __pyx_L5_error)
     }
-    __pyx_t_2 = __Pyx_PyDict_Items(__pyx_v_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L5_error)
+    __pyx_t_2 = __Pyx_PyDict_Items(__pyx_v_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
       __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
       __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L5_error)
+      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L5_error)
+      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     for (;;) {
       if (likely(!__pyx_t_5)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 183, __pyx_L5_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 185, __pyx_L5_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L5_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 183, __pyx_L5_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 185, __pyx_L5_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L5_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_5(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 183, __pyx_L5_error)
+            else __PYX_ERR(0, 185, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
         PyObject* sequence = __pyx_t_2;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 183, __pyx_L5_error)
+          __PYX_ERR(0, 185, __pyx_L5_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         #else
-        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 183, __pyx_L5_error)
+        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 185, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 183, __pyx_L5_error)
+        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 185, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_8 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 183, __pyx_L5_error)
+        __pyx_t_8 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 185, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_9 = Py_TYPE(__pyx_t_8)->tp_iternext;
         index = 0; __pyx_t_6 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_6)) goto __pyx_L8_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_6);
         index = 1; __pyx_t_7 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_7)) goto __pyx_L8_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_7);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 183, __pyx_L5_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 185, __pyx_L5_error)
         __pyx_t_9 = NULL;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L9_unpacking_done;
         __pyx_L8_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __pyx_t_9 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 183, __pyx_L5_error)
+        __PYX_ERR(0, 185, __pyx_L5_error)
         __pyx_L9_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_k, __pyx_t_6);
       __pyx_t_6 = 0;
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_v, __pyx_t_7);
       __pyx_t_7 = 0;
-      __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_7genexpr__pyx_v_v, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L5_error)
+      __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_7genexpr__pyx_v_v, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 183, __pyx_L5_error)
+      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 185, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_10) {
-        if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_k, (PyObject*)__pyx_7genexpr__pyx_v_v))) __PYX_ERR(0, 183, __pyx_L5_error)
+        if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_k, (PyObject*)__pyx_7genexpr__pyx_v_v))) __PYX_ERR(0, 185, __pyx_L5_error)
       }
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_k); __pyx_7genexpr__pyx_v_k = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
     goto __pyx_L11_exit_scope;
     __pyx_L5_error:;
@@ -4549,102 +4404,102 @@
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L11_exit_scope:;
   } /* exit inner scope */
   __Pyx_DECREF_SET(__pyx_v_reward, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":185
+  /* "multimcts/mcts.pyx":187
  *         reward = {k:v for k,v in reward.items() if v!=0}
  * 
  *         while node is not None:             # <<<<<<<<<<<<<<
  *             node.num_visits += 1
  * 
  */
   while (1) {
     __pyx_t_10 = (__pyx_v_node != Py_None);
     __pyx_t_11 = (__pyx_t_10 != 0);
     if (!__pyx_t_11) break;
 
-    /* "multimcts/mcts.pyx":186
+    /* "multimcts/mcts.pyx":188
  * 
  *         while node is not None:
  *             node.num_visits += 1             # <<<<<<<<<<<<<<
  * 
  *             for key in reward:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_num_visits, __pyx_t_3) < 0) __PYX_ERR(0, 186, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_num_visits, __pyx_t_3) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":188
+    /* "multimcts/mcts.pyx":190
  *             node.num_visits += 1
  * 
  *             for key in reward:             # <<<<<<<<<<<<<<
  *                 node.total_reward[key] += reward[key]
  * 
  */
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_reward, 1, ((PyObject *)NULL), (&__pyx_t_12), (&__pyx_t_13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_reward, 1, ((PyObject *)NULL), (&__pyx_t_12), (&__pyx_t_13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_1;
     __pyx_t_1 = 0;
     while (1) {
       __pyx_t_14 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_12, &__pyx_t_4, &__pyx_t_1, NULL, NULL, __pyx_t_13);
       if (unlikely(__pyx_t_14 == 0)) break;
-      if (unlikely(__pyx_t_14 == -1)) __PYX_ERR(0, 188, __pyx_L1_error)
+      if (unlikely(__pyx_t_14 == -1)) __PYX_ERR(0, 190, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "multimcts/mcts.pyx":189
+      /* "multimcts/mcts.pyx":191
  * 
  *             for key in reward:
  *                 node.total_reward[key] += reward[key]             # <<<<<<<<<<<<<<
  * 
  *             node = node.parent
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_key);
       __pyx_t_2 = __pyx_v_key;
-      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 189, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 191, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_reward, __pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 189, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_reward, __pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_8 = PyNumber_InPlaceAdd(__pyx_t_7, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 189, __pyx_L1_error)
+      __pyx_t_8 = PyNumber_InPlaceAdd(__pyx_t_7, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 191, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_2, __pyx_t_8) < 0)) __PYX_ERR(0, 189, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_2, __pyx_t_8) < 0)) __PYX_ERR(0, 191, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":191
+    /* "multimcts/mcts.pyx":193
  *                 node.total_reward[key] += reward[key]
  * 
  *             node = node.parent             # <<<<<<<<<<<<<<
  * 
- *     def get_best_child(self, node:Node) -> Node:
+ *     @cython.cdivision(True)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF_SET(__pyx_v_node, __pyx_t_3);
     __pyx_t_3 = 0;
   }
 
-  /* "multimcts/mcts.pyx":178
+  /* "multimcts/mcts.pyx":180
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:dict):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
@@ -4667,25 +4522,26 @@
   __Pyx_XDECREF(__pyx_v_node);
   __Pyx_XDECREF(__pyx_v_reward);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":193
- *             node = node.parent
+/* "multimcts/mcts.pyx":196
  * 
+ *     @cython.cdivision(True)
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         cur_team = node.state.get_current_team()
- * 
+ *         """Find the child with the highest Upper Confidence Bound (UCB) score.
+ *         ucb = (x / n) + C * sqrt(ln(N) / n)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_13get_best_child = {"get_best_child", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child, METH_VARARGS|METH_KEYWORDS, 0};
+static char __pyx_doc_9multimcts_4mcts_4MCTS_12get_best_child[] = "Find the child with the highest Upper Confidence Bound (UCB) score.\n        ucb = (x / n) + C * sqrt(ln(N) / n)\n        x=reward for this node\n        n=number of simulations for this node\n        N=number of simulations for parent node\n        C=exploration bias\n        ";
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_13get_best_child = {"get_best_child", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_12get_best_child};
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_node = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -4710,768 +4566,443 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, 1); __PYX_ERR(0, 193, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, 1); __PYX_ERR(0, 196, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_best_child") < 0)) __PYX_ERR(0, 193, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_best_child") < 0)) __PYX_ERR(0, 196, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_node = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 193, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 196, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.get_best_child", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(__pyx_self, __pyx_v_self, __pyx_v_node);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_9multimcts_4mcts_4MCTS_14get_best_child_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
-
-/* "multimcts/mcts.pyx":207
- *         for child in node.children:
- *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())             # <<<<<<<<<<<<<<
- *             visits = child.num_visits
- * 
- */
-
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_14get_best_child_genexpr(PyObject *__pyx_self) {
-  struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *__pyx_cur_scope;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("genexpr", 0);
-  __pyx_cur_scope = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *)__pyx_tp_new_9multimcts_4mcts___pyx_scope_struct_1_genexpr(__pyx_ptype_9multimcts_4mcts___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
-  if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *)Py_None);
-    __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 207, __pyx_L1_error)
-  } else {
-    __Pyx_GOTREF(__pyx_cur_scope);
-  }
-  __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *) __pyx_self;
-  __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
-  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
-  {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_9multimcts_4mcts_4MCTS_14get_best_child_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_MCTS_get_best_child_locals_genex, __pyx_n_s_multimcts_mcts); if (unlikely(!gen)) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_cur_scope);
-    __Pyx_RefNannyFinishContext();
-    return (PyObject *) gen;
-  }
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.get_best_child.genexpr", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_gb_9multimcts_4mcts_4MCTS_14get_best_child_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
-{
-  struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *__pyx_cur_scope = ((struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *)__pyx_generator->closure);
-  PyObject *__pyx_r = NULL;
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  Py_ssize_t __pyx_t_4;
-  PyObject *(*__pyx_t_5)(PyObject *);
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("genexpr", 0);
-  switch (__pyx_generator->resume_label) {
-    case 0: goto __pyx_L3_first_run;
-    case 1: goto __pyx_L6_resume_from_yield;
-    default: /* CPython raises the right error here */
-    __Pyx_RefNannyFinishContext();
-    return NULL;
-  }
-  __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 207, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_child)) { __Pyx_RaiseClosureNameError("child"); __PYX_ERR(0, 207, __pyx_L1_error) }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 207, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
-    __pyx_t_3 = __pyx_t_1; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
-    __pyx_t_5 = NULL;
-  } else {
-    __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 207, __pyx_L1_error)
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  for (;;) {
-    if (likely(!__pyx_t_5)) {
-      if (likely(PyList_CheckExact(__pyx_t_3))) {
-        if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 207, __pyx_L1_error)
-        #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        #endif
-      } else {
-        if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 207, __pyx_L1_error)
-        #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        #endif
-      }
-    } else {
-      __pyx_t_1 = __pyx_t_5(__pyx_t_3);
-      if (unlikely(!__pyx_t_1)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 207, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_1);
-    }
-    __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_x);
-    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_x, __pyx_t_1);
-    __Pyx_GIVEREF(__pyx_t_1);
-    __pyx_t_1 = 0;
-    __Pyx_INCREF(__pyx_cur_scope->__pyx_v_x);
-    __pyx_r = __pyx_cur_scope->__pyx_v_x;
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __pyx_cur_scope->__pyx_t_0 = __pyx_t_3;
-    __pyx_cur_scope->__pyx_t_1 = __pyx_t_4;
-    __pyx_cur_scope->__pyx_t_2 = __pyx_t_5;
-    __Pyx_XGIVEREF(__pyx_r);
-    __Pyx_RefNannyFinishContext();
-    __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
-    /* return from generator, yielding value */
-    __pyx_generator->resume_label = 1;
-    return __pyx_r;
-    __pyx_L6_resume_from_yield:;
-    __pyx_t_3 = __pyx_cur_scope->__pyx_t_0;
-    __pyx_cur_scope->__pyx_t_0 = 0;
-    __Pyx_XGOTREF(__pyx_t_3);
-    __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
-    __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 207, __pyx_L1_error)
-  }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
-
-  /* function exit code */
-  PyErr_SetNone(PyExc_StopIteration);
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("genexpr", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
-  #if !CYTHON_USE_EXC_INFO_STACK
-  __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
-  #endif
-  __pyx_generator->resume_label = -1;
-  __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "multimcts/mcts.pyx":193
- *             node = node.parent
- * 
- *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         cur_team = node.state.get_current_team()
- * 
- */
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_node) {
-  struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *__pyx_cur_scope;
-  PyObject *__pyx_v_cur_team = NULL;
   int __pyx_v_visits;
   double __pyx_v_reward;
-  double __pyx_v_score;
+  double __pyx_v_subreward;
+  double __pyx_v_ucb;
   double __pyx_v_exploration_bias;
   double __pyx_v_ln_parent_visits;
-  double __pyx_v_max_score;
-  PyObject *__pyx_v_best = NULL;
-  PyObject *__pyx_gb_9multimcts_4mcts_4MCTS_14get_best_child_2generator = 0;
+  PyObject *__pyx_v_cur_team = NULL;
+  double __pyx_v_best_score;
+  PyObject *__pyx_v_best_child = NULL;
+  PyObject *__pyx_v_child = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
+  double __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
-  double __pyx_t_4;
+  PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
   PyObject *(*__pyx_t_6)(PyObject *);
-  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_7;
   int __pyx_t_8;
-  int __pyx_t_9;
+  PyObject *__pyx_t_9 = NULL;
+  Py_ssize_t __pyx_t_10;
+  PyObject *(*__pyx_t_11)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_best_child", 0);
-  __pyx_cur_scope = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *)__pyx_tp_new_9multimcts_4mcts___pyx_scope_struct__get_best_child(__pyx_ptype_9multimcts_4mcts___pyx_scope_struct__get_best_child, __pyx_empty_tuple, NULL);
-  if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *)Py_None);
-    __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 193, __pyx_L1_error)
-  } else {
-    __Pyx_GOTREF(__pyx_cur_scope);
-  }
 
-  /* "multimcts/mcts.pyx":194
- * 
- *     def get_best_child(self, node:Node) -> Node:
- *         cur_team = node.state.get_current_team()             # <<<<<<<<<<<<<<
- * 
- *         # Initialize UCB variables.
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 194, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_cur_team = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "multimcts/mcts.pyx":199
+  /* "multimcts/mcts.pyx":207
  *         cdef int visits
- *         cdef double reward, score
+ *         cdef double reward, subreward, ucb
  *         cdef double exploration_bias = self.exploration_bias             # <<<<<<<<<<<<<<
  *         cdef double ln_parent_visits = log(node.num_visits)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_exploration_bias = __pyx_t_4;
+  __pyx_v_exploration_bias = __pyx_t_2;
 
-  /* "multimcts/mcts.pyx":200
- *         cdef double reward, score
+  /* "multimcts/mcts.pyx":208
+ *         cdef double reward, subreward, ucb
  *         cdef double exploration_bias = self.exploration_bias
  *         cdef double ln_parent_visits = log(node.num_visits)             # <<<<<<<<<<<<<<
  * 
- *         cdef double max_score = -INFINITY
+ *         cur_team = node.state.get_current_team()
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_ln_parent_visits = log(__pyx_t_4);
+  __pyx_v_ln_parent_visits = log(__pyx_t_2);
 
-  /* "multimcts/mcts.pyx":202
+  /* "multimcts/mcts.pyx":210
  *         cdef double ln_parent_visits = log(node.num_visits)
  * 
- *         cdef double max_score = -INFINITY             # <<<<<<<<<<<<<<
- *         best:Node = None
+ *         cur_team = node.state.get_current_team()             # <<<<<<<<<<<<<<
  * 
+ *         cdef double best_score = -INFINITY
  */
-  __pyx_v_max_score = (-INFINITY);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_v_cur_team = __pyx_t_1;
+  __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":203
+  /* "multimcts/mcts.pyx":212
+ *         cur_team = node.state.get_current_team()
  * 
- *         cdef double max_score = -INFINITY
- *         best:Node = None             # <<<<<<<<<<<<<<
+ *         cdef double best_score = -INFINITY             # <<<<<<<<<<<<<<
+ *         best_child:Node = None
+ * 
+ */
+  __pyx_v_best_score = (-INFINITY);
+
+  /* "multimcts/mcts.pyx":213
+ * 
+ *         cdef double best_score = -INFINITY
+ *         best_child:Node = None             # <<<<<<<<<<<<<<
  * 
  *         for child in node.children:
  */
   __Pyx_INCREF(Py_None);
-  __pyx_v_best = Py_None;
+  __pyx_v_best_child = Py_None;
 
-  /* "multimcts/mcts.pyx":205
- *         best:Node = None
+  /* "multimcts/mcts.pyx":215
+ *         best_child:Node = None
  * 
  *         for child in node.children:             # <<<<<<<<<<<<<<
- *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())
+ *             visits = child.num_visits
+ *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 205, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
-    __pyx_t_3 = __pyx_t_1; __Pyx_INCREF(__pyx_t_3); __pyx_t_5 = 0;
+    __pyx_t_4 = __pyx_t_1; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 205, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 205, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 215, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_6)) {
-      if (likely(PyList_CheckExact(__pyx_t_3))) {
-        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_3)) break;
+      if (likely(PyList_CheckExact(__pyx_t_4))) {
+        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 205, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 215, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 205, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
-        if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
+        if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 205, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 215, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 205, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
-      __pyx_t_1 = __pyx_t_6(__pyx_t_3);
+      __pyx_t_1 = __pyx_t_6(__pyx_t_4);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 205, __pyx_L1_error)
+          else __PYX_ERR(0, 215, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
-    __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_child);
-    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_child, __pyx_t_1);
-    __Pyx_GIVEREF(__pyx_t_1);
+    __Pyx_XDECREF_SET(__pyx_v_child, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":207
+    /* "multimcts/mcts.pyx":216
+ * 
  *         for child in node.children:
+ *             visits = child.num_visits             # <<<<<<<<<<<<<<
+ *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
+ *                 continue
+ */
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_child, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_v_visits = __pyx_t_7;
+
+    /* "multimcts/mcts.pyx":217
+ *         for child in node.children:
+ *             visits = child.num_visits
+ *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...             # <<<<<<<<<<<<<<
+ *                 continue
+ * 
+ */
+    __pyx_t_8 = ((__pyx_v_visits == 0) != 0);
+    if (__pyx_t_8) {
+
+      /* "multimcts/mcts.pyx":218
+ *             visits = child.num_visits
+ *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
+ *                 continue             # <<<<<<<<<<<<<<
+ * 
  *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())             # <<<<<<<<<<<<<<
+ */
+      goto __pyx_L3_continue;
+
+      /* "multimcts/mcts.pyx":217
+ *         for child in node.children:
  *             visits = child.num_visits
+ *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...             # <<<<<<<<<<<<<<
+ *                 continue
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+    }
+
+    /* "multimcts/mcts.pyx":221
+ * 
+ *             # Relative reward is this child's reward minus its siblings' rewards.
+ *             reward = 2 * child.total_reward[cur_team]             # <<<<<<<<<<<<<<
+ *             for subreward in child.total_reward.values():
+ *                 reward -= subreward
+ */
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_cur_team); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_cur_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Multiply(__pyx_int_2, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Multiply(__pyx_int_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __pyx_pf_9multimcts_4mcts_4MCTS_14get_best_child_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_Subtract(__pyx_t_1, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_v_reward = __pyx_t_4;
+    __pyx_v_reward = __pyx_t_2;
 
-    /* "multimcts/mcts.pyx":208
+    /* "multimcts/mcts.pyx":222
  *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())
- *             visits = child.num_visits             # <<<<<<<<<<<<<<
+ *             reward = 2 * child.total_reward[cur_team]
+ *             for subreward in child.total_reward.values():             # <<<<<<<<<<<<<<
+ *                 reward -= subreward
  * 
- *             """UCB := (x / n) + C * sqrt(ln(N) / n)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_child, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 208, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_v_visits = __pyx_t_8;
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_values); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
+      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_9);
+      if (likely(__pyx_t_3)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+        __Pyx_INCREF(__pyx_t_3);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_9, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_9);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
+      __pyx_t_9 = __pyx_t_1; __Pyx_INCREF(__pyx_t_9); __pyx_t_10 = 0;
+      __pyx_t_11 = NULL;
+    } else {
+      __pyx_t_10 = -1; __pyx_t_9 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 222, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_11 = Py_TYPE(__pyx_t_9)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 222, __pyx_L1_error)
+    }
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    for (;;) {
+      if (likely(!__pyx_t_11)) {
+        if (likely(PyList_CheckExact(__pyx_t_9))) {
+          if (__pyx_t_10 >= PyList_GET_SIZE(__pyx_t_9)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_1 = PyList_GET_ITEM(__pyx_t_9, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 222, __pyx_L1_error)
+          #else
+          __pyx_t_1 = PySequence_ITEM(__pyx_t_9, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          #endif
+        } else {
+          if (__pyx_t_10 >= PyTuple_GET_SIZE(__pyx_t_9)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_9, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 222, __pyx_L1_error)
+          #else
+          __pyx_t_1 = PySequence_ITEM(__pyx_t_9, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          #endif
+        }
+      } else {
+        __pyx_t_1 = __pyx_t_11(__pyx_t_9);
+        if (unlikely(!__pyx_t_1)) {
+          PyObject* exc_type = PyErr_Occurred();
+          if (exc_type) {
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            else __PYX_ERR(0, 222, __pyx_L1_error)
+          }
+          break;
+        }
+        __Pyx_GOTREF(__pyx_t_1);
+      }
+      __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 222, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_v_subreward = __pyx_t_2;
 
-    /* "multimcts/mcts.pyx":216
- *             C=exploration bias
- *             """
- *             score = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)             # <<<<<<<<<<<<<<
+      /* "multimcts/mcts.pyx":223
+ *             reward = 2 * child.total_reward[cur_team]
+ *             for subreward in child.total_reward.values():
+ *                 reward -= subreward             # <<<<<<<<<<<<<<
+ * 
+ *             ucb = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
+ */
+      __pyx_v_reward = (__pyx_v_reward - __pyx_v_subreward);
+
+      /* "multimcts/mcts.pyx":222
+ *             # Relative reward is this child's reward minus its siblings' rewards.
+ *             reward = 2 * child.total_reward[cur_team]
+ *             for subreward in child.total_reward.values():             # <<<<<<<<<<<<<<
+ *                 reward -= subreward
  * 
- *             if score > max_score:
  */
-    if (unlikely(__pyx_v_visits == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 216, __pyx_L1_error)
-    }
-    if (unlikely(__pyx_v_visits == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 216, __pyx_L1_error)
     }
-    __pyx_v_score = ((__pyx_v_reward / __pyx_v_visits) + (__pyx_v_exploration_bias * sqrt((__pyx_v_ln_parent_visits / __pyx_v_visits))));
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "multimcts/mcts.pyx":218
- *             score = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
+    /* "multimcts/mcts.pyx":225
+ *                 reward -= subreward
+ * 
+ *             ucb = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)             # <<<<<<<<<<<<<<
  * 
- *             if score > max_score:             # <<<<<<<<<<<<<<
- *                 max_score = score
- *                 best = child
+ *             if ucb > best_score:
  */
-    __pyx_t_9 = ((__pyx_v_score > __pyx_v_max_score) != 0);
-    if (__pyx_t_9) {
+    __pyx_v_ucb = ((__pyx_v_reward / __pyx_v_visits) + (__pyx_v_exploration_bias * sqrt((__pyx_v_ln_parent_visits / __pyx_v_visits))));
 
-      /* "multimcts/mcts.pyx":219
+    /* "multimcts/mcts.pyx":227
+ *             ucb = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
  * 
- *             if score > max_score:
- *                 max_score = score             # <<<<<<<<<<<<<<
- *                 best = child
+ *             if ucb > best_score:             # <<<<<<<<<<<<<<
+ *                 best_score = ucb
+ *                 best_child = child
+ */
+    __pyx_t_8 = ((__pyx_v_ucb > __pyx_v_best_score) != 0);
+    if (__pyx_t_8) {
+
+      /* "multimcts/mcts.pyx":228
+ * 
+ *             if ucb > best_score:
+ *                 best_score = ucb             # <<<<<<<<<<<<<<
+ *                 best_child = child
  * 
  */
-      __pyx_v_max_score = __pyx_v_score;
+      __pyx_v_best_score = __pyx_v_ucb;
 
-      /* "multimcts/mcts.pyx":220
- *             if score > max_score:
- *                 max_score = score
- *                 best = child             # <<<<<<<<<<<<<<
+      /* "multimcts/mcts.pyx":229
+ *             if ucb > best_score:
+ *                 best_score = ucb
+ *                 best_child = child             # <<<<<<<<<<<<<<
  * 
- *         return best
+ *         return best_child
  */
-      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_child);
-      __Pyx_DECREF_SET(__pyx_v_best, __pyx_cur_scope->__pyx_v_child);
+      __Pyx_INCREF(__pyx_v_child);
+      __Pyx_DECREF_SET(__pyx_v_best_child, __pyx_v_child);
 
-      /* "multimcts/mcts.pyx":218
- *             score = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
+      /* "multimcts/mcts.pyx":227
+ *             ucb = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
  * 
- *             if score > max_score:             # <<<<<<<<<<<<<<
- *                 max_score = score
- *                 best = child
+ *             if ucb > best_score:             # <<<<<<<<<<<<<<
+ *                 best_score = ucb
+ *                 best_child = child
  */
     }
 
-    /* "multimcts/mcts.pyx":205
- *         best:Node = None
+    /* "multimcts/mcts.pyx":215
+ *         best_child:Node = None
  * 
  *         for child in node.children:             # <<<<<<<<<<<<<<
- *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())
+ *             visits = child.num_visits
+ *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
  */
+    __pyx_L3_continue:;
   }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":222
- *                 best = child
+  /* "multimcts/mcts.pyx":231
+ *                 best_child = child
  * 
- *         return best             # <<<<<<<<<<<<<<
+ *         return best_child             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_best);
-  __pyx_r = __pyx_v_best;
+  __Pyx_INCREF(__pyx_v_best_child);
+  __pyx_r = __pyx_v_best_child;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":193
- *             node = node.parent
+  /* "multimcts/mcts.pyx":196
  * 
+ *     @cython.cdivision(True)
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         cur_team = node.state.get_current_team()
- * 
+ *         """Find the child with the highest Upper Confidence Bound (UCB) score.
+ *         ucb = (x / n) + C * sqrt(ln(N) / n)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.get_best_child", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_cur_team);
-  __Pyx_XDECREF(__pyx_v_best);
-  __Pyx_XDECREF(__pyx_gb_9multimcts_4mcts_4MCTS_14get_best_child_2generator);
-  __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
+  __Pyx_XDECREF(__pyx_v_best_child);
+  __Pyx_XDECREF(__pyx_v_child);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *__pyx_freelist_9multimcts_4mcts___pyx_scope_struct__get_best_child[8];
-static int __pyx_freecount_9multimcts_4mcts___pyx_scope_struct__get_best_child = 0;
-
-static PyObject *__pyx_tp_new_9multimcts_4mcts___pyx_scope_struct__get_best_child(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_9multimcts_4mcts___pyx_scope_struct__get_best_child > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child)))) {
-    o = (PyObject*)__pyx_freelist_9multimcts_4mcts___pyx_scope_struct__get_best_child[--__pyx_freecount_9multimcts_4mcts___pyx_scope_struct__get_best_child];
-    memset(o, 0, sizeof(struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child));
-    (void) PyObject_INIT(o, t);
-    PyObject_GC_Track(o);
-  } else {
-    o = (*t->tp_alloc)(t, 0);
-    if (unlikely(!o)) return 0;
-  }
-  return o;
-}
-
-static void __pyx_tp_dealloc_9multimcts_4mcts___pyx_scope_struct__get_best_child(PyObject *o) {
-  struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *p = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *)o;
-  PyObject_GC_UnTrack(o);
-  Py_CLEAR(p->__pyx_v_child);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_9multimcts_4mcts___pyx_scope_struct__get_best_child < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child)))) {
-    __pyx_freelist_9multimcts_4mcts___pyx_scope_struct__get_best_child[__pyx_freecount_9multimcts_4mcts___pyx_scope_struct__get_best_child++] = ((struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *)o);
-  } else {
-    (*Py_TYPE(o)->tp_free)(o);
-  }
-}
-
-static int __pyx_tp_traverse_9multimcts_4mcts___pyx_scope_struct__get_best_child(PyObject *o, visitproc v, void *a) {
-  int e;
-  struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *p = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *)o;
-  if (p->__pyx_v_child) {
-    e = (*v)(p->__pyx_v_child, a); if (e) return e;
-  }
-  return 0;
-}
-
-static int __pyx_tp_clear_9multimcts_4mcts___pyx_scope_struct__get_best_child(PyObject *o) {
-  PyObject* tmp;
-  struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *p = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *)o;
-  tmp = ((PyObject*)p->__pyx_v_child);
-  p->__pyx_v_child = Py_None; Py_INCREF(Py_None);
-  Py_XDECREF(tmp);
-  return 0;
-}
-
-static PyTypeObject __pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child = {
-  PyVarObject_HEAD_INIT(0, 0)
-  "multimcts.mcts.__pyx_scope_struct__get_best_child", /*tp_name*/
-  sizeof(struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child), /*tp_basicsize*/
-  0, /*tp_itemsize*/
-  __pyx_tp_dealloc_9multimcts_4mcts___pyx_scope_struct__get_best_child, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
-  0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
-  0, /*tp_getattr*/
-  0, /*tp_setattr*/
-  #if PY_MAJOR_VERSION < 3
-  0, /*tp_compare*/
-  #endif
-  #if PY_MAJOR_VERSION >= 3
-  0, /*tp_as_async*/
-  #endif
-  0, /*tp_repr*/
-  0, /*tp_as_number*/
-  0, /*tp_as_sequence*/
-  0, /*tp_as_mapping*/
-  0, /*tp_hash*/
-  0, /*tp_call*/
-  0, /*tp_str*/
-  0, /*tp_getattro*/
-  0, /*tp_setattro*/
-  0, /*tp_as_buffer*/
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
-  0, /*tp_doc*/
-  __pyx_tp_traverse_9multimcts_4mcts___pyx_scope_struct__get_best_child, /*tp_traverse*/
-  __pyx_tp_clear_9multimcts_4mcts___pyx_scope_struct__get_best_child, /*tp_clear*/
-  0, /*tp_richcompare*/
-  0, /*tp_weaklistoffset*/
-  0, /*tp_iter*/
-  0, /*tp_iternext*/
-  0, /*tp_methods*/
-  0, /*tp_members*/
-  0, /*tp_getset*/
-  0, /*tp_base*/
-  0, /*tp_dict*/
-  0, /*tp_descr_get*/
-  0, /*tp_descr_set*/
-  0, /*tp_dictoffset*/
-  0, /*tp_init*/
-  0, /*tp_alloc*/
-  __pyx_tp_new_9multimcts_4mcts___pyx_scope_struct__get_best_child, /*tp_new*/
-  0, /*tp_free*/
-  0, /*tp_is_gc*/
-  0, /*tp_bases*/
-  0, /*tp_mro*/
-  0, /*tp_cache*/
-  0, /*tp_subclasses*/
-  0, /*tp_weaklist*/
-  0, /*tp_del*/
-  0, /*tp_version_tag*/
-  #if PY_VERSION_HEX >= 0x030400a1
-  0, /*tp_finalize*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-  0, /*tp_vectorcall*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
-};
-
-static struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *__pyx_freelist_9multimcts_4mcts___pyx_scope_struct_1_genexpr[8];
-static int __pyx_freecount_9multimcts_4mcts___pyx_scope_struct_1_genexpr = 0;
-
-static PyObject *__pyx_tp_new_9multimcts_4mcts___pyx_scope_struct_1_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_9multimcts_4mcts___pyx_scope_struct_1_genexpr > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr)))) {
-    o = (PyObject*)__pyx_freelist_9multimcts_4mcts___pyx_scope_struct_1_genexpr[--__pyx_freecount_9multimcts_4mcts___pyx_scope_struct_1_genexpr];
-    memset(o, 0, sizeof(struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr));
-    (void) PyObject_INIT(o, t);
-    PyObject_GC_Track(o);
-  } else {
-    o = (*t->tp_alloc)(t, 0);
-    if (unlikely(!o)) return 0;
-  }
-  return o;
-}
-
-static void __pyx_tp_dealloc_9multimcts_4mcts___pyx_scope_struct_1_genexpr(PyObject *o) {
-  struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *p = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *)o;
-  PyObject_GC_UnTrack(o);
-  Py_CLEAR(p->__pyx_outer_scope);
-  Py_CLEAR(p->__pyx_v_x);
-  Py_CLEAR(p->__pyx_t_0);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_9multimcts_4mcts___pyx_scope_struct_1_genexpr < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr)))) {
-    __pyx_freelist_9multimcts_4mcts___pyx_scope_struct_1_genexpr[__pyx_freecount_9multimcts_4mcts___pyx_scope_struct_1_genexpr++] = ((struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *)o);
-  } else {
-    (*Py_TYPE(o)->tp_free)(o);
-  }
-}
-
-static int __pyx_tp_traverse_9multimcts_4mcts___pyx_scope_struct_1_genexpr(PyObject *o, visitproc v, void *a) {
-  int e;
-  struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *p = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *)o;
-  if (p->__pyx_outer_scope) {
-    e = (*v)(((PyObject *)p->__pyx_outer_scope), a); if (e) return e;
-  }
-  if (p->__pyx_v_x) {
-    e = (*v)(p->__pyx_v_x, a); if (e) return e;
-  }
-  if (p->__pyx_t_0) {
-    e = (*v)(p->__pyx_t_0, a); if (e) return e;
-  }
-  return 0;
-}
-
-static PyTypeObject __pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr = {
-  PyVarObject_HEAD_INIT(0, 0)
-  "multimcts.mcts.__pyx_scope_struct_1_genexpr", /*tp_name*/
-  sizeof(struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr), /*tp_basicsize*/
-  0, /*tp_itemsize*/
-  __pyx_tp_dealloc_9multimcts_4mcts___pyx_scope_struct_1_genexpr, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
-  0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
-  0, /*tp_getattr*/
-  0, /*tp_setattr*/
-  #if PY_MAJOR_VERSION < 3
-  0, /*tp_compare*/
-  #endif
-  #if PY_MAJOR_VERSION >= 3
-  0, /*tp_as_async*/
-  #endif
-  0, /*tp_repr*/
-  0, /*tp_as_number*/
-  0, /*tp_as_sequence*/
-  0, /*tp_as_mapping*/
-  0, /*tp_hash*/
-  0, /*tp_call*/
-  0, /*tp_str*/
-  0, /*tp_getattro*/
-  0, /*tp_setattro*/
-  0, /*tp_as_buffer*/
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
-  0, /*tp_doc*/
-  __pyx_tp_traverse_9multimcts_4mcts___pyx_scope_struct_1_genexpr, /*tp_traverse*/
-  0, /*tp_clear*/
-  0, /*tp_richcompare*/
-  0, /*tp_weaklistoffset*/
-  0, /*tp_iter*/
-  0, /*tp_iternext*/
-  0, /*tp_methods*/
-  0, /*tp_members*/
-  0, /*tp_getset*/
-  0, /*tp_base*/
-  0, /*tp_dict*/
-  0, /*tp_descr_get*/
-  0, /*tp_descr_set*/
-  0, /*tp_dictoffset*/
-  0, /*tp_init*/
-  0, /*tp_alloc*/
-  __pyx_tp_new_9multimcts_4mcts___pyx_scope_struct_1_genexpr, /*tp_new*/
-  0, /*tp_free*/
-  0, /*tp_is_gc*/
-  0, /*tp_bases*/
-  0, /*tp_mro*/
-  0, /*tp_cache*/
-  0, /*tp_subclasses*/
-  0, /*tp_weaklist*/
-  0, /*tp_del*/
-  0, /*tp_version_tag*/
-  #if PY_VERSION_HEX >= 0x030400a1
-  0, /*tp_finalize*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-  0, /*tp_vectorcall*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
-};
-
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
@@ -5528,45 +5059,42 @@
   {&__pyx_kp_s_GameState_must_implement_make_mo, __pyx_k_GameState_must_implement_make_mo, sizeof(__pyx_k_GameState_must_implement_make_mo), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS, __pyx_k_MCTS, sizeof(__pyx_k_MCTS), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS___init, __pyx_k_MCTS___init, sizeof(__pyx_k_MCTS___init), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_backpropagate, __pyx_k_MCTS_backpropagate, sizeof(__pyx_k_MCTS_backpropagate), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_expand, __pyx_k_MCTS_expand, sizeof(__pyx_k_MCTS_expand), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_get_best_child, __pyx_k_MCTS_get_best_child, sizeof(__pyx_k_MCTS_get_best_child), 0, 0, 1, 1},
-  {&__pyx_n_s_MCTS_get_best_child_locals_genex, __pyx_k_MCTS_get_best_child_locals_genex, sizeof(__pyx_k_MCTS_get_best_child_locals_genex), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_search, __pyx_k_MCTS_search, sizeof(__pyx_k_MCTS_search), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_select, __pyx_k_MCTS_select, sizeof(__pyx_k_MCTS_select), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_simulate, __pyx_k_MCTS_simulate, sizeof(__pyx_k_MCTS_simulate), 0, 0, 1, 1},
   {&__pyx_n_s_Node, __pyx_k_Node, sizeof(__pyx_k_Node), 0, 0, 1, 1},
   {&__pyx_n_s_Node___init, __pyx_k_Node___init, sizeof(__pyx_k_Node___init), 0, 0, 1, 1},
   {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
   {&__pyx_kp_s_One_or_more_of_max_time_max_iter, __pyx_k_One_or_more_of_max_time_max_iter, sizeof(__pyx_k_One_or_more_of_max_time_max_iter), 0, 0, 1, 0},
   {&__pyx_kp_s_Represents_a_game_state_node_in, __pyx_k_Represents_a_game_state_node_in, sizeof(__pyx_k_Represents_a_game_state_node_in), 0, 0, 1, 0},
   {&__pyx_kp_s_Tried_to_expand_a_node_with_no_r, __pyx_k_Tried_to_expand_a_node_with_no_r, sizeof(__pyx_k_Tried_to_expand_a_node_with_no_r), 0, 0, 1, 0},
   {&__pyx_n_s_Union, __pyx_k_Union, sizeof(__pyx_k_Union), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
-  {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_backpropagate, __pyx_k_backpropagate, sizeof(__pyx_k_backpropagate), 0, 0, 1, 1},
-  {&__pyx_n_s_best, __pyx_k_best, sizeof(__pyx_k_best), 0, 0, 1, 1},
+  {&__pyx_n_s_best_child, __pyx_k_best_child, sizeof(__pyx_k_best_child), 0, 0, 1, 1},
+  {&__pyx_n_s_best_score, __pyx_k_best_score, sizeof(__pyx_k_best_score), 0, 0, 1, 1},
   {&__pyx_n_s_child, __pyx_k_child, sizeof(__pyx_k_child), 0, 0, 1, 1},
   {&__pyx_n_s_children, __pyx_k_children, sizeof(__pyx_k_children), 0, 0, 1, 1},
   {&__pyx_n_s_choice, __pyx_k_choice, sizeof(__pyx_k_choice), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
   {&__pyx_n_s_collections, __pyx_k_collections, sizeof(__pyx_k_collections), 0, 0, 1, 1},
   {&__pyx_n_s_cur_team, __pyx_k_cur_team, sizeof(__pyx_k_cur_team), 0, 0, 1, 1},
   {&__pyx_n_s_defaultdict, __pyx_k_defaultdict, sizeof(__pyx_k_defaultdict), 0, 0, 1, 1},
   {&__pyx_n_u_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 1, 0, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
   {&__pyx_n_s_end_time, __pyx_k_end_time, sizeof(__pyx_k_end_time), 0, 0, 1, 1},
   {&__pyx_n_s_expand, __pyx_k_expand, sizeof(__pyx_k_expand), 0, 0, 1, 1},
   {&__pyx_n_s_exploration_bias, __pyx_k_exploration_bias, sizeof(__pyx_k_exploration_bias), 0, 0, 1, 1},
   {&__pyx_n_u_float, __pyx_k_float, sizeof(__pyx_k_float), 0, 1, 0, 1},
-  {&__pyx_n_s_genexpr, __pyx_k_genexpr, sizeof(__pyx_k_genexpr), 0, 0, 1, 1},
   {&__pyx_n_s_get_best_child, __pyx_k_get_best_child, sizeof(__pyx_k_get_best_child), 0, 0, 1, 1},
   {&__pyx_n_s_get_current_team, __pyx_k_get_current_team, sizeof(__pyx_k_get_current_team), 0, 0, 1, 1},
   {&__pyx_n_s_get_legal_moves, __pyx_k_get_legal_moves, sizeof(__pyx_k_get_legal_moves), 0, 0, 1, 1},
   {&__pyx_n_s_get_reward, __pyx_k_get_reward, sizeof(__pyx_k_get_reward), 0, 0, 1, 1},
   {&__pyx_n_s_heuristic, __pyx_k_heuristic, sizeof(__pyx_k_heuristic), 0, 0, 1, 1},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
@@ -5577,15 +5105,14 @@
   {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
   {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
   {&__pyx_n_s_ln_parent_visits, __pyx_k_ln_parent_visits, sizeof(__pyx_k_ln_parent_visits), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_make_move, __pyx_k_make_move, sizeof(__pyx_k_make_move), 0, 0, 1, 1},
   {&__pyx_n_s_max_iterations, __pyx_k_max_iterations, sizeof(__pyx_k_max_iterations), 0, 0, 1, 1},
-  {&__pyx_n_s_max_score, __pyx_k_max_score, sizeof(__pyx_k_max_score), 0, 0, 1, 1},
   {&__pyx_n_s_max_time, __pyx_k_max_time, sizeof(__pyx_k_max_time), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_move, __pyx_k_move, sizeof(__pyx_k_move), 0, 0, 1, 1},
   {&__pyx_n_s_multimcts_mcts, __pyx_k_multimcts_mcts, sizeof(__pyx_k_multimcts_mcts), 0, 0, 1, 1},
   {&__pyx_kp_s_multimcts_mcts_pyx, __pyx_k_multimcts_mcts_pyx, sizeof(__pyx_k_multimcts_mcts_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
@@ -5595,285 +5122,282 @@
   {&__pyx_n_s_pop, __pyx_k_pop, sizeof(__pyx_k_pop), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_random, __pyx_k_random, sizeof(__pyx_k_random), 0, 0, 1, 1},
   {&__pyx_n_s_remaining_moves, __pyx_k_remaining_moves, sizeof(__pyx_k_remaining_moves), 0, 0, 1, 1},
   {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
   {&__pyx_n_s_reward, __pyx_k_reward, sizeof(__pyx_k_reward), 0, 0, 1, 1},
-  {&__pyx_n_s_score, __pyx_k_score, sizeof(__pyx_k_score), 0, 0, 1, 1},
   {&__pyx_n_s_search, __pyx_k_search, sizeof(__pyx_k_search), 0, 0, 1, 1},
   {&__pyx_n_s_select, __pyx_k_select, sizeof(__pyx_k_select), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
-  {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
   {&__pyx_n_s_shuffle, __pyx_k_shuffle, sizeof(__pyx_k_shuffle), 0, 0, 1, 1},
   {&__pyx_n_s_simulate, __pyx_k_simulate, sizeof(__pyx_k_simulate), 0, 0, 1, 1},
   {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
   {&__pyx_n_s_staticmethod, __pyx_k_staticmethod, sizeof(__pyx_k_staticmethod), 0, 0, 1, 1},
-  {&__pyx_n_s_sum, __pyx_k_sum, sizeof(__pyx_k_sum), 0, 0, 1, 1},
+  {&__pyx_n_s_subreward, __pyx_k_subreward, sizeof(__pyx_k_subreward), 0, 0, 1, 1},
   {&__pyx_n_s_terminal_team, __pyx_k_terminal_team, sizeof(__pyx_k_terminal_team), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
   {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
   {&__pyx_n_s_total_reward, __pyx_k_total_reward, sizeof(__pyx_k_total_reward), 0, 0, 1, 1},
   {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
+  {&__pyx_n_s_ucb, __pyx_k_ucb, sizeof(__pyx_k_ucb), 0, 0, 1, 1},
   {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {&__pyx_n_s_values, __pyx_k_values, sizeof(__pyx_k_values), 0, 0, 1, 1},
   {&__pyx_n_s_visits, __pyx_k_visits, sizeof(__pyx_k_visits), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 131, __pyx_L1_error)
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 12, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 93, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 138, __pyx_L1_error)
-  __pyx_builtin_sum = __Pyx_GetBuiltinName(__pyx_n_s_sum); if (!__pyx_builtin_sum) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 140, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "multimcts/mcts.pyx":12
+  /* "multimcts/mcts.pyx":14
  *     def get_current_team(self) -> Union[int,str]:
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")             # <<<<<<<<<<<<<<
  * 
  *     def get_legal_moves(self) -> list[Any]:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_get_cur); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_get_cur); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "multimcts/mcts.pyx":16
+  /* "multimcts/mcts.pyx":18
  *     def get_legal_moves(self) -> list[Any]:
  *         """Returns a list of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")             # <<<<<<<<<<<<<<
  * 
  *     def make_move(self, move:Any) -> 'GameState':
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_get_leg); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_get_leg); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "multimcts/mcts.pyx":22
+  /* "multimcts/mcts.pyx":24
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  *         """
  *         raise NotImplementedError("GameState must implement make_move.")             # <<<<<<<<<<<<<<
  * 
  *     def is_terminal(self) -> bool:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_make_mo); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_make_mo); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "multimcts/mcts.pyx":26
+  /* "multimcts/mcts.pyx":28
  *     def is_terminal(self) -> bool:
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
  * 
  *     def get_reward(self) -> Union[float, dict[Union[int,str], float]]:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_is_term); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_is_term); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "multimcts/mcts.pyx":34
+  /* "multimcts/mcts.pyx":36
  *         Note: This method is only called on terminal states.
  *         """
  *         raise NotImplementedError("GameState must implement get_reward.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_get_rew); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_get_rew); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "multimcts/mcts.pyx":93
+  /* "multimcts/mcts.pyx":95
  *         """
  *         if max_time is None and max_iterations is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         node = Node(state)
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "multimcts/mcts.pyx":139
+  /* "multimcts/mcts.pyx":141
  *             move = node.remaining_moves.pop()
  *         except IndexError:
  *             raise IndexError("Tried to expand a node with no remaining moves.")             # <<<<<<<<<<<<<<
  * 
  *         child = Node(node.state.make_move(move), node)
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Tried_to_expand_a_node_with_no_r); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Tried_to_expand_a_node_with_no_r); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "multimcts/mcts.pyx":10
+  /* "multimcts/mcts.pyx":12
  * 
- * class GameState():
+ * class GameState:
  *     def get_current_team(self) -> Union[int,str]:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_current_team, 10, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_current_team, 12, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 12, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":14
+  /* "multimcts/mcts.pyx":16
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> list[Any]:             # <<<<<<<<<<<<<<
  *         """Returns a list of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_legal_moves, 14, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_legal_moves, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 16, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":18
+  /* "multimcts/mcts.pyx":20
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Any) -> 'GameState':             # <<<<<<<<<<<<<<
  *         """Returns a new GameState, which is the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
-  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_move); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_move); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_make_move, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_make_move, 20, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 20, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":24
+  /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_is_terminal, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_is_terminal, 26, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 26, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":28
+  /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float, dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
  *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_reward, 28, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_reward, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 30, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":52
+  /* "multimcts/mcts.pyx":54
  *         remaining_moves (list): A list of moves that have not yet been tried.
  *     """
  *     def __init__(self, state:GameState, parent:'Node'=None):             # <<<<<<<<<<<<<<
  *         self.state = state
  *         self.parent = parent
  */
-  __pyx_tuple__18 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_parent); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_parent); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_init, 52, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 52, __pyx_L1_error)
-  __pyx_tuple__20 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_init, 54, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
 
-  /* "multimcts/mcts.pyx":71
+  /* "multimcts/mcts.pyx":73
  * 
- * class MCTS():
+ * class MCTS:
  *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
  * 
  */
-  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_exploration_bias); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_exploration_bias); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_init, 71, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_init, 73, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 73, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":81
+  /* "multimcts/mcts.pyx":83
  *         self.exploration_bias = exploration_bias
  * 
  *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None) -> GameState:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
  * 
  */
-  __pyx_tuple__23 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_max_time, __pyx_n_s_max_iterations, __pyx_n_s_heuristic, __pyx_n_s_node, __pyx_n_s_end_time, __pyx_n_s_i, __pyx_n_s_child, __pyx_n_s_reward); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_max_time, __pyx_n_s_max_iterations, __pyx_n_s_heuristic, __pyx_n_s_node, __pyx_n_s_end_time, __pyx_n_s_i, __pyx_n_s_child, __pyx_n_s_reward); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(2, 3, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_search, 81, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(2, 3, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_search, 83, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 83, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":118
+  /* "multimcts/mcts.pyx":120
  *         return self.get_best_child(node).state
  * 
  *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
-  __pyx_tuple__25 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_node); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_node); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_select, 118, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_select, 120, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 120, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":132
+  /* "multimcts/mcts.pyx":134
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
-  __pyx_tuple__27 = PyTuple_Pack(3, __pyx_n_s_node, __pyx_n_s_move, __pyx_n_s_child); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(3, __pyx_n_s_node, __pyx_n_s_move, __pyx_n_s_child); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_expand, 132, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_expand, 134, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 134, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":149
+  /* "multimcts/mcts.pyx":151
  *         return child
  * 
  *     def simulate(self, node:Node, *, heuristic=None) -> dict[Union[int,str], float]:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout/rollout)
  *         Play out a game, from the given node to termination, and return the final reward.
  */
-  __pyx_tuple__29 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_heuristic, __pyx_n_s_state, __pyx_n_s_terminal_team, __pyx_n_s_move, __pyx_n_s_reward); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_heuristic, __pyx_n_s_state, __pyx_n_s_terminal_team, __pyx_n_s_move, __pyx_n_s_reward); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 1, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_simulate, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 1, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_simulate, 151, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 151, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":178
+  /* "multimcts/mcts.pyx":180
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:dict):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
-  __pyx_tuple__31 = PyTuple_Pack(5, __pyx_n_s_node, __pyx_n_s_reward, __pyx_n_s_key, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(5, __pyx_n_s_node, __pyx_n_s_reward, __pyx_n_s_key, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_backpropagate, 178, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_backpropagate, 180, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 180, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":193
- *             node = node.parent
+  /* "multimcts/mcts.pyx":196
  * 
+ *     @cython.cdivision(True)
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         cur_team = node.state.get_current_team()
- * 
+ *         """Find the child with the highest Upper Confidence Bound (UCB) score.
+ *         ucb = (x / n) + C * sqrt(ln(N) / n)
  */
-  __pyx_tuple__33 = PyTuple_Pack(13, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_cur_team, __pyx_n_s_visits, __pyx_n_s_reward, __pyx_n_s_score, __pyx_n_s_exploration_bias, __pyx_n_s_ln_parent_visits, __pyx_n_s_max_score, __pyx_n_s_best, __pyx_n_s_child, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_visits, __pyx_n_s_reward, __pyx_n_s_subreward, __pyx_n_s_ucb, __pyx_n_s_exploration_bias, __pyx_n_s_ln_parent_visits, __pyx_n_s_cur_team, __pyx_n_s_best_score, __pyx_n_s_best_child, __pyx_n_s_child); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_best_child, 193, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_best_child, 196, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -5919,40 +5443,18 @@
   /*--- Function export code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child.tp_print = 0;
-  #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child.tp_dictoffset && __pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
-  }
-  __pyx_ptype_9multimcts_4mcts___pyx_scope_struct__get_best_child = &__pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child;
-  if (PyType_Ready(&__pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 207, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr.tp_print = 0;
-  #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
-  }
-  __pyx_ptype_9multimcts_4mcts___pyx_scope_struct_1_genexpr = &__pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr;
   __Pyx_RefNannyFinishContext();
   return 0;
-  __pyx_L1_error:;
-  __Pyx_RefNannyFinishContext();
-  return -1;
 }
 
 static int __Pyx_modinit_type_import_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __Pyx_RefNannyFinishContext();
@@ -6167,15 +5669,15 @@
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  (void)__Pyx_modinit_type_init_code();
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -6248,15 +5750,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "multimcts/mcts.pyx":4
  * from random import shuffle, choice
  * from collections import defaultdict
  * from typing import Union, Any             # <<<<<<<<<<<<<<
  * 
- * from libc.math cimport log, sqrt, INFINITY
+ * import cython
  */
   __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Union);
   __Pyx_GIVEREF(__pyx_n_s_Union);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Union);
   __Pyx_INCREF(__pyx_n_s_Any);
@@ -6271,493 +5773,493 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Any); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Any, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":9
+  /* "multimcts/mcts.pyx":11
  * 
  * 
- * class GameState():             # <<<<<<<<<<<<<<
+ * class GameState:             # <<<<<<<<<<<<<<
  *     def get_current_team(self) -> Union[int,str]:
  *         """The identifier of the current player's team."""
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_GameState, __pyx_n_s_GameState, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_GameState, __pyx_n_s_GameState, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "multimcts/mcts.pyx":10
+  /* "multimcts/mcts.pyx":12
  * 
- * class GameState():
+ * class GameState:
  *     def get_current_team(self) -> Union[int,str]:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Union); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Union); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
   PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)(&PyInt_Type)));
   __Pyx_INCREF(((PyObject *)(&PyString_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyString_Type)));
   PyTuple_SET_ITEM(__pyx_t_4, 1, ((PyObject *)(&PyString_Type)));
-  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team, 0, __pyx_n_s_GameState_get_current_team, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team, 0, __pyx_n_s_GameState_get_current_team, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_current_team, __pyx_t_5) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_current_team, __pyx_t_5) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "multimcts/mcts.pyx":14
+  /* "multimcts/mcts.pyx":16
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> list[Any]:             # <<<<<<<<<<<<<<
  *         """Returns a list of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Any); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Any); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)(&PyList_Type)), __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)(&PyList_Type)), __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_4) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_4) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves, 0, __pyx_n_s_GameState_get_legal_moves, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves, 0, __pyx_n_s_GameState_get_legal_moves, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_legal_moves, __pyx_t_4) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_legal_moves, __pyx_t_4) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":18
+  /* "multimcts/mcts.pyx":20
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Any) -> 'GameState':             # <<<<<<<<<<<<<<
  *         """Returns a new GameState, which is the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Any); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Any); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_move, __pyx_t_5) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_move, __pyx_t_5) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_GameState) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_5make_move, 0, __pyx_n_s_GameState_make_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_GameState) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_5make_move, 0, __pyx_n_s_GameState_make_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_make_move, __pyx_t_5) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_make_move, __pyx_t_5) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "multimcts/mcts.pyx":24
+  /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_7is_terminal, 0, __pyx_n_s_GameState_is_terminal, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_7is_terminal, 0, __pyx_n_s_GameState_is_terminal, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_is_terminal, __pyx_t_4) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_is_terminal, __pyx_t_4) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":28
+  /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float, dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
  *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Union); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Union); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&PyInt_Type)));
   __Pyx_INCREF(((PyObject *)(&PyString_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyString_Type)));
   PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)(&PyString_Type)));
-  __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6);
   __Pyx_INCREF(((PyObject *)(&PyFloat_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyFloat_Type)));
   PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)(&PyFloat_Type)));
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)(&PyDict_Type)), __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)(&PyDict_Type)), __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)(&PyFloat_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyFloat_Type)));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&PyFloat_Type)));
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_t_6) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_t_6) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_9get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_9get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_reward, __pyx_t_6) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_reward, __pyx_t_6) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "multimcts/mcts.pyx":9
+  /* "multimcts/mcts.pyx":11
  * 
  * 
- * class GameState():             # <<<<<<<<<<<<<<
+ * class GameState:             # <<<<<<<<<<<<<<
  *     def get_current_team(self) -> Union[int,str]:
  *         """The identifier of the current player's team."""
  */
-  __pyx_t_6 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_GameState, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_GameState, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_GameState, __pyx_t_6) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_GameState, __pyx_t_6) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":37
+  /* "multimcts/mcts.pyx":39
  * 
  * 
- * class Node():             # <<<<<<<<<<<<<<
+ * class Node:             # <<<<<<<<<<<<<<
  *     """Represents a game state node in the MCTS search tree.
  * 
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Node, __pyx_n_s_Node, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, __pyx_kp_s_Represents_a_game_state_node_in); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Node, __pyx_n_s_Node, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, __pyx_kp_s_Represents_a_game_state_node_in); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "multimcts/mcts.pyx":52
+  /* "multimcts/mcts.pyx":54
  *         remaining_moves (list): A list of moves that have not yet been tried.
  *     """
  *     def __init__(self, state:GameState, parent:'Node'=None):             # <<<<<<<<<<<<<<
  *         self.state = state
  *         self.parent = parent
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_GameState); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_GameState); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_state, __pyx_t_4) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_state, __pyx_t_4) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_parent, __pyx_n_s_Node) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4Node_1__init__, 0, __pyx_n_s_Node___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_parent, __pyx_n_s_Node) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4Node_1__init__, 0, __pyx_n_s_Node___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__20);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_6);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":37
+  /* "multimcts/mcts.pyx":39
  * 
  * 
- * class Node():             # <<<<<<<<<<<<<<
+ * class Node:             # <<<<<<<<<<<<<<
  *     """Represents a game state node in the MCTS search tree.
  * 
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_Node, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_Node, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Node, __pyx_t_4) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Node, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":70
+  /* "multimcts/mcts.pyx":72
  * 
  * 
- * class MCTS():             # <<<<<<<<<<<<<<
+ * class MCTS:             # <<<<<<<<<<<<<<
  *     def __init__(self, exploration_bias:float=1.414):
  *         """Initializes an MCTS agent.
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_MCTS, __pyx_n_s_MCTS, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_MCTS, __pyx_n_s_MCTS, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "multimcts/mcts.pyx":71
+  /* "multimcts/mcts.pyx":73
  * 
- * class MCTS():
+ * class MCTS:
  *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
  * 
  */
-  __pyx_t_4 = PyFloat_FromDouble(((double)1.414)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(((double)1.414)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_exploration_bias, __pyx_n_u_float) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_1__init__, 0, __pyx_n_s_MCTS___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_exploration_bias, __pyx_n_u_float) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_1__init__, 0, __pyx_n_s_MCTS___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_6);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "multimcts/mcts.pyx":81
+  /* "multimcts/mcts.pyx":83
  *         self.exploration_bias = exploration_bias
  * 
  *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None) -> GameState:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_time, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_iterations, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_heuristic, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_time, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_iterations, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_heuristic, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_GameState); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_GameState); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_state, __pyx_t_6) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_state, __pyx_t_6) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Union); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Union); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
   PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)(&PyInt_Type)));
   __Pyx_INCREF(((PyObject *)(&PyFloat_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyFloat_Type)));
   PyTuple_SET_ITEM(__pyx_t_5, 1, ((PyObject *)(&PyFloat_Type)));
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_max_time, __pyx_t_2) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_max_time, __pyx_t_2) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_max_iterations, __pyx_n_u_int) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_GameState); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_max_iterations, __pyx_n_u_int) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_GameState); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_t_2) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_t_2) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_3search, 0, __pyx_n_s_MCTS_search, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_3search, 0, __pyx_n_s_MCTS_search, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_search, __pyx_t_2) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_search, __pyx_t_2) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "multimcts/mcts.pyx":118
+  /* "multimcts/mcts.pyx":120
  *         return self.get_best_child(node).state
  * 
  *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_node, __pyx_t_4) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_node, __pyx_t_4) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_t_4) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_t_4) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_5select, 0, __pyx_n_s_MCTS_select, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_5select, 0, __pyx_n_s_MCTS_select, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_select, __pyx_t_4) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_select, __pyx_t_4) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":132
+  /* "multimcts/mcts.pyx":134
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_node, __pyx_t_2) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_node, __pyx_t_2) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_t_2) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_t_2) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_7expand, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_expand, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_7expand, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_expand, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":131
+  /* "multimcts/mcts.pyx":133
  *         return node
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def expand(node:Node) -> Node:
  *         """Step 2: Expansion
  */
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_expand, __pyx_t_4) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_expand, __pyx_t_4) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":149
+  /* "multimcts/mcts.pyx":151
  *         return child
  * 
  *     def simulate(self, node:Node, *, heuristic=None) -> dict[Union[int,str], float]:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout/rollout)
  *         Play out a game, from the given node to termination, and return the final reward.
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_heuristic, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_heuristic, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Node); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Node); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_node, __pyx_t_3) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_node, __pyx_t_3) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Union); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Union); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
   PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)(&PyInt_Type)));
   __Pyx_INCREF(((PyObject *)(&PyString_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyString_Type)));
   PyTuple_SET_ITEM(__pyx_t_5, 1, ((PyObject *)(&PyString_Type)));
-  __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
   __Pyx_INCREF(((PyObject *)(&PyFloat_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyFloat_Type)));
   PyTuple_SET_ITEM(__pyx_t_5, 1, ((PyObject *)(&PyFloat_Type)));
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)(&PyDict_Type)), __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)(&PyDict_Type)), __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_t_6) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_t_6) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_9simulate, 0, __pyx_n_s_MCTS_simulate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_9simulate, 0, __pyx_n_s_MCTS_simulate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_6, __pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_simulate, __pyx_t_6) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_simulate, __pyx_t_6) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "multimcts/mcts.pyx":178
+  /* "multimcts/mcts.pyx":180
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:dict):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_node, __pyx_t_2) < 0) __PYX_ERR(0, 178, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_node, __pyx_t_2) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_reward, __pyx_n_u_dict) < 0) __PYX_ERR(0, 178, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_backpropagate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_reward, __pyx_n_u_dict) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_backpropagate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_6);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "multimcts/mcts.pyx":177
+  /* "multimcts/mcts.pyx":179
  *         return reward
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def backpropagate(node:Node, reward:dict):
  *         """Step 4: Backpropagation
  */
-  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_backpropagate, __pyx_t_6) < 0) __PYX_ERR(0, 178, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_backpropagate, __pyx_t_6) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "multimcts/mcts.pyx":193
- *             node = node.parent
+  /* "multimcts/mcts.pyx":196
  * 
+ *     @cython.cdivision(True)
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         cur_team = node.state.get_current_team()
- * 
+ *         """Find the child with the highest Upper Confidence Bound (UCB) score.
+ *         ucb = (x / n) + C * sqrt(ln(N) / n)
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_node, __pyx_t_2) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_node, __pyx_t_2) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_t_2) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_t_2) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_13get_best_child, 0, __pyx_n_s_MCTS_get_best_child, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_13get_best_child, 0, __pyx_n_s_MCTS_get_best_child, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_6);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_best_child, __pyx_t_2) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_best_child, __pyx_t_2) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "multimcts/mcts.pyx":70
+  /* "multimcts/mcts.pyx":72
  * 
  * 
- * class MCTS():             # <<<<<<<<<<<<<<
+ * class MCTS:             # <<<<<<<<<<<<<<
  *     def __init__(self, exploration_bias:float=1.414):
  *         """Initializes an MCTS agent.
  */
-  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_MCTS, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_MCTS, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MCTS, __pyx_t_2) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MCTS, __pyx_t_2) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "multimcts/mcts.pyx":1
  * from time import time             # <<<<<<<<<<<<<<
  * from random import shuffle, choice
  * from collections import defaultdict
@@ -8469,59 +7971,14 @@
         return NULL;
     }
     Py_INCREF(value);
     return value;
 }
 #endif
 
-/* None */
-static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname) {
-    PyErr_Format(PyExc_NameError, "free variable '%s' referenced before assignment in enclosing scope", varname);
-}
-
-/* PyObject_GenericGetAttrNoDict */
-#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
-static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
-    PyErr_Format(PyExc_AttributeError,
-#if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, attr_name);
-#else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(attr_name));
-#endif
-    return NULL;
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name) {
-    PyObject *descr;
-    PyTypeObject *tp = Py_TYPE(obj);
-    if (unlikely(!PyString_Check(attr_name))) {
-        return PyObject_GenericGetAttr(obj, attr_name);
-    }
-    assert(!tp->tp_dictoffset);
-    descr = _PyType_Lookup(tp, attr_name);
-    if (unlikely(!descr)) {
-        return __Pyx_RaiseGenericGetAttributeError(tp, attr_name);
-    }
-    Py_INCREF(descr);
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_HAVE_CLASS)))
-    #endif
-    {
-        descrgetfunc f = Py_TYPE(descr)->tp_descr_get;
-        if (unlikely(f)) {
-            PyObject *res = f(descr, obj, (PyObject *)tp);
-            Py_DECREF(descr);
-            return res;
-        }
-    }
-    return descr;
-}
-#endif
-
 /* Import */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
     PyObject *empty_list = 0;
     PyObject *module = 0;
     PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
     PyObject *list;
@@ -10151,1046 +9608,14 @@
     if (likely(PyExceptionClass_Check(err))) {
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
-/* SwapException */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = *type;
-    exc_info->exc_value = *value;
-    exc_info->exc_traceback = *tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = *type;
-    tstate->exc_value = *value;
-    tstate->exc_traceback = *tb;
-    #endif
-    *type = tmp_type;
-    *value = tmp_value;
-    *tb = tmp_tb;
-}
-#else
-static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    PyErr_GetExcInfo(&tmp_type, &tmp_value, &tmp_tb);
-    PyErr_SetExcInfo(*type, *value, *tb);
-    *type = tmp_type;
-    *value = tmp_value;
-    *tb = tmp_tb;
-}
-#endif
-
-/* CoroutineBase */
-#include <structmember.h>
-#include <frameobject.h>
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
-#define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
-static int __Pyx_PyGen__FetchStopIterationValue(CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject **pvalue) {
-    PyObject *et, *ev, *tb;
-    PyObject *value = NULL;
-    __Pyx_ErrFetch(&et, &ev, &tb);
-    if (!et) {
-        Py_XDECREF(tb);
-        Py_XDECREF(ev);
-        Py_INCREF(Py_None);
-        *pvalue = Py_None;
-        return 0;
-    }
-    if (likely(et == PyExc_StopIteration)) {
-        if (!ev) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#if PY_VERSION_HEX >= 0x030300A0
-        else if (Py_TYPE(ev) == (PyTypeObject*)PyExc_StopIteration) {
-            value = ((PyStopIterationObject *)ev)->value;
-            Py_INCREF(value);
-            Py_DECREF(ev);
-        }
-#endif
-        else if (unlikely(PyTuple_Check(ev))) {
-            if (PyTuple_GET_SIZE(ev) >= 1) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                value = PyTuple_GET_ITEM(ev, 0);
-                Py_INCREF(value);
-#else
-                value = PySequence_ITEM(ev, 0);
-#endif
-            } else {
-                Py_INCREF(Py_None);
-                value = Py_None;
-            }
-            Py_DECREF(ev);
-        }
-        else if (!__Pyx_TypeCheck(ev, (PyTypeObject*)PyExc_StopIteration)) {
-            value = ev;
-        }
-        if (likely(value)) {
-            Py_XDECREF(tb);
-            Py_DECREF(et);
-            *pvalue = value;
-            return 0;
-        }
-    } else if (!__Pyx_PyErr_GivenExceptionMatches(et, PyExc_StopIteration)) {
-        __Pyx_ErrRestore(et, ev, tb);
-        return -1;
-    }
-    PyErr_NormalizeException(&et, &ev, &tb);
-    if (unlikely(!PyObject_TypeCheck(ev, (PyTypeObject*)PyExc_StopIteration))) {
-        __Pyx_ErrRestore(et, ev, tb);
-        return -1;
-    }
-    Py_XDECREF(tb);
-    Py_DECREF(et);
-#if PY_VERSION_HEX >= 0x030300A0
-    value = ((PyStopIterationObject *)ev)->value;
-    Py_INCREF(value);
-    Py_DECREF(ev);
-#else
-    {
-        PyObject* args = __Pyx_PyObject_GetAttrStr(ev, __pyx_n_s_args);
-        Py_DECREF(ev);
-        if (likely(args)) {
-            value = PySequence_GetItem(args, 0);
-            Py_DECREF(args);
-        }
-        if (unlikely(!value)) {
-            __Pyx_ErrRestore(NULL, NULL, NULL);
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-    }
-#endif
-    *pvalue = value;
-    return 0;
-}
-static CYTHON_INLINE
-void __Pyx_Coroutine_ExceptionClear(__Pyx_ExcInfoStruct *exc_state) {
-    PyObject *t, *v, *tb;
-    t = exc_state->exc_type;
-    v = exc_state->exc_value;
-    tb = exc_state->exc_traceback;
-    exc_state->exc_type = NULL;
-    exc_state->exc_value = NULL;
-    exc_state->exc_traceback = NULL;
-    Py_XDECREF(t);
-    Py_XDECREF(v);
-    Py_XDECREF(tb);
-}
-#define __Pyx_Coroutine_AlreadyRunningError(gen)  (__Pyx__Coroutine_AlreadyRunningError(gen), (PyObject*)NULL)
-static void __Pyx__Coroutine_AlreadyRunningError(CYTHON_UNUSED __pyx_CoroutineObject *gen) {
-    const char *msg;
-    if ((0)) {
-    #ifdef __Pyx_Coroutine_USED
-    } else if (__Pyx_Coroutine_Check((PyObject*)gen)) {
-        msg = "coroutine already executing";
-    #endif
-    #ifdef __Pyx_AsyncGen_USED
-    } else if (__Pyx_AsyncGen_CheckExact((PyObject*)gen)) {
-        msg = "async generator already executing";
-    #endif
-    } else {
-        msg = "generator already executing";
-    }
-    PyErr_SetString(PyExc_ValueError, msg);
-}
-#define __Pyx_Coroutine_NotStartedError(gen)  (__Pyx__Coroutine_NotStartedError(gen), (PyObject*)NULL)
-static void __Pyx__Coroutine_NotStartedError(CYTHON_UNUSED PyObject *gen) {
-    const char *msg;
-    if ((0)) {
-    #ifdef __Pyx_Coroutine_USED
-    } else if (__Pyx_Coroutine_Check(gen)) {
-        msg = "can't send non-None value to a just-started coroutine";
-    #endif
-    #ifdef __Pyx_AsyncGen_USED
-    } else if (__Pyx_AsyncGen_CheckExact(gen)) {
-        msg = "can't send non-None value to a just-started async generator";
-    #endif
-    } else {
-        msg = "can't send non-None value to a just-started generator";
-    }
-    PyErr_SetString(PyExc_TypeError, msg);
-}
-#define __Pyx_Coroutine_AlreadyTerminatedError(gen, value, closing)  (__Pyx__Coroutine_AlreadyTerminatedError(gen, value, closing), (PyObject*)NULL)
-static void __Pyx__Coroutine_AlreadyTerminatedError(CYTHON_UNUSED PyObject *gen, PyObject *value, CYTHON_UNUSED int closing) {
-    #ifdef __Pyx_Coroutine_USED
-    if (!closing && __Pyx_Coroutine_Check(gen)) {
-        PyErr_SetString(PyExc_RuntimeError, "cannot reuse already awaited coroutine");
-    } else
-    #endif
-    if (value) {
-        #ifdef __Pyx_AsyncGen_USED
-        if (__Pyx_AsyncGen_CheckExact(gen))
-            PyErr_SetNone(__Pyx_PyExc_StopAsyncIteration);
-        else
-        #endif
-        PyErr_SetNone(PyExc_StopIteration);
-    }
-}
-static
-PyObject *__Pyx_Coroutine_SendEx(__pyx_CoroutineObject *self, PyObject *value, int closing) {
-    __Pyx_PyThreadState_declare
-    PyThreadState *tstate;
-    __Pyx_ExcInfoStruct *exc_state;
-    PyObject *retval;
-    assert(!self->is_running);
-    if (unlikely(self->resume_label == 0)) {
-        if (unlikely(value && value != Py_None)) {
-            return __Pyx_Coroutine_NotStartedError((PyObject*)self);
-        }
-    }
-    if (unlikely(self->resume_label == -1)) {
-        return __Pyx_Coroutine_AlreadyTerminatedError((PyObject*)self, value, closing);
-    }
-#if CYTHON_FAST_THREAD_STATE
-    __Pyx_PyThreadState_assign
-    tstate = __pyx_tstate;
-#else
-    tstate = __Pyx_PyThreadState_Current;
-#endif
-    exc_state = &self->gi_exc_state;
-    if (exc_state->exc_type) {
-        #if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
-        #else
-        if (exc_state->exc_traceback) {
-            PyTracebackObject *tb = (PyTracebackObject *) exc_state->exc_traceback;
-            PyFrameObject *f = tb->tb_frame;
-            assert(f->f_back == NULL);
-            #if PY_VERSION_HEX >= 0x030B00A1
-            f->f_back = PyThreadState_GetFrame(tstate);
-            #else
-            Py_XINCREF(tstate->frame);
-            f->f_back = tstate->frame;
-            #endif
-        }
-        #endif
-    }
-#if CYTHON_USE_EXC_INFO_STACK
-    exc_state->previous_item = tstate->exc_info;
-    tstate->exc_info = exc_state;
-#else
-    if (exc_state->exc_type) {
-        __Pyx_ExceptionSwap(&exc_state->exc_type, &exc_state->exc_value, &exc_state->exc_traceback);
-    } else {
-        __Pyx_Coroutine_ExceptionClear(exc_state);
-        __Pyx_ExceptionSave(&exc_state->exc_type, &exc_state->exc_value, &exc_state->exc_traceback);
-    }
-#endif
-    self->is_running = 1;
-    retval = self->body((PyObject *) self, tstate, value);
-    self->is_running = 0;
-#if CYTHON_USE_EXC_INFO_STACK
-    exc_state = &self->gi_exc_state;
-    tstate->exc_info = exc_state->previous_item;
-    exc_state->previous_item = NULL;
-    __Pyx_Coroutine_ResetFrameBackpointer(exc_state);
-#endif
-    return retval;
-}
-static CYTHON_INLINE void __Pyx_Coroutine_ResetFrameBackpointer(__Pyx_ExcInfoStruct *exc_state) {
-    PyObject *exc_tb = exc_state->exc_traceback;
-    if (likely(exc_tb)) {
-#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
-#else
-        PyTracebackObject *tb = (PyTracebackObject *) exc_tb;
-        PyFrameObject *f = tb->tb_frame;
-        Py_CLEAR(f->f_back);
-#endif
-    }
-}
-static CYTHON_INLINE
-PyObject *__Pyx_Coroutine_MethodReturn(CYTHON_UNUSED PyObject* gen, PyObject *retval) {
-    if (unlikely(!retval)) {
-        __Pyx_PyThreadState_declare
-        __Pyx_PyThreadState_assign
-        if (!__Pyx_PyErr_Occurred()) {
-            PyObject *exc = PyExc_StopIteration;
-            #ifdef __Pyx_AsyncGen_USED
-            if (__Pyx_AsyncGen_CheckExact(gen))
-                exc = __Pyx_PyExc_StopAsyncIteration;
-            #endif
-            __Pyx_PyErr_SetNone(exc);
-        }
-    }
-    return retval;
-}
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
-static CYTHON_INLINE
-PyObject *__Pyx_PyGen_Send(PyGenObject *gen, PyObject *arg) {
-#if PY_VERSION_HEX <= 0x030A00A1
-    return _PyGen_Send(gen, arg);
-#else
-    PyObject *result;
-    if (PyIter_Send((PyObject*)gen, arg ? arg : Py_None, &result) == PYGEN_RETURN) {
-        if (PyAsyncGen_CheckExact(gen)) {
-            assert(result == Py_None);
-            PyErr_SetNone(PyExc_StopAsyncIteration);
-        }
-        else if (result == Py_None) {
-            PyErr_SetNone(PyExc_StopIteration);
-        }
-        else {
-            _PyGen_SetStopIterationValue(result);
-        }
-        Py_CLEAR(result);
-    }
-    return result;
-#endif
-}
-#endif
-static CYTHON_INLINE
-PyObject *__Pyx_Coroutine_FinishDelegation(__pyx_CoroutineObject *gen) {
-    PyObject *ret;
-    PyObject *val = NULL;
-    __Pyx_Coroutine_Undelegate(gen);
-    __Pyx_PyGen__FetchStopIterationValue(__Pyx_PyThreadState_Current, &val);
-    ret = __Pyx_Coroutine_SendEx(gen, val, 0);
-    Py_XDECREF(val);
-    return ret;
-}
-static PyObject *__Pyx_Coroutine_Send(PyObject *self, PyObject *value) {
-    PyObject *retval;
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject*) self;
-    PyObject *yf = gen->yieldfrom;
-    if (unlikely(gen->is_running))
-        return __Pyx_Coroutine_AlreadyRunningError(gen);
-    if (yf) {
-        PyObject *ret;
-        gen->is_running = 1;
-        #ifdef __Pyx_Generator_USED
-        if (__Pyx_Generator_CheckExact(yf)) {
-            ret = __Pyx_Coroutine_Send(yf, value);
-        } else
-        #endif
-        #ifdef __Pyx_Coroutine_USED
-        if (__Pyx_Coroutine_Check(yf)) {
-            ret = __Pyx_Coroutine_Send(yf, value);
-        } else
-        #endif
-        #ifdef __Pyx_AsyncGen_USED
-        if (__pyx_PyAsyncGenASend_CheckExact(yf)) {
-            ret = __Pyx_async_gen_asend_send(yf, value);
-        } else
-        #endif
-        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
-        if (PyGen_CheckExact(yf)) {
-            ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
-        } else
-        #endif
-        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03050000 && defined(PyCoro_CheckExact) && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
-        if (PyCoro_CheckExact(yf)) {
-            ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
-        } else
-        #endif
-        {
-            if (value == Py_None)
-                ret = Py_TYPE(yf)->tp_iternext(yf);
-            else
-                ret = __Pyx_PyObject_CallMethod1(yf, __pyx_n_s_send, value);
-        }
-        gen->is_running = 0;
-        if (likely(ret)) {
-            return ret;
-        }
-        retval = __Pyx_Coroutine_FinishDelegation(gen);
-    } else {
-        retval = __Pyx_Coroutine_SendEx(gen, value, 0);
-    }
-    return __Pyx_Coroutine_MethodReturn(self, retval);
-}
-static int __Pyx_Coroutine_CloseIter(__pyx_CoroutineObject *gen, PyObject *yf) {
-    PyObject *retval = NULL;
-    int err = 0;
-    #ifdef __Pyx_Generator_USED
-    if (__Pyx_Generator_CheckExact(yf)) {
-        retval = __Pyx_Coroutine_Close(yf);
-        if (!retval)
-            return -1;
-    } else
-    #endif
-    #ifdef __Pyx_Coroutine_USED
-    if (__Pyx_Coroutine_Check(yf)) {
-        retval = __Pyx_Coroutine_Close(yf);
-        if (!retval)
-            return -1;
-    } else
-    if (__Pyx_CoroutineAwait_CheckExact(yf)) {
-        retval = __Pyx_CoroutineAwait_Close((__pyx_CoroutineAwaitObject*)yf, NULL);
-        if (!retval)
-            return -1;
-    } else
-    #endif
-    #ifdef __Pyx_AsyncGen_USED
-    if (__pyx_PyAsyncGenASend_CheckExact(yf)) {
-        retval = __Pyx_async_gen_asend_close(yf, NULL);
-    } else
-    if (__pyx_PyAsyncGenAThrow_CheckExact(yf)) {
-        retval = __Pyx_async_gen_athrow_close(yf, NULL);
-    } else
-    #endif
-    {
-        PyObject *meth;
-        gen->is_running = 1;
-        meth = __Pyx_PyObject_GetAttrStr(yf, __pyx_n_s_close);
-        if (unlikely(!meth)) {
-            if (!PyErr_ExceptionMatches(PyExc_AttributeError)) {
-                PyErr_WriteUnraisable(yf);
-            }
-            PyErr_Clear();
-        } else {
-            retval = PyObject_CallFunction(meth, NULL);
-            Py_DECREF(meth);
-            if (!retval)
-                err = -1;
-        }
-        gen->is_running = 0;
-    }
-    Py_XDECREF(retval);
-    return err;
-}
-static PyObject *__Pyx_Generator_Next(PyObject *self) {
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject*) self;
-    PyObject *yf = gen->yieldfrom;
-    if (unlikely(gen->is_running))
-        return __Pyx_Coroutine_AlreadyRunningError(gen);
-    if (yf) {
-        PyObject *ret;
-        gen->is_running = 1;
-        #ifdef __Pyx_Generator_USED
-        if (__Pyx_Generator_CheckExact(yf)) {
-            ret = __Pyx_Generator_Next(yf);
-        } else
-        #endif
-        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
-        if (PyGen_CheckExact(yf)) {
-            ret = __Pyx_PyGen_Send((PyGenObject*)yf, NULL);
-        } else
-        #endif
-        #ifdef __Pyx_Coroutine_USED
-        if (__Pyx_Coroutine_Check(yf)) {
-            ret = __Pyx_Coroutine_Send(yf, Py_None);
-        } else
-        #endif
-            ret = Py_TYPE(yf)->tp_iternext(yf);
-        gen->is_running = 0;
-        if (likely(ret)) {
-            return ret;
-        }
-        return __Pyx_Coroutine_FinishDelegation(gen);
-    }
-    return __Pyx_Coroutine_SendEx(gen, Py_None, 0);
-}
-static PyObject *__Pyx_Coroutine_Close_Method(PyObject *self, CYTHON_UNUSED PyObject *arg) {
-    return __Pyx_Coroutine_Close(self);
-}
-static PyObject *__Pyx_Coroutine_Close(PyObject *self) {
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
-    PyObject *retval, *raised_exception;
-    PyObject *yf = gen->yieldfrom;
-    int err = 0;
-    if (unlikely(gen->is_running))
-        return __Pyx_Coroutine_AlreadyRunningError(gen);
-    if (yf) {
-        Py_INCREF(yf);
-        err = __Pyx_Coroutine_CloseIter(gen, yf);
-        __Pyx_Coroutine_Undelegate(gen);
-        Py_DECREF(yf);
-    }
-    if (err == 0)
-        PyErr_SetNone(PyExc_GeneratorExit);
-    retval = __Pyx_Coroutine_SendEx(gen, NULL, 1);
-    if (unlikely(retval)) {
-        const char *msg;
-        Py_DECREF(retval);
-        if ((0)) {
-        #ifdef __Pyx_Coroutine_USED
-        } else if (__Pyx_Coroutine_Check(self)) {
-            msg = "coroutine ignored GeneratorExit";
-        #endif
-        #ifdef __Pyx_AsyncGen_USED
-        } else if (__Pyx_AsyncGen_CheckExact(self)) {
-#if PY_VERSION_HEX < 0x03060000
-            msg = "async generator ignored GeneratorExit - might require Python 3.6+ finalisation (PEP 525)";
-#else
-            msg = "async generator ignored GeneratorExit";
-#endif
-        #endif
-        } else {
-            msg = "generator ignored GeneratorExit";
-        }
-        PyErr_SetString(PyExc_RuntimeError, msg);
-        return NULL;
-    }
-    raised_exception = PyErr_Occurred();
-    if (likely(!raised_exception || __Pyx_PyErr_GivenExceptionMatches2(raised_exception, PyExc_GeneratorExit, PyExc_StopIteration))) {
-        if (raised_exception) PyErr_Clear();
-        Py_INCREF(Py_None);
-        return Py_None;
-    }
-    return NULL;
-}
-static PyObject *__Pyx__Coroutine_Throw(PyObject *self, PyObject *typ, PyObject *val, PyObject *tb,
-                                        PyObject *args, int close_on_genexit) {
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
-    PyObject *yf = gen->yieldfrom;
-    if (unlikely(gen->is_running))
-        return __Pyx_Coroutine_AlreadyRunningError(gen);
-    if (yf) {
-        PyObject *ret;
-        Py_INCREF(yf);
-        if (__Pyx_PyErr_GivenExceptionMatches(typ, PyExc_GeneratorExit) && close_on_genexit) {
-            int err = __Pyx_Coroutine_CloseIter(gen, yf);
-            Py_DECREF(yf);
-            __Pyx_Coroutine_Undelegate(gen);
-            if (err < 0)
-                return __Pyx_Coroutine_MethodReturn(self, __Pyx_Coroutine_SendEx(gen, NULL, 0));
-            goto throw_here;
-        }
-        gen->is_running = 1;
-        if (0
-        #ifdef __Pyx_Generator_USED
-            || __Pyx_Generator_CheckExact(yf)
-        #endif
-        #ifdef __Pyx_Coroutine_USED
-            || __Pyx_Coroutine_Check(yf)
-        #endif
-            ) {
-            ret = __Pyx__Coroutine_Throw(yf, typ, val, tb, args, close_on_genexit);
-        #ifdef __Pyx_Coroutine_USED
-        } else if (__Pyx_CoroutineAwait_CheckExact(yf)) {
-            ret = __Pyx__Coroutine_Throw(((__pyx_CoroutineAwaitObject*)yf)->coroutine, typ, val, tb, args, close_on_genexit);
-        #endif
-        } else {
-            PyObject *meth = __Pyx_PyObject_GetAttrStr(yf, __pyx_n_s_throw);
-            if (unlikely(!meth)) {
-                Py_DECREF(yf);
-                if (!PyErr_ExceptionMatches(PyExc_AttributeError)) {
-                    gen->is_running = 0;
-                    return NULL;
-                }
-                PyErr_Clear();
-                __Pyx_Coroutine_Undelegate(gen);
-                gen->is_running = 0;
-                goto throw_here;
-            }
-            if (likely(args)) {
-                ret = PyObject_CallObject(meth, args);
-            } else {
-                ret = PyObject_CallFunctionObjArgs(meth, typ, val, tb, NULL);
-            }
-            Py_DECREF(meth);
-        }
-        gen->is_running = 0;
-        Py_DECREF(yf);
-        if (!ret) {
-            ret = __Pyx_Coroutine_FinishDelegation(gen);
-        }
-        return __Pyx_Coroutine_MethodReturn(self, ret);
-    }
-throw_here:
-    __Pyx_Raise(typ, val, tb, NULL);
-    return __Pyx_Coroutine_MethodReturn(self, __Pyx_Coroutine_SendEx(gen, NULL, 0));
-}
-static PyObject *__Pyx_Coroutine_Throw(PyObject *self, PyObject *args) {
-    PyObject *typ;
-    PyObject *val = NULL;
-    PyObject *tb = NULL;
-    if (!PyArg_UnpackTuple(args, (char *)"throw", 1, 3, &typ, &val, &tb))
-        return NULL;
-    return __Pyx__Coroutine_Throw(self, typ, val, tb, args, 1);
-}
-static CYTHON_INLINE int __Pyx_Coroutine_traverse_excstate(__Pyx_ExcInfoStruct *exc_state, visitproc visit, void *arg) {
-    Py_VISIT(exc_state->exc_type);
-    Py_VISIT(exc_state->exc_value);
-    Py_VISIT(exc_state->exc_traceback);
-    return 0;
-}
-static int __Pyx_Coroutine_traverse(__pyx_CoroutineObject *gen, visitproc visit, void *arg) {
-    Py_VISIT(gen->closure);
-    Py_VISIT(gen->classobj);
-    Py_VISIT(gen->yieldfrom);
-    return __Pyx_Coroutine_traverse_excstate(&gen->gi_exc_state, visit, arg);
-}
-static int __Pyx_Coroutine_clear(PyObject *self) {
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
-    Py_CLEAR(gen->closure);
-    Py_CLEAR(gen->classobj);
-    Py_CLEAR(gen->yieldfrom);
-    __Pyx_Coroutine_ExceptionClear(&gen->gi_exc_state);
-#ifdef __Pyx_AsyncGen_USED
-    if (__Pyx_AsyncGen_CheckExact(self)) {
-        Py_CLEAR(((__pyx_PyAsyncGenObject*)gen)->ag_finalizer);
-    }
-#endif
-    Py_CLEAR(gen->gi_code);
-    Py_CLEAR(gen->gi_frame);
-    Py_CLEAR(gen->gi_name);
-    Py_CLEAR(gen->gi_qualname);
-    Py_CLEAR(gen->gi_modulename);
-    return 0;
-}
-static void __Pyx_Coroutine_dealloc(PyObject *self) {
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
-    PyObject_GC_UnTrack(gen);
-    if (gen->gi_weakreflist != NULL)
-        PyObject_ClearWeakRefs(self);
-    if (gen->resume_label >= 0) {
-        PyObject_GC_Track(self);
-#if PY_VERSION_HEX >= 0x030400a1 && CYTHON_USE_TP_FINALIZE
-        if (PyObject_CallFinalizerFromDealloc(self))
-#else
-        Py_TYPE(gen)->tp_del(self);
-        if (Py_REFCNT(self) > 0)
-#endif
-        {
-            return;
-        }
-        PyObject_GC_UnTrack(self);
-    }
-#ifdef __Pyx_AsyncGen_USED
-    if (__Pyx_AsyncGen_CheckExact(self)) {
-        /* We have to handle this case for asynchronous generators
-           right here, because this code has to be between UNTRACK
-           and GC_Del. */
-        Py_CLEAR(((__pyx_PyAsyncGenObject*)self)->ag_finalizer);
-    }
-#endif
-    __Pyx_Coroutine_clear(self);
-    PyObject_GC_Del(gen);
-}
-static void __Pyx_Coroutine_del(PyObject *self) {
-    PyObject *error_type, *error_value, *error_traceback;
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
-    __Pyx_PyThreadState_declare
-    if (gen->resume_label < 0) {
-        return;
-    }
-#if !CYTHON_USE_TP_FINALIZE
-    assert(self->ob_refcnt == 0);
-    __Pyx_SET_REFCNT(self, 1);
-#endif
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&error_type, &error_value, &error_traceback);
-#ifdef __Pyx_AsyncGen_USED
-    if (__Pyx_AsyncGen_CheckExact(self)) {
-        __pyx_PyAsyncGenObject *agen = (__pyx_PyAsyncGenObject*)self;
-        PyObject *finalizer = agen->ag_finalizer;
-        if (finalizer && !agen->ag_closed) {
-            PyObject *res = __Pyx_PyObject_CallOneArg(finalizer, self);
-            if (unlikely(!res)) {
-                PyErr_WriteUnraisable(self);
-            } else {
-                Py_DECREF(res);
-            }
-            __Pyx_ErrRestore(error_type, error_value, error_traceback);
-            return;
-        }
-    }
-#endif
-    if (unlikely(gen->resume_label == 0 && !error_value)) {
-#ifdef __Pyx_Coroutine_USED
-#ifdef __Pyx_Generator_USED
-    if (!__Pyx_Generator_CheckExact(self))
-#endif
-        {
-        PyObject_GC_UnTrack(self);
-#if PY_MAJOR_VERSION >= 3  || defined(PyErr_WarnFormat)
-        if (unlikely(PyErr_WarnFormat(PyExc_RuntimeWarning, 1, "coroutine '%.50S' was never awaited", gen->gi_qualname) < 0))
-            PyErr_WriteUnraisable(self);
-#else
-        {PyObject *msg;
-        char *cmsg;
-        #if CYTHON_COMPILING_IN_PYPY
-        msg = NULL;
-        cmsg = (char*) "coroutine was never awaited";
-        #else
-        char *cname;
-        PyObject *qualname;
-        qualname = gen->gi_qualname;
-        cname = PyString_AS_STRING(qualname);
-        msg = PyString_FromFormat("coroutine '%.50s' was never awaited", cname);
-        if (unlikely(!msg)) {
-            PyErr_Clear();
-            cmsg = (char*) "coroutine was never awaited";
-        } else {
-            cmsg = PyString_AS_STRING(msg);
-        }
-        #endif
-        if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning, cmsg, 1) < 0))
-            PyErr_WriteUnraisable(self);
-        Py_XDECREF(msg);}
-#endif
-        PyObject_GC_Track(self);
-        }
-#endif
-    } else {
-        PyObject *res = __Pyx_Coroutine_Close(self);
-        if (unlikely(!res)) {
-            if (PyErr_Occurred())
-                PyErr_WriteUnraisable(self);
-        } else {
-            Py_DECREF(res);
-        }
-    }
-    __Pyx_ErrRestore(error_type, error_value, error_traceback);
-#if !CYTHON_USE_TP_FINALIZE
-    assert(Py_REFCNT(self) > 0);
-    if (--self->ob_refcnt == 0) {
-        return;
-    }
-    {
-        Py_ssize_t refcnt = Py_REFCNT(self);
-        _Py_NewReference(self);
-        __Pyx_SET_REFCNT(self, refcnt);
-    }
-#if CYTHON_COMPILING_IN_CPYTHON
-    assert(PyType_IS_GC(Py_TYPE(self)) &&
-           _Py_AS_GC(self)->gc.gc_refs != _PyGC_REFS_UNTRACKED);
-    _Py_DEC_REFTOTAL;
-#endif
-#ifdef COUNT_ALLOCS
-    --Py_TYPE(self)->tp_frees;
-    --Py_TYPE(self)->tp_allocs;
-#endif
-#endif
-}
-static PyObject *
-__Pyx_Coroutine_get_name(__pyx_CoroutineObject *self, CYTHON_UNUSED void *context)
-{
-    PyObject *name = self->gi_name;
-    if (unlikely(!name)) name = Py_None;
-    Py_INCREF(name);
-    return name;
-}
-static int
-__Pyx_Coroutine_set_name(__pyx_CoroutineObject *self, PyObject *value, CYTHON_UNUSED void *context)
-{
-    PyObject *tmp;
-#if PY_MAJOR_VERSION >= 3
-    if (unlikely(value == NULL || !PyUnicode_Check(value)))
-#else
-    if (unlikely(value == NULL || !PyString_Check(value)))
-#endif
-    {
-        PyErr_SetString(PyExc_TypeError,
-                        "__name__ must be set to a string object");
-        return -1;
-    }
-    tmp = self->gi_name;
-    Py_INCREF(value);
-    self->gi_name = value;
-    Py_XDECREF(tmp);
-    return 0;
-}
-static PyObject *
-__Pyx_Coroutine_get_qualname(__pyx_CoroutineObject *self, CYTHON_UNUSED void *context)
-{
-    PyObject *name = self->gi_qualname;
-    if (unlikely(!name)) name = Py_None;
-    Py_INCREF(name);
-    return name;
-}
-static int
-__Pyx_Coroutine_set_qualname(__pyx_CoroutineObject *self, PyObject *value, CYTHON_UNUSED void *context)
-{
-    PyObject *tmp;
-#if PY_MAJOR_VERSION >= 3
-    if (unlikely(value == NULL || !PyUnicode_Check(value)))
-#else
-    if (unlikely(value == NULL || !PyString_Check(value)))
-#endif
-    {
-        PyErr_SetString(PyExc_TypeError,
-                        "__qualname__ must be set to a string object");
-        return -1;
-    }
-    tmp = self->gi_qualname;
-    Py_INCREF(value);
-    self->gi_qualname = value;
-    Py_XDECREF(tmp);
-    return 0;
-}
-static PyObject *
-__Pyx_Coroutine_get_frame(__pyx_CoroutineObject *self, CYTHON_UNUSED void *context)
-{
-    PyObject *frame = self->gi_frame;
-    if (!frame) {
-        if (unlikely(!self->gi_code)) {
-            Py_RETURN_NONE;
-        }
-        frame = (PyObject *) PyFrame_New(
-            PyThreadState_Get(),            /*PyThreadState *tstate,*/
-            (PyCodeObject*) self->gi_code,  /*PyCodeObject *code,*/
-            __pyx_d,                 /*PyObject *globals,*/
-            0                               /*PyObject *locals*/
-        );
-        if (unlikely(!frame))
-            return NULL;
-        self->gi_frame = frame;
-    }
-    Py_INCREF(frame);
-    return frame;
-}
-static __pyx_CoroutineObject *__Pyx__Coroutine_New(
-            PyTypeObject* type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
-            PyObject *name, PyObject *qualname, PyObject *module_name) {
-    __pyx_CoroutineObject *gen = PyObject_GC_New(__pyx_CoroutineObject, type);
-    if (unlikely(!gen))
-        return NULL;
-    return __Pyx__Coroutine_NewInit(gen, body, code, closure, name, qualname, module_name);
-}
-static __pyx_CoroutineObject *__Pyx__Coroutine_NewInit(
-            __pyx_CoroutineObject *gen, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
-            PyObject *name, PyObject *qualname, PyObject *module_name) {
-    gen->body = body;
-    gen->closure = closure;
-    Py_XINCREF(closure);
-    gen->is_running = 0;
-    gen->resume_label = 0;
-    gen->classobj = NULL;
-    gen->yieldfrom = NULL;
-    gen->gi_exc_state.exc_type = NULL;
-    gen->gi_exc_state.exc_value = NULL;
-    gen->gi_exc_state.exc_traceback = NULL;
-#if CYTHON_USE_EXC_INFO_STACK
-    gen->gi_exc_state.previous_item = NULL;
-#endif
-    gen->gi_weakreflist = NULL;
-    Py_XINCREF(qualname);
-    gen->gi_qualname = qualname;
-    Py_XINCREF(name);
-    gen->gi_name = name;
-    Py_XINCREF(module_name);
-    gen->gi_modulename = module_name;
-    Py_XINCREF(code);
-    gen->gi_code = code;
-    gen->gi_frame = NULL;
-    PyObject_GC_Track(gen);
-    return gen;
-}
-
-/* PatchModuleWithCoroutine */
-static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code) {
-#if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
-    int result;
-    PyObject *globals, *result_obj;
-    globals = PyDict_New();  if (unlikely(!globals)) goto ignore;
-    result = PyDict_SetItemString(globals, "_cython_coroutine_type",
-    #ifdef __Pyx_Coroutine_USED
-        (PyObject*)__pyx_CoroutineType);
-    #else
-        Py_None);
-    #endif
-    if (unlikely(result < 0)) goto ignore;
-    result = PyDict_SetItemString(globals, "_cython_generator_type",
-    #ifdef __Pyx_Generator_USED
-        (PyObject*)__pyx_GeneratorType);
-    #else
-        Py_None);
-    #endif
-    if (unlikely(result < 0)) goto ignore;
-    if (unlikely(PyDict_SetItemString(globals, "_module", module) < 0)) goto ignore;
-    if (unlikely(PyDict_SetItemString(globals, "__builtins__", __pyx_b) < 0)) goto ignore;
-    result_obj = PyRun_String(py_code, Py_file_input, globals, globals);
-    if (unlikely(!result_obj)) goto ignore;
-    Py_DECREF(result_obj);
-    Py_DECREF(globals);
-    return module;
-ignore:
-    Py_XDECREF(globals);
-    PyErr_WriteUnraisable(module);
-    if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning, "Cython module failed to patch module with custom type", 1) < 0)) {
-        Py_DECREF(module);
-        module = NULL;
-    }
-#else
-    py_code++;
-#endif
-    return module;
-}
-
-/* PatchGeneratorABC */
-#ifndef CYTHON_REGISTER_ABCS
-#define CYTHON_REGISTER_ABCS 1
-#endif
-#if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
-static PyObject* __Pyx_patch_abc_module(PyObject *module);
-static PyObject* __Pyx_patch_abc_module(PyObject *module) {
-    module = __Pyx_Coroutine_patch_module(
-        module, ""
-"if _cython_generator_type is not None:\n"
-"    try: Generator = _module.Generator\n"
-"    except AttributeError: pass\n"
-"    else: Generator.register(_cython_generator_type)\n"
-"if _cython_coroutine_type is not None:\n"
-"    try: Coroutine = _module.Coroutine\n"
-"    except AttributeError: pass\n"
-"    else: Coroutine.register(_cython_coroutine_type)\n"
-    );
-    return module;
-}
-#endif
-static int __Pyx_patch_abc(void) {
-#if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
-    static int abc_patched = 0;
-    if (CYTHON_REGISTER_ABCS && !abc_patched) {
-        PyObject *module;
-        module = PyImport_ImportModule((PY_MAJOR_VERSION >= 3) ? "collections.abc" : "collections");
-        if (!module) {
-            PyErr_WriteUnraisable(NULL);
-            if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning,
-                    ((PY_MAJOR_VERSION >= 3) ?
-                        "Cython module failed to register with collections.abc module" :
-                        "Cython module failed to register with collections module"), 1) < 0)) {
-                return -1;
-            }
-        } else {
-            module = __Pyx_patch_abc_module(module);
-            abc_patched = 1;
-            if (unlikely(!module))
-                return -1;
-            Py_DECREF(module);
-        }
-        module = PyImport_ImportModule("backports_abc");
-        if (module) {
-            module = __Pyx_patch_abc_module(module);
-            Py_XDECREF(module);
-        }
-        if (!module) {
-            PyErr_Clear();
-        }
-    }
-#else
-    if ((0)) __Pyx_Coroutine_patch_module(NULL, NULL);
-#endif
-    return 0;
-}
-
-/* Generator */
-static PyMethodDef __pyx_Generator_methods[] = {
-    {"send", (PyCFunction) __Pyx_Coroutine_Send, METH_O,
-     (char*) PyDoc_STR("send(arg) -> send 'arg' into generator,\nreturn next yielded value or raise StopIteration.")},
-    {"throw", (PyCFunction) __Pyx_Coroutine_Throw, METH_VARARGS,
-     (char*) PyDoc_STR("throw(typ[,val[,tb]]) -> raise exception in generator,\nreturn next yielded value or raise StopIteration.")},
-    {"close", (PyCFunction) __Pyx_Coroutine_Close_Method, METH_NOARGS,
-     (char*) PyDoc_STR("close() -> raise GeneratorExit inside generator.")},
-    {0, 0, 0, 0}
-};
-static PyMemberDef __pyx_Generator_memberlist[] = {
-    {(char *) "gi_running", T_BOOL, offsetof(__pyx_CoroutineObject, is_running), READONLY, NULL},
-    {(char*) "gi_yieldfrom", T_OBJECT, offsetof(__pyx_CoroutineObject, yieldfrom), READONLY,
-     (char*) PyDoc_STR("object being iterated by 'yield from', or None")},
-    {(char*) "gi_code", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_code), READONLY, NULL},
-    {0, 0, 0, 0, 0}
-};
-static PyGetSetDef __pyx_Generator_getsets[] = {
-    {(char *) "__name__", (getter)__Pyx_Coroutine_get_name, (setter)__Pyx_Coroutine_set_name,
-     (char*) PyDoc_STR("name of the generator"), 0},
-    {(char *) "__qualname__", (getter)__Pyx_Coroutine_get_qualname, (setter)__Pyx_Coroutine_set_qualname,
-     (char*) PyDoc_STR("qualified name of the generator"), 0},
-    {(char *) "gi_frame", (getter)__Pyx_Coroutine_get_frame, NULL,
-     (char*) PyDoc_STR("Frame of the generator"), 0},
-    {0, 0, 0, 0, 0}
-};
-static PyTypeObject __pyx_GeneratorType_type = {
-    PyVarObject_HEAD_INIT(0, 0)
-    "generator",
-    sizeof(__pyx_CoroutineObject),
-    0,
-    (destructor) __Pyx_Coroutine_dealloc,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_HAVE_FINALIZE,
-    0,
-    (traverseproc) __Pyx_Coroutine_traverse,
-    0,
-    0,
-    offsetof(__pyx_CoroutineObject, gi_weakreflist),
-    0,
-    (iternextfunc) __Pyx_Generator_Next,
-    __pyx_Generator_methods,
-    __pyx_Generator_memberlist,
-    __pyx_Generator_getsets,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-#if CYTHON_USE_TP_FINALIZE
-    0,
-#else
-    __Pyx_Coroutine_del,
-#endif
-    0,
-#if CYTHON_USE_TP_FINALIZE
-    __Pyx_Coroutine_del,
-#elif PY_VERSION_HEX >= 0x030400a1
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-    0,
-#endif
-};
-static int __pyx_Generator_init(void) {
-    __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
-    __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
-    __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
-    if (unlikely(!__pyx_GeneratorType)) {
-        return -1;
-    }
-    return 0;
-}
-
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
     char ctversion[5];
     int same=1, i, found_dot;
     const char* rt_from_call = Py_GetVersion();
     PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
     found_dot = 0;
```

### Comparing `multimcts-0.2.1/multimcts/mcts.pyx` & `multimcts-0.2.2/multimcts/mcts.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from time import time
 from random import shuffle, choice
 from collections import defaultdict
 from typing import Union, Any
 
+import cython
+
 from libc.math cimport log, sqrt, INFINITY
 
 
-class GameState():
+class GameState:
     def get_current_team(self) -> Union[int,str]:
         """The identifier of the current player's team."""
         raise NotImplementedError("GameState must implement get_current_team.")
 
     def get_legal_moves(self) -> list[Any]:
         """Returns a list of all legal moves from this state."""
         raise NotImplementedError("GameState must implement get_legal_moves.")
@@ -30,15 +32,15 @@
         Typically 1 for win, -1 for loss, 0 for draw.
         Alternatively, returns a dict of teams/rewards: {team1:reward1, team2:reward2, ...}
         Note: This method is only called on terminal states.
         """
         raise NotImplementedError("GameState must implement get_reward.")
 
 
-class Node():
+class Node:
     """Represents a game state node in the MCTS search tree.
 
     Args:
         state (GameState): The game state at the current node.
         parent (Node): The parent of the current node in the search tree.
 
     Attributes:
@@ -50,28 +52,28 @@
         remaining_moves (list): A list of moves that have not yet been tried.
     """
     def __init__(self, state:GameState, parent:'Node'=None):
         self.state = state
         self.parent = parent
 
         self.children:list['Node'] = []
-        self.num_visits:int = 0
+        self.num_visits = 0
         self.total_reward = defaultdict(float)
 
         self.is_terminal:bool = self.state.is_terminal()
         self.is_fully_expanded:bool = self.is_terminal
 
         if self.is_fully_expanded:
             self.remaining_moves = []
         else:
             self.remaining_moves = self.state.get_legal_moves()
             shuffle(self.remaining_moves)
 
 
-class MCTS():
+class MCTS:
     def __init__(self, exploration_bias:float=1.414):
         """Initializes an MCTS agent.
 
         Args:
             exploration_bias (float): The exploration bias, often denoted as C in the UCB formula.
                 It determines the balance between exploration (choosing a move with uncertain outcome) and exploitation (choosing a move with known high reward).
                 Default is 1.414, which is sqrt(2) and often used in practice.
@@ -186,37 +188,44 @@
             node.num_visits += 1
 
             for key in reward:
                 node.total_reward[key] += reward[key]
 
             node = node.parent
 
+    @cython.cdivision(True)
     def get_best_child(self, node:Node) -> Node:
-        cur_team = node.state.get_current_team()
-
+        """Find the child with the highest Upper Confidence Bound (UCB) score.
+        ucb = (x / n) + C * sqrt(ln(N) / n)
+        x=reward for this node
+        n=number of simulations for this node
+        N=number of simulations for parent node
+        C=exploration bias
+        """
         # Initialize UCB variables.
         cdef int visits
-        cdef double reward, score
+        cdef double reward, subreward, ucb
         cdef double exploration_bias = self.exploration_bias
         cdef double ln_parent_visits = log(node.num_visits)
 
-        cdef double max_score = -INFINITY
-        best:Node = None
+        cur_team = node.state.get_current_team()
+
+        cdef double best_score = -INFINITY
+        best_child:Node = None
 
         for child in node.children:
-            # Relative reward is this child's reward minus its siblings' rewards.
-            reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())
             visits = child.num_visits
+            if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
+                continue
+
+            # Relative reward is this child's reward minus its siblings' rewards.
+            reward = 2 * child.total_reward[cur_team]
+            for subreward in child.total_reward.values():
+                reward -= subreward
+
+            ucb = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
 
-            """UCB := (x / n) + C * sqrt(ln(N) / n)
-            x=reward for this node
-            n=number of simulations for this node
-            N=number of simulations for parent node
-            C=exploration bias
-            """
-            score = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
-
-            if score > max_score:
-                max_score = score
-                best = child
+            if ucb > best_score:
+                best_score = ucb
+                best_child = child
 
-        return best
+        return best_child
```

### Comparing `multimcts-0.2.1/multimcts.egg-info/PKG-INFO` & `multimcts-0.2.2/multimcts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimcts
-Version: 0.2.1
+Version: 0.2.2
 Summary: Monte Carlo Tree Search for multiple teams
 Home-page: https://github.com/taylorvance/multimcts
 Author: Taylor Vance
 Author-email: mirrors.cities0w@icloud.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `multimcts-0.2.1/setup.py` & `multimcts-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from Cython.Build import cythonize
 
 setup(
     name="multimcts",
-    version="0.2.1",
+    version="0.2.2",
     author="Taylor Vance",
     author_email="mirrors.cities0w@icloud.com",
     url="https://github.com/taylorvance/multimcts",
     description="Monte Carlo Tree Search for multiple teams",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT",
```

