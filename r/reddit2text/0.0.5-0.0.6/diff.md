# Comparing `tmp/reddit2text-0.0.5.tar.gz` & `tmp/reddit2text-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit2text-0.0.5.tar", last modified: Sat Apr  6 18:57:03 2024, max compression
+gzip compressed data, was "reddit2text-0.0.6.tar", last modified: Sat Apr  6 20:59:46 2024, max compression
```

## Comparing `reddit2text-0.0.5.tar` & `reddit2text-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:57:03.766055 reddit2text-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 18:57:00.000000 reddit2text-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-06 18:57:03.766055 reddit2text-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-06 18:57:00.000000 reddit2text-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:57:03.762055 reddit2text-0.0.5/reddit2text/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-06 18:57:00.000000 reddit2text-0.0.5/reddit2text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-06 18:57:00.000000 reddit2text-0.0.5/reddit2text/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:57:03.766055 reddit2text-0.0.5/reddit2text.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-06 18:57:03.000000 reddit2text-0.0.5/reddit2text.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-06 18:57:03.000000 reddit2text-0.0.5/reddit2text.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:57:03.000000 reddit2text-0.0.5/reddit2text.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-06 18:57:03.000000 reddit2text-0.0.5/reddit2text.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 18:57:03.000000 reddit2text-0.0.5/reddit2text.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:57:03.766055 reddit2text-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-06 18:57:00.000000 reddit2text-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 20:59:46.787539 reddit2text-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-03-05 18:59:10.000000 reddit2text-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-06 20:59:46.787539 reddit2text-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2806 2024-04-06 20:46:04.000000 reddit2text-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 20:59:46.783539 reddit2text-0.0.6/reddit2text/
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-06 20:45:56.000000 reddit2text-0.0.6/reddit2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-04-06 20:45:56.000000 reddit2text-0.0.6/reddit2text/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 20:59:46.787539 reddit2text-0.0.6/reddit2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-06 20:59:46.000000 reddit2text-0.0.6/reddit2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      244 2024-04-06 20:59:46.000000 reddit2text-0.0.6/reddit2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 20:59:46.000000 reddit2text-0.0.6/reddit2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-06 20:59:46.000000 reddit2text-0.0.6/reddit2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-06 20:59:46.000000 reddit2text-0.0.6/reddit2text.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 20:59:46.787539 reddit2text-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-04-06 20:45:56.000000 reddit2text-0.0.6/setup.py
```

### Comparing `reddit2text-0.0.5/LICENSE` & `reddit2text-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit2text-0.0.5/PKG-INFO` & `reddit2text-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit2text
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convert Reddit posts to text
 Author: Nicholas Hansen-Feruch
 Author-email: nicholas.feruch@gmail.com
 Keywords: python,reddit,text conversion,reddit api,praw,reddit to text,reddit comments,social media analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `reddit2text-0.0.5/reddit2text/main.py` & `reddit2text-0.0.6/reddit2text/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,91 @@
 import praw
+from typing import Optional
 
-class Client:
+class Reddit2Text:
 	def __init__(
 		self,
 		client_id: str,
 		client_secret: str,
 		user_agent: str,
+		*,
+		max_comment_depth: Optional[int] = None,
+		comment_delim: str = "|",
+		save_output_to: Optional[str] = None
 	) -> None:
 		self.client_id = client_id
 		self.client_secret = client_secret
 		self.user_agent = user_agent
+		self.max_comment_depth = max_comment_depth
+		self.comment_delim = comment_delim
+		self.save_output_to = save_output_to
 
-		self.praw_reddit = praw.Reddit(
+		self._praw_reddit = praw.Reddit(
 			client_id=self.client_id,
 			client_secret=self.client_secret,
 			user_agent=self.user_agent,
 		)
 
-	def _process_comments(self, comments: praw.models.comment_forest, depth=0) -> str:
+	def _handle_output(self, output: str) -> None:
+		if self.save_output_to:
+			with open(self.save_output_to, 'w') as f:
+				f.write(output)
+
+	def _process_comments(self, comments: praw.models.comment_forest.CommentForest, depth: int = 1) -> str:
 		comments_str = ""
 		for comment in comments:
+
+			# Skip any 'MoreComments' objects
 			if isinstance(comment, praw.models.MoreComments):
-				continue  # Skip any 'MoreComments' objects
+				continue
 
-			prefix = "| " * (depth + 1)
+			# Stop processing comments if depth exceeds max_comment_depth
+			if self.max_comment_depth not in (None, -1) and depth > self.max_comment_depth:
+				break
+
+			prefix = f"{self.comment_delim} " * depth
 
 			# Safe-guard for deleted comments where the author would be None
 			author = comment.author.name if comment.author else "deleted"
-			upvotes = comment.score
+			score = comment.score
+			upvotes_or_downvotes = 'upvotes' if score >= 0 else 'downvotes'
 			comment_body = comment.body.replace('\n', '\\n')  # Replace newlines to avoid breaking the tree structure
 
-			comments_str += f"{prefix}{author} ({upvotes} upvotes): {comment_body}\n"
+			comments_str += f"{prefix}{author} ({score} {upvotes_or_downvotes}): {comment_body}\n"
 
 			# Recursively process the replies to each comment
 			comments_str += self._process_comments(comment.replies, depth + 1)
 
 		return comments_str
 
-	def textualize_post(self, url: str) -> str:
-		# Extract the post ID from the URL
-		post_id = url.split('/')[-3]
-
-		# Fetch the post by ID
-		post = self.praw_reddit.submission(id=post_id)
-
+	def _process_original_post(self, post: praw.models.Submission) -> None:
 		# Fetch the title, author, upvotes, and post text
+		# OP's info
 		title = post.title
 		author = post.author.name if post.author else "deleted"
 		upvotes = post.score
 		selftext = post.selftext.replace('\n', ' ')  # Replace newlines to avoid breaking the structure
 
 		# Ensure all comments are fetched
 		post.comments.replace_more(limit=None)
 
 		# Start building the final output string
-		final_output = f"title: {title}\nauthor/upvotes: {author}/{upvotes}\npost text: {selftext}\n\n"
+		original_post_output = f"title: {title}\nauthor/upvotes: {author}/{upvotes}\npost text: {selftext}\n\n"
+
+		return original_post_output
+
+	def textualize_post(self, url: str) -> str:
+		# Extract the post ID from the URL
+		post_id = url.split('/')[-3]
+		post = self._praw_reddit.submission(id=post_id)
+
+		# Convert the original post and all the comments to text individually
+		text_post = self._process_original_post(post)
+		text_comments = self._process_comments(post.comments)
+
+		# Combine the original post and comments into a single string
+		final_output = text_post + text_comments
 
-		# Add the processed comments and replies to the final output
-		final_output += self._process_comments(post.comments)
+		# Handle the output based on the user's preference
+		# self._handle_output(final_output)
 
 		return final_output
```

### Comparing `reddit2text-0.0.5/reddit2text.egg-info/PKG-INFO` & `reddit2text-0.0.6/reddit2text.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit2text
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convert Reddit posts to text
 Author: Nicholas Hansen-Feruch
 Author-email: nicholas.feruch@gmail.com
 Keywords: python,reddit,text conversion,reddit api,praw,reddit to text,reddit comments,social media analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `reddit2text-0.0.5/setup.py` & `reddit2text-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'  # Consider starting with a semantic versioning scheme
+VERSION = '0.0.6'  # Consider starting with a semantic versioning scheme
 DESCRIPTION = 'Convert Reddit posts to text'
 LONG_DESCRIPTION = """
 A Python package for converting Reddit posts into structured text representations.
 This includes the post's title, author, upvotes, and body, along with all comments
 and their hierarchical structure. Ideal for processing, analysis, or feeding into
 natural language models.
 """
@@ -16,15 +16,15 @@
     author="Nicholas Hansen-Feruch",
     author_email="nicholas.feruch@gmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',  # Specify the LONG_DESCRIPTION is in Markdown
     packages=find_packages(),
     install_requires=[
-        'praw',  # Ensure you have listed all necessary dependencies
+        'praw',
     ],
     keywords=['python', 'reddit', 'text conversion', 'reddit api', 'praw', 'reddit to text', 'reddit comments', 'social media analysis'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",  # Updated to reflect a more accurate audience
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3",  # Specify Python 3, as Python 2 is deprecated
```

