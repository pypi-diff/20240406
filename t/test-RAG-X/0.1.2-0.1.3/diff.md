# Comparing `tmp/test_RAG_X-0.1.2.tar.gz` & `tmp/test_RAG_X-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_RAG_X-0.1.2.tar", last modified: Fri Apr  5 11:09:18 2024, max compression
+gzip compressed data, was "test_RAG_X-0.1.3.tar", last modified: Sat Apr  6 04:58:19 2024, max compression
```

## Comparing `test_RAG_X-0.1.2.tar` & `test_RAG_X-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ankitbaliyan   (501) staff       (20)        0 2024-04-05 11:09:18.350726 test_RAG_X-0.1.2/
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     1073 2024-04-02 17:20:52.000000 test_RAG_X-0.1.2/LICENSE
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     2785 2024-04-05 11:09:18.350127 test_RAG_X-0.1.2/PKG-INFO
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     1952 2024-04-05 11:08:52.000000 test_RAG_X-0.1.2/README.md
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)       38 2024-04-05 11:09:18.350816 test_RAG_X-0.1.2/setup.cfg
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     1644 2024-04-05 11:06:29.000000 test_RAG_X-0.1.2/setup.py
-drwxr-xr-x   0 ankitbaliyan   (501) staff       (20)        0 2024-04-05 11:09:18.347437 test_RAG_X-0.1.2/test_RAG_X/
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)        0 2024-04-03 14:43:42.000000 test_RAG_X-0.1.2/test_RAG_X/__init__.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     4877 2024-04-03 06:18:19.000000 test_RAG_X-0.1.2/test_RAG_X/chunk_it.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     1868 2024-04-02 15:58:56.000000 test_RAG_X-0.1.2/test_RAG_X/clean_it.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)      919 2024-04-02 15:58:21.000000 test_RAG_X-0.1.2/test_RAG_X/extractor.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     5596 2024-04-01 11:46:39.000000 test_RAG_X-0.1.2/test_RAG_X/get_evaluation_question.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     5563 2024-04-05 10:32:10.000000 test_RAG_X-0.1.2/test_RAG_X/prag.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     5440 2024-04-02 16:09:16.000000 test_RAG_X-0.1.2/test_RAG_X/trulens.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     4129 2024-04-02 15:32:42.000000 test_RAG_X-0.1.2/test_RAG_X/utils.py
-drwxr-xr-x   0 ankitbaliyan   (501) staff       (20)        0 2024-04-05 11:09:18.349547 test_RAG_X-0.1.2/test_RAG_X.egg-info/
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     2785 2024-04-05 11:09:18.000000 test_RAG_X-0.1.2/test_RAG_X.egg-info/PKG-INFO
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)      387 2024-04-05 11:09:18.000000 test_RAG_X-0.1.2/test_RAG_X.egg-info/SOURCES.txt
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)        1 2024-04-05 11:09:18.000000 test_RAG_X-0.1.2/test_RAG_X.egg-info/dependency_links.txt
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)      135 2024-04-05 11:09:18.000000 test_RAG_X-0.1.2/test_RAG_X.egg-info/requires.txt
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)       11 2024-04-05 11:09:18.000000 test_RAG_X-0.1.2/test_RAG_X.egg-info/top_level.txt
+drwxr-xr-x   0 ankitbaliyan   (501) staff       (20)        0 2024-04-06 04:58:19.569289 test_RAG_X-0.1.3/
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)     1073 2024-04-02 17:20:52.000000 test_RAG_X-0.1.3/LICENSE
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)     3769 2024-04-06 04:58:19.568934 test_RAG_X-0.1.3/PKG-INFO
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)     2936 2024-04-06 04:46:14.000000 test_RAG_X-0.1.3/README.md
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)       38 2024-04-06 04:58:19.569370 test_RAG_X-0.1.3/setup.cfg
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)     1644 2024-04-06 04:47:48.000000 test_RAG_X-0.1.3/setup.py
+drwxr-xr-x   0 ankitbaliyan   (501) staff       (20)        0 2024-04-06 04:58:19.567473 test_RAG_X-0.1.3/test_RAG_X/
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)        0 2024-04-03 14:43:42.000000 test_RAG_X-0.1.3/test_RAG_X/__init__.py
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)     4885 2024-04-06 04:55:59.000000 test_RAG_X-0.1.3/test_RAG_X/chunk_it.py
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)     1868 2024-04-02 15:58:56.000000 test_RAG_X-0.1.3/test_RAG_X/clean_it.py
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)      919 2024-04-02 15:58:21.000000 test_RAG_X-0.1.3/test_RAG_X/extractor.py
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)     5596 2024-04-01 11:46:39.000000 test_RAG_X-0.1.3/test_RAG_X/get_evaluation_question.py
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)     5617 2024-04-06 04:55:36.000000 test_RAG_X-0.1.3/test_RAG_X/prag.py
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)     5440 2024-04-02 16:09:16.000000 test_RAG_X-0.1.3/test_RAG_X/trulens.py
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)     3686 2024-04-06 04:56:53.000000 test_RAG_X-0.1.3/test_RAG_X/utils.py
+drwxr-xr-x   0 ankitbaliyan   (501) staff       (20)        0 2024-04-06 04:58:19.568542 test_RAG_X-0.1.3/test_RAG_X.egg-info/
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)     3769 2024-04-06 04:58:19.000000 test_RAG_X-0.1.3/test_RAG_X.egg-info/PKG-INFO
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)      387 2024-04-06 04:58:19.000000 test_RAG_X-0.1.3/test_RAG_X.egg-info/SOURCES.txt
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)        1 2024-04-06 04:58:19.000000 test_RAG_X-0.1.3/test_RAG_X.egg-info/dependency_links.txt
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)      135 2024-04-06 04:58:19.000000 test_RAG_X-0.1.3/test_RAG_X.egg-info/requires.txt
+-rw-r--r--   0 ankitbaliyan   (501) staff       (20)       11 2024-04-06 04:58:19.000000 test_RAG_X-0.1.3/test_RAG_X.egg-info/top_level.txt
```

### Comparing `test_RAG_X-0.1.2/LICENSE` & `test_RAG_X-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `test_RAG_X-0.1.2/PKG-INFO` & `test_RAG_X-0.1.3/test_RAG_X.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: test_RAG_X
-Version: 0.1.2
+Name: test-RAG-X
+Version: 0.1.3
 Summary: This library is to search the best parameters across different steps of the RAG process.
 Home-page: https://github.com/hidevscommunity/gen-ai-library/tree/main/Ankit
 Author: Ankit
 Author-email: a.baliyan008@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -47,31 +47,31 @@
 ```bash
 pip install test-RAG-X
 ```
 
 To verify the installation and view library details, execute:
 
 ```bash
-pip show RAG-X
+pip show test_RAG_X
 ```
 
 ### Setting Up Your Environment
 
-Before diving into the functionality of RAG-X, ensure that your environment variables are properly configured with your OpenAI API key and your Hugging Face token:
+Before diving into the functionality of test-RAG-X, ensure that your environment variables are properly configured with your OpenAI API key and your Hugging Face token:
 
 ```python
 import os
 
 os.environ['OPENAI_API_KEY'] = "YOUR_OPENAI_API_KEY"
 os.environ['HF_TOKEN'] = "YOUR_HUGGINGFACE_TOKEN"
 ```
 
 ## Usage
 
-The following steps guide you through the process of utilizing the RAG-X library to optimize your RAG parameters:
+The following steps guide you through the process of utilizing the test-RAG-X library to optimize your RAG parameters:
 
 ```python
 from test_RAG_X.prag import parent_class
 
 # Specify the path to your PDF document
 file_path = "PATH_TO_YOUR_PDF_FILE"
 
@@ -81,7 +81,34 @@
 # Generate the optimal RAG parameters for your document
 score_card = my_instance.get_best_param()
 
 # Output the results
 print(score_card)
 ```
 
+
+## Set parameters
+
+If you wish to analyse the performance of your parameters, you can pass the parameters as below:
+```python
+kwarg = {
+        'number_of_questions': 5, # Number of questions: type(int)
+        'chunk_size': 250, # Chunk size: type(int)
+        'chunk_overlap': 0, # Chunk overlap size: type(int)
+        'separator': '',  # Separator to be used for chunking if any, type(str)
+        'strip_whitespace': False, # Strip white space, type(bool)
+        'sentence_buffer_window': 3, # Sentence Buffer window, type(int) 
+        'sentence_cutoff_percentile': 80, # Sentence chunk split percentile for spliting context, type(int), range(1,100)
+        }
+
+# Specify the path to your PDF document
+file_path = "PATH_TO_YOUR_PDF_FILE"
+
+# Initialize the RAG-X instance
+my_instance = parent_class(file_path, **kwargs)
+
+# Generate the optimal RAG parameters for your document
+score_card = my_instance.get_best_param()
+
+# Output the results
+print(score_card)
+```
```

### Comparing `test_RAG_X-0.1.2/README.md` & `test_RAG_X-0.1.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -25,31 +25,31 @@
 ```bash
 pip install test-RAG-X
 ```
 
 To verify the installation and view library details, execute:
 
 ```bash
-pip show RAG-X
+pip show test_RAG_X
 ```
 
 ### Setting Up Your Environment
 
-Before diving into the functionality of RAG-X, ensure that your environment variables are properly configured with your OpenAI API key and your Hugging Face token:
+Before diving into the functionality of test-RAG-X, ensure that your environment variables are properly configured with your OpenAI API key and your Hugging Face token:
 
 ```python
 import os
 
 os.environ['OPENAI_API_KEY'] = "YOUR_OPENAI_API_KEY"
 os.environ['HF_TOKEN'] = "YOUR_HUGGINGFACE_TOKEN"
 ```
 
 ## Usage
 
-The following steps guide you through the process of utilizing the RAG-X library to optimize your RAG parameters:
+The following steps guide you through the process of utilizing the test-RAG-X library to optimize your RAG parameters:
 
 ```python
 from test_RAG_X.prag import parent_class
 
 # Specify the path to your PDF document
 file_path = "PATH_TO_YOUR_PDF_FILE"
 
@@ -59,7 +59,34 @@
 # Generate the optimal RAG parameters for your document
 score_card = my_instance.get_best_param()
 
 # Output the results
 print(score_card)
 ```
 
+
+## Set parameters
+
+If you wish to analyse the performance of your parameters, you can pass the parameters as below:
+```python
+kwarg = {
+        'number_of_questions': 5, # Number of questions: type(int)
+        'chunk_size': 250, # Chunk size: type(int)
+        'chunk_overlap': 0, # Chunk overlap size: type(int)
+        'separator': '',  # Separator to be used for chunking if any, type(str)
+        'strip_whitespace': False, # Strip white space, type(bool)
+        'sentence_buffer_window': 3, # Sentence Buffer window, type(int) 
+        'sentence_cutoff_percentile': 80, # Sentence chunk split percentile for spliting context, type(int), range(1,100)
+        }
+
+# Specify the path to your PDF document
+file_path = "PATH_TO_YOUR_PDF_FILE"
+
+# Initialize the RAG-X instance
+my_instance = parent_class(file_path, **kwargs)
+
+# Generate the optimal RAG parameters for your document
+score_card = my_instance.get_best_param()
+
+# Output the results
+print(score_card)
+```
```

### Comparing `test_RAG_X-0.1.2/setup.py` & `test_RAG_X-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='test_RAG_X',
-    version='0.1.2', # all versions prior to launch will go into 0.0.1.--
+    version='0.1.3', # all versions prior to launch will go into 0.0.1.--
     packages=find_packages(),
     license='MIT',
     description='This library is to search the best parameters across different steps of the RAG process.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ankit',
     author_email='a.baliyan008@gmail.com',
```

### Comparing `test_RAG_X-0.1.2/test_RAG_X/chunk_it.py` & `test_RAG_X-0.1.3/test_RAG_X/chunk_it.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     # Chunking Method: 1
     def SimpleTextSplitter(self):
         """
         This function uses the CharacterTextSplitter from the langchain.text_splitter module to split the input text into chunks.
         The chunking parameters are taken from the parent instance.
         The function returns a list of chunks and a dictionary containing the chunking parameters.
         """
-        params = self.parent_instance.get_params()
+        params = self.parent_instance.reset_params()
         text_splitter = CharacterTextSplitter(chunk_size=self.parent_instance.chunk_size, 
                                               chunk_overlap=self.parent_instance.chunk_overlap, 
                                               separator=self.parent_instance.separator, 
                                               strip_whitespace=self.parent_instance.strip_whitespace)
         
         split_text = text_splitter.create_documents([self.clean_text])
         
@@ -38,30 +38,30 @@
     # Chunking Method: 2
     def RecursiveCharTextSplitter(self):
         """
         This function uses the RecursiveCharacterTextSplitter from the langchain.text_splitter module to split the input text into chunks.
         The chunking parameters are taken from the parent instance.
         The function returns a list of chunks and a dictionary containing the chunking parameters.
         """
-        params = self.parent_instance.get_params()
+        params = self.parent_instance.reset_params()
         text_splitter = RecursiveCharacterTextSplitter(chunk_size = self.parent_instance.chunk_size, chunk_overlap=self.parent_instance.chunk_overlap)
         split_text = text_splitter.create_documents([self.clean_text])
         params['chunk_size'] = self.parent_instance.chunk_size
         params['chunk_overlap'] = self.parent_instance.chunk_overlap
         
         return split_text, params
 
     # Chunking Method: 3
     def SentenseWindowSplitter(self):
         """
         This function takes the input text and splits it into chunks based on the sentence window buffer.
         The chunking parameters are taken from the parent instance.
         The function returns a list of chunks and a dictionary containing the chunking parameters.
         """
-        params = self.parent_instance.get_params()
+        params = self.parent_instance.reset_params()
         input_text = str(self.clean_text)
         single_sentences_list = re.split(r'(?<=[.?!])\s+', input_text)
         sentences = [{'sentence': x, 'index' : i} for i, x in enumerate(single_sentences_list)]
         sentences = combine_sentences(sentences, buffer_size=self.parent_instance.sentence_buffer_window)
         chunks=[]
         for i, sentence in enumerate(sentences):
           doc = Document(page_content=sentence['combined_sentence'], metadata={"source": f"chunk:{i}"})
@@ -74,15 +74,15 @@
     # Chunking Method: 4
     def SemanticSentenseSplitter(self):
       """
       This function takes the input text and splits it into semantically similar sentences using the OpenAI API.
       The chunking parameters are taken from the parent instance.
       The function returns a list of chunks and a dictionary containing the chunking parameters.
       """
-      params = self.parent_instance.get_params()
+      params = self.parent_instance.reset_params()
       input_text = str(self.clean_text)
       single_sentences_list = re.split(r'(?<=[.?!])\s+', input_text)
       sentences = [{'sentence': x, 'index' : i} for i, x in enumerate(single_sentences_list)]
       sentences = combine_sentences(sentences, buffer_size=self.parent_instance.sentence_buffer_window)
       oaiembeds = OpenAIEmbeddings()
       embeddings = oaiembeds.embed_documents([x['combined_sentence'] for x in sentences])
       for i, sentence in enumerate(sentences):
```

### Comparing `test_RAG_X-0.1.2/test_RAG_X/clean_it.py` & `test_RAG_X-0.1.3/test_RAG_X/clean_it.py`

 * *Files identical despite different names*

### Comparing `test_RAG_X-0.1.2/test_RAG_X/extractor.py` & `test_RAG_X-0.1.3/test_RAG_X/extractor.py`

 * *Files identical despite different names*

### Comparing `test_RAG_X-0.1.2/test_RAG_X/get_evaluation_question.py` & `test_RAG_X-0.1.3/test_RAG_X/get_evaluation_question.py`

 * *Files identical despite different names*

### Comparing `test_RAG_X-0.1.2/test_RAG_X/prag.py` & `test_RAG_X-0.1.3/test_RAG_X/prag.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from .trulens import *
 
 from dotenv import load_dotenv
 
 load_dotenv()
 
-class parent_class:
+class ChunkEvaluator:
     def __init__(self, file_path, **kwargs):
         expected_types = {
                 'number_of_questions': int,
                 'chunk_size': int, 
                 'chunk_overlap': int, 
                 'separator': str, 
                 'strip_whitespace': bool,
@@ -48,31 +48,29 @@
 
         def __str__(self):
             return self.text    
 
 
 
 
-    def get_params(self):
+    def reset_params(self):
         """
-        Returns a dictionary containing the parameters used in the chunking process.
-
-        This function reset all the parameters.
+        Resets all parameters to their default values.
         """
         return {
                 'chunk_size': '-', 
                 'chunk_overlap': '-', 
                 'separator': '-', 
                 'strip_whitespace': '-',
                 'sentence_buffer_window': '-',
                 'sentence_cutoff_percentile': '-',
             }
     
 
-    def eval_function(self, chunks, method_name, eval_questions):
+    def evaluate_chunk(self, chunks, method_name, eval_questions):
         """
         Evaluate the performance of a chunking method using the TruLens framework.
 
         Parameters
         ----------
         chunks : list of str
             The list of chunks to evaluate.
@@ -83,51 +81,53 @@
 
         Returns
         -------
         float
             The performance score (Padas DataFrame) of the chunking method.
 
         """
-        persist_directory="01_coding/crucible/db"
+        # persist_directory="01_coding/crucible/db"
         embedding_function = SentenceTransformerEmbeddings(model_name="sentence-transformers/all-MiniLM-l6-v2")
 
-        db = Chroma.from_documents(chunks, embedding_function, persist_directory=persist_directory)
+        # db = Chroma.from_documents(chunks, embedding_function, persist_directory=persist_directory)
+        db = Chroma.from_documents(chunks, embedding_function)
         score = trulens_evaluation(evalation_questions = eval_questions, 
                             vectorstore=db, chunking_type=method_name)
         return score
 
     
-    def get_best_param(self):
+    def find_best_params(self):
         """
         This function returns the best parameters for the chunking method based on the evaluation of the performance of the chunking method.
 
         Returns:
             pandas.DataFrame: The parameters summary for the chunking method based on the evaluation of the performance of the chunking method.
         """
         extractor_instance = DocumentExtractor(file_path=self.file_path)
         uncleaned_text = extractor_instance.extract_data()
 
         cleaner_instance = TextCleaner(uncleaned_text=uncleaned_text)
         cleaned_text = cleaner_instance.unstructured_text()
 
-        eval_questions = GenerateEvaluationQuestions(document=cleaned_text, number_of_questions=self.number_of_questions).get_evaluation_questions()
+        eval_questions_instance = GenerateEvaluationQuestions(document=cleaned_text, number_of_questions=self.number_of_questions)
+        eval_questions = eval_questions_instance.get_evaluation_questions()
 
         methods_list = [method for method in dir(Chunker)
                 if callable(getattr(Chunker, method)) and not method.startswith('__')]
         
         chunk_instance = Chunker(clean_text=cleaned_text, parent_instance=self)
 
         method_eval_score = []
         for method_name in methods_list:
             print(method_name)
             method = getattr(chunk_instance, method_name, None)  
             if method:
                 chunks, params = method()
                 
-                model_results = self.eval_function(chunks=chunks, method_name=method_name, eval_questions=eval_questions)
+                model_results = self.evaluate_chunk(chunks=chunks, method_name=method_name, eval_questions=eval_questions)
                 params_df = pd.DataFrame([params])
                 repeated_params_df = pd.concat([params_df] * len(model_results), ignore_index=True)
 
                 out = pd.concat([model_results, repeated_params_df], axis=1)
                 method_eval_score.append(out)
```

### Comparing `test_RAG_X-0.1.2/test_RAG_X/trulens.py` & `test_RAG_X-0.1.3/test_RAG_X/trulens.py`

 * *Files identical despite different names*

### Comparing `test_RAG_X-0.1.2/test_RAG_X/utils.py` & `test_RAG_X-0.1.3/test_RAG_X/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,26 +95,7 @@
     chunks_doc = []
     for i, chunk in enumerate(chunks):
       doc = Document(page_content=chunk, metadata={"source": f"chunk:{i}"})
       chunks_doc.append(doc)
 
     return chunks_doc
 
-
-
-
-from langchain_community.embeddings import HuggingFaceInferenceAPIEmbeddings
-
-
-def create_embeddings(chunks):
-  embedding_function = HuggingFaceInferenceAPIEmbeddings(
-        api_key=os.environ["HF_TOKEN"], model_name="sentence-transformers/all-MiniLM-l6-v2"
-    )
-  chunk_embeddings = []
-
-  for chunk in chunks:
-    chunk_embed = embedding_function.embed_query(chunk)
-    chunk_embeddings.append(chunk_embed)
-
-  return chunk_embeddings
-
-
```

### Comparing `test_RAG_X-0.1.2/test_RAG_X.egg-info/PKG-INFO` & `test_RAG_X-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_RAG_X
-Version: 0.1.2
+Version: 0.1.3
 Summary: This library is to search the best parameters across different steps of the RAG process.
 Home-page: https://github.com/hidevscommunity/gen-ai-library/tree/main/Ankit
 Author: Ankit
 Author-email: a.baliyan008@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -47,31 +47,31 @@
 ```bash
 pip install test-RAG-X
 ```
 
 To verify the installation and view library details, execute:
 
 ```bash
-pip show RAG-X
+pip show test_RAG_X
 ```
 
 ### Setting Up Your Environment
 
-Before diving into the functionality of RAG-X, ensure that your environment variables are properly configured with your OpenAI API key and your Hugging Face token:
+Before diving into the functionality of test-RAG-X, ensure that your environment variables are properly configured with your OpenAI API key and your Hugging Face token:
 
 ```python
 import os
 
 os.environ['OPENAI_API_KEY'] = "YOUR_OPENAI_API_KEY"
 os.environ['HF_TOKEN'] = "YOUR_HUGGINGFACE_TOKEN"
 ```
 
 ## Usage
 
-The following steps guide you through the process of utilizing the RAG-X library to optimize your RAG parameters:
+The following steps guide you through the process of utilizing the test-RAG-X library to optimize your RAG parameters:
 
 ```python
 from test_RAG_X.prag import parent_class
 
 # Specify the path to your PDF document
 file_path = "PATH_TO_YOUR_PDF_FILE"
 
@@ -81,7 +81,34 @@
 # Generate the optimal RAG parameters for your document
 score_card = my_instance.get_best_param()
 
 # Output the results
 print(score_card)
 ```
 
+
+## Set parameters
+
+If you wish to analyse the performance of your parameters, you can pass the parameters as below:
+```python
+kwarg = {
+        'number_of_questions': 5, # Number of questions: type(int)
+        'chunk_size': 250, # Chunk size: type(int)
+        'chunk_overlap': 0, # Chunk overlap size: type(int)
+        'separator': '',  # Separator to be used for chunking if any, type(str)
+        'strip_whitespace': False, # Strip white space, type(bool)
+        'sentence_buffer_window': 3, # Sentence Buffer window, type(int) 
+        'sentence_cutoff_percentile': 80, # Sentence chunk split percentile for spliting context, type(int), range(1,100)
+        }
+
+# Specify the path to your PDF document
+file_path = "PATH_TO_YOUR_PDF_FILE"
+
+# Initialize the RAG-X instance
+my_instance = parent_class(file_path, **kwargs)
+
+# Generate the optimal RAG parameters for your document
+score_card = my_instance.get_best_param()
+
+# Output the results
+print(score_card)
+```
```

