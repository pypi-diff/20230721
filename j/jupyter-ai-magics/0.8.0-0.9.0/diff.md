# Comparing `tmp/jupyter_ai_magics-0.8.0.tar.gz` & `tmp/jupyter_ai_magics-0.9.0.tar.gz`

## Comparing `jupyter_ai_magics-0.8.0.tar` & `jupyter_ai_magics-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/setup.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/_version.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/aliases.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/embedding_providers.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/exception.py
--rw-r--r--   0        0        0    21622 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/magics.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/parsers.py
--rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/providers.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/tests/__init__.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/LICENSE
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/README.md
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/setup.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/_version.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/aliases.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/embedding_providers.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/exception.py
+-rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/magics.py
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/parsers.py
+-rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/providers.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/tests/__init__.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/LICENSE
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/README.md
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/PKG-INFO
```

### Comparing `jupyter_ai_magics-0.8.0/package.json` & `jupyter_ai_magics-0.9.0/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'scripts'": '{\'dev-install\': \'pip install -e ".[dev,all]"\'}', "'version'": "'0.9.0'"}*

```diff
@@ -13,12 +13,12 @@
     "name": "@jupyter-ai/magics",
     "private": true,
     "repository": {
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-ai.git"
     },
     "scripts": {
-        "dev-install": "pip install -e \".[all]\"",
+        "dev-install": "pip install -e \".[dev,all]\"",
         "dev-uninstall": "pip uninstall jupyter_ai_magics -y"
     },
-    "version": "0.8.0"
+    "version": "0.9.0"
 }
```

### Comparing `jupyter_ai_magics-0.8.0/jupyter_ai_magics/__init__.py` & `jupyter_ai_magics-0.9.0/jupyter_ai_magics/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from ._version import __version__
+
+# expose embedding model providers on the package root
+from .embedding_providers import (
+    CohereEmbeddingsProvider,
+    HfHubEmbeddingsProvider,
+    OpenAIEmbeddingsProvider,
+)
 from .exception import store_exception
 from .magics import AiMagics
 
 # expose model providers on the package root
 from .providers import (
     AI21Provider,
     AnthropicProvider,
+    BaseProvider,
+    ChatOpenAINewProvider,
+    ChatOpenAIProvider,
     CohereProvider,
     HfHubProvider,
     OpenAIProvider,
-    ChatOpenAIProvider,
-    ChatOpenAINewProvider,
-    SmEndpointProvider
-)
-# expose embedding model providers on the package root
-from .embedding_providers import (
-    OpenAIEmbeddingsProvider,
-    CohereEmbeddingsProvider,
-    HfHubEmbeddingsProvider
+    SmEndpointProvider,
 )
-from .providers import BaseProvider
+
 
 def load_ipython_extension(ipython):
     ipython.register_magics(AiMagics)
     ipython.set_custom_exc((BaseException,), store_exception)
 
+
 def unload_ipython_extension(ipython):
     ipython.set_custom_exc((BaseException,), ipython.CustomTB)
```

### Comparing `jupyter_ai_magics-0.8.0/jupyter_ai_magics/embedding_providers.py` & `jupyter_ai_magics-0.9.0/jupyter_ai_magics/embedding_providers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from typing import ClassVar, List, Type
+
 from jupyter_ai_magics.providers import AuthStrategy, EnvAuthStrategy, Field
-from pydantic import BaseModel, Extra
-from langchain.embeddings import OpenAIEmbeddings, CohereEmbeddings, HuggingFaceHubEmbeddings
+from langchain.embeddings import (
+    CohereEmbeddings,
+    HuggingFaceHubEmbeddings,
+    OpenAIEmbeddings,
+)
 from langchain.embeddings.base import Embeddings
+from pydantic import BaseModel, Extra
 
 
 class BaseEmbeddingsProvider(BaseModel):
     """Base class for embedding providers"""
 
     class Config:
         extra = Extra.allow
@@ -29,44 +34,38 @@
 
     auth_strategy: ClassVar[AuthStrategy] = None
     """Authentication/authorization strategy. Declares what credentials are
     required to use this model provider. Generally should not be `None`."""
 
     model_id: str
 
-    provider_klass: ClassVar[Type[Embeddings]]    
+    provider_klass: ClassVar[Type[Embeddings]]
 
     registry: ClassVar[bool] = False
     """Whether this provider is a registry provider."""
 
     fields: ClassVar[List[Field]] = []
     """Fields expected by this provider in its constructor. Each `Field` `f`
     should be passed as a keyword argument, keyed by `f.key`."""
-    
+
 
 class OpenAIEmbeddingsProvider(BaseEmbeddingsProvider):
     id = "openai"
     name = "OpenAI"
-    models = [
-        "text-embedding-ada-002"
-    ]
+    models = ["text-embedding-ada-002"]
     model_id_key = "model"
     pypi_package_deps = ["openai"]
     auth_strategy = EnvAuthStrategy(name="OPENAI_API_KEY")
     provider_klass = OpenAIEmbeddings
 
 
 class CohereEmbeddingsProvider(BaseEmbeddingsProvider):
     id = "cohere"
     name = "Cohere"
-    models = [
-        'large',
-        'multilingual-22-12',
-        'small'
-    ]
+    models = ["large", "multilingual-22-12", "small"]
     model_id_key = "model"
     pypi_package_deps = ["cohere"]
     auth_strategy = EnvAuthStrategy(name="COHERE_API_KEY")
     provider_klass = CohereEmbeddings
 
 
 class HfHubEmbeddingsProvider(BaseEmbeddingsProvider):
```

### Comparing `jupyter_ai_magics-0.8.0/jupyter_ai_magics/exception.py` & `jupyter_ai_magics-0.9.0/jupyter_ai_magics/exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-from IPython.core.magic import register_line_magic
+import traceback
+
 from IPython.core.getipython import get_ipython
+from IPython.core.magic import register_line_magic
 from IPython.core.ultratb import ListTB
 
-import traceback
 
 def store_exception(shell, etype, evalue, tb, tb_offset=None):
     # A structured traceback (a list of strings) or None
- 
+
     if issubclass(etype, SyntaxError):
         # Disable ANSI color strings
         shell.SyntaxTB.color_toggle()
         # Don't display a stacktrace because a syntax error has no stacktrace
         stb = shell.SyntaxTB.structured_traceback(etype, evalue, [])
         stb_text = shell.SyntaxTB.stb2text(stb)
         # Re-enable ANSI color strings
         shell.SyntaxTB.color_toggle()
     else:
         # Disable ANSI color strings
         shell.InteractiveTB.color_toggle()
-        stb = shell.InteractiveTB.structured_traceback(etype, evalue, tb, tb_offset=tb_offset)
+        stb = shell.InteractiveTB.structured_traceback(
+            etype, evalue, tb, tb_offset=tb_offset
+        )
         stb_text = shell.InteractiveTB.stb2text(stb)
         # Re-enable ANSI color strings
         shell.InteractiveTB.color_toggle()
 
     etraceback = shell.showtraceback()
 
     styled_exception = str(stb_text)
 
     prompt_number = shell.execution_count
     err = shell.user_ns.get("Err", {})
     err[prompt_number] = styled_exception
     shell.user_ns["Err"] = err
-    
-    # Return 
+
+    # Return
     return etraceback
```

### Comparing `jupyter_ai_magics-0.8.0/jupyter_ai_magics/magics.py` & `jupyter_ai_magics-0.9.0/jupyter_ai_magics/magics.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,416 +5,445 @@
 import re
 import sys
 import warnings
 from typing import Optional
 
 import click
 from IPython import get_ipython
-from IPython.core.magic import Magics, magics_class, line_cell_magic
+from IPython.core.magic import Magics, line_cell_magic, magics_class
 from IPython.display import HTML, JSON, Markdown, Math
 from jupyter_ai_magics.utils import decompose_model_id, load_providers
+from langchain.chains import LLMChain
 
-from .providers import BaseProvider
-from .parsers import (cell_magic_parser,
-    line_magic_parser,
+from .parsers import (
     CellArgs,
     DeleteArgs,
     ErrorArgs,
     HelpArgs,
     ListArgs,
     RegisterArgs,
-    UpdateArgs)
-
-from langchain.chains import LLMChain
+    UpdateArgs,
+    cell_magic_parser,
+    line_magic_parser,
+)
+from .providers import BaseProvider
 
 MODEL_ID_ALIASES = {
     "gpt2": "huggingface_hub:gpt2",
     "gpt3": "openai:text-davinci-003",
     "chatgpt": "openai-chat:gpt-3.5-turbo",
     "gpt4": "openai-chat:gpt-4",
 }
 
-class TextOrMarkdown(object):
 
+class TextOrMarkdown:
     def __init__(self, text, markdown):
         self.text = text
         self.markdown = markdown
 
     def _repr_mimebundle_(self, include=None, exclude=None):
-        return (
-            {
-                'text/plain': self.text,
-                'text/markdown': self.markdown
-            }
-        )
+        return {"text/plain": self.text, "text/markdown": self.markdown}
 
 
-class TextWithMetadata(object):
+class TextWithMetadata:
     def __init__(self, text, metadata):
         self.text = text
         self.metadata = metadata
 
+    def __str__(self):
+        return self.text
+
     def _repr_mimebundle_(self, include=None, exclude=None):
-        return ({'text/plain': self.text}, self.metadata)
+        return ({"text/plain": self.text}, self.metadata)
 
 
 class Base64Image:
     def __init__(self, mimeData, metadata):
-        mimeDataParts = mimeData.split(',')
-        self.data = base64.b64decode(mimeDataParts[1]);
-        self.mimeType = re.sub(r';base64$', '', mimeDataParts[0])
+        mimeDataParts = mimeData.split(",")
+        self.data = base64.b64decode(mimeDataParts[1])
+        self.mimeType = re.sub(r";base64$", "", mimeDataParts[0])
         self.metadata = metadata
 
     def _repr_mimebundle_(self, include=None, exclude=None):
         return ({self.mimeType: self.data}, self.metadata)
 
 
 DISPLAYS_BY_FORMAT = {
     "code": None,
     "html": HTML,
     "image": Base64Image,
     "markdown": Markdown,
     "math": Math,
     "md": Markdown,
     "json": JSON,
-    "text": TextWithMetadata
+    "text": TextWithMetadata,
 }
 
 NA_MESSAGE = '<abbr title="Not applicable">N/A</abbr>'
 
-MARKDOWN_PROMPT_TEMPLATE = '{prompt}\n\nProduce output in markdown format only.'
+MARKDOWN_PROMPT_TEMPLATE = "{prompt}\n\nProduce output in markdown format only."
 
-PROVIDER_NO_MODELS = 'This provider does not define a list of models.'
+PROVIDER_NO_MODELS = "This provider does not define a list of models."
 
 CANNOT_DETERMINE_MODEL_TEXT = """Cannot determine model provider from model ID '{0}'.
 
 To see a list of models you can use, run '%ai list'"""
 
 CANNOT_DETERMINE_MODEL_MARKDOWN = """Cannot determine model provider from model ID `{0}`.
 
 To see a list of models you can use, run `%ai list`"""
 
 
 PROMPT_TEMPLATES_BY_FORMAT = {
-    "code": '{prompt}\n\nProduce output as source code only, with no text or explanation before or after it.',
-    "html": '{prompt}\n\nProduce output in HTML format only, with no markup before or afterward.',
-    "image": '{prompt}\n\nProduce output as an image only, with no text before or after it.',
+    "code": "{prompt}\n\nProduce output as source code only, with no text or explanation before or after it.",
+    "html": "{prompt}\n\nProduce output in HTML format only, with no markup before or afterward.",
+    "image": "{prompt}\n\nProduce output as an image only, with no text before or after it.",
     "markdown": MARKDOWN_PROMPT_TEMPLATE,
     "md": MARKDOWN_PROMPT_TEMPLATE,
-    "math": '{prompt}\n\nProduce output in LaTeX format only, with $$ at the beginning and end.',
-    "json": '{prompt}\n\nProduce output in JSON format only, with nothing before or after it.',
-    "text": '{prompt}' # No customization
+    "math": "{prompt}\n\nProduce output in LaTeX format only, with $$ at the beginning and end.",
+    "json": "{prompt}\n\nProduce output in JSON format only, with nothing before or after it.",
+    "text": "{prompt}",  # No customization
 }
 
-AI_COMMANDS = { "delete", "error", "help", "list", "register", "update" }
+AI_COMMANDS = {"delete", "error", "help", "list", "register", "update"}
+
 
 class FormatDict(dict):
     """Subclass of dict to be passed to str#format(). Suppresses KeyError and
     leaves replacement field unchanged if replacement field is not associated
     with a value."""
-    def __missing__(self, key): 
+
+    def __missing__(self, key):
         return key.join("{}")
 
+
 class EnvironmentError(BaseException):
     pass
 
+
 class CellMagicError(BaseException):
     pass
 
+
 @magics_class
 class AiMagics(Magics):
     def __init__(self, shell):
-        super(AiMagics, self).__init__(shell)
+        super().__init__(shell)
         self.transcript_openai = []
 
         # suppress warning when using old OpenAIChat provider
-        warnings.filterwarnings("ignore", message="You are trying to use a chat model. This way of initializing it is "
+        warnings.filterwarnings(
+            "ignore",
+            message="You are trying to use a chat model. This way of initializing it is "
             "no longer supported. Instead, please use: "
-            "`from langchain.chat_models import ChatOpenAI`")
+            "`from langchain.chat_models import ChatOpenAI`",
+        )
 
         self.providers = load_providers()
-        
+
         # initialize a registry of custom model/chain names
         self.custom_model_registry = MODEL_ID_ALIASES
-    
+
     def _ai_bulleted_list_models_for_provider(self, provider_id, Provider):
         output = ""
-        if (len(Provider.models) == 1 and Provider.models[0] == "*"):
+        if len(Provider.models) == 1 and Provider.models[0] == "*":
             output += f"* {PROVIDER_NO_MODELS}\n"
         else:
             for model_id in Provider.models:
-                output += f"* {provider_id}:{model_id}\n";
-        output += "\n" # End of bulleted list
-        
+                output += f"* {provider_id}:{model_id}\n"
+        output += "\n"  # End of bulleted list
+
         return output
 
     def _ai_inline_list_models_for_provider(self, provider_id, Provider):
         output = ""
 
-        if (len(Provider.models) == 1 and Provider.models[0] == "*"):
+        if len(Provider.models) == 1 and Provider.models[0] == "*":
             return PROVIDER_NO_MODELS
 
         for model_id in Provider.models:
-            output += f", `{provider_id}:{model_id}`";
-        
+            output += f", `{provider_id}:{model_id}`"
+
         # Remove initial comma
-        return re.sub(r'^, ', '', output)
-    
+        return re.sub(r"^, ", "", output)
+
     # Is the required environment variable set?
     def _ai_env_status_for_provider_markdown(self, provider_id):
-        na_message = 'Not applicable. | ' + NA_MESSAGE
+        na_message = "Not applicable. | " + NA_MESSAGE
+
+        if (
+            provider_id not in self.providers
+            or self.providers[provider_id].auth_strategy == None
+        ):
+            return na_message  # No emoji
 
-        if (provider_id not in self.providers or
-            self.providers[provider_id].auth_strategy == None):
-            return na_message # No emoji
-        
         try:
             env_var = self.providers[provider_id].auth_strategy.name
-        except AttributeError: # No "name" attribute
+        except AttributeError:  # No "name" attribute
             return na_message
-        
+
         output = f"`{env_var}` | "
-        if (os.getenv(env_var) == None):
-            output += ("<abbr title=\"You have not set this environment variable, "
-            + "so you cannot use this provider's models.\">❌</abbr>"); 
+        if os.getenv(env_var) == None:
+            output += (
+                '<abbr title="You have not set this environment variable, '
+                + "so you cannot use this provider's models.\">❌</abbr>"
+            )
         else:
-            output += ("<abbr title=\"You have set this environment variable, "
-            + "so you can use this provider's models.\">✅</abbr>");
-        
+            output += (
+                '<abbr title="You have set this environment variable, '
+                + "so you can use this provider's models.\">✅</abbr>"
+            )
+
         return output
 
     def _ai_env_status_for_provider_text(self, provider_id):
-        if (provider_id not in self.providers or
-            self.providers[provider_id].auth_strategy == None):
-            return '' # No message necessary
-        
-        try:        
+        if (
+            provider_id not in self.providers
+            or self.providers[provider_id].auth_strategy == None
+        ):
+            return ""  # No message necessary
+
+        try:
             env_var = self.providers[provider_id].auth_strategy.name
-        except AttributeError: # No "name" attribute
-            return ''
-        
+        except AttributeError:  # No "name" attribute
+            return ""
+
         output = f"Requires environment variable {env_var} "
-        if (os.getenv(env_var) != None):
+        if os.getenv(env_var) != None:
             output += "(set)"
         else:
             output += "(not set)"
-        
+
         return output + "\n"
 
     # Is this a name of a Python variable that can be called as a LangChain chain?
     def _is_langchain_chain(self, name):
         # Reserved word in Python?
-        if (keyword.iskeyword(name)):
-            return False;
-    
-        acceptable_name = re.compile('^[a-zA-Z0-9_]+$')
-        if (not acceptable_name.match(name)):
-            return False;
-        
+        if keyword.iskeyword(name):
+            return False
+
+        acceptable_name = re.compile("^[a-zA-Z0-9_]+$")
+        if not acceptable_name.match(name):
+            return False
+
         ipython = get_ipython()
-        return(name in ipython.user_ns and isinstance(ipython.user_ns[name], LLMChain))
+        return name in ipython.user_ns and isinstance(ipython.user_ns[name], LLMChain)
 
     # Is this an acceptable name for an alias?
     def _validate_name(self, register_name):
         # A registry name contains ASCII letters, numbers, hyphens, underscores,
         # and periods. No other characters, including a colon, are permitted
-        acceptable_name = re.compile('^[a-zA-Z0-9._-]+$')
-        if (not acceptable_name.match(register_name)):
-            raise ValueError('A registry name may contain ASCII letters, numbers, hyphens, underscores, '
-                + 'and periods. No other characters, including a colon, are permitted')
+        acceptable_name = re.compile("^[a-zA-Z0-9._-]+$")
+        if not acceptable_name.match(register_name):
+            raise ValueError(
+                "A registry name may contain ASCII letters, numbers, hyphens, underscores, "
+                + "and periods. No other characters, including a colon, are permitted"
+            )
 
     # Initially set or update an alias to a target
     def _safely_set_target(self, register_name, target):
         # If target is a string, treat this as an alias to another model.
         if self._is_langchain_chain(target):
             ip = get_ipython()
             self.custom_model_registry[register_name] = ip.user_ns[target]
         else:
             # Ensure that the destination is properly formatted
-            if (':' not in target):
+            if ":" not in target:
                 raise ValueError(
-                    'Target model must be an LLMChain object or a model name in PROVIDER_ID:MODEL_NAME format')
+                    "Target model must be an LLMChain object or a model name in PROVIDER_ID:MODEL_NAME format"
+                )
 
             self.custom_model_registry[register_name] = target
 
     def handle_delete(self, args: DeleteArgs):
-        if (args.name in AI_COMMANDS):
-            raise ValueError(f"Reserved command names, including {args.name}, cannot be deleted")
-        
-        if (args.name not in self.custom_model_registry):
+        if args.name in AI_COMMANDS:
+            raise ValueError(
+                f"Reserved command names, including {args.name}, cannot be deleted"
+            )
+
+        if args.name not in self.custom_model_registry:
             raise ValueError(f"There is no alias called {args.name}")
-        
+
         del self.custom_model_registry[args.name]
         output = f"Deleted alias `{args.name}`"
         return TextOrMarkdown(output, output)
 
     def handle_register(self, args: RegisterArgs):
         # Existing command names are not allowed
-        if (args.name in AI_COMMANDS):
+        if args.name in AI_COMMANDS:
             raise ValueError(f"The name {args.name} is reserved for a command")
-        
+
         # Existing registered names are not allowed
-        if (args.name in self.custom_model_registry):
-            raise ValueError(f"The name {args.name} is already associated with a custom model; "
-                + 'use %ai update to change its target')
-        
+        if args.name in self.custom_model_registry:
+            raise ValueError(
+                f"The name {args.name} is already associated with a custom model; "
+                + "use %ai update to change its target"
+            )
+
         # Does the new name match expected format?
         self._validate_name(args.name)
 
         self._safely_set_target(args.name, args.target)
         output = f"Registered new alias `{args.name}`"
         return TextOrMarkdown(output, output)
 
     def handle_update(self, args: UpdateArgs):
-        if (args.name in AI_COMMANDS):
-            raise ValueError(f"Reserved command names, including {args.name}, cannot be updated")
-        
-        if (args.name not in self.custom_model_registry):
+        if args.name in AI_COMMANDS:
+            raise ValueError(
+                f"Reserved command names, including {args.name}, cannot be updated"
+            )
+
+        if args.name not in self.custom_model_registry:
             raise ValueError(f"There is no alias called {args.name}")
-        
+
         self._safely_set_target(args.name, args.target)
         output = f"Updated target of alias `{args.name}`"
         return TextOrMarkdown(output, output)
 
     def _ai_list_command_markdown(self, single_provider=None):
-        output = ("| Provider | Environment variable | Set? | Models |\n"
-            + "|----------|----------------------|------|--------|\n")
-        if (single_provider is not None and single_provider not in self.providers):
-            return f"There is no model provider with ID `{single_provider}`.";
+        output = (
+            "| Provider | Environment variable | Set? | Models |\n"
+            + "|----------|----------------------|------|--------|\n"
+        )
+        if single_provider is not None and single_provider not in self.providers:
+            return f"There is no model provider with ID `{single_provider}`."
 
         for provider_id, Provider in self.providers.items():
-            if (single_provider is not None and provider_id != single_provider):
-                continue;
+            if single_provider is not None and provider_id != single_provider:
+                continue
 
-            output += (f"| `{provider_id}` | "
-                + self._ai_env_status_for_provider_markdown(provider_id) + " | "
+            output += (
+                f"| `{provider_id}` | "
+                + self._ai_env_status_for_provider_markdown(provider_id)
+                + " | "
                 + self._ai_inline_list_models_for_provider(provider_id, Provider)
-                + " |\n")
+                + " |\n"
+            )
 
         # Also list aliases.
-        if (single_provider is None and len(self.custom_model_registry) > 0):
-            output += ("\nAliases and custom commands:\n\n"
+        if single_provider is None and len(self.custom_model_registry) > 0:
+            output += (
+                "\nAliases and custom commands:\n\n"
                 + "| Name | Target |\n"
-                + "|------|--------|\n")
+                + "|------|--------|\n"
+            )
             for key, value in self.custom_model_registry.items():
                 output += f"| `{key}` | "
                 if isinstance(value, str):
                     output += f"`{value}`"
                 else:
                     output += "*custom chain*"
-                
+
                 output += " |\n"
 
         return output
 
     def _ai_list_command_text(self, single_provider=None):
         output = ""
-        if (single_provider is not None and single_provider not in self.providers):
-            return f"There is no model provider with ID '{single_provider}'.";
+        if single_provider is not None and single_provider not in self.providers:
+            return f"There is no model provider with ID '{single_provider}'."
 
         for provider_id, Provider in self.providers.items():
-            if (single_provider is not None and provider_id != single_provider):
-                continue;
+            if single_provider is not None and provider_id != single_provider:
+                continue
 
-            output += (f"{provider_id}\n"
-                + self._ai_env_status_for_provider_text(provider_id) # includes \n if nonblank
-                + self._ai_bulleted_list_models_for_provider(provider_id, Provider))
+            output += (
+                f"{provider_id}\n"
+                + self._ai_env_status_for_provider_text(
+                    provider_id
+                )  # includes \n if nonblank
+                + self._ai_bulleted_list_models_for_provider(provider_id, Provider)
+            )
 
         # Also list aliases.
-        if (single_provider is None and len(self.custom_model_registry) > 0):
+        if single_provider is None and len(self.custom_model_registry) > 0:
             output += "\nAliases and custom commands:\n"
             for key, value in self.custom_model_registry.items():
                 output += f"{key} - "
                 if isinstance(value, str):
                     output += value
                 else:
                     output += "custom chain"
-                
+
                 output += "\n"
 
         return output
 
     def handle_error(self, args: ErrorArgs):
         no_errors = "There have been no errors since the kernel started."
 
         # Find the most recent error.
         ip = get_ipython()
-        if ('Err' not in ip.user_ns):
+        if "Err" not in ip.user_ns:
             return TextOrMarkdown(no_errors, no_errors)
 
-        err = ip.user_ns['Err']
+        err = ip.user_ns["Err"]
         # Start from the previous execution count
         excount = ip.execution_count - 1
         last_error = None
-        while (excount >= 0 and last_error is None):
-            if(excount in err):
+        while excount >= 0 and last_error is None:
+            if excount in err:
                 last_error = err[excount]
             else:
-                excount = excount - 1;
+                excount = excount - 1
 
-        if (last_error is None):
+        if last_error is None:
             return TextOrMarkdown(no_errors, no_errors)
 
         prompt = f"Explain the following error:\n\n{last_error}"
         # Set CellArgs based on ErrorArgs
         cell_args = CellArgs(
-            type="root",
-            model_id=args.model_id,
-            format=args.format,
-            reset=False)
+            type="root", model_id=args.model_id, format=args.format, reset=False
+        )
         return self.run_ai_cell(cell_args, prompt)
 
     def _append_exchange_openai(self, prompt: str, output: str):
         """Appends a conversational exchange between user and an OpenAI Chat
         model to a transcript that will be included in future exchanges."""
-        self.transcript_openai.append({
-            "role": "user",
-            "content": prompt
-        })
-        self.transcript_openai.append({
-            "role": "assistant",
-            "content": output
-        })
+        self.transcript_openai.append({"role": "user", "content": prompt})
+        self.transcript_openai.append({"role": "assistant", "content": output})
 
     def _decompose_model_id(self, model_id: str):
         """Breaks down a model ID into a two-tuple (provider_id, local_model_id). Returns (None, None) if indeterminate."""
         if model_id in self.custom_model_registry:
             model_id = self.custom_model_registry[model_id]
 
         return decompose_model_id(model_id, self.providers)
 
     def _get_provider(self, provider_id: Optional[str]) -> BaseProvider:
         """Returns the model provider ID and class for a model ID. Returns None if indeterminate."""
         if provider_id is None or provider_id not in self.providers:
             return None
 
         return self.providers[provider_id]
-    
+
     def display_output(self, output, display_format, md):
         # build output display
         DisplayClass = DISPLAYS_BY_FORMAT[display_format]
 
         # if the user wants code, add another cell with the output.
-        if display_format == 'code':
+        if display_format == "code":
             # Strip a leading language indicator and trailing triple-backticks
-            lang_indicator = r'^```[a-zA-Z0-9]*\n'
-            output = re.sub(lang_indicator, '', output)
-            output = re.sub(r'\n```$', '', output)
+            lang_indicator = r"^```[a-zA-Z0-9]*\n"
+            output = re.sub(lang_indicator, "", output)
+            output = re.sub(r"\n```$", "", output)
             new_cell_payload = dict(
-                source='set_next_input',
+                source="set_next_input",
                 text=output,
                 replace=False,
             )
             ip = get_ipython()
             ip.payload_manager.write_payload(new_cell_payload)
-            return HTML('AI generated code inserted below &#11015;&#65039;', metadata=md);
+            return HTML(
+                "AI generated code inserted below &#11015;&#65039;", metadata=md
+            )
 
         if DisplayClass is None:
             return output
-        if display_format == 'json':
+        if display_format == "json":
             # JSON display expects a dict, not a JSON string
             output = json.loads(output)
         output_display = DisplayClass(output, metadata=md)
 
         # finally, display output display
         return output_display
 
@@ -422,79 +451,78 @@
         # The line parser's help function prints both cell and line help
         with click.Context(line_magic_parser, info_name="%ai") as ctx:
             click.echo(line_magic_parser.get_help(ctx))
 
     def handle_list(self, args: ListArgs):
         return TextOrMarkdown(
             self._ai_list_command_text(args.provider_id),
-            self._ai_list_command_markdown(args.provider_id)
+            self._ai_list_command_markdown(args.provider_id),
         )
 
     def run_ai_cell(self, args: CellArgs, prompt: str):
         # Apply a prompt template.
-        prompt = PROMPT_TEMPLATES_BY_FORMAT[args.format].format(prompt = prompt)
+        prompt = PROMPT_TEMPLATES_BY_FORMAT[args.format].format(prompt=prompt)
 
         # interpolate user namespace into prompt
         ip = get_ipython()
         prompt = prompt.format_map(FormatDict(ip.user_ns))
 
         # Determine provider and local model IDs
         # If this is a custom chain, send the message to the custom chain.
-        if (args.model_id in self.custom_model_registry and
-            isinstance(self.custom_model_registry[args.model_id], LLMChain)):
-            
+        if args.model_id in self.custom_model_registry and isinstance(
+            self.custom_model_registry[args.model_id], LLMChain
+        ):
             return self.display_output(
                 self.custom_model_registry[args.model_id].run(prompt),
                 args.format,
-                {
-                    "jupyter_ai": {
-                        "custom_chain_id": args.model_id
-                    }
-                })
+                {"jupyter_ai": {"custom_chain_id": args.model_id}},
+            )
 
         provider_id, local_model_id = self._decompose_model_id(args.model_id)
         Provider = self._get_provider(provider_id)
         if Provider is None:
             return TextOrMarkdown(
-                CANNOT_DETERMINE_MODEL_TEXT.format(args.model_id) + "\n\n"
+                CANNOT_DETERMINE_MODEL_TEXT.format(args.model_id)
+                + "\n\n"
                 + "If you were trying to run a command, run '%ai help' to see a list of commands.",
-                CANNOT_DETERMINE_MODEL_MARKDOWN.format(args.model_id) + "\n\n"
-                + "If you were trying to run a command, run `%ai help` to see a list of commands."
+                CANNOT_DETERMINE_MODEL_MARKDOWN.format(args.model_id)
+                + "\n\n"
+                + "If you were trying to run a command, run `%ai help` to see a list of commands.",
             )
 
         # if `--reset` is specified, reset transcript and return early
-        if (provider_id == "openai-chat" and args.reset):
+        if provider_id == "openai-chat" and args.reset:
             self.transcript_openai = []
             return
 
         # validate presence of authn credentials
         auth_strategy = self.providers[provider_id].auth_strategy
         if auth_strategy:
             # TODO: handle auth strategies besides EnvAuthStrategy
             if auth_strategy.type == "env" and auth_strategy.name not in os.environ:
-                raise EnvironmentError(
+                raise OSError(
                     f"Authentication environment variable {auth_strategy.name} not provided.\n"
                     f"An authentication token is required to use models from the {Provider.name} provider.\n"
                     f"Please specify it via `%env {auth_strategy.name}=token`. "
                 ) from None
 
         # configure and instantiate provider
-        provider_params = { "model_id": local_model_id }
+        provider_params = {"model_id": local_model_id}
         if provider_id == "openai-chat":
             provider_params["prefix_messages"] = self.transcript_openai
         # for SageMaker, validate that required params are specified
         if provider_id == "sagemaker-endpoint":
             if (
-                args.region_name is None or
-                args.request_schema is None or
-                args.response_path is None
+                args.region_name is None
+                or args.request_schema is None
+                or args.response_path is None
             ):
                 raise ValueError(
-                    "When using the sagemaker-endpoint provider, you must specify all of " +
-                    "the --region-name, --request-schema, and --response-path options."
+                    "When using the sagemaker-endpoint provider, you must specify all of "
+                    + "the --region-name, --request-schema, and --response-path options."
                 )
             provider_params["region_name"] = args.region_name
             provider_params["request_schema"] = args.request_schema
             provider_params["response_path"] = args.response_path
 
         provider = Provider(**provider_params)
 
@@ -502,26 +530,21 @@
         result = provider.generate([prompt])
         output = result.generations[0][0].text
 
         # if openai-chat, append exchange to transcript
         if provider_id == "openai-chat":
             self._append_exchange_openai(prompt, output)
 
-        md = {
-            "jupyter_ai": {
-                "provider_id": provider_id,
-                "model_id": local_model_id
-            }
-        }
+        md = {"jupyter_ai": {"provider_id": provider_id, "model_id": local_model_id}}
 
         return self.display_output(output, args.format, md)
 
     @line_cell_magic
     def ai(self, line, cell=None):
-        raw_args = line.split(' ')
+        raw_args = line.split(" ")
         if cell:
             args = cell_magic_parser(raw_args, prog_name="%%ai", standalone_mode=False)
         else:
             args = line_magic_parser(raw_args, prog_name="%ai", standalone_mode=False)
 
         if args == 0:
             # this happens when `--help` is called on the root command, in which
@@ -550,16 +573,16 @@
         args: CellArgs = args
 
         if not cell:
             raise CellMagicError(
                 """[0.8+]: To invoke a language model, you must use the `%%ai`
                 cell magic. The `%ai` line magic is only for use with
                 subcommands."""
-            ) 
+            )
 
         prompt = cell.strip()
-        
+
         # interpolate user namespace into prompt
         ip = get_ipython()
         prompt = prompt.format_map(FormatDict(ip.user_ns))
 
         return self.run_ai_cell(args, prompt)
```

### Comparing `jupyter_ai_magics-0.8.0/jupyter_ai_magics/parsers.py` & `jupyter_ai_magics-0.9.0/jupyter_ai_magics/parsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,162 +1,227 @@
+from typing import Literal, Optional, get_args
+
 import click
 from pydantic import BaseModel
-from typing import Optional, Literal, get_args
 
-FORMAT_CHOICES_TYPE = Literal["code", "html", "image", "json", "markdown", "math", "md", "text"]
+FORMAT_CHOICES_TYPE = Literal[
+    "code", "html", "image", "json", "markdown", "math", "md", "text"
+]
 FORMAT_CHOICES = list(get_args(FORMAT_CHOICES_TYPE))
 FORMAT_HELP = """IPython display to use when rendering output. [default="markdown"]"""
 
-REGION_NAME_SHORT_OPTION = '-n'
-REGION_NAME_LONG_OPTION = '--region-name'
-REGION_NAME_HELP = ("AWS region name, e.g. 'us-east-1'. Required for SageMaker provider; " +
-    "does nothing with other providers.")
-
-REQUEST_SCHEMA_SHORT_OPTION = '-q'
-REQUEST_SCHEMA_LONG_OPTION = '--request-schema'
-REQUEST_SCHEMA_HELP = ("The JSON object the endpoint expects, with the prompt being " +
-    "substituted into any value that matches the string literal '<prompt>'. " +
-    "Required for SageMaker provider; does nothing with other providers.")
-
-RESPONSE_PATH_SHORT_OPTION = '-p'
-RESPONSE_PATH_LONG_OPTION = '--response-path'
-RESPONSE_PATH_HELP = ("A JSONPath string that retrieves the language model's output " +
-    "from the endpoint's JSON response. Required for SageMaker provider; " +
-    "does nothing with other providers.")
+REGION_NAME_SHORT_OPTION = "-n"
+REGION_NAME_LONG_OPTION = "--region-name"
+REGION_NAME_HELP = (
+    "AWS region name, e.g. 'us-east-1'. Required for SageMaker provider; "
+    + "does nothing with other providers."
+)
+
+REQUEST_SCHEMA_SHORT_OPTION = "-q"
+REQUEST_SCHEMA_LONG_OPTION = "--request-schema"
+REQUEST_SCHEMA_HELP = (
+    "The JSON object the endpoint expects, with the prompt being "
+    + "substituted into any value that matches the string literal '<prompt>'. "
+    + "Required for SageMaker provider; does nothing with other providers."
+)
+
+RESPONSE_PATH_SHORT_OPTION = "-p"
+RESPONSE_PATH_LONG_OPTION = "--response-path"
+RESPONSE_PATH_HELP = (
+    "A JSONPath string that retrieves the language model's output "
+    + "from the endpoint's JSON response. Required for SageMaker provider; "
+    + "does nothing with other providers."
+)
+
 
 class CellArgs(BaseModel):
     type: Literal["root"] = "root"
     model_id: str
     format: FORMAT_CHOICES_TYPE
     reset: bool
     # The following parameters are required only for SageMaker models
     region_name: Optional[str]
     request_schema: Optional[str]
     response_path: Optional[str]
 
+
 # Should match CellArgs, but without "reset"
 class ErrorArgs(BaseModel):
     type: Literal["error"] = "error"
     model_id: str
     format: FORMAT_CHOICES_TYPE
     # The following parameters are required only for SageMaker models
     region_name: Optional[str]
     request_schema: Optional[str]
     response_path: Optional[str]
 
+
 class HelpArgs(BaseModel):
     type: Literal["help"] = "help"
 
+
 class ListArgs(BaseModel):
     type: Literal["list"] = "list"
     provider_id: Optional[str]
 
+
 class RegisterArgs(BaseModel):
     type: Literal["register"] = "register"
     name: str
     target: str
 
+
 class DeleteArgs(BaseModel):
     type: Literal["delete"] = "delete"
     name: str
 
+
 class UpdateArgs(BaseModel):
     type: Literal["update"] = "update"
     name: str
     target: str
 
+
 class LineMagicGroup(click.Group):
     """Helper class to print the help string for cell magics as well when
     `%ai --help` is called."""
+
     def get_help(self, ctx):
         with click.Context(cell_magic_parser, info_name="%%ai") as ctx:
             click.echo(cell_magic_parser.get_help(ctx))
-        click.echo('-' * 78)
+        click.echo("-" * 78)
         with click.Context(line_magic_parser, info_name="%ai") as ctx:
             click.echo(super().get_help(ctx))
 
+
 @click.command()
-@click.argument('model_id')
-@click.option('-f', '--format',
+@click.argument("model_id")
+@click.option(
+    "-f",
+    "--format",
     type=click.Choice(FORMAT_CHOICES, case_sensitive=False),
     default="markdown",
-    help=FORMAT_HELP
+    help=FORMAT_HELP,
 )
-@click.option('-r', '--reset', is_flag=True,
+@click.option(
+    "-r",
+    "--reset",
+    is_flag=True,
     help="""Clears the conversation transcript used when interacting with an
-    OpenAI chat model provider. Does nothing with other providers."""
+    OpenAI chat model provider. Does nothing with other providers.""",
+)
+@click.option(
+    REGION_NAME_SHORT_OPTION,
+    REGION_NAME_LONG_OPTION,
+    required=False,
+    help=REGION_NAME_HELP,
+)
+@click.option(
+    REQUEST_SCHEMA_SHORT_OPTION,
+    REQUEST_SCHEMA_LONG_OPTION,
+    required=False,
+    help=REQUEST_SCHEMA_HELP,
+)
+@click.option(
+    RESPONSE_PATH_SHORT_OPTION,
+    RESPONSE_PATH_LONG_OPTION,
+    required=False,
+    help=RESPONSE_PATH_HELP,
 )
-@click.option(REGION_NAME_SHORT_OPTION, REGION_NAME_LONG_OPTION, required=False, help=REGION_NAME_HELP)
-@click.option(REQUEST_SCHEMA_SHORT_OPTION, REQUEST_SCHEMA_LONG_OPTION, required=False, help=REQUEST_SCHEMA_HELP)
-@click.option(RESPONSE_PATH_SHORT_OPTION, RESPONSE_PATH_LONG_OPTION, required=False, help=RESPONSE_PATH_HELP)
 def cell_magic_parser(**kwargs):
     """
     Invokes a language model identified by MODEL_ID, with the prompt being
     contained in all lines after the first. Both local model IDs and global
     model IDs (with the provider ID explicitly prefixed, followed by a colon)
     are accepted.
 
     To view available language models, please run `%ai list`.
     """
     return CellArgs(**kwargs)
 
+
 @click.group(cls=LineMagicGroup)
 def line_magic_parser():
     """
     Invokes a subcommand.
     """
 
-@line_magic_parser.command(name='error')
-@click.argument('model_id')
-@click.option('-f', '--format',
+
+@line_magic_parser.command(name="error")
+@click.argument("model_id")
+@click.option(
+    "-f",
+    "--format",
     type=click.Choice(FORMAT_CHOICES, case_sensitive=False),
     default="markdown",
-    help=FORMAT_HELP
+    help=FORMAT_HELP,
+)
+@click.option(
+    REGION_NAME_SHORT_OPTION,
+    REGION_NAME_LONG_OPTION,
+    required=False,
+    help=REGION_NAME_HELP,
+)
+@click.option(
+    REQUEST_SCHEMA_SHORT_OPTION,
+    REQUEST_SCHEMA_LONG_OPTION,
+    required=False,
+    help=REQUEST_SCHEMA_HELP,
+)
+@click.option(
+    RESPONSE_PATH_SHORT_OPTION,
+    RESPONSE_PATH_LONG_OPTION,
+    required=False,
+    help=RESPONSE_PATH_HELP,
 )
-@click.option(REGION_NAME_SHORT_OPTION, REGION_NAME_LONG_OPTION, required=False, help=REGION_NAME_HELP)
-@click.option(REQUEST_SCHEMA_SHORT_OPTION, REQUEST_SCHEMA_LONG_OPTION, required=False, help=REQUEST_SCHEMA_HELP)
-@click.option(RESPONSE_PATH_SHORT_OPTION, RESPONSE_PATH_LONG_OPTION, required=False, help=RESPONSE_PATH_HELP)
 def error_subparser(**kwargs):
     """
     Explains the most recent error. Takes the same options (except -r) as
     the basic `%%ai` command.
     """
     return ErrorArgs(**kwargs)
 
-@line_magic_parser.command(name='help')
+
+@line_magic_parser.command(name="help")
 def help_subparser():
     """Show this message and exit."""
     return HelpArgs()
 
-@line_magic_parser.command(name='list',
-    short_help="List language models. See `%ai list --help` for options."
+
+@line_magic_parser.command(
+    name="list", short_help="List language models. See `%ai list --help` for options."
 )
-@click.argument('provider_id', required=False)
+@click.argument("provider_id", required=False)
 def list_subparser(**kwargs):
     """List language models, optionally scoped to PROVIDER_ID."""
     return ListArgs(**kwargs)
 
-@line_magic_parser.command(name='register',
-    short_help="Register a new alias. See `%ai register --help` for options."
+
+@line_magic_parser.command(
+    name="register",
+    short_help="Register a new alias. See `%ai register --help` for options.",
 )
-@click.argument('name')
-@click.argument('target')
+@click.argument("name")
+@click.argument("target")
 def register_subparser(**kwargs):
     """Register a new alias called NAME for the model or chain named TARGET."""
     return RegisterArgs(**kwargs)
 
-@line_magic_parser.command(name='delete',
-    short_help="Delete an alias. See `%ai delete --help` for options."
+
+@line_magic_parser.command(
+    name="delete", short_help="Delete an alias. See `%ai delete --help` for options."
 )
-@click.argument('name')
+@click.argument("name")
 def register_subparser(**kwargs):
     """Delete an alias called NAME."""
     return DeleteArgs(**kwargs)
 
-@line_magic_parser.command(name='update',
-    short_help="Update the target of an alias. See `%ai update --help` for options."
+
+@line_magic_parser.command(
+    name="update",
+    short_help="Update the target of an alias. See `%ai update --help` for options.",
 )
-@click.argument('name')
-@click.argument('target')
+@click.argument("name")
+@click.argument("target")
 def register_subparser(**kwargs):
     """Update an alias called NAME to refer to the model or chain named TARGET."""
     return UpdateArgs(**kwargs)
```

### Comparing `jupyter_ai_magics-0.8.0/jupyter_ai_magics/providers.py` & `jupyter_ai_magics-0.9.0/jupyter_ai_magics/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,68 +1,75 @@
-from typing import Any, ClassVar, Dict, List, Union, Literal, Optional
 import base64
+import copy
 import io
 import json
-import copy
+from typing import Any, ClassVar, Dict, List, Literal, Optional, Union
 
 from jsonpath_ng import jsonpath, parse
-from langchain.schema import BaseModel as BaseLangchainProvider
+from langchain.chat_models import ChatOpenAI
 from langchain.llms import (
     AI21,
     Anthropic,
     Cohere,
     HuggingFaceHub,
     OpenAI,
     OpenAIChat,
-    SagemakerEndpoint
+    SagemakerEndpoint,
 )
 from langchain.llms.sagemaker_endpoint import LLMContentHandler
-from langchain.utils import get_from_dict_or_env
 from langchain.llms.utils import enforce_stop_tokens
-
+from langchain.schema import BaseModel as BaseLangchainProvider
+from langchain.utils import get_from_dict_or_env
 from pydantic import BaseModel, Extra, root_validator
-from langchain.chat_models import ChatOpenAI
+
 
 class EnvAuthStrategy(BaseModel):
     """Require one auth token via an environment variable."""
+
     type: Literal["env"] = "env"
     name: str
 
 
 class MultiEnvAuthStrategy(BaseModel):
     """Require multiple auth tokens via multiple environment variables."""
+
     type: Literal["file"] = "file"
     names: List[str]
 
 
 class AwsAuthStrategy(BaseModel):
     """Require AWS authentication via Boto3"""
+
     type: Literal["aws"] = "aws"
 
 
 AuthStrategy = Optional[
     Union[
         EnvAuthStrategy,
         MultiEnvAuthStrategy,
         AwsAuthStrategy,
     ]
 ]
 
+
 class TextField(BaseModel):
     type: Literal["text"] = "text"
     key: str
     label: str
 
+
 class MultilineTextField(BaseModel):
     type: Literal["text-multiline"] = "text-multiline"
     key: str
     label: str
 
+
 Field = Union[TextField, MultilineTextField]
 
+
 class BaseProvider(BaseLangchainProvider):
     #
     # pydantic config
     #
     class Config:
         extra = Extra.allow
 
@@ -89,34 +96,36 @@
     """Authentication/authorization strategy. Declares what credentials are
     required to use this model provider. Generally should not be `None`."""
 
     registry: ClassVar[bool] = False
     """Whether this provider is a registry provider."""
 
     fields: ClassVar[List[Field]] = []
-    """User inputs expected by this provider when initializing it. Each `Field` `f` 
+    """User inputs expected by this provider when initializing it. Each `Field` `f`
     should be passed in the constructor as a keyword argument, keyed by `f.key`."""
 
     #
     # instance attrs
     #
     model_id: str
 
     def __init__(self, *args, **kwargs):
         try:
             assert kwargs["model_id"]
         except:
-            raise AssertionError("model_id was not specified. Please specify it as a keyword argument.")
+            raise AssertionError(
+                "model_id was not specified. Please specify it as a keyword argument."
+            )
 
         model_kwargs = {}
         model_kwargs[self.__class__.model_id_key] = kwargs["model_id"]
 
         super().__init__(*args, **kwargs, **model_kwargs)
 
-    
+
 class AI21Provider(BaseProvider, AI21):
     id = "ai21"
     name = "AI21"
     models = [
         "j1-large",
         "j1-grande",
         "j1-jumbo",
@@ -127,37 +136,45 @@
         "j2-grande-instruct",
         "j2-jumbo-instruct",
     ]
     model_id_key = "model"
     pypi_package_deps = ["ai21"]
     auth_strategy = EnvAuthStrategy(name="AI21_API_KEY")
 
+
 class AnthropicProvider(BaseProvider, Anthropic):
     id = "anthropic"
     name = "Anthropic"
     models = [
         "claude-v1",
         "claude-v1.0",
         "claude-v1.2",
         "claude-instant-v1",
         "claude-instant-v1.0",
     ]
     model_id_key = "model"
     pypi_package_deps = ["anthropic"]
     auth_strategy = EnvAuthStrategy(name="ANTHROPIC_API_KEY")
 
+
 class CohereProvider(BaseProvider, Cohere):
     id = "cohere"
     name = "Cohere"
     models = ["medium", "xlarge"]
     model_id_key = "model"
     pypi_package_deps = ["cohere"]
     auth_strategy = EnvAuthStrategy(name="COHERE_API_KEY")
 
-HUGGINGFACE_HUB_VALID_TASKS = ("text2text-generation", "text-generation", "text-to-image")
+
+HUGGINGFACE_HUB_VALID_TASKS = (
+    "text2text-generation",
+    "text-generation",
+    "text-to-image",
+)
+
 
 class HfHubProvider(BaseProvider, HuggingFaceHub):
     id = "huggingface_hub"
     name = "HuggingFace Hub"
     models = ["*"]
     model_id_key = "repo_id"
     # ipywidgets needed to suppress tqdm warning
@@ -191,15 +208,15 @@
             values["client"] = client
         except ImportError:
             raise ValueError(
                 "Could not import huggingface_hub python package. "
                 "Please install it with `pip install huggingface_hub`."
             )
         return values
-    
+
     # Handle image outputs
     def _call(self, prompt: str, stop: Optional[List[str]] = None) -> str:
         """Call out to HuggingFace Hub's inference endpoint.
 
         Args:
             prompt: The prompt to pass into the model.
             stop: Optional list of stop words to use when generating.
@@ -216,29 +233,29 @@
         response = self.client(inputs=prompt, params=_model_kwargs)
 
         if type(response) is dict and "error" in response:
             raise ValueError(f"Error raised by inference API: {response['error']}")
 
         # Custom code for responding to image generation responses
         if self.client.task == "text-to-image":
-            imageFormat = response.format # Presume it's a PIL ImageFile
-            mimeType = ''
-            if (imageFormat == 'JPEG'):
-                mimeType = 'image/jpeg'
-            elif (imageFormat == 'PNG'):
-                mimeType = 'image/png'
-            elif (imageFormat == 'GIF'):
-                mimeType = 'image/gif'
+            imageFormat = response.format  # Presume it's a PIL ImageFile
+            mimeType = ""
+            if imageFormat == "JPEG":
+                mimeType = "image/jpeg"
+            elif imageFormat == "PNG":
+                mimeType = "image/png"
+            elif imageFormat == "GIF":
+                mimeType = "image/gif"
             else:
                 raise ValueError(f"Unrecognized image format {imageFormat}")
-            
+
             buffer = io.BytesIO()
             response.save(buffer, format=imageFormat)
             # Encode image data to Base64 bytes, then decode bytes to str
-            return (mimeType + ';base64,' + base64.b64encode(buffer.getvalue()).decode())
+            return mimeType + ";base64," + base64.b64encode(buffer.getvalue()).decode()
 
         if self.client.task == "text-generation":
             # Text generation return includes the starter text.
             text = response[0]["generated_text"][len(prompt) :]
         elif self.client.task == "text2text-generation":
             text = response[0]["generated_text"]
         else:
@@ -248,14 +265,15 @@
             )
         if stop is not None:
             # This is a bit hacky, but I can't figure out a better way to enforce
             # stop tokens when making calls to huggingface_hub.
             text = enforce_stop_tokens(text, stop)
         return text
 
+
 class OpenAIProvider(BaseProvider, OpenAI):
     id = "openai"
     name = "OpenAI"
     models = [
         "text-davinci-003",
         "text-davinci-002",
         "text-curie-001",
@@ -266,14 +284,15 @@
         "babbage",
         "ada",
     ]
     model_id_key = "model_name"
     pypi_package_deps = ["openai"]
     auth_strategy = EnvAuthStrategy(name="OPENAI_API_KEY")
 
+
 class ChatOpenAIProvider(BaseProvider, OpenAIChat):
     id = "openai-chat"
     name = "OpenAI"
     models = [
         "gpt-4",
         "gpt-4-0314",
         "gpt-4-32k",
@@ -284,22 +303,17 @@
     model_id_key = "model_name"
     pypi_package_deps = ["openai"]
     auth_strategy = EnvAuthStrategy(name="OPENAI_API_KEY")
 
     def append_exchange(self, prompt: str, output: str):
         """Appends a conversational exchange between user and an OpenAI Chat
         model to a transcript that will be included in future exchanges."""
-        self.prefix_messages.append({
-            "role": "user",
-            "content": prompt
-        })
-        self.prefix_messages.append({
-            "role": "assistant",
-            "content": output
-        })
+        self.prefix_messages.append({"role": "user", "content": prompt})
+        self.prefix_messages.append({"role": "assistant", "content": output})
+
 
 # uses the new OpenAIChat provider. temporarily living as a separate class until
 # conflicts can be resolved
 class ChatOpenAINewProvider(BaseProvider, ChatOpenAI):
     id = "openai-chat-new"
     name = "OpenAI"
     models = [
@@ -310,14 +324,15 @@
         "gpt-3.5-turbo",
         "gpt-3.5-turbo-0301",
     ]
     model_id_key = "model_name"
     pypi_package_deps = ["openai"]
     auth_strategy = EnvAuthStrategy(name="OPENAI_API_KEY")
 
+
 class JsonContentHandler(LLMContentHandler):
     content_type = "application/json"
     accepts = "application/json"
 
     def __init__(self, request_schema, response_path):
         self.request_schema = json.loads(request_schema)
         self.response_path = response_path
@@ -326,28 +341,29 @@
     def replace_values(self, old_val, new_val, d: Dict[str, Any]):
         """Replaces values of a dictionary recursively."""
         for key, val in d.items():
             if val == old_val:
                 d[key] = new_val
             if isinstance(val, dict):
                 self.replace_values(old_val, new_val, val)
-        
+
         return d
 
     def transform_input(self, prompt: str, model_kwargs: Dict) -> bytes:
         request_obj = copy.deepcopy(self.request_schema)
         self.replace_values("<prompt>", prompt, request_obj)
-        request = json.dumps(request_obj).encode('utf-8')
+        request = json.dumps(request_obj).encode("utf-8")
         return request
-    
+
     def transform_output(self, output: bytes) -> str:
         response_json = json.loads(output.read().decode("utf-8"))
         matches = self.response_parser.find(response_json)
         return matches[0].value
 
+
 class SmEndpointProvider(BaseProvider, SagemakerEndpoint):
     id = "sagemaker-endpoint"
     name = "Sagemaker Endpoint"
     models = ["*"]
     model_id_key = "endpoint_name"
     pypi_package_deps = ["boto3"]
     auth_strategy = AwsAuthStrategy()
@@ -360,16 +376,17 @@
         MultilineTextField(
             key="request_schema",
             label="Request schema",
         ),
         TextField(
             key="response_path",
             label="Response path",
-        )
+        ),
     ]
-    
+
     def __init__(self, *args, **kwargs):
-        request_schema = kwargs.pop('request_schema')
-        response_path = kwargs.pop('response_path')
-        content_handler = JsonContentHandler(request_schema=request_schema, response_path=response_path)
+        request_schema = kwargs.pop("request_schema")
+        response_path = kwargs.pop("response_path")
+        content_handler = JsonContentHandler(
+            request_schema=request_schema, response_path=response_path
+        )
         super().__init__(*args, **kwargs, content_handler=content_handler)
-
```

### Comparing `jupyter_ai_magics-0.8.0/jupyter_ai_magics/utils.py` & `jupyter_ai_magics-0.9.0/jupyter_ai_magics/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import logging
 from typing import Dict, Optional, Tuple, Union
+
 from importlib_metadata import entry_points
 from jupyter_ai_magics.aliases import MODEL_ID_ALIASES
-
 from jupyter_ai_magics.embedding_providers import BaseEmbeddingsProvider
-
 from jupyter_ai_magics.providers import BaseProvider
 
-
 Logger = Union[logging.Logger, logging.LoggerAdapter]
 
 
 def load_providers(log: Optional[Logger] = None) -> Dict[str, BaseProvider]:
     if not log:
         log = logging.getLogger()
         log.addHandler(logging.NullHandler())
@@ -19,52 +17,61 @@
     providers = {}
     eps = entry_points()
     model_provider_eps = eps.select(group="jupyter_ai.model_providers")
     for model_provider_ep in model_provider_eps:
         try:
             provider = model_provider_ep.load()
         except:
-            log.error(f"Unable to load model provider class from entry point `{model_provider_ep.name}`.")
+            log.error(
+                f"Unable to load model provider class from entry point `{model_provider_ep.name}`."
+            )
             continue
         providers[provider.id] = provider
         log.info(f"Registered model provider `{provider.id}`.")
-    
+
     return providers
 
 
-def load_embedding_providers(log: Optional[Logger] = None) -> Dict[str, BaseEmbeddingsProvider]:
+def load_embedding_providers(
+    log: Optional[Logger] = None,
+) -> Dict[str, BaseEmbeddingsProvider]:
     if not log:
         log = logging.getLogger()
         log.addHandler(logging.NullHandler())
     providers = {}
     eps = entry_points()
     model_provider_eps = eps.select(group="jupyter_ai.embeddings_model_providers")
     for model_provider_ep in model_provider_eps:
         try:
             provider = model_provider_ep.load()
         except:
-            log.error(f"Unable to load embeddings model provider class from entry point `{model_provider_ep.name}`.")
+            log.error(
+                f"Unable to load embeddings model provider class from entry point `{model_provider_ep.name}`."
+            )
             continue
         providers[provider.id] = provider
         log.info(f"Registered embeddings model provider `{provider.id}`.")
-    
+
     return providers
 
-def decompose_model_id(model_id: str, providers: Dict[str, BaseProvider]) -> Tuple[str, str]:
-        """Breaks down a model ID into a two-tuple (provider_id, local_model_id). Returns (None, None) if indeterminate."""
-        if model_id in MODEL_ID_ALIASES:
-            model_id = MODEL_ID_ALIASES[model_id]
-
-        if ":" not in model_id:
-            # case: model ID was not provided with a prefix indicating the provider
-            # ID. try to infer the provider ID before returning (None, None).
-
-            # naively search through the dictionary and return the first provider
-            # that provides a model of the same ID.
-            for provider_id, provider in providers.items():
-                if model_id in provider.models:
-                    return (provider_id, model_id)
-            
-            return (None, None)
 
-        provider_id, local_model_id = model_id.split(":", 1)
-        return (provider_id, local_model_id)
+def decompose_model_id(
+    model_id: str, providers: Dict[str, BaseProvider]
+) -> Tuple[str, str]:
+    """Breaks down a model ID into a two-tuple (provider_id, local_model_id). Returns (None, None) if indeterminate."""
+    if model_id in MODEL_ID_ALIASES:
+        model_id = MODEL_ID_ALIASES[model_id]
+
+    if ":" not in model_id:
+        # case: model ID was not provided with a prefix indicating the provider
+        # ID. try to infer the provider ID before returning (None, None).
+
+        # naively search through the dictionary and return the first provider
+        # that provides a model of the same ID.
+        for provider_id, provider in providers.items():
+            if model_id in provider.models:
+                return (provider_id, model_id)
+
+        return (None, None)
+
+    provider_id, local_model_id = model_id.split(":", 1)
+    return (provider_id, local_model_id)
```

### Comparing `jupyter_ai_magics-0.8.0/.gitignore` & `jupyter_ai_magics-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.8.0/LICENSE` & `jupyter_ai_magics-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.8.0/pyproject.toml` & `jupyter_ai_magics-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     "langchain==0.0.159",
     "typing_extensions==4.5.0",
     "click~=8.0",
     "jsonpath-ng~=1.5.3",
 ]
 
 [project.optional-dependencies]
+dev = [
+    "pre-commit~=3.3.3"
+]
+
 test = [
     "coverage",
     "pytest",
     "pytest-asyncio",
     "pytest-cov"
 ]
```

### Comparing `jupyter_ai_magics-0.8.0/PKG-INFO` & `jupyter_ai_magics-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_magics
-Version: 0.8.0
+Version: 0.9.0
 Summary: Jupyter AI magics Python package. Not published on NPM.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -57,14 +57,16 @@
 Requires-Dist: anthropic; extra == 'all'
 Requires-Dist: boto3; extra == 'all'
 Requires-Dist: cohere; extra == 'all'
 Requires-Dist: huggingface-hub; extra == 'all'
 Requires-Dist: ipywidgets; extra == 'all'
 Requires-Dist: openai; extra == 'all'
 Requires-Dist: pillow; extra == 'all'
+Provides-Extra: dev
+Requires-Dist: pre-commit~=3.3.3; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
```

