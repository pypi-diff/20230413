# Comparing `tmp/ExpdFtpService-0.5.0.tar.gz` & `tmp/ExpdFtpService-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ExpdFtpService-0.5.0.tar", last modified: Fri Apr  7 08:47:19 2023, max compression
+gzip compressed data, was "dist\ExpdFtpService-0.6.0.tar", last modified: Thu Apr 13 01:57:24 2023, max compression
```

## Comparing `ExpdFtpService-0.5.0.tar` & `ExpdFtpService-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 08:47:19.000000 ExpdFtpService-0.5.0/
--rw-rw-rw-   0        0        0      305 2023-04-07 08:47:19.000000 ExpdFtpService-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-03-02 11:07:57.000000 ExpdFtpService-0.5.0/README.md
--rw-rw-rw-   0        0        0      115 2023-04-07 08:47:19.000000 ExpdFtpService-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      441 2023-04-07 08:12:41.000000 ExpdFtpService-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 08:47:19.000000 ExpdFtpService-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 08:47:19.000000 ExpdFtpService-0.5.0/src/ExpdFtpService/
--rw-rw-rw-   0        0        0     4573 2023-04-07 08:46:33.000000 ExpdFtpService-0.5.0/src/ExpdFtpService/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 08:47:19.000000 ExpdFtpService-0.5.0/src/ExpdFtpService.egg-info/
--rw-rw-rw-   0        0        0      305 2023-04-07 08:47:19.000000 ExpdFtpService-0.5.0/src/ExpdFtpService.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-04-07 08:47:19.000000 ExpdFtpService-0.5.0/src/ExpdFtpService.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 08:47:19.000000 ExpdFtpService-0.5.0/src/ExpdFtpService.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-07 08:47:19.000000 ExpdFtpService-0.5.0/src/ExpdFtpService.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-07 08:47:19.000000 ExpdFtpService-0.5.0/src/ExpdFtpService.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/
+-rw-rw-rw-   0        0        0      305 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2023-04-07 09:01:05.000000 ExpdFtpService-0.6.0/README.md
+-rw-rw-rw-   0        0        0      115 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      441 2023-04-13 01:56:30.000000 ExpdFtpService-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService/
+-rw-rw-rw-   0        0        0     4348 2023-04-13 01:57:14.000000 ExpdFtpService-0.6.0/src/ExpdFtpService/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService.egg-info/
+-rw-rw-rw-   0        0        0      305 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService.egg-info/top_level.txt
```

### Comparing `ExpdFtpService-0.5.0/README.md` & `ExpdFtpService-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     pip install ExpdFtpService
 
 
 How to use with download methods:
 
     from ExpdFtpService.download import ExpdDownloadFtpServerFile
-    ExpdDownloadFtpServerFile(hostname, username, password, destfolder, savefolder, fstartwith).download(numbers)
+    ExpdDownloadFtpServerFile(hostname, username, password, destfolder, savefolder, fstartwith).download(numbers=10)
     
 
 How to use with upload methods:
 
     from ExpdFtpService.upload import ExpdUploadFtpServerFile
     ExpdUploadFtpServerFile(hostname, username, password, destfolder).upload_file_to_serve(r"D:\Solutions\2431295471_PIE_E433593539.pdf")
```

### Comparing `ExpdFtpService-0.5.0/src/ExpdFtpService/__init__.py` & `ExpdFtpService-0.6.0/src/ExpdFtpService/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     """    
     def __init__(self, hostname, username, password):
         self.ftp = FTP()
         self.ftp.connect(host=hostname, port=21)
         self.ftp.sendcmd('OPTS UTF8 ON')
         self.ftp.set_pasv(True)
         self.ftp.login(user=username, passwd=password)
-        # logger.debug(self.ftp.getwelcome())
 
 
 class ExpdDownloadFtpServerFile(ConnFtpServer):
     def __init__(self, hostname, username, password, destfolder, savefolder, fstartwith=None, filendwith=None):
         super().__init__(hostname, username, password)
         self.destfolder = destfolder
         self.savefolder = savefolder
@@ -34,18 +33,14 @@
         self.ftp.cwd(self.destfolder)
         if self.fstartwith is not None:
             files = [x for x in self.ftp.nlst() if x.startswith(self.fstartwith)]
         elif self.filendwith is not None:
             files = [x for x in self.ftp.nlst() if x.endswith(self.filendwith)]
         else:
             files = [x for x in self.ftp.nlst() if str(x).lower() != 'history']
-        if len(files) == 0:
-            logger.warning("No files to download, scripting will be exiting")
-            sys.exit()
-        else:
             logger.debug(f"server total files: [{len(files)}]")
         return files
     
     def archive(self, from_file, to_path, to_file):
         history = self.ftp.nlst(to_path)
         if to_file not in history:
             self.ftp.rename(f"{from_file}", f"{to_path}\{to_file}")
@@ -54,20 +49,19 @@
             logger.warning(f"file exist in history folder, delete: {from_file}")
             self.ftp.delete(from_file)
 
     @logger.catch(reraise=True)
     def download(self, numbers):
         try:
             for count, file in enumerate(self.files, 1):
-                with open(path.join(self.savefolder, f"{file}"), 'wb') as rd:
-                    self.ftp.retrbinary('RETR %s' % file, rd.write)
-                self.archive(file, "History", file)
-                logger.debug(f"NO.{count}: file {file} download & archived successfully")
-                if count == numbers:
-                    break
+                if count <= numbers:
+                    with open(path.join(self.savefolder, f"{file}"), 'wb') as rd:
+                        self.ftp.retrbinary('RETR %s' % file, rd.write)
+                    self.archive(file, "History", file)
+                    logger.debug(f"NO.{count}: file {file} download & archived successfully")
         finally:
             self.ftp.quit()
     
 
 class ExpdUploadFtpServerFile(ConnFtpServer):
     """Class is used for connecting to a FTP Server and upload files.
         The constructor accepts the following parameters with the indicated types:
@@ -97,12 +91,12 @@
                 logger.debug(f"{local_file} uploaded successfully")
         finally:
             self.ftp.quit()
     
 
 if __name__ == '__main__':
     ExpdUploadFtpServerFile(
-        hostname="sha-comm02.sha.ei",
+        hostname="xxx",
         username="xxx",
         password="xxx",
-        destfolder="/ftp/GEO/testpath这话",
+        destfolder="/ftp/GEO/testpath",
     ).upload_file_to_server(r"D:\Solutions\edoc_upload_sourth_korea\server\data\History\E13I2100055\R4382481_PIE_E433594030.pdf")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

