# Comparing `tmp/aws-cdk.aws-sagemaker-alpha-2.73.0a0.tar.gz` & `tmp/aws-cdk.aws-sagemaker-alpha-2.74.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src656217235/src/packages/@aws-cdk/aws-sagemaker/dist/python/aws-cdk.aws-sagemaker-alpha-2.73.0a0.tar", last modified: Wed Apr  5 23:25:46 2023, max compression
+gzip compressed data, was "/codebuild/output/src988541908/src/packages/@aws-cdk/aws-sagemaker-alpha/dist/python/aws-cdk.aws-sagemaker-alpha-2.74.0a0.tar", last modified: Thu Apr 13 16:41:19 2023, max compression
```

## Comparing `aws-cdk.aws-sagemaker-alpha-2.73.0a0.tar` & `aws-cdk.aws-sagemaker-alpha-2.74.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-04-05 23:25:34.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-05 23:25:34.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-04-05 23:25:34.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9636 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8631 2023-04-05 23:25:34.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-05 23:25:34.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1884 2023-04-05 23:25:34.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk/aws_sagemaker_alpha/
--rw-r--r--   0 root         (0) root         (0)   238470 2023-04-05 23:25:34.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk/aws_sagemaker_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-05 23:25:34.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91232 2023-04-05 23:25:34.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/aws-sagemaker-alpha@2.73.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 23:25:34.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk/aws_sagemaker_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9636 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-05 23:25:46.000000 aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-04-13 16:41:09.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 16:41:09.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-04-13 16:41:09.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9936 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8931 2023-04-13 16:41:09.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-13 16:41:09.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-04-13 16:41:09.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk/aws_sagemaker_alpha/
+-rw-r--r--   0 root         (0) root         (0)   239805 2023-04-13 16:41:09.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk/aws_sagemaker_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-13 16:41:09.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92613 2023-04-13 16:41:09.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/aws-sagemaker-alpha@2.74.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 16:41:09.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk/aws_sagemaker_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9936 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      551 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-13 16:41:19.000000 aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.73.0a0/LICENSE` & `aws-cdk.aws-sagemaker-alpha-2.74.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-sagemaker-alpha-2.73.0a0/PKG-INFO` & `aws-cdk.aws-sagemaker-alpha-2.74.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-sagemaker-alpha
-Version: 2.73.0a0
+Version: 2.74.0a0
 Summary: The CDK Construct Library for AWS::SageMaker
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -129,14 +129,28 @@
 import aws_cdk.aws_sagemaker_alpha as sagemaker
 
 
 repository = ecr.Repository.from_repository_name(self, "Repository", "repo")
 image = sagemaker.ContainerImage.from_ecr_repository(repository, "tag")
 ```
 
+#### DLC Image
+
+Reference a deep learning container image:
+
+```python
+import aws_cdk.aws_sagemaker_alpha as sagemaker
+
+
+repository_name = "huggingface-pytorch-training"
+tag = "1.13.1-transformers4.26.0-gpu-py39-cu117-ubuntu20.04"
+
+image = sagemaker.ContainerImage.from_dlc(repository_name, tag)
+```
+
 ### Model Artifacts
 
 If you choose to decouple your model artifacts from your inference code (as is natural given
 different rates of change between inference code and model artifacts), the artifacts can be
 specified via the `modelData` property which accepts a class that extends the `ModelData` abstract
 base class. The default is to have no model artifacts associated with a model.
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.73.0a0/README.md` & `aws-cdk.aws-sagemaker-alpha-2.74.0a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,28 @@
 import aws_cdk.aws_sagemaker_alpha as sagemaker
 
 
 repository = ecr.Repository.from_repository_name(self, "Repository", "repo")
 image = sagemaker.ContainerImage.from_ecr_repository(repository, "tag")
 ```
 
+#### DLC Image
+
+Reference a deep learning container image:
+
+```python
+import aws_cdk.aws_sagemaker_alpha as sagemaker
+
+
+repository_name = "huggingface-pytorch-training"
+tag = "1.13.1-transformers4.26.0-gpu-py39-cu117-ubuntu20.04"
+
+image = sagemaker.ContainerImage.from_dlc(repository_name, tag)
+```
+
 ### Model Artifacts
 
 If you choose to decouple your model artifacts from your inference code (as is natural given
 different rates of change between inference code and model artifacts), the artifacts can be
 specified via the `modelData` property which accepts a class that extends the `ModelData` abstract
 base class. The default is to have no model artifacts associated with a model.
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.73.0a0/setup.py` & `aws-cdk.aws-sagemaker-alpha-2.74.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-sagemaker-alpha",
-    "version": "2.73.0.a0",
+    "version": "2.74.0.a0",
     "description": "The CDK Construct Library for AWS::SageMaker",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.aws_sagemaker_alpha",
         "aws_cdk.aws_sagemaker_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_sagemaker_alpha._jsii": [
-            "aws-sagemaker-alpha@2.73.0-alpha.0.jsii.tgz"
+            "aws-sagemaker-alpha@2.74.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_sagemaker_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.73.0",
+        "aws-cdk-lib==2.74.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.78.1, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk/aws_sagemaker_alpha/__init__.py` & `aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk/aws_sagemaker_alpha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,28 @@
 import aws_cdk.aws_sagemaker_alpha as sagemaker
 
 
 repository = ecr.Repository.from_repository_name(self, "Repository", "repo")
 image = sagemaker.ContainerImage.from_ecr_repository(repository, "tag")
 ```
 
+#### DLC Image
+
+Reference a deep learning container image:
+
+```python
+import aws_cdk.aws_sagemaker_alpha as sagemaker
+
+
+repository_name = "huggingface-pytorch-training"
+tag = "1.13.1-transformers4.26.0-gpu-py39-cu117-ubuntu20.04"
+
+image = sagemaker.ContainerImage.from_dlc(repository_name, tag)
+```
+
 ### Model Artifacts
 
 If you choose to decouple your model artifacts from your inference code (as is natural given
 different rates of change between inference code and model artifacts), the artifacts can be
 specified via the `modelData` property which accepts a class that extends the `ModelData` abstract
 base class. The default is to have no model artifacts associated with a model.
 
@@ -522,28 +536,20 @@
     '''(experimental) Constructs for types of container images.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
+        import aws_cdk.aws_ecr as ecr
         import aws_cdk.aws_sagemaker_alpha as sagemaker
-        import path as path
         
         
-        image = sagemaker.ContainerImage.from_asset(path.join("path", "to", "Dockerfile", "directory"))
-        model_data = sagemaker.ModelData.from_asset(path.join("path", "to", "artifact", "file.tar.gz"))
-        
-        model = sagemaker.Model(self, "PrimaryContainerModel",
-            containers=[sagemaker.ContainerDefinition(
-                image=image,
-                model_data=model_data
-            )
-            ]
-        )
+        repository = ecr.Repository.from_repository_name(self, "Repository", "repo")
+        image = sagemaker.ContainerImage.from_ecr_repository(repository, "tag")
     '''
 
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
@@ -607,14 +613,37 @@
             exclude=exclude,
             follow_symlinks=follow_symlinks,
             ignore_mode=ignore_mode,
         )
 
         return typing.cast("ContainerImage", jsii.sinvoke(cls, "fromAsset", [directory, options]))
 
+    @jsii.member(jsii_name="fromDlc")
+    @builtins.classmethod
+    def from_dlc(
+        cls,
+        repository_name: builtins.str,
+        tag: builtins.str,
+        account_id: typing.Optional[builtins.str] = None,
+    ) -> "ContainerImage":
+        '''(experimental) Reference an AWS Deep Learning Container image.
+
+        :param repository_name: -
+        :param tag: -
+        :param account_id: -
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1513460df0eb3c0b61b69d154112f40a5df89d65be52eaf732e84d2228fbc690)
+            check_type(argname="argument repository_name", value=repository_name, expected_type=type_hints["repository_name"])
+            check_type(argname="argument tag", value=tag, expected_type=type_hints["tag"])
+            check_type(argname="argument account_id", value=account_id, expected_type=type_hints["account_id"])
+        return typing.cast("ContainerImage", jsii.sinvoke(cls, "fromDlc", [repository_name, tag, account_id]))
+
     @jsii.member(jsii_name="fromEcrRepository")
     @builtins.classmethod
     def from_ecr_repository(
         cls,
         repository: _aws_cdk_aws_ecr_ceddda9d.IRepository,
         tag: typing.Optional[builtins.str] = None,
     ) -> "ContainerImage":
@@ -4677,14 +4706,22 @@
     exclude: typing.Optional[typing.Sequence[builtins.str]] = None,
     follow_symlinks: typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode] = None,
     ignore_mode: typing.Optional[_aws_cdk_ceddda9d.IgnoreMode] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__1513460df0eb3c0b61b69d154112f40a5df89d65be52eaf732e84d2228fbc690(
+    repository_name: builtins.str,
+    tag: builtins.str,
+    account_id: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__569a37621d1835097789a734af04a62735f0ad58fe58c164f1a5c562b7894999(
     repository: _aws_cdk_aws_ecr_ceddda9d.IRepository,
     tag: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-sagemaker-alpha
-Version: 2.73.0a0
+Version: 2.74.0a0
 Summary: The CDK Construct Library for AWS::SageMaker
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -129,14 +129,28 @@
 import aws_cdk.aws_sagemaker_alpha as sagemaker
 
 
 repository = ecr.Repository.from_repository_name(self, "Repository", "repo")
 image = sagemaker.ContainerImage.from_ecr_repository(repository, "tag")
 ```
 
+#### DLC Image
+
+Reference a deep learning container image:
+
+```python
+import aws_cdk.aws_sagemaker_alpha as sagemaker
+
+
+repository_name = "huggingface-pytorch-training"
+tag = "1.13.1-transformers4.26.0-gpu-py39-cu117-ubuntu20.04"
+
+image = sagemaker.ContainerImage.from_dlc(repository_name, tag)
+```
+
 ### Model Artifacts
 
 If you choose to decouple your model artifacts from your inference code (as is natural given
 different rates of change between inference code and model artifacts), the artifacts can be
 specified via the `modelData` property which accepts a class that extends the `ModelData` abstract
 base class. The default is to have no model artifacts associated with a model.
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.73.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-sagemaker-alpha-2.74.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_sagemaker_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_sagemaker_alpha.egg-info/requires.txt
 src/aws_cdk.aws_sagemaker_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_sagemaker_alpha/__init__.py
 src/aws_cdk/aws_sagemaker_alpha/py.typed
 src/aws_cdk/aws_sagemaker_alpha/_jsii/__init__.py
-src/aws_cdk/aws_sagemaker_alpha/_jsii/aws-sagemaker-alpha@2.73.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_sagemaker_alpha/_jsii/aws-sagemaker-alpha@2.74.0-alpha.0.jsii.tgz
```

