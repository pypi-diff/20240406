# Comparing `tmp/llm-quantkit-0.23.tar.gz` & `tmp/llm-quantkit-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-quantkit-0.23.tar", last modified: Tue Apr  2 20:50:34 2024, max compression
+gzip compressed data, was "llm-quantkit-0.24.tar", last modified: Sat Apr  6 06:53:26 2024, max compression
```

## Comparing `llm-quantkit-0.23.tar` & `llm-quantkit-0.24.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:34.992478 llm-quantkit-0.23/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 20:50:24.000000 llm-quantkit-0.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-02 20:50:34.992478 llm-quantkit-0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-02 20:50:24.000000 llm-quantkit-0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:34.992478 llm-quantkit-0.23/llm_quantkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-02 20:50:34.000000 llm-quantkit-0.23/llm_quantkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-02 20:50:34.000000 llm-quantkit-0.23/llm_quantkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:50:34.000000 llm-quantkit-0.23/llm_quantkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 20:50:34.000000 llm-quantkit-0.23/llm_quantkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-02 20:50:34.000000 llm-quantkit-0.23/llm_quantkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 20:50:34.000000 llm-quantkit-0.23/llm_quantkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-02 20:50:24.000000 llm-quantkit-0.23/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:34.992478 llm-quantkit-0.23/quantkit/
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-02 20:50:24.000000 llm-quantkit-0.23/quantkit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    61155 2024-04-02 20:50:24.000000 llm-quantkit-0.23/quantkit/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15932 2024-04-02 20:50:24.000000 llm-quantkit-0.23/quantkit/quantkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-02 20:50:24.000000 llm-quantkit-0.23/quantkit/safetensor.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:50:34.992478 llm-quantkit-0.23/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:53:26.845376 llm-quantkit-0.24/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-06 06:53:17.000000 llm-quantkit-0.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-06 06:53:26.845376 llm-quantkit-0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-06 06:53:17.000000 llm-quantkit-0.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:53:26.845376 llm-quantkit-0.24/llm_quantkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-06 06:53:26.000000 llm-quantkit-0.24/llm_quantkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 06:53:26.000000 llm-quantkit-0.24/llm_quantkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 06:53:26.000000 llm-quantkit-0.24/llm_quantkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-06 06:53:26.000000 llm-quantkit-0.24/llm_quantkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-06 06:53:26.000000 llm-quantkit-0.24/llm_quantkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 06:53:26.000000 llm-quantkit-0.24/llm_quantkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-06 06:53:17.000000 llm-quantkit-0.24/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:53:26.845376 llm-quantkit-0.24/quantkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-06 06:53:17.000000 llm-quantkit-0.24/quantkit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64290 2024-04-06 06:53:17.000000 llm-quantkit-0.24/quantkit/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15954 2024-04-06 06:53:17.000000 llm-quantkit-0.24/quantkit/quantkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-06 06:53:17.000000 llm-quantkit-0.24/quantkit/safetensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 06:53:26.845376 llm-quantkit-0.24/setup.cfg
```

### Comparing `llm-quantkit-0.23/LICENSE` & `llm-quantkit-0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-quantkit-0.23/PKG-INFO` & `llm-quantkit-0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-quantkit
-Version: 0.23
+Version: 0.24
 Summary: cli tool for downloading and quantizing LLMs
 Author-email: xhedit <jevd@protonmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/xhedit/quantkit
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `llm-quantkit-0.23/README.md` & `llm-quantkit-0.24/README.md`

 * *Files identical despite different names*

### Comparing `llm-quantkit-0.23/llm_quantkit.egg-info/PKG-INFO` & `llm-quantkit-0.24/llm_quantkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-quantkit
-Version: 0.23
+Version: 0.24
 Summary: cli tool for downloading and quantizing LLMs
 Author-email: xhedit <jevd@protonmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/xhedit/quantkit
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `llm-quantkit-0.23/pyproject.toml` & `llm-quantkit-0.24/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llm-quantkit"
 description = "cli tool for downloading and quantizing LLMs"
 readme = "README.md"
 license = { text = "MIT License" }
-version = "0.23"
+version = "0.24"
 authors = [{ name = "xhedit", email = "jevd@protonmail.com" }]
 dependencies = [
     "click",
     "torch>=2.0.0",
     "einops",
     "tqdm",
     "transformers",
```

### Comparing `llm-quantkit-0.23/quantkit/cli.py` & `llm-quantkit-0.24/quantkit/cli.py`

 * *Files identical despite different names*

### Comparing `llm-quantkit-0.23/quantkit/convert.py` & `llm-quantkit-0.24/quantkit/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 import mmap
 import os
 import pickle
 import re
 import signal
 import struct
 import sys
+import textwrap
 import time
 import zipfile
-from abc import ABCMeta, abstractmethod
+from abc import ABC, abstractmethod
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from dataclasses import dataclass
 from pathlib import Path
-from typing import IO, TYPE_CHECKING, Any, Callable, Iterable, Literal, TypeVar
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, IO, Iterable, Literal, Protocol, TypeVar, runtime_checkable
 
 import numpy as np
 from sentencepiece import SentencePieceProcessor
 
 if 'NO_LOCAL_GGUF' not in os.environ:
     sys.path.insert(1, str(Path(__file__).parent / 'gguf-py'))
 import gguf
@@ -39,14 +40,17 @@
 
 NDArray: TypeAlias = 'np.ndarray[Any, Any]'
 
 ARCH = gguf.MODEL_ARCH.LLAMA
 
 DEFAULT_CONCURRENCY = 8
 
+ADDED_TOKENS_FILE = 'added_tokens.json'
+FAST_TOKENIZER_FILE = 'tokenizer.json'
+
 #
 # data types
 #
 
 
 @dataclass(frozen=True)
 class DataType:
@@ -184,16 +188,18 @@
             n_layer = next(i for i in itertools.count() if f"model.layers.{i}.self_attn.q_proj.weight" not in model)
         elif "model.layers.0.self_attn.W_pack.weight" in model:   # next: try baichuan naming
             n_layer = next(i for i in itertools.count() if f"model.layers.{i}.self_attn.W_pack.weight" not in model)
         else:
             n_layer = next(i for i in itertools.count() if f"layers.{i}.attention.wq.weight" not in model)
 
         if n_layer < 1:
-            raise Exception("failed to guess 'n_layer'. This model is unknown or unsupported.\n"
-                            "Suggestion: provide 'config.json' of the model in the same directory containing model files.")
+            msg = """\
+                failed to guess 'n_layer'. This model is unknown or unsupported.
+                Suggestion: provide 'config.json' of the model in the same directory containing model files."""
+            raise KeyError(textwrap.dedent(msg))
 
         n_head = n_embd // 128 # guessed
         n_mult = 256           # guessed
 
         # TODO: verify this
         n_ff = int(2 * (4 * n_embd) / 3)
         n_ff = n_mult * ((n_ff + n_mult - 1) // n_mult)
@@ -207,15 +213,16 @@
             n_head     = n_head,
             n_head_kv  = n_head,
             f_norm_eps = 1e-5,
         )
 
     @staticmethod
     def loadHFTransformerJson(model: LazyModel, config_path: Path) -> Params:
-        config = json.load(open(config_path))
+        with open(config_path) as f:
+            config = json.load(f)
 
         rope_scaling_type = f_rope_scale = n_orig_ctx = rope_finetuned = None
         rope_scaling = config.get("rope_scaling")
 
         if rope_scaling is not None and (typ := rope_scaling.get("type")):
             rope_factor = rope_scaling.get("factor")
             f_rope_scale = rope_factor
@@ -229,16 +236,18 @@
                 raise NotImplementedError(f'Unknown rope scaling type: {typ}')
 
         if "max_sequence_length" in config:
             n_ctx = config["max_sequence_length"]
         elif "max_position_embeddings" in config:
             n_ctx = config["max_position_embeddings"]
         else:
-            raise Exception("failed to guess 'n_ctx'. This model is unknown or unsupported.\n"
-                            "Suggestion: provide 'config.json' of the model in the same directory containing model files.")
+            msg = """\
+                failed to guess 'n_ctx'. This model is unknown or unsupported.
+                Suggestion: provide 'config.json' of the model in the same directory containing model files."""
+            raise KeyError(textwrap.dedent(msg))
 
         n_experts      = None
         n_experts_used = None
 
         if "num_local_experts" in config:
             n_experts = config["num_local_experts"]
             n_experts_used = config["num_experts_per_tok"]
@@ -261,15 +270,16 @@
             rope_finetuned    = rope_finetuned,
         )
 
     # LLaMA v2 70B params.json
     # {"dim": 8192, "multiple_of": 4096, "ffn_dim_multiplier": 1.3, "n_heads": 64, "n_kv_heads": 8, "n_layers": 80, "norm_eps": 1e-05, "vocab_size": -1}
     @staticmethod
     def loadOriginalParamsJson(model: LazyModel, config_path: Path) -> Params:
-        config = json.load(open(config_path))
+        with open(config_path) as f:
+            config = json.load(f)
 
         n_experts      = None
         n_experts_used = None
         f_rope_freq_base = None
 
         # hack to determine LLaMA v1 vs v2 vs CodeLlama
         if config.get("moe"):
@@ -327,52 +337,94 @@
         return params
 
 
 #
 # vocab
 #
 
-class BpeVocab:
-    def __init__(self, fname_tokenizer: Path, fname_added_tokens: Path | None) -> None:
-        self.bpe_tokenizer = json.loads(open(str(fname_tokenizer), encoding="utf-8").read())
-        if isinstance(self.bpe_tokenizer.get('model'), dict):
-            self.vocab = self.bpe_tokenizer["model"]["vocab"]
-        else:
-            self.vocab = self.bpe_tokenizer
-        added_tokens: dict[str, int]
-        if fname_added_tokens is not None:
-            # FIXME: Verify that added tokens here _cannot_ overlap with the main vocab.
-            added_tokens = json.load(open(fname_added_tokens, encoding="utf-8"))
+@runtime_checkable
+class BaseVocab(Protocol):
+    tokenizer_model: ClassVar[str]
+    name: ClassVar[str]
+
+
+class NoVocab(BaseVocab):
+    tokenizer_model = "no_vocab"
+    name = "no_vocab"
+
+    def __repr__(self) -> str:
+        return "<NoVocab for a model without integrated vocabulary>"
+
+
+@runtime_checkable
+class Vocab(BaseVocab, Protocol):
+    vocab_size: int
+    added_tokens_dict: dict[str, int]
+    added_tokens_list: list[str]
+    fname_tokenizer: Path
+
+    def __init__(self, base_path: Path): ...
+    def all_tokens(self) -> Iterable[tuple[bytes, float, gguf.TokenType]]: ...
+
+
+class BpeVocab(Vocab):
+    tokenizer_model = "gpt2"
+    name = "bpe"
+
+    def __init__(self, base_path: Path):
+        added_tokens: dict[str, int] = {}
+
+        if (fname_tokenizer := base_path / 'vocab.json').exists():
+            # "slow" tokenizer
+            with open(fname_tokenizer, encoding="utf-8") as f:
+                self.vocab = json.load(f)
+
+            try:
+                # FIXME: Verify that added tokens here _cannot_ overlap with the main vocab.
+                with open(base_path / ADDED_TOKENS_FILE, encoding="utf-8") as f:
+                    added_tokens = json.load(f)
+            except FileNotFoundError:
+                pass
         else:
-            # Fall back to trying to find the added tokens in tokenizer.json
-            tokenizer_json_file = fname_tokenizer.parent / 'tokenizer.json'
-            if not tokenizer_json_file.is_file():
-                added_tokens = {}
-            else:
-                tokenizer_json = json.load(open(tokenizer_json_file, encoding="utf-8"))
-                added_tokens = dict(
-                    (item['content'], item['id'])
-                    for item in tokenizer_json.get('added_tokens', [])
-                    # Added tokens here can be duplicates of the main vocabulary.
-                    if item['content'] not in self.bpe_tokenizer)
-
-        vocab_size: int = len(self.vocab)
-        expected_ids    = list(range(vocab_size, vocab_size + len(added_tokens)))
-        actual_ids      = sorted(added_tokens.values())
+            # "fast" tokenizer
+            fname_tokenizer = base_path / FAST_TOKENIZER_FILE
+
+            # if this fails, FileNotFoundError propagates to caller
+            with open(fname_tokenizer, encoding="utf-8") as f:
+                tokenizer_json = json.load(f)
+
+            tokenizer_model: dict[str, Any] = tokenizer_json['model']
+            if (
+                tokenizer_model['type'] != 'BPE' or tokenizer_model.get('byte_fallback', False)
+                or tokenizer_json['decoder']['type'] != 'ByteLevel'
+            ):
+                raise FileNotFoundError('Cannot find GPT-2 BPE tokenizer')
+
+            self.vocab = tokenizer_model["vocab"]
+
+            if (added := tokenizer_json.get('added_tokens')) is not None:
+                # Added tokens here can be duplicates of the main vocabulary.
+                added_tokens = {item['content']: item['id']
+                                for item in added
+                                if item['content'] not in self.vocab}
+
+        vocab_size   = len(self.vocab)
+        expected_ids = list(range(vocab_size, vocab_size + len(added_tokens)))
+        actual_ids   = sorted(added_tokens.values())
         if expected_ids != actual_ids:
             expected_end_id = vocab_size + len(actual_ids) - 1
-            raise Exception(f"Expected the {len(actual_ids)} added token ID(s) to be sequential in the range {vocab_size} - {expected_end_id}; got {actual_ids}")
+            raise ValueError(f"Expected the {len(actual_ids)} added token ID(s) to be sequential in the range "
+                             f"{vocab_size} - {expected_end_id}; got {actual_ids}")
 
         items = sorted(added_tokens.items(), key=lambda text_idx: text_idx[1])
         self.added_tokens_dict    = added_tokens
         self.added_tokens_list    = [text for (text, idx) in items]
-        self.vocab_size_base: int = vocab_size
-        self.vocab_size: int      = self.vocab_size_base + len(self.added_tokens_list)
+        self.vocab_size_base      = vocab_size
+        self.vocab_size           = self.vocab_size_base + len(self.added_tokens_list)
         self.fname_tokenizer      = fname_tokenizer
-        self.fname_added_tokens   = fname_added_tokens
 
     def bpe_tokens(self) -> Iterable[tuple[bytes, float, gguf.TokenType]]:
         reverse_vocab = {id: encoded_tok for encoded_tok, id in self.vocab.items()}
 
         for i, _ in enumerate(self.vocab):
             yield reverse_vocab[i], 0.0, gguf.TokenType.NORMAL
 
@@ -385,45 +437,53 @@
         yield from self.bpe_tokens()
         yield from self.added_tokens()
 
     def __repr__(self) -> str:
         return f"<BpeVocab with {self.vocab_size_base} base tokens and {len(self.added_tokens_list)} added tokens>"
 
 
-class SentencePieceVocab:
-    def __init__(self, fname_tokenizer: Path, fname_added_tokens: Path | None) -> None:
-        self.sentencepiece_tokenizer = SentencePieceProcessor(str(fname_tokenizer))
-        added_tokens: dict[str, int]
-        if fname_added_tokens is not None:
-            added_tokens = json.load(open(fname_added_tokens, encoding="utf-8"))
-        else:
-            added_tokens = {}
+class SentencePieceVocab(Vocab):
+    tokenizer_model = "llama"
+    name = "spm"
+
+    def __init__(self, base_path: Path):
+        added_tokens: dict[str, int] = {}
+        if (fname_tokenizer := base_path / 'tokenizer.model').exists():
+            # normal location
+            try:
+                with open(base_path / ADDED_TOKENS_FILE, encoding="utf-8") as f:
+                    added_tokens = json.load(f)
+            except FileNotFoundError:
+                pass
+        elif not (fname_tokenizer := base_path.parent / 'tokenizer.model').exists():
+            # not found in alternate location either
+            raise FileNotFoundError('Cannot find tokenizer.model')
 
-        vocab_size: int = self.sentencepiece_tokenizer.vocab_size()
+        self.sentencepiece_tokenizer = SentencePieceProcessor(str(fname_tokenizer))
+        vocab_size = self.sentencepiece_tokenizer.vocab_size()
 
         new_tokens       = {id: piece for piece, id in added_tokens.items() if id >= vocab_size}
         expected_new_ids = list(range(vocab_size, vocab_size + len(new_tokens)))
         actual_new_ids   = sorted(new_tokens.keys())
 
         if expected_new_ids != actual_new_ids:
             raise ValueError(f"Expected new token IDs {expected_new_ids} to be sequential; got {actual_new_ids}")
 
         # Token pieces that were added to the base vocabulary.
-        self.added_tokens_dict = added_tokens
+        self.added_tokens_dict  = added_tokens
         self.added_tokens_list  = [new_tokens[id] for id in actual_new_ids]
         self.vocab_size_base    = vocab_size
         self.vocab_size         = self.vocab_size_base + len(self.added_tokens_list)
         self.fname_tokenizer    = fname_tokenizer
-        self.fname_added_tokens = fname_added_tokens
 
     def sentencepiece_tokens(self) -> Iterable[tuple[bytes, float, gguf.TokenType]]:
         tokenizer = self.sentencepiece_tokenizer
         for i in range(tokenizer.vocab_size()):
             piece = tokenizer.id_to_piece(i)
-            text: bytes = piece.encode("utf-8")
+            text         = piece.encode("utf-8")
             score: float = tokenizer.get_score(i)
 
             toktype = gguf.TokenType.NORMAL
             if tokenizer.is_unknown(i):
                 toktype = gguf.TokenType.UNKNOWN
             if tokenizer.is_control(i):
                 toktype = gguf.TokenType.CONTROL
@@ -448,32 +508,50 @@
         yield from self.sentencepiece_tokens()
         yield from self.added_tokens()
 
     def __repr__(self) -> str:
         return f"<SentencePieceVocab with {self.vocab_size_base} base tokens and {len(self.added_tokens_list)} added tokens>"
 
 
-class HfVocab:
-    def __init__(self, fname_tokenizer: Path, fname_added_tokens: Path | None = None) -> None:
+class LlamaHfVocab(Vocab):
+    tokenizer_model = "llama"
+    name = "hfft"
+
+    def __init__(self, base_path: Path, ignore_nonllama: bool = False):
+        fname_tokenizer = base_path / FAST_TOKENIZER_FILE
+        # if this fails, FileNotFoundError propagates to caller
+        with open(fname_tokenizer, encoding='utf-8') as f:
+            tokenizer_json = json.load(f)
+
+        # pre-check so we know if we need transformers
+        tokenizer_model: dict[str, Any] = tokenizer_json['model']
+        if ignore_nonllama:
+            pass  # workaround incorrect use of this class for WordPiece
+        elif (
+            tokenizer_model['type'] != 'BPE' or not tokenizer_model.get('byte_fallback', False)
+            or tokenizer_json['decoder']['type'] != 'Sequence'
+        ):
+            raise FileNotFoundError('Cannot find Llama BPE tokenizer')
+
         try:
             from transformers import AutoTokenizer
         except ImportError as e:
             raise ImportError(
-                "To use HfVocab, please install the `transformers` package. "
+                "To use LlamaHfVocab, please install the `transformers` package. "
                 "You can install it with `pip install transformers`."
             ) from e
 
-        print("fname_tokenizer:", fname_tokenizer)
         # Allow the tokenizer to default to slow or fast versions.
         # Explicitly set tokenizer to use local paths.
         self.tokenizer = AutoTokenizer.from_pretrained(
-            fname_tokenizer,
-            cache_dir=fname_tokenizer,
+            base_path,
+            cache_dir=base_path,
             local_files_only=True,
         )
+        assert self.tokenizer.is_fast  # assume tokenizer.json is used
 
         # Initialize lists and dictionaries for added tokens
         self.added_tokens_list = []
         self.added_tokens_dict = dict()
         self.added_tokens_ids  = set()
 
         # Process added tokens
@@ -493,16 +571,15 @@
         }
         self.special_ids = set(self.tokenizer.all_special_ids)
 
         # Set vocabulary sizes
         self.vocab_size_base = self.tokenizer.vocab_size
         self.vocab_size      = self.vocab_size_base + len(self.added_tokens_list)
 
-        self.fname_tokenizer    = fname_tokenizer
-        self.fname_added_tokens = fname_added_tokens
+        self.fname_tokenizer = fname_tokenizer
 
     def hf_tokens(self) -> Iterable[tuple[bytes, float, gguf.TokenType]]:
         reverse_vocab = {
             id: encoded_tok for encoded_tok, id in self.tokenizer.get_vocab().items()
         }
 
         for token_id in range(self.vocab_size_base):
@@ -546,18 +623,15 @@
         return "<0x0A>" in self.tokenizer.vocab or "\n" in self.tokenizer.vocab
 
     def all_tokens(self) -> Iterable[tuple[bytes, float, gguf.TokenType]]:
         yield from self.hf_tokens()
         yield from self.added_tokens()
 
     def __repr__(self) -> str:
-        return f"<HfVocab with {self.vocab_size_base} base tokens and {len(self.added_tokens_list)} added tokens>"
-
-
-Vocab: TypeAlias = "BpeVocab | SentencePieceVocab | HfVocab"
+        return f"<LlamaHfVocab with {self.vocab_size_base} base tokens and {len(self.added_tokens_list)} added tokens>"
 
 
 #
 # data loading
 # TODO: reuse (probably move to gguf.py?)
 #
 
@@ -567,15 +641,15 @@
     if n_head_kv is not None and n_head != n_head_kv:
         n_head = n_head_kv
     return (weights.reshape(n_head, 2, weights.shape[0] // n_head // 2, *weights.shape[1:])
             .swapaxes(1, 2)
             .reshape(weights.shape))
 
 
-class Tensor(metaclass=ABCMeta):
+class Tensor(ABC):
     data_type: DataType
 
     @abstractmethod
     def astype(self, data_type: DataType) -> Tensor: ...
     @abstractmethod
     def permute(self, n_head: int, n_head_kv: int) -> Tensor: ...
     @abstractmethod
@@ -589,15 +663,15 @@
 def bf16_to_fp32(bf16_arr: np.ndarray[Any, np.dtype[np.uint16]]) -> NDArray:
     assert bf16_arr.dtype == np.uint16, f"Input array should be of dtype uint16, but got {bf16_arr.dtype}"
     fp32_arr = bf16_arr.astype(np.uint32) << 16
     return fp32_arr.view(np.float32)
 
 
 class UnquantizedTensor(Tensor):
-    def __init__(self, ndarray: NDArray) -> None:
+    def __init__(self, ndarray: NDArray):
         assert isinstance(ndarray, np.ndarray)
         self.ndarray = ndarray
         self.data_type = NUMPY_TYPE_TO_DATA_TYPE[ndarray.dtype]
 
     def astype(self, data_type: DataType) -> Tensor:
         dtype = data_type.dtype
         if self.data_type == DT_BF16:
@@ -668,24 +742,24 @@
 
 
 @dataclass
 class ModelPlus:
     model: LazyModel
     paths: list[Path]  # Where this was read from.
     format: Literal['ggml', 'torch', 'safetensors', 'none']
-    vocab: Vocab | None  # For GGML models (which have vocab built in), the vocab.
+    vocab: BaseVocab | None  # For GGML models (which have vocab built in), the vocab.
 
 
 def merge_sharded(models: list[LazyModel]) -> LazyModel:
     # Original LLaMA models have each file contain one part of each tensor.
     # Use a dict instead of a set to preserve order.
     names = {name: None for model in models for name in model}
 
     def convert(name: str) -> LazyTensor:
-        lazy_tensors: list[LazyTensor] = [model[name] for model in models]
+        lazy_tensors = [model[name] for model in models]
         if len(lazy_tensors) == 1:
             # only one file; don't go through this procedure since there might
             # be quantized tensors
             return lazy_tensors[0]
         if len(lazy_tensors[0].shape) == 1:
             # the tensor is just duplicated in every file
             return lazy_tensors[0]
@@ -698,15 +772,15 @@
             # split by rows
             axis = 0
         concatenated_shape = list(lazy_tensors[0].shape)
         concatenated_shape[axis] = sum(tensor.shape[axis] for tensor in lazy_tensors)
 
         def load() -> UnquantizedTensor:
             ndarrays = [load_unquantized(tensor) for tensor in lazy_tensors]
-            concatenated: NDArray = np.concatenate(ndarrays, axis=axis)
+            concatenated = np.concatenate(ndarrays, axis=axis)
             return UnquantizedTensor(concatenated)
         description = 'concatenated[[' + '] | ['.join(lt.description for lt in lazy_tensors) + ']]'
         return LazyTensor(load, concatenated_shape, lazy_tensors[0].data_type, description)
     return {name: convert(name) for name in names}
 
 
 def merge_multifile_models(models_plus: list[ModelPlus]) -> ModelPlus:
@@ -750,14 +824,23 @@
     def load() -> Tensor:
         return lazy_tensor.load().part(n_part)
     s = lazy_tensor.shape.copy()
     s[0] = s[0] // 3
     return LazyTensor(load, s, lazy_tensor.data_type, 'part ' + lazy_tensor.description)
 
 
+def pack_experts_lazy(lazy_tensors: list[LazyTensor]) -> LazyTensor:
+    def load() -> Tensor:
+        tensors = [lazy_tensor.load() for lazy_tensor in lazy_tensors]
+        return UnquantizedTensor(np.array([tensor.ndarray for tensor in tensors]))
+    s = lazy_tensors[0].shape.copy()
+    s.insert(0, len(lazy_tensors))
+    return LazyTensor(load, s, lazy_tensors[0].data_type, 'pack_experts ' + ' | '.join(lt.description for lt in lazy_tensors))
+
+
 # Functionality that simulates `torch.load` but where individual tensors are
 # only loaded into memory on demand, not all at once.
 # PyTorch can't do this natively as of time of writing:
 # - https://github.com/pytorch/pytorch/issues/64327
 # This allows us to de-shard without multiplying RAM usage, and also
 # conveniently drops the PyTorch dependency (though we still need numpy).
 
@@ -786,18 +869,18 @@
         data_type = pid[1].data_type
         filename_stem = pid[2]
         filename = f'{self.data_base_path}/{filename_stem}'
         info = self.zip_file.getinfo(filename)
 
         def load(offset: int, elm_count: int) -> NDArray:
             dtype = data_type.dtype
-            fp = self.zip_file.open(info)
-            fp.seek(offset * dtype.itemsize)
-            size = elm_count * dtype.itemsize
-            data = fp.read(size)
+            with self.zip_file.open(info) as fp:
+                fp.seek(offset * dtype.itemsize)
+                size = elm_count * dtype.itemsize
+                data = fp.read(size)
             assert len(data) == size
             return np.frombuffer(data, dtype)
         description = f'storage data_type={data_type} path-in-zip={filename} path={self.zip_file.filename}'
         return LazyStorage(load=load, kind=pid[1], description=description)
 
     @staticmethod
     def lazy_rebuild_tensor_v2(storage: Any, storage_offset: Any, size: Any, stride: Any,
@@ -810,15 +893,15 @@
         description = f'pickled storage_offset={storage_offset} in {storage.description}'
         return LazyTensor(load, list(size), storage.kind.data_type, description)
 
     @staticmethod
     def rebuild_from_type_v2(func, new_type, args, state):
         return func(*args)
 
-    CLASSES: dict[tuple[str, str], Any] = {
+    CLASSES = {
         # getattr used here as a workaround for mypy not being smart enough to determine
         # the staticmethods have a __func__ attribute.
         ('torch._tensor', '_rebuild_from_type_v2'): getattr(rebuild_from_type_v2, '__func__'),
         ('torch._utils', '_rebuild_tensor_v2'): getattr(lazy_rebuild_tensor_v2, '__func__'),
         ('torch', 'BFloat16Storage'): LazyStorageKind(DT_BF16),
         ('torch', 'HalfStorage'): LazyStorageKind(DT_F16),
         ('torch', 'FloatStorage'): LazyStorageKind(DT_F32),
@@ -869,15 +952,15 @@
     model = {name: convert(info) for (name, info) in header.items() if name != '__metadata__'}
     return ModelPlus(model=model, paths=[path], format='safetensors', vocab=None)
 
 
 def must_read(fp: IO[bytes], length: int) -> bytes:
     ret = fp.read(length)
     if len(ret) < length:
-        raise Exception("unexpectedly reached end of file")
+        raise EOFError("unexpectedly reached end of file")
     return ret
 
 
 @functools.lru_cache(maxsize=None)
 def lazy_load_file(path: Path) -> ModelPlus:
     fp = open(path, 'rb')
     first8 = fp.read(8)
@@ -927,20 +1010,23 @@
                     futures.append(executor.submit(func, next(iterable)))
                 except StopIteration:
                     done = True
                     break
             yield result
 
 
-def check_vocab_size(params: Params, vocab: Vocab, pad_vocab: bool = False) -> None:
+def check_vocab_size(params: Params, vocab: BaseVocab, pad_vocab: bool = False) -> None:
     # Handle special case where the model's vocab size is not set
     if params.n_vocab == -1:
         raise ValueError(
-            f"The model's vocab size is set to -1 in params.json. Please update it manually. Maybe {vocab.vocab_size}?"
+            "The model's vocab size is set to -1 in params.json. Please update it manually."
+            + (f" Maybe {vocab.vocab_size}?" if isinstance(vocab, Vocab) else ""),
         )
+    if not isinstance(vocab, Vocab):
+        return  # model has no vocab
 
     # Check for a vocab size mismatch
     if params.n_vocab == vocab.vocab_size:
         print("Ignoring added_tokens.json since model matches vocab size without it.")
         return
 
     if pad_vocab and params.n_vocab > vocab.vocab_size:
@@ -956,19 +1042,19 @@
 
     msg = f"Vocab size mismatch (model has {params.n_vocab}, but {vocab.fname_tokenizer} has {vocab.vocab_size})."
     if vocab.vocab_size < params.n_vocab < vocab.vocab_size + 20:
         msg += f"  Most likely you are missing added_tokens.json (should be in {vocab.fname_tokenizer.parent})."
     if vocab.vocab_size < params.n_vocab:
         msg += " Add the --pad-vocab option and try again."
 
-    raise Exception(msg)
+    raise ValueError(msg)
 
 
 class OutputFile:
-    def __init__(self, fname_out: Path, endianess:gguf.GGUFEndian = gguf.GGUFEndian.LITTLE) -> None:
+    def __init__(self, fname_out: Path, endianess:gguf.GGUFEndian = gguf.GGUFEndian.LITTLE):
         self.gguf = gguf.GGUFWriter(fname_out, gguf.MODEL_ARCH_NAMES[ARCH], endianess=endianess)
 
     def add_meta_arch(self, params: Params) -> None:
         name = "LLaMA"
 
         # TODO: better logic to determine model name
         if params.n_ctx == 4096:
@@ -1009,28 +1095,14 @@
 
         if params.rope_finetuned is not None:
             self.gguf.add_rope_scaling_finetuned(params.rope_finetuned)
 
         if params.ftype is not None:
             self.gguf.add_file_type(params.ftype)
 
-    def handle_tokenizer_model(self, vocab: Vocab) -> str:
-        # Map the vocab types to the supported tokenizer models
-        tokenizer_model = {
-            SentencePieceVocab: "llama",
-            HfVocab: "llama",
-            BpeVocab: "gpt2",
-        }.get(type(vocab))
-
-        # Block if vocab type is not predefined
-        if tokenizer_model is None:
-            raise ValueError("Unknown vocab type: Not supported")
-
-        return tokenizer_model
-
     def extract_vocabulary_from_model(self, vocab: Vocab) -> tuple[list[bytes], list[float], list[gguf.TokenType]]:
         tokens = []
         scores = []
         toktypes = []
 
         # NOTE: `all_tokens` returns the base vocabulary and added tokens
         for text, score, toktype in vocab.all_tokens():
@@ -1039,19 +1111,16 @@
             toktypes.append(toktype)
 
         assert len(tokens) == vocab.vocab_size
 
         return tokens, scores, toktypes
 
     def add_meta_vocab(self, vocab: Vocab) -> None:
-        # Handle the tokenizer model
-        tokenizer_model = self.handle_tokenizer_model(vocab)
-
         # Ensure that tokenizer_model is added to the GGUF model
-        self.gguf.add_tokenizer_model(tokenizer_model)
+        self.gguf.add_tokenizer_model(vocab.tokenizer_model)
 
         # Extract model vocabulary for model conversion
         tokens, scores, toktypes = self.extract_vocabulary_from_model(vocab)
 
         # Add extracted token information for model conversion
         self.gguf.add_token_list(tokens)
         self.gguf.add_token_scores(scores)
@@ -1070,23 +1139,43 @@
     def write_meta(self) -> None:
         self.gguf.write_header_to_file()
         self.gguf.write_kv_data_to_file()
 
     def write_tensor_info(self) -> None:
         self.gguf.write_ti_data_to_file()
 
+    def write_tensor_data(self, ftype: GGMLFileType, model: LazyModel, concurrency: int) -> None:
+        ndarrays_inner = bounded_parallel_map(OutputFile.do_item, model.items(), concurrency=concurrency)
+        if ftype == GGMLFileType.MostlyQ8_0:
+            ndarrays = bounded_parallel_map(
+                OutputFile.maybe_do_quantize, ndarrays_inner, concurrency=concurrency, max_workers=concurrency,
+                use_processpool_executor=True,
+            )
+        else:
+            ndarrays = map(OutputFile.maybe_do_quantize, ndarrays_inner)
+
+        start = time.time()
+        for i, ((name, lazy_tensor), ndarray) in enumerate(zip(model.items(), ndarrays)):
+            elapsed = time.time() - start
+            size = ' x '.join(f"{dim:6d}" for dim in lazy_tensor.shape)
+            padi = len(str(len(model)))
+            print(
+                f"[{i + 1:{padi}d}/{len(model)}] Writing tensor {name:38s} | size {size:16} | type {lazy_tensor.data_type.name:4} | T+{int(elapsed):4}"
+            )
+            self.gguf.write_tensor_data(ndarray)
+
     def close(self) -> None:
         self.gguf.close()
 
     @staticmethod
     def write_vocab_only(
         fname_out: Path, params: Params, vocab: Vocab, svocab: gguf.SpecialVocab,
         endianess: gguf.GGUFEndian = gguf.GGUFEndian.LITTLE, pad_vocab: bool = False,
     ) -> None:
-        check_vocab_size(params, vocab, pad_vocab = pad_vocab)
+        check_vocab_size(params, vocab, pad_vocab=pad_vocab)
 
         of = OutputFile(fname_out, endianess=endianess)
 
         # meta data
         of.add_meta_arch(params)
         of.add_meta_vocab(vocab)
         of.add_meta_special_vocab(svocab)
@@ -1106,83 +1195,85 @@
         dt, arr = item
         if not isinstance(dt, QuantizedDataType):
             return arr
         return dt.quantize(arr)
 
     @staticmethod
     def write_all(
-        fname_out: Path, ftype: GGMLFileType, params: Params, model: LazyModel, vocab: Vocab, svocab: gguf.SpecialVocab,
+        fname_out: Path, ftype: GGMLFileType, params: Params, model: LazyModel, vocab: BaseVocab, svocab: gguf.SpecialVocab,
         concurrency: int = DEFAULT_CONCURRENCY, endianess: gguf.GGUFEndian = gguf.GGUFEndian.LITTLE,
         pad_vocab: bool = False,
     ) -> None:
         check_vocab_size(params, vocab, pad_vocab=pad_vocab)
 
         of = OutputFile(fname_out, endianess=endianess)
 
         # meta data
         of.add_meta_arch(params)
-        of.add_meta_vocab(vocab)
-        of.add_meta_special_vocab(svocab)
+        if isinstance(vocab, Vocab):
+            of.add_meta_vocab(vocab)
+            of.add_meta_special_vocab(svocab)
+        else:  # NoVocab
+            of.gguf.add_tokenizer_model(vocab.tokenizer_model)
 
         # tensor info
         for name, lazy_tensor in model.items():
             of.add_tensor_info(name, lazy_tensor)
 
         of.write_meta()
         of.write_tensor_info()
 
         # tensor data
-        ndarrays_inner = bounded_parallel_map(OutputFile.do_item, model.items(), concurrency = concurrency)
-        if ftype == GGMLFileType.MostlyQ8_0:
-            ndarrays = bounded_parallel_map(
-                OutputFile.maybe_do_quantize, ndarrays_inner, concurrency=concurrency, max_workers=concurrency,
-                use_processpool_executor=True,
-            )
-        else:
-            ndarrays = map(OutputFile.maybe_do_quantize, ndarrays_inner)
-
-        start = time.time()
-        for i, ((name, lazy_tensor), ndarray) in enumerate(zip(model.items(), ndarrays)):
-            elapsed = time.time() - start
-            size = ' x '.join(f"{dim:6d}" for dim in lazy_tensor.shape)
-            padi = len(str(len(model)))
-            print(
-                f"[{i+1:{padi}d}/{len(model)}] Writing tensor {name:38s} | size {size:16} | type {lazy_tensor.data_type.name:4} | T+{int(elapsed):4}"
-            )
-            of.gguf.write_tensor_data(ndarray)
+        of.write_tensor_data(ftype, model, concurrency)
 
         of.close()
 
 
 def pick_output_type(model: LazyModel, output_type_str: str | None) -> GGMLFileType:
     wq_type = model[gguf.TENSOR_NAMES[gguf.MODEL_TENSOR.ATTN_Q].format(bid=0) + ".weight"].data_type
 
-    if output_type_str == "f32" or (output_type_str is None and wq_type == DT_F32):
+    if output_type_str == "f32" or (output_type_str is None and wq_type in (DT_F32, DT_BF16)):
         return GGMLFileType.AllF32
-    if output_type_str == "f16" or (output_type_str is None and wq_type in (DT_F16, DT_BF16)):
+    if output_type_str == "f16" or (output_type_str is None and wq_type == DT_F16):
         return GGMLFileType.MostlyF16
     if output_type_str == "q8_0":
         return GGMLFileType.MostlyQ8_0
 
     name_to_type = {name: lazy_tensor.data_type for (name, lazy_tensor) in model.items()}
 
-    raise Exception(f"Unexpected combination of types: {name_to_type}")
+    raise ValueError(f"Unexpected combination of types: {name_to_type}")
 
 
 def convert_to_output_type(model: LazyModel, output_type: GGMLFileType) -> LazyModel:
     return {name: tensor.astype(output_type.type_for_tensor(name, tensor))
             for (name, tensor) in model.items()}
 
 
 def convert_model_names(model: LazyModel, params: Params, skip_unknown: bool) -> LazyModel:
     tmap = gguf.TensorNameMap(ARCH, params.n_layer)
-    should_skip: set[gguf.MODEL_TENSOR] = set(gguf.MODEL_TENSOR_SKIP.get(ARCH, []))
+    should_skip = set(gguf.MODEL_TENSOR_SKIP.get(ARCH, []))
 
     tmp = model
 
+    # merge experts into one tensor
+    if params.n_experts and params.n_experts > 0:
+        for i_l in range(params.n_layer):
+            for w in range(1, 4):
+                experts = []
+                for e in range(params.n_experts):
+                    if f"layers.{i_l}.feed_forward.experts.{e}.w{w}.weight" in model:
+                        experts.append(model[f"layers.{i_l}.feed_forward.experts.{e}.w{w}.weight"])
+                        del tmp[f"layers.{i_l}.feed_forward.experts.{e}.w{w}.weight"]
+                    elif f"model.layers.{i_l}.block_sparse_moe.experts.{e}.w{w}.weight" in model:
+                        experts.append(model[f"model.layers.{i_l}.block_sparse_moe.experts.{e}.w{w}.weight"])
+                        del tmp[f"model.layers.{i_l}.block_sparse_moe.experts.{e}.w{w}.weight"]
+                    else:
+                        raise ValueError(f"Expert tensor not found: layers.{i_l}.feed_forward.experts.{e}.w{w}.weight")
+                tmp[f"layers.{i_l}.feed_forward.experts.w{w}.weight"] = pack_experts_lazy(experts)
+
     # HF models permut or pack some of the tensors, so we need to undo that
     for i in itertools.count():
         if f"model.layers.{i}.self_attn.q_proj.weight" in model:
             print(f"Permuting layer {i}")
             tmp[f"model.layers.{i}.self_attn.q_proj.weight"] = permute_lazy(model[f"model.layers.{i}.self_attn.q_proj.weight"], params.n_head, params.n_head)
             tmp[f"model.layers.{i}.self_attn.k_proj.weight"] = permute_lazy(model[f"model.layers.{i}.self_attn.k_proj.weight"], params.n_head, params.n_head_kv)
             # tmp[f"model.layers.{i}.self_attn.v_proj.weight"] =              model[f"model.layers.{i}.self_attn.v_proj.weight"]
@@ -1198,16 +1289,15 @@
     out: LazyModel = {}
     for name, lazy_tensor in model.items():
         tensor_type, name_new = tmap.get_type_and_name(name, try_suffixes = (".weight", ".bias")) or (None, None)
         if name_new is None:
             if skip_unknown:
                 print(f"Unexpected tensor name: {name} - skipping")
                 continue
-            else:
-                raise Exception(f"Unexpected tensor name: {name}. Use --skip-unknown to ignore it (e.g. LLaVA)")
+            raise ValueError(f"Unexpected tensor name: {name}. Use --skip-unknown to ignore it (e.g. LLaVA)")
 
         if tensor_type in should_skip:
             print(f"skipping tensor {name_new}")
             continue
 
         print(f"{name:48s} -> {name_new:40s} | {lazy_tensor.data_type.name:6s} | {lazy_tensor.shape}")
         out[name_new] = lazy_tensor
@@ -1216,15 +1306,15 @@
 
 
 def nth_multifile_path(path: Path, n: int) -> Path | None:
     '''Given any path belonging to a multi-file model (e.g. foo.bin.1), return
     the nth path in the model.
     '''
     # Support the following patterns:
-    patterns: list[tuple[str, str]] = [
+    patterns = [
         # - x.00.pth, x.01.pth, etc.
         (r'\.[0-9]{2}\.pth$', f'.{n:02}.pth'),
         # - x-00001-of-00002.bin, x-00002-of-00002.bin, etc.
         (r'-[0-9]{5}-of-(.*)$', fr'-{n:05}-of-\1'),
         # x.bin, x.bin.1, etc.
         (r'(\.[0-9]+)?$', r'\1' if n == 0 else fr'\1.{n}')
     ]
@@ -1262,91 +1352,75 @@
         globs = ["model-00001-of-*.safetensors", "model.safetensors"]
         files = [file for glob in globs for file in path.glob(glob)]
         if not files:
             # Try the PyTorch patterns too, with lower priority
             globs = ["consolidated.00.pth", "pytorch_model-00001-of-*.bin", "*.pt", "pytorch_model.bin"]
             files = [file for glob in globs for file in path.glob(glob)]
         if not files:
-            raise Exception(f"Can't find model in directory {path}")
+            raise FileNotFoundError(f"Can't find model in directory {path}")
         if len(files) > 1:
-            raise Exception(f"Found multiple models in {path}, not sure which to pick: {files}")
+            raise ValueError(f"Found multiple models in {path}, not sure which to pick: {files}")
         path = files[0]
 
     paths = find_multifile_paths(path)
     models_plus: list[ModelPlus] = []
     for path in paths:
         print(f"Loading model file {path}")
         models_plus.append(lazy_load_file(path))
 
     model_plus = merge_multifile_models(models_plus)
     return model_plus
 
 
 class VocabFactory:
-    _FILES = {"spm": "tokenizer.model", "bpe": "vocab.json", "hfft": "tokenizer.json"}
+    _VOCAB_CLASSES: list[type[Vocab]] = [SentencePieceVocab, BpeVocab, LlamaHfVocab]
 
     def __init__(self, path: Path):
         self.path = path
-        self.file_paths = self._detect_files()
-        print(f"Found vocab files: {self.file_paths}")
-
-    def _detect_files(self) -> dict[str, Path | None]:
-        def locate(file: str) -> Path | None:
-            if (path := self.path / file).exists():
-                return path
-            if (path := self.path.parent / file).exists():
-                return path
-            return None
 
-        return {vt: locate(f) for vt, f in self._FILES.items()}
-
-    def _select_file(self, vocab_types: list[str]) -> tuple[str, Path]:
-        for vtype in vocab_types:
-            try:
-                path = self.file_paths[vtype]
-            except KeyError:
-                raise ValueError(f"Unsupported vocabulary type {vtype}") from None
-            if path is not None:
-                return vtype, path
-        raise FileNotFoundError(f"Could not find any of {[self._FILES[vt] for vt in vocab_types]}")
-
-    def _create_special_vocab(self, vocab: Vocab, vocabtype: str, model_parent_path: Path) -> gguf.SpecialVocab:
-        load_merges = vocabtype == "bpe"
-        n_vocab = vocab.vocab_size if hasattr(vocab, "vocab_size") else None
+    def _create_special_vocab(self, vocab: BaseVocab, model_parent_path: Path) -> gguf.SpecialVocab:
+        load_merges = vocab.name == "bpe"
+        n_vocab = vocab.vocab_size if isinstance(vocab, Vocab) else None
         return gguf.SpecialVocab(
             model_parent_path,
             load_merges=load_merges,
             special_token_types=None,  # Predetermined or passed as a parameter
             n_vocab=n_vocab,
         )
 
-    def load_vocab(self, vocab_types: list[str], model_parent_path: Path) -> tuple[Vocab, gguf.SpecialVocab]:
-        vocab_type, path = self._select_file(vocab_types)
-        print(f"Loading vocab file {path!r}, type {vocab_type!r}")
-
-        added_tokens_path = path.parent / "added_tokens.json"
-        vocab: Vocab
-        if vocab_type == "bpe":
-            vocab = BpeVocab(
-                path, added_tokens_path if added_tokens_path.exists() else None
-            )
-        elif vocab_type == "spm":
-            vocab = SentencePieceVocab(
-                path, added_tokens_path if added_tokens_path.exists() else None
-            )
-        elif vocab_type == "hfft":
-            vocab = HfVocab(
-                path.parent, added_tokens_path if added_tokens_path.exists() else None
-            )
+    def _create_vocab_by_path(self, vocab_types: list[str]) -> Vocab:
+        vocab_classes: dict[str, type[Vocab]] = {cls.name: cls for cls in self._VOCAB_CLASSES}
+        selected_vocabs: dict[str, type[Vocab]] = {}
+        for vtype in vocab_types:
+            try:
+                selected_vocabs[vtype] = vocab_classes[vtype]
+            except KeyError:
+                raise ValueError(f"Unsupported vocabulary type {vtype}") from None
+
+        for vtype, cls in selected_vocabs.items():
+            try:
+                vocab = cls(self.path)
+                break
+            except FileNotFoundError:
+                pass  # ignore unavailable tokenizers
         else:
-            raise ValueError(vocab_type)
+            raise FileNotFoundError(f"Could not find a tokenizer matching any of {vocab_types}")
+
+        print(f"Loaded vocab file {vocab.fname_tokenizer!r}, type {vocab.name!r}")
+        return vocab
+
+    def load_vocab(self, vocab_types: list[str] | None, model_parent_path: Path) -> tuple[BaseVocab, gguf.SpecialVocab]:
+        vocab: BaseVocab
+        if vocab_types is None:
+            vocab = NoVocab()
+        else:
+            vocab = self._create_vocab_by_path(vocab_types)
         # FIXME: Respect --vocab-dir?
         special_vocab = self._create_special_vocab(
             vocab,
-            vocab_type,
             model_parent_path,
         )
         return vocab, special_vocab
 
 
 def default_outfile(model_paths: list[Path], file_type: GGMLFileType) -> Path:
     namestr = {
@@ -1367,89 +1441,38 @@
     print(f"model_plus.paths = {model_plus.paths!r}")
     print(f"model_plus.format = {model_plus.format!r}")
     print(f"model_plus.vocab = {model_plus.vocab!r}")
     for name, lazy_tensor in model_plus.model.items():
         print(f"{name}: shape={lazy_tensor.shape} type={lazy_tensor.data_type}; {lazy_tensor.description}")
 
 
-def do_gguf_conversion(model: str, output: str, out_type: str, vocab_dir: str, vocab_type: str, context: int, pad_vocab: bool, concurrency: bool, big_endian: bool) -> None:
-    model_plus = load_some_model(model)
-
-    endianess = gguf.GGUFEndian.LITTLE
-    if big_endian:
-        endianess = gguf.GGUFEndian.BIG
-    print(f"endianess = {endianess}")
-
-    params = Params.load(model_plus)
-
-    if params.n_ctx == -1:
-        if context is None:
-            context = 4096
-        params.n_ctx = context
-    print(f"context = {context}")
-
-    if out_type is not None:
-        params.ftype = {
-            "f32": GGMLFileType.AllF32,
-            "f16": GGMLFileType.MostlyF16,
-            "q8_0": GGMLFileType.MostlyQ8_0,
-        }[out_type]
-
-    print(f"params = {params}")
-
-    model_parent_path = model_plus.paths[0].parent
-
-    if vocab_dir is not None:
-        vocab_path = Path(vocab_dir)
-    else:
-        vocab_path = Path(model or model_parent_path)
-
-    vocab_factory = VocabFactory(vocab_path)
-    vocab, special_vocab = vocab_factory.load_vocab(vocab_type.split(","), model_parent_path)
-
-    if model_plus.vocab is not None and vocab_dir is None:
-        vocab = model_plus.vocab
-
-    print(f"Vocab info: {vocab}")
-    print(f"Special vocab info: {special_vocab}")
-
-    model   = model_plus.model
-    model   = convert_model_names(model, params, False) #skip_unknown
-    ftype   = pick_output_type(model, out_type)
-    model   = convert_to_output_type(model, ftype)
-    outfile = output or default_outfile(model_plus.paths, ftype)
-
-    params.ftype = ftype
-    print(f"Writing {outfile}, format {ftype}")
-
-    OutputFile.write_all(output, ftype, params, model, vocab, special_vocab,
-                         concurrency=concurrency, endianess=endianess, pad_vocab=pad_vocab)
-    print(f"Wrote {outfile}")
-
 def main(args_in: list[str] | None = None) -> None:
     output_choices = ["f32", "f16"]
     if np.uint32(1) == np.uint32(1).newbyteorder("<"):
         # We currently only support Q8_0 output on little endian systems.
         output_choices.append("q8_0")
     parser = argparse.ArgumentParser(description="Convert a LLaMA model to a GGML compatible file")
     parser.add_argument("--dump",         action="store_true",    help="don't convert, just show what's in the model")
     parser.add_argument("--dump-single",  action="store_true",    help="don't convert, just show what's in a single model file")
     parser.add_argument("--vocab-only",   action="store_true",    help="extract only the vocab")
+    parser.add_argument("--no-vocab",     action="store_true",    help="store model without the vocab")
     parser.add_argument("--outtype",      choices=output_choices, help="output format - note: q8_0 may be very slow (default: f16 or f32 based on input)")
     parser.add_argument("--vocab-dir",    type=Path,              help="directory containing tokenizer.model, if separate from model file")
     parser.add_argument("--vocab-type",                           help="vocab types to try in order, choose from 'spm', 'bpe', 'hfft' (default: spm,hfft)", default="spm,hfft")
     parser.add_argument("--outfile",      type=Path,              help="path to write to; default: based on input")
     parser.add_argument("model",          type=Path,              help="directory containing model file, or model file itself (*.pth, *.pt, *.bin)")
     parser.add_argument("--ctx",          type=int,               help="model training context (default: based on input)")
     parser.add_argument("--concurrency",  type=int,               help=f"concurrency used for conversion (default: {DEFAULT_CONCURRENCY})", default=DEFAULT_CONCURRENCY)
     parser.add_argument("--big-endian",   action="store_true",    help="model is executed on big endian machine")
     parser.add_argument("--pad-vocab",    action="store_true",    help="add pad tokens when model vocab expects more than tokenizer metadata provides")
     parser.add_argument("--skip-unknown", action="store_true",    help="skip unknown tensor names instead of failing")
 
     args = parser.parse_args(args_in)
+    if args.no_vocab and args.vocab_only:
+        raise ValueError("--vocab-only does not make sense with --no-vocab")
 
     if args.dump_single:
         model_plus = lazy_load_file(args.model)
         do_dump_model(model_plus)
         return
 
     if not args.vocab_only:
@@ -1463,44 +1486,48 @@
     endianess = gguf.GGUFEndian.LITTLE
     if args.big_endian:
         endianess = gguf.GGUFEndian.BIG
 
     params = Params.load(model_plus)
     if params.n_ctx == -1:
         if args.ctx is None:
-            raise Exception("The model doesn't have a context size, and you didn't specify one with --ctx\n"
-                            "Please specify one with --ctx:\n"
-                            " - LLaMA v1: --ctx 2048\n"
-                            " - LLaMA v2: --ctx 4096\n")
+            msg = """\
+                The model doesn't have a context size, and you didn't specify one with --ctx
+                Please specify one with --ctx:
+                 - LLaMA v1: --ctx 2048
+                 - LLaMA v2: --ctx 4096"""
+            parser.error(textwrap.dedent(msg))
         params.n_ctx = args.ctx
 
     if args.outtype:
         params.ftype = {
             "f32": GGMLFileType.AllF32,
             "f16": GGMLFileType.MostlyF16,
             "q8_0": GGMLFileType.MostlyQ8_0,
         }[args.outtype]
 
     print(f"params = {params}")
 
     model_parent_path = model_plus.paths[0].parent
     vocab_path = Path(args.vocab_dir or args.model or model_parent_path)
     vocab_factory = VocabFactory(vocab_path)
-    vocab, special_vocab = vocab_factory.load_vocab(args.vocab_type.split(","), model_parent_path)
+    vocab_types = None if args.no_vocab else args.vocab_type.split(",")
+    vocab, special_vocab = vocab_factory.load_vocab(vocab_types, model_parent_path)
 
     if args.vocab_only:
+        assert isinstance(vocab, Vocab)
         if not args.outfile:
             raise ValueError("need --outfile if using --vocab-only")
         outfile = args.outfile
         OutputFile.write_vocab_only(outfile, params, vocab, special_vocab,
                                     endianess=endianess, pad_vocab=args.pad_vocab)
         print(f"Wrote {outfile}")
         return
 
-    if model_plus.vocab is not None and args.vocab_dir is None:
+    if model_plus.vocab is not None and args.vocab_dir is None and not args.no_vocab:
         vocab = model_plus.vocab
 
     print(f"Vocab info: {vocab}")
     print(f"Special vocab info: {special_vocab}")
 
     model   = model_plus.model
     model   = convert_model_names(model, params, args.skip_unknown)
@@ -1514,7 +1541,62 @@
     OutputFile.write_all(outfile, ftype, params, model, vocab, special_vocab,
                          concurrency=args.concurrency, endianess=endianess, pad_vocab=args.pad_vocab)
     print(f"Wrote {outfile}")
 
 
 if __name__ == '__main__':
     main()
+
+def do_gguf_conversion(model: str, output: str, out_type: str, vocab_dir: str, vocab_type: str, context: int, pad_vocab: bool, concurrency: bool, big_endian: bool) -> None:
+    model_plus = load_some_model(model)
+
+    endianess = gguf.GGUFEndian.LITTLE
+    if big_endian:
+        endianess = gguf.GGUFEndian.BIG
+    print(f"endianess = {endianess}")
+
+    params = Params.load(model_plus)
+
+    if params.n_ctx == -1:
+        if context is None:
+            context = 4096
+        params.n_ctx = context
+    print(f"context = {context}")
+
+    if out_type is not None:
+        params.ftype = {
+            "f32": GGMLFileType.AllF32,
+            "f16": GGMLFileType.MostlyF16,
+            "q8_0": GGMLFileType.MostlyQ8_0,
+        }[out_type]
+
+    print(f"params = {params}")
+
+    model_parent_path = model_plus.paths[0].parent
+
+    if vocab_dir is not None:
+        vocab_path = Path(vocab_dir)
+    else:
+        vocab_path = Path(model or model_parent_path)
+
+    vocab_factory = VocabFactory(vocab_path)
+    vocab_types = vocab_type.split(",")
+    vocab, special_vocab = vocab_factory.load_vocab(vocab_types, model_parent_path)
+
+    if model_plus.vocab is not None and vocab_dir is None:
+        vocab = model_plus.vocab
+
+    print(f"Vocab info: {vocab}")
+    print(f"Special vocab info: {special_vocab}")
+
+    model   = model_plus.model
+    model   = convert_model_names(model, params, True) #skip_unknown
+    ftype   = pick_output_type(model, out_type)
+    model   = convert_to_output_type(model, ftype)
+    outfile = output or default_outfile(model_plus.paths, ftype)
+
+    params.ftype = ftype
+    print(f"Writing {outfile}, format {ftype}")
+
+    OutputFile.write_all(output, ftype, params, model, vocab, special_vocab,
+                         concurrency=concurrency, endianess=endianess, pad_vocab=pad_vocab)
+    print(f"Wrote {outfile}")
```

### Comparing `llm-quantkit-0.23/quantkit/quantkit.py` & `llm-quantkit-0.24/quantkit/quantkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     if output is None:
         model_dir = model.split("/")[1]
         path = Path(model_dir)
     else:
         path = Path(output)
 
     from huggingface_hub import snapshot_download
-    snapshot_download(model, local_dir=path, local_dir_use_symlinks=hf_cache, force_download=force_download, resume_download=resume_download, ignore_patterns='pytorch_model*' if safetensors_only else None)
+    snapshot_download(model, local_dir=path, local_dir_use_symlinks=hf_cache, force_download=force_download, resume_download=resume_download, ignore_patterns=['pytorch_model*', 'consolidated*.pt'] if safetensors_only else None)
 
 def run_safetensor(model, delete_original):
     path = Path(model)
     if path.is_dir():
         if Path(path / "config.json").is_file():
             # convert
             convert_multi(model, del_pytorch_model=delete_original)
```

### Comparing `llm-quantkit-0.23/quantkit/safetensor.py` & `llm-quantkit-0.24/quantkit/safetensor.py`

 * *Files identical despite different names*

