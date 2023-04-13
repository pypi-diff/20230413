# Comparing `tmp/ontoloviz-1.5.7.tar.gz` & `tmp/ontoloviz-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontoloviz-1.5.7.tar", max compression
+gzip compressed data, was "ontoloviz-1.5.8.tar", max compression
```

## Comparing `ontoloviz-1.5.7.tar` & `ontoloviz-1.5.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1090 2023-01-19 15:10:20.455810 ontoloviz-1.5.7/LICENSE
--rw-r--r--   0        0        0     1283 2023-03-30 06:45:50.008816 ontoloviz-1.5.7/pyproject.toml
--rw-r--r--   0        0        0    12995 2023-03-28 12:58:44.966237 ontoloviz-1.5.7/README.md
--rw-r--r--   0        0        0      136 2023-03-28 10:42:47.939554 ontoloviz-1.5.7/src/ontoloviz/__init__.py
--rw-r--r--   0        0        0      188 2023-03-28 09:03:18.306372 ontoloviz-1.5.7/src/ontoloviz/__main__.py
--rw-r--r--   0        0        0    90615 2023-03-28 12:58:44.968237 ontoloviz-1.5.7/src/ontoloviz/app.py
--rw-r--r--   0        0        0     2557 2023-03-24 16:20:52.682125 ontoloviz-1.5.7/src/ontoloviz/app_test.py
--rw-r--r--   0        0        0    72658 2023-03-27 16:12:35.656096 ontoloviz-1.5.7/src/ontoloviz/core.py
--rw-r--r--   0        0        0    13905 1970-01-01 00:00:00.000000 ontoloviz-1.5.7/setup.py
--rw-r--r--   0        0        0    14264 1970-01-01 00:00:00.000000 ontoloviz-1.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-13 11:21:27.456032 ontoloviz-1.5.8/LICENSE
+-rw-r--r--   0        0        0     1288 2023-04-13 13:12:44.429435 ontoloviz-1.5.8/pyproject.toml
+-rw-r--r--   0        0        0    12765 2023-04-13 11:46:00.664220 ontoloviz-1.5.8/README.md
+-rw-r--r--   0        0        0      136 2023-04-13 11:21:27.459820 ontoloviz-1.5.8/src/ontoloviz/__init__.py
+-rw-r--r--   0        0        0      188 2023-04-13 11:21:27.459820 ontoloviz-1.5.8/src/ontoloviz/__main__.py
+-rw-r--r--   0        0        0    91284 2023-04-13 13:10:35.210685 ontoloviz-1.5.8/src/ontoloviz/app.py
+-rw-r--r--   0        0        0     2557 2023-04-13 11:21:27.460826 ontoloviz-1.5.8/src/ontoloviz/app_test.py
+-rw-r--r--   0        0        0    73044 2023-04-13 12:35:01.987516 ontoloviz-1.5.8/src/ontoloviz/core.py
+-rw-r--r--   0        0        0    13680 1970-01-01 00:00:00.000000 ontoloviz-1.5.8/setup.py
+-rw-r--r--   0        0        0    13993 1970-01-01 00:00:00.000000 ontoloviz-1.5.8/PKG-INFO
```

### Comparing `ontoloviz-1.5.7/LICENSE` & `ontoloviz-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ontoloviz-1.5.7/pyproject.toml` & `ontoloviz-1.5.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ontoloviz"
-version = "1.5.7"
+version = "1.5.8"
 description = "OntoloViz drug- and phenotype-ontology visualization GUI"
 authors = ["Matthias Ley <matthias.ley@delta4.ai>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
@@ -14,22 +14,22 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["MeSH", "ATC", "ontology", "visualization", "sunburst", "drug", "phenotype", "GUI"]
-repository = "https://github.com/Mnikley/OntoloViz"
+repository = "https://github.com/Delta4AI/OntoloViz"
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/Mnikley/OntoloViz/issues"
-"Releases" = "https://github.com/Mnikley/OntoloViz/releases"
+"Bug Tracker" = "https://github.com/Delta4AI/OntoloViz/issues"
+"Releases" = "https://github.com/Delta4AI/OntoloViz/releases"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.7.1"
 plotly = "^5.13.1"
 openpyxl = "^3.1.2"
 packaging = "^23.0"
 
 [tool.poetry.scripts]
 ontoloviz = "ontoloviz.app:run_app"
```

### Comparing `ontoloviz-1.5.7/README.md` & `ontoloviz-1.5.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [![Pypi version](https://img.shields.io/pypi/v/OntoloViz.svg)](https://pypi.python.org/pypi/ontoloviz)
 [![Pypi python version](https://img.shields.io/pypi/pyversions/ontoloviz)](https://img.shields.io/pypi/pyversions/ontoloviz)
-[![Python package](https://github.com/Mnikley/OntoloViz/actions/workflows/python-package.yml/badge.svg)](https://github.com/Mnikley/OntoloViz/actions/workflows/python-package.yml)
-[![pylint-badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Mnikley/303283c4b9026d59cda9e9dd9f697110/raw/pylint_badge.json)](https://github.com/Mnikley/OntoloViz/actions/workflows/pylint.yml)
+[![Python package](https://github.com/Delta4AI/OntoloViz/actions/workflows/python-package.yml/badge.svg)](https://github.com/Delta4AI/OntoloViz/actions/workflows/python-package.yml)
+[![pylint-badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Delta4AI/303283c4b9026d59cda9e9dd9f697110/raw/pylint_badge.json)](https://github.com/Delta4AI/OntoloViz/actions/workflows/pylint.yml)
 <!--- documentation for pylint-badge: https://github.com/marketplace/actions/dynamic-badges --->
-<!--- [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5a8acbc6ebf541878336b75a1816beef)](https://www.codacy.com?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Mnikley/OntoloViz&amp;utm_campaign=Badge_Grade) --->
 
 OntoloViz
 =========
 
 OntoloViz is a graphical user interface for the creation of interactive sunburst plots of phenotype and drug ontologies.
 You might find it useful to quickly visualize your data for reports or to share the generated plots with collaborators.
 Take a look at the [screenshot and demos section](#screenshots-and-demos) or explore examples in `.html` format from the
-provided [templates.zip](https://github.com/Mnikley/OntoloViz/releases/download/v1.0.3/templates.zip) archive to get a 
+provided [templates.zip](https://github.com/Delta4AI/OntoloViz/releases/download/v1.0.3/templates.zip) archive to get a 
 better understanding of the scope of the package.  
 
 Quickstart
 ==========
-The GUI can be run by downloading the latest [release](https://github.com/Mnikley/OntoloViz/releases) 
+The GUI can be run by downloading the latest [release](https://github.com/Delta4AI/OntoloViz/releases) 
 or by installing the package via PyPi (OS independent, requires **Python 3.7+**):
 
     pip install ontoloviz
 
 After the installation you can run the GUI from the command line with the following command:
 
     ontoloviz
 
 Empty templates or pre-populated examples can be found in the `templates.zip` file in the 
-[release](https://github.com/Mnikley/OntoloViz/releases) section as well.
+[release](https://github.com/Delta4AI/OntoloViz/releases) section as well.
 Alternatively, you can clone this repository, install the required dependencies and launch the GUI:
 
-    git clone https://github.com/Mnikley/OntoloViz.git
+    git clone https://github.com/Delta4AI/OntoloViz.git
     
     # optional: install and activate venv
     python -m venv  # python3 on linux
     venv\scripts\activate  # source venv/bin/activate on linux
     
     # install dependencies
     pip install plotly>=5 openpyxl>=3
@@ -147,15 +146,15 @@
 | 4            | Counts [Name] | Required count for wedge weights, `Name` will be used as figure title          |
 | 5            | Color         | Optional color for the sunburst wedges, must be hex-string in format `#FFFFFF` |
 
 
 Templates and Examples
 ======================
 Templates and examples can be found in the provided 
-[templates.zip](https://github.com/Mnikley/OntoloViz/releases/download/v1.0.3/templates.zip) archive.
+[templates.zip](https://github.com/Delta4AI/OntoloViz/releases/download/v1.0.3/templates.zip) archive.
 
 - `pubmed_documents_mapped_to_mesh.tsv`: based on the [MeSH](https://meshb.nlm.nih.gov/treeView) subtree `C` from 2022. 
   Disease-related MeSH terms were extracted from the publicly available [PubMed](https://pubmed.ncbi.nlm.nih.gov/) 
   database (title + abstract) and further mapped to the nodes.
 
 -  `mesh_tree_template.tsv`: empty template of the [MeSH](https://meshb.nlm.nih.gov/treeView) tree `C` and `F03`]. 
   Terms are unique and mapped to all related parent nodes.
@@ -175,15 +174,15 @@
 =====================
 <img width="90%" alt="demo_creation_of_template" src="https://user-images.githubusercontent.com/75040444/228224565-af02a994-00c7-4572-b1da-f1eeec8b6f8f.gif">
 
 > **_Demo 1:_** Minimal example for creating a phenotype based ontology
 
 <img width="90%" alt="demo_creation_of_template" src="https://user-images.githubusercontent.com/75040444/228226839-2ed34f87-7a7d-498a-9f16-fd940d05c18d.gif">
 
-> **_Demo 2:_** Showcase of some of the features available in OntoloViz (used template: <a href="https://github.com/Mnikley/OntoloViz/files/11088919/test_tree.zip">test_tree.zip</a>)
+> **_Demo 2:_** Showcase of some of the features available in OntoloViz (used template: <a href="https://github.com/Delta4AI/OntoloViz/files/11088919/test_tree.zip">test_tree.zip</a>)
 
 <img width="90%" alt="drug_single" src="https://user-images.githubusercontent.com/75040444/228172370-a042b9d1-81af-4172-8b41-4f8c9e9287b7.png">
 
 > **_Screenshot 1:_**  Drug sunburst plot with enabled labels, counts propagated up to level 3
 
 <img width="90%" alt="phenotype_overview" src="https://user-images.githubusercontent.com/75040444/228174582-82aaad41-f3d8-4152-8161-b8f9b1dfec67.png">
```

### Comparing `ontoloviz-1.5.7/src/ontoloviz/app.py` & `ontoloviz-1.5.8/src/ontoloviz/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,14 +285,15 @@
         self.show_border = None
         self.show_border_btn_mesh = None
         self.show_border_btn_atc = None
         self.show_border_tt_template = None
         self.load_file_btn = None
         self.atc_file_loaded = ""
         self.mesh_file_loaded = ""
+        self.performance_warning_shown = False
 
         # various templates
         self.alt_text_db = "This functionality requires a valid database"
         self.alt_text = "This functionality requires a valid database or a loaded file"
         self.color_scale_tt_template = str("Define a custom color scale for the sunburst.\n"
                                            "Requires active propagation, overwrites colors defined "
                                            "in file. \nCurrent scale: ")
@@ -1205,14 +1206,22 @@
             if not self.check_init(obj):
                 return
             populate_data_source(asset, datasource)
 
         # update settings of core object based on current GUI configuration
         configure()
 
+        # show warning once in case labels and summary plot is enabled
+        if not self.performance_warning_shown and obj.s[f"{mode}_summary_plot"] and obj.s[f"{mode}_labels"] == "all":
+            messagebox.showwarning(title="Performance of plot",
+                                   message="Displaying very large ontologies as a summary plot and displaying all "
+                                           "associated labels may result in longer loading times and less responsive "
+                                           "interaction in the browser.")
+            self.performance_warning_shown = True
+
         # launch plot creation as thread
         thread = Thread(target=obj.plot, args=())
         thread.start()
 
         # disable UI
         self.toggle_widgets(enable=False, mode="recent")
```

### Comparing `ontoloviz-1.5.7/src/ontoloviz/app_test.py` & `ontoloviz-1.5.8/src/ontoloviz/app_test.py`

 * *Files identical despite different names*

### Comparing `ontoloviz-1.5.7/src/ontoloviz/core.py` & `ontoloviz-1.5.8/src/ontoloviz/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,15 +732,21 @@
         ) for idx, v in enumerate(plot_tree.values())]
 
         # plot configuration
         config = {"displaylogo": False,
                   "responsive": True,
                   "scrollZoom": True,
                   "displayModeBar": True,
-                  "showLink": False}
+                  "showLink": False,
+                  "toImageButtonOptions": {
+                      "format": "png",  # one of png, svg, jpeg, webp
+                      "height": None,  # download at the currently-rendered size by setting height and width to None
+                      "width": None,
+                      "scale": 3  # Multiply title/legend/axis/canvas sizes by this factor
+                  }}
 
         # generate headers
         headers, summary_plot, title, file_name = None, None, None, None
         if isinstance(self, PhenotypeSunburst):
             headers = [v[k]["label"] for k, v in sorted(self.mesh_tree.items())
                        if k in plot_tree.keys()]
             summary_plot = self.s["mesh_summary_plot"]
```

### Comparing `ontoloviz-1.5.7/setup.py` & `ontoloviz-1.5.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 ['openpyxl>=3.1.2,<4.0.0', 'packaging>=23.0,<24.0', 'plotly>=5.13.1,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['ontoloviz = ontoloviz.app:run_app']}
 
 setup_kwargs = {
     'name': 'ontoloviz',
-    'version': '1.5.7',
+    'version': '1.5.8',
     'description': 'OntoloViz drug- and phenotype-ontology visualization GUI',
-    'long_description': '[![Pypi version](https://img.shields.io/pypi/v/OntoloViz.svg)](https://pypi.python.org/pypi/ontoloviz)\n[![Pypi python version](https://img.shields.io/pypi/pyversions/ontoloviz)](https://img.shields.io/pypi/pyversions/ontoloviz)\n[![Python package](https://github.com/Mnikley/OntoloViz/actions/workflows/python-package.yml/badge.svg)](https://github.com/Mnikley/OntoloViz/actions/workflows/python-package.yml)\n[![pylint-badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Mnikley/303283c4b9026d59cda9e9dd9f697110/raw/pylint_badge.json)](https://github.com/Mnikley/OntoloViz/actions/workflows/pylint.yml)\n<!--- documentation for pylint-badge: https://github.com/marketplace/actions/dynamic-badges --->\n<!--- [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5a8acbc6ebf541878336b75a1816beef)](https://www.codacy.com?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Mnikley/OntoloViz&amp;utm_campaign=Badge_Grade) --->\n\nOntoloViz\n=========\n\nOntoloViz is a graphical user interface for the creation of interactive sunburst plots of phenotype and drug ontologies.\nYou might find it useful to quickly visualize your data for reports or to share the generated plots with collaborators.\nTake a look at the [screenshot and demos section](#screenshots-and-demos) or explore examples in `.html` format from the\nprovided [templates.zip](https://github.com/Mnikley/OntoloViz/releases/download/v1.0.3/templates.zip) archive to get a \nbetter understanding of the scope of the package.  \n\nQuickstart\n==========\nThe GUI can be run by downloading the latest [release](https://github.com/Mnikley/OntoloViz/releases) \nor by installing the package via PyPi (OS independent, requires **Python 3.7+**):\n\n    pip install ontoloviz\n\nAfter the installation you can run the GUI from the command line with the following command:\n\n    ontoloviz\n\nEmpty templates or pre-populated examples can be found in the `templates.zip` file in the \n[release](https://github.com/Mnikley/OntoloViz/releases) section as well.\nAlternatively, you can clone this repository, install the required dependencies and launch the GUI:\n\n    git clone https://github.com/Mnikley/OntoloViz.git\n    \n    # optional: install and activate venv\n    python -m venv  # python3 on linux\n    venv\\scripts\\activate  # source venv/bin/activate on linux\n    \n    # install dependencies\n    pip install plotly>=5 openpyxl>=3\n    \n    # launch GUI\n    cd OntoloViz/src\n    python -c "from ontoloviz import run_app; run_app()"\n\nUsage\n=====\n\nThe application allows importing `.tsv` and `.xlsx` files, but the use of `.tsv` and `tab` as a \nseparator is recommended. The GUI can create two types of sunburst diagrams to represent either phenotype or drug \nontologies, which is determined by the structure of the loaded files. Any numbers entered in the file will be converted \nto integers.\n\nGUI Options\n-----------\n<img height=250px alt="gui_small" src="https://user-images.githubusercontent.com/75040444/228182954-fb48a953-ec56-46db-81ad-816d9f356206.png">\n\n- **Load File**: load an `.tsv` or `.xlsx` file containing drug- or phenotype-ontology data\n- General\n  - **Set Color Scale**: define a custom color scale for the sunburst color scaling when color propagation is active\n  - **Set Border**: configures the border properties drawn around sunburst wedges\n- Display\n  - **Drop empty nodes** (phenotype sunburst only): drops nodes who have no further children and 0 counts\n  - **Wedge Width** (drug sunburst only): switch from full outer circle (total) to count-based wedge widths (remainder)\n  - **Display Labels**: controls display of labels inside sunburst wedges, available options:\n    - `all`\n    - `propagation`\n    - `drugs` (drug sunburst only)\n    - `none`\n- Propagation\n  - **Enable**: enables count- and color propagation from child to parent nodes\n  - **Color**: controls color propagation by the options:\n    - `off`: color scale is based on \'Color\' column from imported file\n    - `specific`: color scale is based on the maximum values of the corresponding subtree\n    - `global`: color scale is based on the maximum values of the entire tree ontology\n    - `phenotype` (phenotype sunburst only): Only the most outer phenotype in a branch is colored\n  - **Counts**: controls count propagation by the options:\n    - `off`: no counts are propagated, counts equal imported values\n    - `level`: counts are propagated up to defined level, values above threshold remain unchanged\n    - `all`: counts are propagated up to central node, imported values are corrected and overwritten\n  - **Level**: controls color- and count-propagation from outer to inner levels up to defined level\n    - affects color propagation when **Color** is set to `specific` or `global`\n    - affects count propagation when **Counts** is set to `level`\n    - drug sunburst: 1 corresponds to the central node, 5 to the outermost node (=drug)\n    - phenotype sunburst: 0 corresponds to the central node, 13 to the outermost node\n- Summary Plot\n  - **Enable**: displays all available subtrees in a single view\n    (resource intensive, set Labels to `none` for faster loading)\n  - **Columns**: defines the amount of columns when summary plot is enabled\n- **Save**: when enabled, an interactive `.html` file is generated for later use\n- **Plot**: Process and generate plot, opens in a Browser window\n\nPhenotype Sunbursts\n-------------------\nThe phenotype sunburst structure follows the principles of the \n[MeSH tree](https://www.nlm.nih.gov/mesh/intro_trees.html).\n- A Tree ID is defined by a **combination of three numbers or letters**, for example `C01`.\n- Levels are separated by a **dot `.`**, for example `C01.001`.\n- Ontologies **up to thirteen hierarchical levels** are supported.\n- A single phenotype end-node can be assigned to multiple parent-nodes by specifying the parents tree ids as \n  pipe separated string in the column `Tree ID`.\n- When defining a child element which has no valid parent, the GUI will automatically generate the parent with the \n  default color and a 0 value. This will happen recursively. For example, if the input file defines a node with the \n  id `123.001.001`, but the nodes `123` and `123.001` are non-existent, they will be created.\n- Counts entered in the file will be converted to integers. If a node should be displayed without counts, use `0`.\n- The loaded file must contain **7 columns** and follow the below structure to be correctly recognized:\n\nPhenotype Ontology File Structure\n---------------------------------\n\n| Column Index | Header Text   | Description                                                                    |\n|--------------|---------------|--------------------------------------------------------------------------------|\n| 0            | MeSH ID       | Required primary identifier of a node in format `C01.001`                      |\n| 1            | Tree ID       | Required pipe delimited list of Tree IDs of a node (allows 1:N mappings)       |\n| 2            | Name          | Optional label to be displayed inside the sunburst wedges                      |\n| 3            | Description   | Optional description displayed in the sunburst wedge tooltip                   |\n| 4            | Comment       | Optional comment displayed in the sunburst wedge tooltip                       |\n| 5            | Counts [Name] | Required count for wedge weights, `Name` will be used as figure title          | \n| 6            | Color         | Optional color for the sunburst wedges, must be hex-string in format `#FFFFFF` |\n\n\nDrug Sunbursts\n--------------\nThe drug sunburst structure follows the principles of the \n[ATC tree](https://www.who.int/tools/atc-ddd-toolkit/atc-classification).\n- ATC codes are divided into **five levels**, which must follow the following naming conventions:\n  - 1st level: letter\n  - 2nd level: two numbers\n  - 3rd level: letter\n  - 4th level: letter\n  - 5th level: two numbers\n- Example ATC code: **A10BA02**\n- The hierarchy is built based on the above-mentioned format and does only allow 1:1 child-parent relationships\n  (contrary to the phenotype structure). For example, if the drug `deltatonin` should be assigned to the \n  parent nodes `A01AA` and `B01BB`, it must be defined twice with the ids `A01AA01` and `B01BB01`.\n- The loaded file must contain **6 columns** and follow the below structure to be correctly recognized as a phenotype \n  ontology:\n\nDrug Ontology File Structure\n----------------------------\n\n| Column Index | Header Text   | Description                                                                    |\n|--------------|---------------|--------------------------------------------------------------------------------|\n| 0            | ATC code      | Required primary identifier of a node in format `A10BA02`                      |\n| 1            | Level         | Optional level as number, not used for building tree                           |\n| 2            | Label         | Optional label to be displayed inside the sunburst wedges                      |\n| 3            | Comment       | Optional comment displayed in the sunburst wedge tooltip                       |\n| 4            | Counts [Name] | Required count for wedge weights, `Name` will be used as figure title          |\n| 5            | Color         | Optional color for the sunburst wedges, must be hex-string in format `#FFFFFF` |\n\n\nTemplates and Examples\n======================\nTemplates and examples can be found in the provided \n[templates.zip](https://github.com/Mnikley/OntoloViz/releases/download/v1.0.3/templates.zip) archive.\n\n- `pubmed_documents_mapped_to_mesh.tsv`: based on the [MeSH](https://meshb.nlm.nih.gov/treeView) subtree `C` from 2022. \n  Disease-related MeSH terms were extracted from the publicly available [PubMed](https://pubmed.ncbi.nlm.nih.gov/) \n  database (title + abstract) and further mapped to the nodes.\n\n-  `mesh_tree_template.tsv`: empty template of the [MeSH](https://meshb.nlm.nih.gov/treeView) tree `C` and `F03`]. \n  Terms are unique and mapped to all related parent nodes.\n\n-  `covid_drugs_trial_summary.tsv`: based on [publicly available clinical trial data](https://clinicaltrials.gov/) \n  related to COVID-19. One count represents one clinical trial.\n\n- `atc_tree_template.tsv`: empty template of the [ATC](https://www.who.int/tools/atc-ddd-toolkit/atc-classification) \n  tree based on the manually curated chemical database of bioactive \n  molecules [ChEMBL v29](https://chembl.gitbook.io/chembl-interface-documentation/downloads).\n\n- `drug_sunburst_example.html`: sample plot generated with the provided `covid_drugs_trial_summary.tsv` file.\n\n- `phenotype_sunburst_example.html`: sample plot generated with the provided `covid_drugs_trial_summary.tsv` file.\n\nScreenshots and Demos\n=====================\n<img width="90%" alt="demo_creation_of_template" src="https://user-images.githubusercontent.com/75040444/228224565-af02a994-00c7-4572-b1da-f1eeec8b6f8f.gif">\n\n> **_Demo 1:_** Minimal example for creating a phenotype based ontology\n\n<img width="90%" alt="demo_creation_of_template" src="https://user-images.githubusercontent.com/75040444/228226839-2ed34f87-7a7d-498a-9f16-fd940d05c18d.gif">\n\n> **_Demo 2:_** Showcase of some of the features available in OntoloViz (used template: <a href="https://github.com/Mnikley/OntoloViz/files/11088919/test_tree.zip">test_tree.zip</a>)\n\n<img width="90%" alt="drug_single" src="https://user-images.githubusercontent.com/75040444/228172370-a042b9d1-81af-4172-8b41-4f8c9e9287b7.png">\n\n> **_Screenshot 1:_**  Drug sunburst plot with enabled labels, counts propagated up to level 3\n\n<img width="90%" alt="phenotype_overview" src="https://user-images.githubusercontent.com/75040444/228174582-82aaad41-f3d8-4152-8161-b8f9b1dfec67.png">\n\n> **_Screenshot 2:_**  Summary phenotype sunburst plot with tooltip, counts propagated up to the central node, color coded\n\n<table>\n    <tr>\n        <td>\n            <img height=300px alt="color_scale" src="https://user-images.githubusercontent.com/75040444/228183209-6a591a3c-8729-45c9-a73b-817dce9252c1.png">\n        </td>\n        <td>\n            <img height=300px alt="color_scale" src="https://user-images.githubusercontent.com/75040444/228183234-e6aecf82-64b4-4737-b5c3-95eb87b0fb59.png">\n        </td>\n    </tr>\n</table>\n\n> **_Screenshot 3 & 4:_**  Left: define automatic color scales based on defined counts with thresholds and hex color codes, Right: define border properties (width, opacity, colors) or disable them entirely\n\nSpecial Thanks to\n=================\n\n* Paul Perco, who had the initial idea for this package and provided support throughout the entire process\n* Andreas Heinzel, for inspiration regarding architectural- and software-related topics\n* The Delta4 GmbH team for providing helpful inputs\n',
+    'long_description': '[![Pypi version](https://img.shields.io/pypi/v/OntoloViz.svg)](https://pypi.python.org/pypi/ontoloviz)\n[![Pypi python version](https://img.shields.io/pypi/pyversions/ontoloviz)](https://img.shields.io/pypi/pyversions/ontoloviz)\n[![Python package](https://github.com/Delta4AI/OntoloViz/actions/workflows/python-package.yml/badge.svg)](https://github.com/Delta4AI/OntoloViz/actions/workflows/python-package.yml)\n[![pylint-badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Delta4AI/303283c4b9026d59cda9e9dd9f697110/raw/pylint_badge.json)](https://github.com/Delta4AI/OntoloViz/actions/workflows/pylint.yml)\n<!--- documentation for pylint-badge: https://github.com/marketplace/actions/dynamic-badges --->\n\nOntoloViz\n=========\n\nOntoloViz is a graphical user interface for the creation of interactive sunburst plots of phenotype and drug ontologies.\nYou might find it useful to quickly visualize your data for reports or to share the generated plots with collaborators.\nTake a look at the [screenshot and demos section](#screenshots-and-demos) or explore examples in `.html` format from the\nprovided [templates.zip](https://github.com/Delta4AI/OntoloViz/releases/download/v1.0.3/templates.zip) archive to get a \nbetter understanding of the scope of the package.  \n\nQuickstart\n==========\nThe GUI can be run by downloading the latest [release](https://github.com/Delta4AI/OntoloViz/releases) \nor by installing the package via PyPi (OS independent, requires **Python 3.7+**):\n\n    pip install ontoloviz\n\nAfter the installation you can run the GUI from the command line with the following command:\n\n    ontoloviz\n\nEmpty templates or pre-populated examples can be found in the `templates.zip` file in the \n[release](https://github.com/Delta4AI/OntoloViz/releases) section as well.\nAlternatively, you can clone this repository, install the required dependencies and launch the GUI:\n\n    git clone https://github.com/Delta4AI/OntoloViz.git\n    \n    # optional: install and activate venv\n    python -m venv  # python3 on linux\n    venv\\scripts\\activate  # source venv/bin/activate on linux\n    \n    # install dependencies\n    pip install plotly>=5 openpyxl>=3\n    \n    # launch GUI\n    cd OntoloViz/src\n    python -c "from ontoloviz import run_app; run_app()"\n\nUsage\n=====\n\nThe application allows importing `.tsv` and `.xlsx` files, but the use of `.tsv` and `tab` as a \nseparator is recommended. The GUI can create two types of sunburst diagrams to represent either phenotype or drug \nontologies, which is determined by the structure of the loaded files. Any numbers entered in the file will be converted \nto integers.\n\nGUI Options\n-----------\n<img height=250px alt="gui_small" src="https://user-images.githubusercontent.com/75040444/228182954-fb48a953-ec56-46db-81ad-816d9f356206.png">\n\n- **Load File**: load an `.tsv` or `.xlsx` file containing drug- or phenotype-ontology data\n- General\n  - **Set Color Scale**: define a custom color scale for the sunburst color scaling when color propagation is active\n  - **Set Border**: configures the border properties drawn around sunburst wedges\n- Display\n  - **Drop empty nodes** (phenotype sunburst only): drops nodes who have no further children and 0 counts\n  - **Wedge Width** (drug sunburst only): switch from full outer circle (total) to count-based wedge widths (remainder)\n  - **Display Labels**: controls display of labels inside sunburst wedges, available options:\n    - `all`\n    - `propagation`\n    - `drugs` (drug sunburst only)\n    - `none`\n- Propagation\n  - **Enable**: enables count- and color propagation from child to parent nodes\n  - **Color**: controls color propagation by the options:\n    - `off`: color scale is based on \'Color\' column from imported file\n    - `specific`: color scale is based on the maximum values of the corresponding subtree\n    - `global`: color scale is based on the maximum values of the entire tree ontology\n    - `phenotype` (phenotype sunburst only): Only the most outer phenotype in a branch is colored\n  - **Counts**: controls count propagation by the options:\n    - `off`: no counts are propagated, counts equal imported values\n    - `level`: counts are propagated up to defined level, values above threshold remain unchanged\n    - `all`: counts are propagated up to central node, imported values are corrected and overwritten\n  - **Level**: controls color- and count-propagation from outer to inner levels up to defined level\n    - affects color propagation when **Color** is set to `specific` or `global`\n    - affects count propagation when **Counts** is set to `level`\n    - drug sunburst: 1 corresponds to the central node, 5 to the outermost node (=drug)\n    - phenotype sunburst: 0 corresponds to the central node, 13 to the outermost node\n- Summary Plot\n  - **Enable**: displays all available subtrees in a single view\n    (resource intensive, set Labels to `none` for faster loading)\n  - **Columns**: defines the amount of columns when summary plot is enabled\n- **Save**: when enabled, an interactive `.html` file is generated for later use\n- **Plot**: Process and generate plot, opens in a Browser window\n\nPhenotype Sunbursts\n-------------------\nThe phenotype sunburst structure follows the principles of the \n[MeSH tree](https://www.nlm.nih.gov/mesh/intro_trees.html).\n- A Tree ID is defined by a **combination of three numbers or letters**, for example `C01`.\n- Levels are separated by a **dot `.`**, for example `C01.001`.\n- Ontologies **up to thirteen hierarchical levels** are supported.\n- A single phenotype end-node can be assigned to multiple parent-nodes by specifying the parents tree ids as \n  pipe separated string in the column `Tree ID`.\n- When defining a child element which has no valid parent, the GUI will automatically generate the parent with the \n  default color and a 0 value. This will happen recursively. For example, if the input file defines a node with the \n  id `123.001.001`, but the nodes `123` and `123.001` are non-existent, they will be created.\n- Counts entered in the file will be converted to integers. If a node should be displayed without counts, use `0`.\n- The loaded file must contain **7 columns** and follow the below structure to be correctly recognized:\n\nPhenotype Ontology File Structure\n---------------------------------\n\n| Column Index | Header Text   | Description                                                                    |\n|--------------|---------------|--------------------------------------------------------------------------------|\n| 0            | MeSH ID       | Required primary identifier of a node in format `C01.001`                      |\n| 1            | Tree ID       | Required pipe delimited list of Tree IDs of a node (allows 1:N mappings)       |\n| 2            | Name          | Optional label to be displayed inside the sunburst wedges                      |\n| 3            | Description   | Optional description displayed in the sunburst wedge tooltip                   |\n| 4            | Comment       | Optional comment displayed in the sunburst wedge tooltip                       |\n| 5            | Counts [Name] | Required count for wedge weights, `Name` will be used as figure title          | \n| 6            | Color         | Optional color for the sunburst wedges, must be hex-string in format `#FFFFFF` |\n\n\nDrug Sunbursts\n--------------\nThe drug sunburst structure follows the principles of the \n[ATC tree](https://www.who.int/tools/atc-ddd-toolkit/atc-classification).\n- ATC codes are divided into **five levels**, which must follow the following naming conventions:\n  - 1st level: letter\n  - 2nd level: two numbers\n  - 3rd level: letter\n  - 4th level: letter\n  - 5th level: two numbers\n- Example ATC code: **A10BA02**\n- The hierarchy is built based on the above-mentioned format and does only allow 1:1 child-parent relationships\n  (contrary to the phenotype structure). For example, if the drug `deltatonin` should be assigned to the \n  parent nodes `A01AA` and `B01BB`, it must be defined twice with the ids `A01AA01` and `B01BB01`.\n- The loaded file must contain **6 columns** and follow the below structure to be correctly recognized as a phenotype \n  ontology:\n\nDrug Ontology File Structure\n----------------------------\n\n| Column Index | Header Text   | Description                                                                    |\n|--------------|---------------|--------------------------------------------------------------------------------|\n| 0            | ATC code      | Required primary identifier of a node in format `A10BA02`                      |\n| 1            | Level         | Optional level as number, not used for building tree                           |\n| 2            | Label         | Optional label to be displayed inside the sunburst wedges                      |\n| 3            | Comment       | Optional comment displayed in the sunburst wedge tooltip                       |\n| 4            | Counts [Name] | Required count for wedge weights, `Name` will be used as figure title          |\n| 5            | Color         | Optional color for the sunburst wedges, must be hex-string in format `#FFFFFF` |\n\n\nTemplates and Examples\n======================\nTemplates and examples can be found in the provided \n[templates.zip](https://github.com/Delta4AI/OntoloViz/releases/download/v1.0.3/templates.zip) archive.\n\n- `pubmed_documents_mapped_to_mesh.tsv`: based on the [MeSH](https://meshb.nlm.nih.gov/treeView) subtree `C` from 2022. \n  Disease-related MeSH terms were extracted from the publicly available [PubMed](https://pubmed.ncbi.nlm.nih.gov/) \n  database (title + abstract) and further mapped to the nodes.\n\n-  `mesh_tree_template.tsv`: empty template of the [MeSH](https://meshb.nlm.nih.gov/treeView) tree `C` and `F03`]. \n  Terms are unique and mapped to all related parent nodes.\n\n-  `covid_drugs_trial_summary.tsv`: based on [publicly available clinical trial data](https://clinicaltrials.gov/) \n  related to COVID-19. One count represents one clinical trial.\n\n- `atc_tree_template.tsv`: empty template of the [ATC](https://www.who.int/tools/atc-ddd-toolkit/atc-classification) \n  tree based on the manually curated chemical database of bioactive \n  molecules [ChEMBL v29](https://chembl.gitbook.io/chembl-interface-documentation/downloads).\n\n- `drug_sunburst_example.html`: sample plot generated with the provided `covid_drugs_trial_summary.tsv` file.\n\n- `phenotype_sunburst_example.html`: sample plot generated with the provided `covid_drugs_trial_summary.tsv` file.\n\nScreenshots and Demos\n=====================\n<img width="90%" alt="demo_creation_of_template" src="https://user-images.githubusercontent.com/75040444/228224565-af02a994-00c7-4572-b1da-f1eeec8b6f8f.gif">\n\n> **_Demo 1:_** Minimal example for creating a phenotype based ontology\n\n<img width="90%" alt="demo_creation_of_template" src="https://user-images.githubusercontent.com/75040444/228226839-2ed34f87-7a7d-498a-9f16-fd940d05c18d.gif">\n\n> **_Demo 2:_** Showcase of some of the features available in OntoloViz (used template: <a href="https://github.com/Delta4AI/OntoloViz/files/11088919/test_tree.zip">test_tree.zip</a>)\n\n<img width="90%" alt="drug_single" src="https://user-images.githubusercontent.com/75040444/228172370-a042b9d1-81af-4172-8b41-4f8c9e9287b7.png">\n\n> **_Screenshot 1:_**  Drug sunburst plot with enabled labels, counts propagated up to level 3\n\n<img width="90%" alt="phenotype_overview" src="https://user-images.githubusercontent.com/75040444/228174582-82aaad41-f3d8-4152-8161-b8f9b1dfec67.png">\n\n> **_Screenshot 2:_**  Summary phenotype sunburst plot with tooltip, counts propagated up to the central node, color coded\n\n<table>\n    <tr>\n        <td>\n            <img height=300px alt="color_scale" src="https://user-images.githubusercontent.com/75040444/228183209-6a591a3c-8729-45c9-a73b-817dce9252c1.png">\n        </td>\n        <td>\n            <img height=300px alt="color_scale" src="https://user-images.githubusercontent.com/75040444/228183234-e6aecf82-64b4-4737-b5c3-95eb87b0fb59.png">\n        </td>\n    </tr>\n</table>\n\n> **_Screenshot 3 & 4:_**  Left: define automatic color scales based on defined counts with thresholds and hex color codes, Right: define border properties (width, opacity, colors) or disable them entirely\n\nSpecial Thanks to\n=================\n\n* Paul Perco, who had the initial idea for this package and provided support throughout the entire process\n* Andreas Heinzel, for inspiration regarding architectural- and software-related topics\n* The Delta4 GmbH team for providing helpful inputs\n',
     'author': 'Matthias Ley',
     'author_email': 'matthias.ley@delta4.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/Mnikley/OntoloViz',
+    'url': 'https://github.com/Delta4AI/OntoloViz',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.7.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `ontoloviz-1.5.7/PKG-INFO` & `ontoloviz-1.5.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,70 @@
 Metadata-Version: 2.1
 Name: ontoloviz
-Version: 1.5.7
+Version: 1.5.8
 Summary: OntoloViz drug- and phenotype-ontology visualization GUI
-Home-page: https://github.com/Mnikley/OntoloViz
+Home-page: https://github.com/Delta4AI/OntoloViz
 License: MIT
 Keywords: MeSH,ATC,ontology,visualization,sunburst,drug,phenotype,GUI
 Author: Matthias Ley
 Author-email: matthias.ley@delta4.ai
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: plotly (>=5.13.1,<6.0.0)
-Project-URL: Bug Tracker, https://github.com/Mnikley/OntoloViz/issues
-Project-URL: Repository, https://github.com/Mnikley/OntoloViz
-Project-URL: Releases, https://github.com/Mnikley/OntoloViz/releases
+Project-URL: Bug Tracker, https://github.com/Delta4AI/OntoloViz/issues
+Project-URL: Repository, https://github.com/Delta4AI/OntoloViz
+Project-URL: Releases, https://github.com/Delta4AI/OntoloViz/releases
 Description-Content-Type: text/markdown
 
 [![Pypi version](https://img.shields.io/pypi/v/OntoloViz.svg)](https://pypi.python.org/pypi/ontoloviz)
 [![Pypi python version](https://img.shields.io/pypi/pyversions/ontoloviz)](https://img.shields.io/pypi/pyversions/ontoloviz)
-[![Python package](https://github.com/Mnikley/OntoloViz/actions/workflows/python-package.yml/badge.svg)](https://github.com/Mnikley/OntoloViz/actions/workflows/python-package.yml)
-[![pylint-badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Mnikley/303283c4b9026d59cda9e9dd9f697110/raw/pylint_badge.json)](https://github.com/Mnikley/OntoloViz/actions/workflows/pylint.yml)
+[![Python package](https://github.com/Delta4AI/OntoloViz/actions/workflows/python-package.yml/badge.svg)](https://github.com/Delta4AI/OntoloViz/actions/workflows/python-package.yml)
+[![pylint-badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Delta4AI/303283c4b9026d59cda9e9dd9f697110/raw/pylint_badge.json)](https://github.com/Delta4AI/OntoloViz/actions/workflows/pylint.yml)
 <!--- documentation for pylint-badge: https://github.com/marketplace/actions/dynamic-badges --->
-<!--- [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5a8acbc6ebf541878336b75a1816beef)](https://www.codacy.com?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Mnikley/OntoloViz&amp;utm_campaign=Badge_Grade) --->
 
 OntoloViz
 =========
 
 OntoloViz is a graphical user interface for the creation of interactive sunburst plots of phenotype and drug ontologies.
 You might find it useful to quickly visualize your data for reports or to share the generated plots with collaborators.
 Take a look at the [screenshot and demos section](#screenshots-and-demos) or explore examples in `.html` format from the
-provided [templates.zip](https://github.com/Mnikley/OntoloViz/releases/download/v1.0.3/templates.zip) archive to get a 
+provided [templates.zip](https://github.com/Delta4AI/OntoloViz/releases/download/v1.0.3/templates.zip) archive to get a 
 better understanding of the scope of the package.  
 
 Quickstart
 ==========
-The GUI can be run by downloading the latest [release](https://github.com/Mnikley/OntoloViz/releases) 
+The GUI can be run by downloading the latest [release](https://github.com/Delta4AI/OntoloViz/releases) 
 or by installing the package via PyPi (OS independent, requires **Python 3.7+**):
 
     pip install ontoloviz
 
 After the installation you can run the GUI from the command line with the following command:
 
     ontoloviz
 
 Empty templates or pre-populated examples can be found in the `templates.zip` file in the 
-[release](https://github.com/Mnikley/OntoloViz/releases) section as well.
+[release](https://github.com/Delta4AI/OntoloViz/releases) section as well.
 Alternatively, you can clone this repository, install the required dependencies and launch the GUI:
 
-    git clone https://github.com/Mnikley/OntoloViz.git
+    git clone https://github.com/Delta4AI/OntoloViz.git
     
     # optional: install and activate venv
     python -m venv  # python3 on linux
     venv\scripts\activate  # source venv/bin/activate on linux
     
     # install dependencies
     pip install plotly>=5 openpyxl>=3
@@ -180,15 +178,15 @@
 | 4            | Counts [Name] | Required count for wedge weights, `Name` will be used as figure title          |
 | 5            | Color         | Optional color for the sunburst wedges, must be hex-string in format `#FFFFFF` |
 
 
 Templates and Examples
 ======================
 Templates and examples can be found in the provided 
-[templates.zip](https://github.com/Mnikley/OntoloViz/releases/download/v1.0.3/templates.zip) archive.
+[templates.zip](https://github.com/Delta4AI/OntoloViz/releases/download/v1.0.3/templates.zip) archive.
 
 - `pubmed_documents_mapped_to_mesh.tsv`: based on the [MeSH](https://meshb.nlm.nih.gov/treeView) subtree `C` from 2022. 
   Disease-related MeSH terms were extracted from the publicly available [PubMed](https://pubmed.ncbi.nlm.nih.gov/) 
   database (title + abstract) and further mapped to the nodes.
 
 -  `mesh_tree_template.tsv`: empty template of the [MeSH](https://meshb.nlm.nih.gov/treeView) tree `C` and `F03`]. 
   Terms are unique and mapped to all related parent nodes.
@@ -208,15 +206,15 @@
 =====================
 <img width="90%" alt="demo_creation_of_template" src="https://user-images.githubusercontent.com/75040444/228224565-af02a994-00c7-4572-b1da-f1eeec8b6f8f.gif">
 
 > **_Demo 1:_** Minimal example for creating a phenotype based ontology
 
 <img width="90%" alt="demo_creation_of_template" src="https://user-images.githubusercontent.com/75040444/228226839-2ed34f87-7a7d-498a-9f16-fd940d05c18d.gif">
 
-> **_Demo 2:_** Showcase of some of the features available in OntoloViz (used template: <a href="https://github.com/Mnikley/OntoloViz/files/11088919/test_tree.zip">test_tree.zip</a>)
+> **_Demo 2:_** Showcase of some of the features available in OntoloViz (used template: <a href="https://github.com/Delta4AI/OntoloViz/files/11088919/test_tree.zip">test_tree.zip</a>)
 
 <img width="90%" alt="drug_single" src="https://user-images.githubusercontent.com/75040444/228172370-a042b9d1-81af-4172-8b41-4f8c9e9287b7.png">
 
 > **_Screenshot 1:_**  Drug sunburst plot with enabled labels, counts propagated up to level 3
 
 <img width="90%" alt="phenotype_overview" src="https://user-images.githubusercontent.com/75040444/228174582-82aaad41-f3d8-4152-8161-b8f9b1dfec67.png">
```

