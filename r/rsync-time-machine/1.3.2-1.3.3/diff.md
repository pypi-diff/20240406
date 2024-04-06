# Comparing `tmp/rsync-time-machine-1.3.2.tar.gz` & `tmp/rsync-time-machine-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsync-time-machine-1.3.2.tar", last modified: Tue Feb 27 02:21:58 2024, max compression
+gzip compressed data, was "rsync-time-machine-1.3.3.tar", last modified: Sat Apr  6 07:48:31 2024, max compression
```

## Comparing `rsync-time-machine-1.3.2.tar` & `rsync-time-machine-1.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 02:21:58.730917 rsync-time-machine-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-27 02:21:43.000000 rsync-time-machine-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13182 2024-02-27 02:21:58.730917 rsync-time-machine-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-02-27 02:21:43.000000 rsync-time-machine-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-02-27 02:21:43.000000 rsync-time-machine-1.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 02:21:58.730917 rsync-time-machine-1.3.2/rsync_time_machine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13182 2024-02-27 02:21:58.000000 rsync-time-machine-1.3.2/rsync_time_machine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-27 02:21:58.000000 rsync-time-machine-1.3.2/rsync_time_machine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 02:21:58.000000 rsync-time-machine-1.3.2/rsync_time_machine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-27 02:21:58.000000 rsync-time-machine-1.3.2/rsync_time_machine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-27 02:21:58.000000 rsync-time-machine-1.3.2/rsync_time_machine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-27 02:21:58.000000 rsync-time-machine-1.3.2/rsync_time_machine.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    29207 2024-02-27 02:21:43.000000 rsync-time-machine-1.3.2/rsync_time_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 02:21:58.730917 rsync-time-machine-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 02:21:58.730917 rsync-time-machine-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-02-27 02:21:43.000000 rsync-time-machine-1.3.2/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:48:31.966391 rsync-time-machine-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 07:48:20.000000 rsync-time-machine-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13182 2024-04-06 07:48:31.966391 rsync-time-machine-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-04-06 07:48:20.000000 rsync-time-machine-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-06 07:48:20.000000 rsync-time-machine-1.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:48:31.966391 rsync-time-machine-1.3.3/rsync_time_machine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13182 2024-04-06 07:48:31.000000 rsync-time-machine-1.3.3/rsync_time_machine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-06 07:48:31.000000 rsync-time-machine-1.3.3/rsync_time_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 07:48:31.000000 rsync-time-machine-1.3.3/rsync_time_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-06 07:48:31.000000 rsync-time-machine-1.3.3/rsync_time_machine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-06 07:48:31.000000 rsync-time-machine-1.3.3/rsync_time_machine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 07:48:31.000000 rsync-time-machine-1.3.3/rsync_time_machine.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29495 2024-04-06 07:48:20.000000 rsync-time-machine-1.3.3/rsync_time_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 07:48:31.966391 rsync-time-machine-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:48:31.966391 rsync-time-machine-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-04-06 07:48:20.000000 rsync-time-machine-1.3.3/tests/test_app.py
```

### Comparing `rsync-time-machine-1.3.2/LICENSE` & `rsync-time-machine-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rsync-time-machine-1.3.2/PKG-INFO` & `rsync-time-machine-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsync-time-machine
-Version: 1.3.2
+Version: 1.3.3
 Summary: rsync-time-machine.py is a wrapper around rsync to make it easier to create and maintain Time Machine style backups.
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/rsync-time-machine.py
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: test
```

### Comparing `rsync-time-machine-1.3.2/README.md` & `rsync-time-machine-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `rsync-time-machine-1.3.2/pyproject.toml` & `rsync-time-machine-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rsync-time-machine-1.3.2/rsync_time_machine.egg-info/PKG-INFO` & `rsync-time-machine-1.3.3/rsync_time_machine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsync-time-machine
-Version: 1.3.2
+Version: 1.3.3
 Summary: rsync-time-machine.py is a wrapper around rsync to make it easier to create and maintain Time Machine style backups.
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/rsync-time-machine.py
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: test
```

### Comparing `rsync-time-machine-1.3.2/rsync_time_machine.py` & `rsync-time-machine-1.3.3/rsync_time_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,19 @@
     cmd: str
     src_folder: str
     dest_folder: str
     port: str
     id_rsa: str | None
 
 
+def dest_is_ssh(ssh: SSH | None) -> SSH | None:
+    """Returns the SSH object only if the destination is remote."""
+    return ssh if ssh and ssh.dest_folder_prefix else None
+
+
 COLORS = {
     "green": "\033[92m",
     "magenta": "\033[95m",
     "yellow": "\033[93m",
     "red": "\033[91m",
     "orange": "\033[33m",
 }
@@ -253,15 +258,15 @@
 
 def find_backups(dest_folder: str, ssh: SSH | None = None) -> list[str]:
     """Return a list of all available backups in the destination folder, sorted by date.
 
     (Replaces 'fn_find_backups' in the Bash script).
     """
     cmd = f"find '{dest_folder}/' -maxdepth 1 -type d -name '????-??-??-??????' -prune | sort -r"
-    return run_cmd(cmd, ssh).stdout.splitlines()
+    return run_cmd(cmd, dest_is_ssh(ssh)).stdout.splitlines()
 
 
 def expire_backup(
     backup_path: str,
     ssh: SSH | None,
 ) -> None:
     """Expire the given backup folder after checking if it's on a backup destination."""
@@ -355,15 +360,15 @@
     """Return the path to the backup marker file."""
     return os.path.join(folder, "backup.marker")
 
 
 def find_backup_marker(folder: str, ssh: SSH | None = None) -> str | None:
     """Find the backup marker file in the given folder."""
     marker_path = backup_marker_path(folder)
-    output = find(marker_path, ssh)
+    output = find(marker_path, dest_is_ssh(ssh))
     return marker_path if output else None
 
 
 class CmdResult(NamedTuple):
     """Command result."""
 
     stdout: str
@@ -468,17 +473,17 @@
 
 
 def ln(src: str, dest: str, ssh: SSH | None = None) -> None:
     """Create a symlink."""
     run_cmd(f"ln -s -- '{src}' '{dest}'", ssh)
 
 
-def test_file_exists_src(path: str) -> bool:
+def test_file_exists_src(path: str, ssh: SSH | None = None) -> bool:
     """Test if a file exists."""
-    return run_cmd(f"test -e '{path}'", None).returncode == 0
+    return run_cmd(f"test -e '{path}'", ssh).returncode == 0
 
 
 def get_file_system_type(path: str, ssh: SSH | None = None) -> str:
     """Get the filesystem type of the given path."""
     lines = run_cmd(f"df -T '{path}'", ssh).stdout.split("\n")
     if len(lines) > 1:
         return lines[1].split()[1]  # filesystem type is in the second column
@@ -611,16 +616,16 @@
     if rsync_set_flags:
         rsync_flags = rsync_set_flags.split()
 
     if rsync_append_flags:
         rsync_flags += rsync_append_flags.split()
 
     if (
-        get_file_system_type(src_folder).lower() == "fat"
-        or get_file_system_type(dest_folder, ssh).lower() == "fat"
+        get_file_system_type(src_folder, ssh).lower() == "fat"
+        or get_file_system_type(dest_folder, dest_is_ssh(ssh)).lower() == "fat"
     ):
         log_info("File-system is a version of FAT.")
         log_info("Using the --modify-window rsync parameter with value 2.")
         rsync_flags.append("--modify-window=2")
 
     if ssh is not None:
         rsync_flags.append("--compress")
@@ -809,19 +814,19 @@
         dest_folder,
         ssh_port=port,
         id_rsa=id_rsa,
         exclusion_file=exclusion_file,
         allow_host_only=allow_host_only,
     )
 
-    if not test_file_exists_src(src_folder):
+    if not test_file_exists_src(src_folder, ssh):
         log_error(f"Source folder '{src_folder}' does not exist - aborting.")
         sys.exit(1)
 
-    check_dest_is_backup_folder(dest_folder, ssh)
+    check_dest_is_backup_folder(dest_folder, dest_is_ssh(ssh))
 
     now = now_str()
     dest = os.path.join(dest_folder, now)
     _backups = sorted(find_backups(dest_folder, ssh), reverse=True)
     previous_dest = _backups[0] if _backups else None
     inprogress_file = os.path.join(dest_folder, "backup.inprogress")
     mypid = os.getpid()
@@ -889,19 +894,19 @@
             auto_expire=auto_expire,
         )
         if not retry:
             break
 
     check_rsync_errors(log_file, auto_delete_log)
 
-    rm_file(os.path.join(dest_folder, "latest"), ssh)
+    rm_file(os.path.join(dest_folder, "latest"), dest_is_ssh(ssh))
     ln(
         os.path.basename(dest),
         os.path.join(dest_folder, "latest"),
-        ssh,
+        dest_is_ssh(ssh),
     )
 
     rm_file(inprogress_file, ssh)
 
 
 def main() -> None:
     """Main function."""
```

### Comparing `rsync-time-machine-1.3.2/tests/test_app.py` & `rsync-time-machine-1.3.3/tests/test_app.py`

 * *Files identical despite different names*

