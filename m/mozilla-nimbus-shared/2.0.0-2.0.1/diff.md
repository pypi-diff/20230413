# Comparing `tmp/mozilla_nimbus_shared-2.0.0.tar.gz` & `tmp/mozilla_nimbus_shared-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla_nimbus_shared-2.0.0.tar", max compression
+gzip compressed data, was "mozilla_nimbus_shared-2.0.1.tar", max compression
```

## Comparing `mozilla_nimbus_shared-2.0.0.tar` & `mozilla_nimbus_shared-2.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      628 2022-06-16 17:41:54.490623 mozilla_nimbus_shared-2.0.0/README.md
--rw-r--r--   0        0        0     1660 2022-06-16 17:38:10.474193 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/__init__.py
--rw-r--r--   0        0        0    27260 2023-03-08 17:02:15.452435 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/data.json
--rw-r--r--   0        0        0    13525 2022-06-16 17:43:18.604934 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/experiments/NimbusExperiment.json
--rw-r--r--   0        0        0     2559 2022-06-16 17:43:18.605127 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/features/Feature.json
--rw-r--r--   0        0        0    25972 2022-06-16 17:43:18.606633 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/messaging/SimpleCFRMessage.json
--rw-r--r--   0        0        0     9789 2022-06-16 17:43:18.606730 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/messaging/SpecialMessageActionSchemas.json
--rw-r--r--   0        0        0     4368 2022-06-16 17:43:18.606822 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/messaging/TriggerActionSchemas.json
--rw-r--r--   0        0        0      493 2022-06-16 17:43:18.606224 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/AddonRollbackArguments.json
--rw-r--r--   0        0        0      689 2022-06-16 17:43:18.605834 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/AddonRolloutArguments.json
--rw-r--r--   0        0        0     2015 2022-06-16 17:43:18.606125 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/BranchedAddonStudyArguments.json
--rw-r--r--   0        0        0      434 2022-06-16 17:43:18.605338 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/ConsoleLogArguments.json
--rw-r--r--   0        0        0     2528 2022-06-16 17:43:18.606031 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/MessagingExperimentArguments.json
--rw-r--r--   0        0        0     4064 2022-06-16 17:43:18.606327 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/MultiPreferenceExperimentArguments.json
--rw-r--r--   0        0        0    18244 2022-06-16 17:43:18.605742 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/NormandyRecipe.json
--rw-r--r--   0        0        0     1149 2022-06-16 17:43:18.606422 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/OptOutStudyArguments.json
--rw-r--r--   0        0        0     3038 2022-06-16 17:43:18.605537 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/PreferenceExperimentArguments.json
--rw-r--r--   0        0        0      467 2022-06-16 17:43:18.605443 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRollbackArguments.json
--rw-r--r--   0        0        0     1280 2022-06-16 17:43:18.605928 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRolloutArguments.json
--rw-r--r--   0        0        0     2077 2022-06-16 17:43:18.605633 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/ShowHeartbeatArguments.json
--rw-r--r--   0        0        0    13302 2023-03-08 17:02:15.454267 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/experiments/NimbusExperiment.json
--rw-r--r--   0        0        0     2559 2023-03-08 17:02:15.454465 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/features/Feature.json
--rw-r--r--   0        0        0      493 2023-03-08 17:02:15.455590 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRollbackArguments.json
--rw-r--r--   0        0        0      689 2023-03-08 17:02:15.455191 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRolloutArguments.json
--rw-r--r--   0        0        0     2015 2023-03-08 17:02:15.455491 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/BranchedAddonStudyArguments.json
--rw-r--r--   0        0        0      434 2023-03-08 17:02:15.454671 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/ConsoleLogArguments.json
--rw-r--r--   0        0        0     2528 2023-03-08 17:02:15.455393 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/MessagingExperimentArguments.json
--rw-r--r--   0        0        0     4064 2023-03-08 17:02:15.455693 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/MultiPreferenceExperimentArguments.json
--rw-r--r--   0        0        0    18244 2023-03-08 17:02:15.455095 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/NormandyRecipe.json
--rw-r--r--   0        0        0     1149 2023-03-08 17:02:15.455786 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/OptOutStudyArguments.json
--rw-r--r--   0        0        0     3038 2023-03-08 17:02:15.454883 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceExperimentArguments.json
--rw-r--r--   0        0        0      467 2023-03-08 17:02:15.454780 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRollbackArguments.json
--rw-r--r--   0        0        0     1280 2023-03-08 17:02:15.455291 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRolloutArguments.json
--rw-r--r--   0        0        0     2077 2023-03-08 17:02:15.454991 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/ShowHeartbeatArguments.json
--rw-r--r--   0        0        0      736 2023-03-08 17:02:15.454067 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/targeting/Audience.json
--rw-r--r--   0        0        0      449 2023-03-08 17:02:15.453853 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/test/FoodColors.json
--rw-r--r--   0        0        0      736 2022-06-16 17:43:18.604745 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/targeting/Audience.json
--rw-r--r--   0        0        0      449 2022-06-16 17:43:18.604538 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/test/FoodColors.json
--rw-r--r--   0        0        0      999 2022-06-16 17:38:10.474263 mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/test.py
--rw-r--r--   0        0        0      524 2023-03-08 16:59:14.163208 mozilla_nimbus_shared-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 mozilla_nimbus_shared-2.0.0/setup.py
--rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 mozilla_nimbus_shared-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      628 2022-06-16 17:41:54.490623 mozilla_nimbus_shared-2.0.1/README.md
+-rw-r--r--   0        0        0     1660 2022-06-16 17:38:10.474193 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/__init__.py
+-rw-r--r--   0        0        0    27260 2023-04-13 15:03:58.331157 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/data.json
+-rw-r--r--   0        0        0    13302 2023-04-13 15:03:58.333225 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/experiments/NimbusExperiment.json
+-rw-r--r--   0        0        0     2559 2023-04-13 15:03:58.333426 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/features/Feature.json
+-rw-r--r--   0        0        0    25972 2022-06-16 17:43:18.606633 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/messaging/SimpleCFRMessage.json
+-rw-r--r--   0        0        0     9789 2022-06-16 17:43:18.606730 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/messaging/SpecialMessageActionSchemas.json
+-rw-r--r--   0        0        0     4368 2022-06-16 17:43:18.606822 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/messaging/TriggerActionSchemas.json
+-rw-r--r--   0        0        0      493 2023-04-13 15:03:58.334627 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/AddonRollbackArguments.json
+-rw-r--r--   0        0        0      689 2023-04-13 15:03:58.334180 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/AddonRolloutArguments.json
+-rw-r--r--   0        0        0     2015 2023-04-13 15:03:58.334522 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/BranchedAddonStudyArguments.json
+-rw-r--r--   0        0        0      434 2023-04-13 15:03:58.333627 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/ConsoleLogArguments.json
+-rw-r--r--   0        0        0     2528 2023-04-13 15:03:58.334417 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/MessagingExperimentArguments.json
+-rw-r--r--   0        0        0     4064 2023-04-13 15:03:58.334738 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/MultiPreferenceExperimentArguments.json
+-rw-r--r--   0        0        0    18244 2023-04-13 15:03:58.334076 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/NormandyRecipe.json
+-rw-r--r--   0        0        0     1149 2023-04-13 15:03:58.334844 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/OptOutStudyArguments.json
+-rw-r--r--   0        0        0     3038 2023-04-13 15:03:58.333850 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/PreferenceExperimentArguments.json
+-rw-r--r--   0        0        0      467 2023-04-13 15:03:58.333742 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/PreferenceRollbackArguments.json
+-rw-r--r--   0        0        0     1280 2023-04-13 15:03:58.334299 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/PreferenceRolloutArguments.json
+-rw-r--r--   0        0        0     2077 2023-04-13 15:03:58.333960 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/ShowHeartbeatArguments.json
+-rw-r--r--   0        0        0    13302 2023-03-08 17:02:15.454267 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/experiments/NimbusExperiment.json
+-rw-r--r--   0        0        0     2559 2023-03-08 17:02:15.454465 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/features/Feature.json
+-rw-r--r--   0        0        0      493 2023-03-08 17:02:15.455590 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRollbackArguments.json
+-rw-r--r--   0        0        0      689 2023-03-08 17:02:15.455191 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRolloutArguments.json
+-rw-r--r--   0        0        0     2015 2023-03-08 17:02:15.455491 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/BranchedAddonStudyArguments.json
+-rw-r--r--   0        0        0      434 2023-03-08 17:02:15.454671 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/ConsoleLogArguments.json
+-rw-r--r--   0        0        0     2528 2023-03-08 17:02:15.455393 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/MessagingExperimentArguments.json
+-rw-r--r--   0        0        0     4064 2023-03-08 17:02:15.455693 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/MultiPreferenceExperimentArguments.json
+-rw-r--r--   0        0        0    18244 2023-03-08 17:02:15.455095 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/NormandyRecipe.json
+-rw-r--r--   0        0        0     1149 2023-03-08 17:02:15.455786 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/OptOutStudyArguments.json
+-rw-r--r--   0        0        0     3038 2023-03-08 17:02:15.454883 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceExperimentArguments.json
+-rw-r--r--   0        0        0      467 2023-03-08 17:02:15.454780 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRollbackArguments.json
+-rw-r--r--   0        0        0     1280 2023-03-08 17:02:15.455291 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRolloutArguments.json
+-rw-r--r--   0        0        0     2077 2023-03-08 17:02:15.454991 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/ShowHeartbeatArguments.json
+-rw-r--r--   0        0        0      736 2023-03-08 17:02:15.454067 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/targeting/Audience.json
+-rw-r--r--   0        0        0      449 2023-03-08 17:02:15.453853 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/test/FoodColors.json
+-rw-r--r--   0        0        0      736 2023-04-13 15:03:58.333045 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/targeting/Audience.json
+-rw-r--r--   0        0        0      449 2023-04-13 15:03:58.332844 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/test/FoodColors.json
+-rw-r--r--   0        0        0      999 2022-06-16 17:38:10.474263 mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/test.py
+-rw-r--r--   0        0        0      524 2023-04-13 15:03:58.322442 mozilla_nimbus_shared-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 mozilla_nimbus_shared-2.0.1/setup.py
+-rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 mozilla_nimbus_shared-2.0.1/PKG-INFO
```

### Comparing `mozilla_nimbus_shared-2.0.0/README.md` & `mozilla_nimbus_shared-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/__init__.py` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/data.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/data.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/experiments/NimbusExperiment.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/experiments/NimbusExperiment.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986979093989156%*

 * *Differences: {"'definitions'": "{'NimbusExperiment': {'properties': {'branches': {'anyOf': {0: {'items': "*

 * *                  "{'properties': {'feature': {'properties': {delete: ['enabled']}}}}}, 1: "*

 * *                  "{'items': {'properties': {'features': {'items': {'properties': {delete: "*

 * *                  "['enabled']}}}}}}, 2: {'items': {'properties': {'features': {'items': "*

 * *                  "{'properties': {delete: ['enabled']}}}}}}}}, 'featureValidationOptOut': "*

 * *                  "OrderedDict([('type', 'boolea […]*

```diff
@@ -17,18 +17,14 @@
                     "anyOf": [
                         {
                             "items": {
                                 "properties": {
                                     "feature": {
                                         "description": "A single feature configuration",
                                         "properties": {
-                                            "enabled": {
-                                                "description": "This can be used to turn the whole feature on/off",
-                                                "type": "boolean"
-                                            },
                                             "featureId": {
                                                 "description": "The identifier for the feature flag",
                                                 "type": "string"
                                             },
                                             "value": {
                                                 "additionalProperties": {},
                                                 "description": "Optional extra params for the feature (this should be validated against a schema)",
@@ -86,18 +82,14 @@
                                         ],
                                         "type": "object"
                                     },
                                     "features": {
                                         "description": "An array of feature configurations",
                                         "items": {
                                             "properties": {
-                                                "enabled": {
-                                                    "description": "This can be used to turn the whole feature on/off",
-                                                    "type": "boolean"
-                                                },
                                                 "featureId": {
                                                     "description": "The identifier for the feature flag",
                                                     "type": "string"
                                                 },
                                                 "value": {
                                                     "additionalProperties": {},
                                                     "description": "Optional extra params for the feature (this should be validated against a schema)",
@@ -135,18 +127,14 @@
                         {
                             "items": {
                                 "properties": {
                                     "features": {
                                         "description": "An array of feature configurations",
                                         "items": {
                                             "properties": {
-                                                "enabled": {
-                                                    "description": "This can be used to turn the whole feature on/off",
-                                                    "type": "boolean"
-                                                },
                                                 "featureId": {
                                                     "description": "The identifier for the feature flag",
                                                     "type": "string"
                                                 },
                                                 "value": {
                                                     "additionalProperties": {},
                                                     "description": "Optional extra params for the feature (this should be validated against a schema)",
@@ -240,30 +228,40 @@
                 "featureIds": {
                     "description": "A list of featureIds the experiment contains configurations for.",
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
-                "filter_expression": {
-                    "description": "This is NOT used by Nimbus, but has special functionality in Remote Settings. See https://remote-settings.readthedocs.io/en/latest/target-filters.html#how",
-                    "type": "string"
+                "featureValidationOptOut": {
+                    "description": "Opt out of feature schema validation. Only supported on desktop.",
+                    "type": "boolean"
                 },
                 "id": {
                     "description": "Unique identifier for the experiment. This is a duplicate of slug, but is a required field for all Remote Settings records.",
                     "type": "string"
                 },
                 "isEnrollmentPaused": {
                     "description": "When this property is set to true, the the SDK should not enroll new users into the experiment that have not already been enrolled.",
                     "type": "boolean"
                 },
                 "isRollout": {
                     "description": "When this property is set to true, treat this experiment as a rollout. Rollouts are currently handled as single-branch experiments separated from the bucketing namespace for normal experiments. See also: https://mozilla-hub.atlassian.net/browse/SDK-405",
                     "type": "boolean"
                 },
+                "localizations": {
+                    "additionalProperties": {
+                        "additionalProperties": {
+                            "type": "string"
+                        },
+                        "type": "object"
+                    },
+                    "description": "Per-locale localization substitutions.\n\nThe top level key is the locale (e.g., \"en-US\" or \"fr\"). Each entry is a mapping of string IDs to their localized equivalents.\n\nOnly supported on desktop.",
+                    "type": "object"
+                },
                 "outcomes": {
                     "description": "A list of outcomes relevant to the experiment analysis.",
                     "items": {
                         "properties": {
                             "priority": {
                                 "description": "e.g. \"primary\" or \"secondary\"",
                                 "type": "string"
```

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/features/Feature.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/features/Feature.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/messaging/SimpleCFRMessage.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/messaging/SimpleCFRMessage.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/messaging/SpecialMessageActionSchemas.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/messaging/SpecialMessageActionSchemas.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/messaging/TriggerActionSchemas.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/messaging/TriggerActionSchemas.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/AddonRolloutArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/AddonRolloutArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/BranchedAddonStudyArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/BranchedAddonStudyArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/MessagingExperimentArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/MessagingExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/MultiPreferenceExperimentArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/MultiPreferenceExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/NormandyRecipe.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/NormandyRecipe.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/OptOutStudyArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/OptOutStudyArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/PreferenceExperimentArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/PreferenceExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRolloutArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/PreferenceRolloutArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/normandy/ShowHeartbeatArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/normandy/ShowHeartbeatArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/experiments/NimbusExperiment.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/experiments/NimbusExperiment.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/features/Feature.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/features/Feature.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRolloutArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRolloutArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/BranchedAddonStudyArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/BranchedAddonStudyArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/MessagingExperimentArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/MessagingExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/MultiPreferenceExperimentArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/MultiPreferenceExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/NormandyRecipe.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/NormandyRecipe.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/OptOutStudyArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/OptOutStudyArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceExperimentArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRolloutArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRolloutArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/normandy/ShowHeartbeatArguments.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/normandy/ShowHeartbeatArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/schemas/targeting/Audience.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/schemas/targeting/Audience.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/schemas/targeting/Audience.json` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/schemas/targeting/Audience.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/mozilla_nimbus_shared/test.py` & `mozilla_nimbus_shared-2.0.1/mozilla_nimbus_shared/test.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.0.0/pyproject.toml` & `mozilla_nimbus_shared-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "mozilla_nimbus_shared"
 description = "Shared data and schemas for Project Nimbus"
 readme = "README.md"
 authors = ["Michael Cooper <mcooper@mozilla.com>"]
-version = "2.0.0"
+version = "2.0.1"
 license = "MPL-2.0"
 include = [
   "mozilla_nimbus_shared/schemas/**/*.json",
   "mozilla_nimbus_shared/data.json",
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `mozilla_nimbus_shared-2.0.0/setup.py` & `mozilla_nimbus_shared-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                            'schemas/test/*']}
 
 install_requires = \
 ['jsonschema>=4.17.3,<5.0.0']
 
 setup_kwargs = {
     'name': 'mozilla-nimbus-shared',
-    'version': '2.0.0',
+    'version': '2.0.1',
     'description': 'Shared data and schemas for Project Nimbus',
     'long_description': '# Nimbus Shared ![CircleCI](https://img.shields.io/circleci/build/github/mozilla/nimbus-shared) ![npm (scoped)](https://img.shields.io/npm/v/@mozilla/nimbus-shared)\n\nThis is a place to define data and schemas used across Project Nimbus.\n\nAny data that moves between systems should have TypeScript types defined here, which will be\nautomatically converted to JSON Schema. Any data that needs to be re-used by multiple systems should\nbe stored here to be shared.\n\nFor more information on the data and schemas included here, how to use them, and how to add to them,\nsee the documentation at https://mozilla.github.io/nimbus-shared\n',
     'author': 'Michael Cooper',
     'author_email': 'mcooper@mozilla.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mozilla_nimbus_shared-2.0.0/PKG-INFO` & `mozilla_nimbus_shared-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-nimbus-shared
-Version: 2.0.0
+Version: 2.0.1
 Summary: Shared data and schemas for Project Nimbus
 License: MPL-2.0
 Author: Michael Cooper
 Author-email: mcooper@mozilla.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

