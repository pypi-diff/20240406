# Comparing `tmp/Information_Retrieval-1.0.tar.gz` & `tmp/Information_Retrieval-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Information_Retrieval-1.0.tar", last modified: Sat Mar 30 15:56:17 2024, max compression
+gzip compressed data, was "Information_Retrieval-2.0.tar", last modified: Fri Apr  5 15:43:30 2024, max compression
```

## Comparing `Information_Retrieval-1.0.tar` & `Information_Retrieval-2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kushpai    (501) staff       (20)        0 2024-03-30 15:56:17.646221 Information_Retrieval-1.0/
-drwxr-xr-x   0 kushpai    (501) staff       (20)        0 2024-03-30 15:56:17.645159 Information_Retrieval-1.0/Information_Retrieval/
--rw-r--r--   0 kushpai    (501) staff       (20)      500 2024-03-30 15:55:33.000000 Information_Retrieval-1.0/Information_Retrieval/__init__.py
--rw-r--r--   0 kushpai    (501) staff       (20)    10502 2024-03-30 15:55:26.000000 Information_Retrieval-1.0/Information_Retrieval/main.py
-drwxr-xr-x   0 kushpai    (501) staff       (20)        0 2024-03-30 15:56:17.645885 Information_Retrieval-1.0/Information_Retrieval.egg-info/
--rw-r--r--   0 kushpai    (501) staff       (20)      144 2024-03-30 15:56:17.000000 Information_Retrieval-1.0/Information_Retrieval.egg-info/PKG-INFO
--rw-r--r--   0 kushpai    (501) staff       (20)      300 2024-03-30 15:56:17.000000 Information_Retrieval-1.0/Information_Retrieval.egg-info/SOURCES.txt
--rw-r--r--   0 kushpai    (501) staff       (20)        1 2024-03-30 15:56:17.000000 Information_Retrieval-1.0/Information_Retrieval.egg-info/dependency_links.txt
--rw-r--r--   0 kushpai    (501) staff       (20)       55 2024-03-30 15:56:17.000000 Information_Retrieval-1.0/Information_Retrieval.egg-info/entry_points.txt
--rw-r--r--   0 kushpai    (501) staff       (20)       22 2024-03-30 15:56:17.000000 Information_Retrieval-1.0/Information_Retrieval.egg-info/top_level.txt
--rw-r--r--   0 kushpai    (501) staff       (20)      144 2024-03-30 15:56:17.646050 Information_Retrieval-1.0/PKG-INFO
--rw-r--r--   0 kushpai    (501) staff       (20)       38 2024-03-30 15:56:17.646281 Information_Retrieval-1.0/setup.cfg
--rw-r--r--   0 kushpai    (501) staff       (20)      317 2024-03-30 15:55:38.000000 Information_Retrieval-1.0/setup.py
+drwxr-xr-x   0 kushpai    (501) staff       (20)        0 2024-04-05 15:43:30.400295 Information_Retrieval-2.0/
+drwxr-xr-x   0 kushpai    (501) staff       (20)        0 2024-04-05 15:43:30.399228 Information_Retrieval-2.0/Information_Retrieval/
+-rw-r--r--   0 kushpai    (501) staff       (20)      602 2024-04-05 15:38:46.000000 Information_Retrieval-2.0/Information_Retrieval/__init__.py
+-rw-r--r--   0 kushpai    (501) staff       (20)    14040 2024-04-05 15:43:14.000000 Information_Retrieval-2.0/Information_Retrieval/main.py
+drwxr-xr-x   0 kushpai    (501) staff       (20)        0 2024-04-05 15:43:30.399966 Information_Retrieval-2.0/Information_Retrieval.egg-info/
+-rw-r--r--   0 kushpai    (501) staff       (20)      144 2024-04-05 15:43:30.000000 Information_Retrieval-2.0/Information_Retrieval.egg-info/PKG-INFO
+-rw-r--r--   0 kushpai    (501) staff       (20)      300 2024-04-05 15:43:30.000000 Information_Retrieval-2.0/Information_Retrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 kushpai    (501) staff       (20)        1 2024-04-05 15:43:30.000000 Information_Retrieval-2.0/Information_Retrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 kushpai    (501) staff       (20)       55 2024-04-05 15:43:30.000000 Information_Retrieval-2.0/Information_Retrieval.egg-info/entry_points.txt
+-rw-r--r--   0 kushpai    (501) staff       (20)       22 2024-04-05 15:43:30.000000 Information_Retrieval-2.0/Information_Retrieval.egg-info/top_level.txt
+-rw-r--r--   0 kushpai    (501) staff       (20)      144 2024-04-05 15:43:30.400119 Information_Retrieval-2.0/PKG-INFO
+-rw-r--r--   0 kushpai    (501) staff       (20)       38 2024-04-05 15:43:30.400362 Information_Retrieval-2.0/setup.cfg
+-rw-r--r--   0 kushpai    (501) staff       (20)      317 2024-04-05 15:43:24.000000 Information_Retrieval-2.0/setup.py
```

### Comparing `Information_Retrieval-1.0/Information_Retrieval/main.py` & `Information_Retrieval-2.0/Information_Retrieval/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,123 @@
 def hello():
     print("Hello World!!!")
 
 
 
 
 
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 # Stop Word
 import nltk
 import re
 from nltk.corpus import stopwords
 
 nltk.download('stopwords')
  
 def Stop_Word_Removal_Code(filename):
-    with open(filename, 'r') as file:
-        data = file.read()
- 
-    clean_data = re.sub(r'[^\w\s]', '', data).lower()
- 
+    with open(filename, 'r', encoding='UTF-8') as file:
+        data = file.read().lower()
+
+    clean_data = re.sub(r'[^\w\s]', '', data)
+
     clean_data_list = clean_data.split()
- 
-    clean_data_list = [word for word in clean_data_list if word not in stopwords.words('english')]
+
+    clean_data_list = sorted([word for word in clean_data_list if word not in stopwords.words('english')])
 
     return clean_data_list
 
 
 
 
 
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 # Incident Matrix
 from collections import OrderedDict
 
 import sys
 sys.path.insert(1, 'P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1')
 
 def Incident_Matrix_Creation_Code(documents):
-    def Add_Words(dict_incident_matrix, *lists):
-        for lst in lists:
-            for word in lst:
-                if word not in dict_incident_matrix:
-                    presense = [0] * len(lists)
-                else:
-                    dict_incident_matrix[word]
-    
-                presense[lists.index(lst)] = 1
-                dict_incident_matrix[word] = presense
-    
-        return dict_incident_matrix
-
-    documents_n = []
-    for file in documents:
-        documents_n.append(Stop_Word_Removal_Code(file))
-
-    dict_incident_matrix = Add_Words({}, *documents_n)
-
-    sorted_dict_incident_matrix = OrderedDict(sorted(dict_incident_matrix.items()))
-
-    header = "Word".ljust(20)
-    for i in range(1, len(documents_n) + 1):
-        header += f"{'Document ' + str(i): <20}"
-
-    print(header, end="\n\n")
-
-    for word, presence in sorted_dict_incident_matrix.items():
-        output = word.ljust(20)
-        for i in range(len(documents_n)):
-            output += f"{presence[i]: <20}"
-        print(output)
+    document_n = []
+    for doc in documents:
+        document_n.append(Stop_Word_Removal_Code(doc))
+
+    merged_documents = []
+    for doc in document_n:
+        merged_documents = sorted(list(set(merged_documents).union(set(doc))))
+
+    Incident_Matrix = []
+    for word in merged_documents:
+        flag = []
+        
+        for i in range(len(document_n)):
+            if word in document_n[i]:
+                flag.append(1)
+            else:
+                flag.append(0)
+
+        Incident_Matrix.append([word] + flag + [' ', ' ', ' ', ' ', ' ', ' ', ' '])
 
-    return sorted_dict_incident_matrix
+    for word in Incident_Matrix:
+        print(f'{word[0]: <20}\t{word[1]}\t{word[2]}\t{word[3]}\t{word[4]}\t{word[5]}\t{word[6]}\t{word[7]}')
+        
+    print('\n\n')
 
 
 # Add document paths
 # print(Incident_Matrix_Creation_Code([
 #     'P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_1.txt',
 #     'P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_2.txt',
 #     'P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_3.txt',
@@ -80,14 +125,38 @@
 #     ]))
 
 
 
 
 
 
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 # Query Resolver
 documents = [
     'P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_1.txt',
     'P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_2.txt',
     'P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_3.txt',
     'P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_4.txt'
     ]
@@ -118,40 +187,64 @@
     int_bin2 = int(bin2, 2)
 
     result = int_bin1 | int_bin2
 
     return bin(result)[2:].zfill(len(documents))
 
 
-query = str(input("Enter query : "))
-query_list = query.split(' ')
+query = str(input('Enter a query : '))
+query_list = query.upper().split()
+
+print(query)
+print(query_list)
+
+for i in range(len(query_list)):
+    if query_list[i] == 'NOT':
+        query_list[i+1] = flip_bits(query_list[i+1])
+
+print(query_list)
+
+for entry in query_list:
+    if entry == 'NOT':
+        query_list.remove(entry)
+
+print(query_list)
+
+for i in range(1, len(query_list), 2):
+    if query_list[i] == 'AND':
+        query_list[i+1] = bitwise_and(query_list[i-1], query_list[i+1])
+    elif query_list[i] == 'OR':
+        query_list[i+1] = bitwise_or(query_list[i-1], query_list[i+1])
+
+print(query_list)
+print(query_list[-1])
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 
-for i in range(0, len(query_list)):
-    if query_list[i] != "AND" and query_list[i] != "OR" and query_list[i] != "NOT":
-        query_list[i] = ''.join(map(str, sorted_dict_incident_matrix[query_list[i]]))
 
-for i in range(0, len(query_list)):
-    if query_list[i] == "NOT":
-        query_list[i + 1] = flip_bits(query_list[i + 1])
 
-query_list = [x for x in query_list if x != "NOT"]
 
-result = ''
 
-for i in range (1, len(query_list), 2):
-    if query_list[i] == "AND":
-        result = bitwise_and(query_list[i-1], query_list[i+1])
-    elif query_list[i] == "OR":
-        result = bitwise_or(query_list[i-1], query_list[i+1])
 
-result_list = [*result]
 
-for i in range(len(result_list)):
-    if result_list[i] == '1':
-        print(f'File is present in File {i + 1}')
 
 
 
 
 
 # K-gram
 def K_Gram_Code():
@@ -171,106 +264,301 @@
 
     print(output)
 
 
 
 
 
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+# Crawler
+import requests
+from bs4 import BeautifulSoup
+from urllib.parse import urljoin
+
+def Crawler(url):
+    response = requests.get(url)
+    soup = BeautifulSoup(response.text, 'html.parser')
+
+    text = soup.get_text(' ')
+    images = soup.find_all('img')
+    links = soup.find_all('a')
+
+    print(text)
+    print('\n\n\n')
+
+    for image in images:
+        crawled_image = image.get('src')
+        print(crawled_image, end='\n')
+
+    print('\n\n\n')
+
+    for link in links:
+        crawled_link = link.get('href')
+        absolute_link = urljoin(url, crawled_link)
+        print(absolute_link, end='\n')
+
+url = 'https://unsplash.com'
+Crawler(url)
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 # Edit Distance
 def Edit_Distance_Code():
-    def compute_edit_distance(s1, s2):
-        len_s1 = len(s1)
-        len_s2 = len(s2)
+    def Edit_Distance(word1, word2):
+        edit_matrix = []
+        word1_list = [*word_1]
+        word2_list = [*word_2]
+
+        for i in range(len(word1) + 1):
+            mat = []
+            for j in range(len(word2) + 1):
+                mat.append(i+j)
+            edit_matrix.append(mat)
+
+        for i in range (1, len(edit_matrix)):
+            for j in range(1, len(edit_matrix[i])):
+                if word1_list[i-1] == word2_list[j-1]:
+                    edit_matrix[i][j] = min((edit_matrix[i-1][j] + 1), (edit_matrix[i-1][j-1]), (edit_matrix[i][j-1] + 1))
+                elif word1_list[i-1] != word2_list[j-1]:
+                    edit_matrix[i][j] = min((edit_matrix[i-1][j] + 1), (edit_matrix[i-1][j-1] + 1), (edit_matrix[i][j-1] + 1))
+
+        return edit_matrix[-1][-1]
+
+
+    word_1 = 'ALICE'
+    word_2 = 'PARIS'
+
+    edit_distance = Edit_Distance(word_1, word_2)
+
+    print(f'\nThe edit distance between {word_1} and {word_2} is {edit_distance}')
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 
-        matrix = [[0 for _ in range(len_s1 + 1)] for _ in range(len_s2 + 1)]
 
-        for i in range(len_s1 + 1):
-            matrix[0][i] = i
 
-        for i in range(len_s2 + 1):
-            matrix[i][0] = i
 
-        for i in range(1, len_s2 + 1):
-            for j in range(1, len_s1 + 1):
-                if s1[j - 1] == s2[i - 1]:
-                    matrix[i][j] = matrix[i - 1][j - 1]
-                else:
-                    matrix[i][j] = min(matrix[i - 1][j], matrix[i][j - 1], matrix[i - 1][j - 1]) + 1
 
-        return matrix[len_s2][len_s1]
 
-    s1 = "ALICE"
-    s2 = "PARIS"
 
-    print(f"\n\nThe edit distance between {s1} and {s2} is {compute_edit_distance(s1.upper(), s2.upper())}")
 
 
 
 
 
 # Cosine Similarity
 from sklearn.feature_extraction.text import TfidfVectorizer
+from sklearn.metrics.pairwise import cosine_similarity
+
+def Cosine_Similarity():
+    with open('Paragraph_1.txt', 'r', encoding='UTF-8') as file:
+        doc1 = file.read()
+
+    with open('Paragraph_2.txt', 'r', encoding='UTF-8') as file:
+        doc2 = file.read()
+
+    with open('Paragraph_3.txt', 'r', encoding='UTF-8') as file:
+        doc3 = file.read()
+
+    with open('Paragraph_4.txt', 'r', encoding='UTF-8') as file:
+        doc4 = file.read()
+
+    with open('Paragraph_5.txt', 'r', encoding='UTF-8') as file:
+        doc5 = file.read()
+
+    vectorizer = TfidfVectorizer()
+
+    tfidf_matrix = vectorizer.fit_transform([doc1, doc2, doc3, doc4, doc5])
+
+    similarity_matrix = cosine_similarity(tfidf_matrix)
+
+    print('Similarity Matrix')
+    print(similarity_matrix)
+
+    for i in range(len(similarity_matrix)):
+        for j in range(len(similarity_matrix[i])):
+            if similarity_matrix[i][j] > 0.7 and similarity_matrix[i][j] < 0.9999999:
+                print(f'Documents {i} and {j} have cosine similarity of {similarity_matrix[i][j]}')
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+# Cosine Similarity 2
+from sklearn.feature_extraction.text import TfidfVectorizer
 import pandas as pd
 import numpy as np
 import nltk
 from nltk.corpus import stopwords
 from nltk.tokenize import word_tokenize
 
 nltk.download('stopwords')
 nltk.download('punkt')
 
-def cosine_similarity(v1, v2):
-    dot_product = np.dot(v1, v2)
-    nv1 = np.linalg.norm(v1)
-    nv2 = np.linalg.norm(v2)
-
-    if nv1 == 0 or nv2 == 0:
-        return 0
-    else:
-        return dot_product / (nv1 * nv2)
-
-def preprocess_text(text):
-    stop_words = set(stopwords.words('english'))
-    words = word_tokenize(text)
-    words = [word.lower() for word in words if word.isalnum() and word.lower() not in stop_words]
-    return ' '.join(words)
+def Cosine_Similarity_2():
+    def cosine_similarity(v1, v2):
+        dot_product = np.dot(v1, v2)
+        nv1 = np.linalg.norm(v1)
+        nv2 = np.linalg.norm(v2)
+
+        if nv1 == 0 or nv2 == 0:
+            return 0
+        else:
+            return dot_product / (nv1 * nv2)
+
+    def preprocess_text(text):
+        stop_words = set(stopwords.words('english'))
+        words = word_tokenize(text)
+        words = [word.lower() for word in words if word.isalnum() and word.lower() not in stop_words]
+        return ' '.join(words)
+
+    def compute_similarity(data):
+        vectorizer = TfidfVectorizer()
+        tfidf_matrix = vectorizer.fit_transform(data)
+
+        tf_array = tfidf_matrix.toarray()
+        tf_terms = vectorizer.get_feature_names_out()
+
+        df = pd.DataFrame(tf_array, columns=tf_terms)
+
+        arr = np.zeros((len(tf_array), len(tf_array)))
+
+        for i in range(len(arr)):
+            for j in range(len(arr)):
+                arr[i][j] = cosine_similarity(tf_array[i], tf_array[j])
+
+        df_arr = pd.DataFrame(arr)
+        print(df_arr, end="\n\n")
+
+        for i in range(len(df_arr)):
+            for j in range(i + 1, len(df_arr)):
+                if df_arr.iloc[i, j] > 0.7:
+                    print(f"Documents {i+1} and {j+1} have cosine similarity: {df_arr.iloc[i, j]}")
+
+    file_paths = [
+        "P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_1.txt",
+        "P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_2.txt",
+        "P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_3.txt",
+        "P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_4.txt",
+        "P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_5.txt"
+    ]
+    data = [preprocess_text(open(i, 'r').read()) for i in file_paths]
+
+    compute_similarity(data)
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 
-def compute_similarity(data):
-    vectorizer = TfidfVectorizer()
-    tfidf_matrix = vectorizer.fit_transform(data)
 
-    tf_array = tfidf_matrix.toarray()
-    tf_terms = vectorizer.get_feature_names_out()
 
-    df = pd.DataFrame(tf_array, columns=tf_terms)
 
-    arr = np.zeros((len(tf_array), len(tf_array)))
 
-    for i in range(len(arr)):
-        for j in range(len(arr)):
-            arr[i][j] = cosine_similarity(tf_array[i], tf_array[j])
 
-    df_arr = pd.DataFrame(arr)
-    print(df_arr, end="\n\n")
 
-    for i in range(len(df_arr)):
-        for j in range(i + 1, len(df_arr)):
-            if df_arr.iloc[i, j] > 0.7:
-                print(f"Documents {i+1} and {j+1} have cosine similarity: {df_arr.iloc[i, j]}")
 
-file_paths = [
-    "P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_1.txt",
-    "P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_2.txt",
-    "P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_3.txt",
-    "P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_4.txt",
-    "P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_1/Paragraph_5.txt"
-]
-data = [preprocess_text(open(i, 'r').read()) for i in file_paths]
 
-compute_similarity(data)
 
 
 
 
 
 # Soundex
 def Soundex_Code():
@@ -308,14 +596,38 @@
 
     print("Soundex key without consecutive duplicates and without '0':", new_soundex_word[:4])
 
 
 
 
 
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 # Page Rank
 import numpy as np 
 
 def Page_Rank_Code():
     mat = np.array([
         [1/3, 1/2, 0],
         [1/3, 0, 1/2],
@@ -344,14 +656,38 @@
         iteration += 1
         print(ini_mat)
 
 
 
 
 
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 # Porter Stemmer
 from nltk.stem import PorterStemmer
 
 def Porter_Stemmer_Code():
     porter = PorterStemmer()
 
     words = ["running", "flies", "agreed", "plastered", "motoring", "conflated", "hunger", "fluttering"]
@@ -360,14 +696,38 @@
         stemmed_word = porter.stem(word)
         print(f"{word} -> {stemmed_word}")
 
 
 
 
 
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 # Collaborative Filtering
 import csv
 import numpy as np
 from sklearn.metrics.pairwise import cosine_similarity
 
 def Collaborative_Filtering():
     matrix_file = 'P2_INFORMATION_RETRIEVAL/PRACTICAL/Practical_10/data.csv' 
@@ -409,8 +769,108 @@
 
     n = 9
 
     predicted_rating = ((matrix[max_1][n] * cosine_similarity_score[max_1]) +
                         (matrix[max_2][n] * cosine_similarity_score[max_2])) / (
                             cosine_similarity_score[max_1] + cosine_similarity_score[max_2])
 
+    print(f"The predicted rating is {round(predicted_rating, 3)}")
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+# Collaborative Cosine
+
+import pandas as pd
+from sklearn.metrics.pairwise import cosine_similarity
+
+def Collab_Cosine():
+    matrix_df = pd.read_csv('data.csv', header=None)
+
+    print(matrix_df)
+
+    cosine_similarities = cosine_similarity(matrix_df)
+    print(cosine_similarities)
+
+    max_similarities = cosine_similarities.max(axis=1)
+    most_similar_indices = max_similarities.argsort()[-2:][::-1]
+
+    index = 9
+    predicted_rating = (matrix_df.iloc[most_similar_indices[0], index] * max_similarities[most_similar_indices[0]] +
+                        matrix_df.iloc[most_similar_indices[1], index] * max_similarities[most_similar_indices[1]]) / (
+                            max_similarities[most_similar_indices[0]] + max_similarities[most_similar_indices[1]])
+
+    print(f"The predicted rating is {round(predicted_rating, 3)}")
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+# Colaborative Nearest
+def Collab_Nearest():
+    import pandas as pd
+    from sklearn.neighbors import NearestNeighbors
+    from sklearn.metrics.pairwise import cosine_similarity
+
+    matrix_df = pd.read_csv('data.csv', header=None)
+
+    nn_model = NearestNeighbors(n_neighbors=2, metric='cosine')
+
+    nn_model.fit(matrix_df)
+
+    distances, indices = nn_model.kneighbors(matrix_df)
+    cosine_similarities = cosine_similarity(matrix_df)
+
+    most_similar_indices = indices[:, 1]
+
+    index = 9 
+    predicted_rating = (matrix_df.iloc[most_similar_indices[0], index] + matrix_df.iloc[most_similar_indices[1], index]) / 2
+
     print(f"The predicted rating is {round(predicted_rating, 3)}")
```

