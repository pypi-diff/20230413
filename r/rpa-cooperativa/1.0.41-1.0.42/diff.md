# Comparing `tmp/rpa_cooperativa-1.0.41.tar.gz` & `tmp/rpa_cooperativa-1.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.41.tar", last modified: Mon Apr 10 14:01:59 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.42.tar", last modified: Thu Apr 13 13:19:23 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.41.tar` & `rpa_cooperativa-1.0.42.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:01:59.747887 rpa_cooperativa-1.0.41/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.41/LICENSE
--rw-rw-rw-   0        0        0     5578 2023-04-10 14:01:59.742065 rpa_cooperativa-1.0.41/PKG-INFO
--rw-rw-rw-   0        0        0     4429 2023-04-10 13:24:59.000000 rpa_cooperativa-1.0.41/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 14:01:59.410355 rpa_cooperativa-1.0.41/rpa_coop/
--rw-rw-rw-   0        0        0      528 2023-04-10 13:18:19.000000 rpa_cooperativa-1.0.41/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:01:59.651274 rpa_cooperativa-1.0.41/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.41/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.41/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.41/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.41/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.41/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.41/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      347 2023-02-28 19:51:44.000000 rpa_cooperativa-1.0.41/rpa_coop/img/siac_verde.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.41/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0      336 2023-02-28 19:52:19.000000 rpa_cooperativa-1.0.41/rpa_coop/img/siat_verde.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.41/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.41/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    65069 2023-04-10 14:00:48.000000 rpa_cooperativa-1.0.41/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:01:59.723355 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     5578 2023-04-10 14:01:58.000000 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-04-10 14:01:58.000000 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:01:58.000000 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-10 14:01:58.000000 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      544 2023-04-10 14:01:58.000000 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-10 14:01:58.000000 rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 14:01:59.750886 rpa_cooperativa-1.0.41/setup.cfg
--rw-rw-rw-   0        0        0     2305 2023-04-10 12:54:19.000000 rpa_cooperativa-1.0.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:19:23.852287 rpa_cooperativa-1.0.42/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.42/LICENSE
+-rw-rw-rw-   0        0        0     5578 2023-04-13 13:19:23.843387 rpa_cooperativa-1.0.42/PKG-INFO
+-rw-rw-rw-   0        0        0     4429 2023-04-10 13:24:59.000000 rpa_cooperativa-1.0.42/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 13:19:23.567706 rpa_cooperativa-1.0.42/rpa_coop/
+-rw-rw-rw-   0        0        0      528 2023-04-10 13:18:19.000000 rpa_cooperativa-1.0.42/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:19:23.702805 rpa_cooperativa-1.0.42/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.42/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.42/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.42/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.42/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.42/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.42/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      347 2023-02-28 19:51:44.000000 rpa_cooperativa-1.0.42/rpa_coop/img/siac_verde.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.42/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0      336 2023-02-28 19:52:19.000000 rpa_cooperativa-1.0.42/rpa_coop/img/siat_verde.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.42/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.42/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    66470 2023-04-13 13:16:12.000000 rpa_cooperativa-1.0.42/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:19:23.832158 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     5578 2023-04-13 13:19:22.000000 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-04-13 13:19:23.000000 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 13:19:22.000000 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-13 13:19:22.000000 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      544 2023-04-13 13:19:22.000000 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 13:19:22.000000 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 13:19:23.854287 rpa_cooperativa-1.0.42/setup.cfg
+-rw-rw-rw-   0        0        0     2305 2023-04-13 13:18:16.000000 rpa_cooperativa-1.0.42/setup.py
```

### Comparing `rpa_cooperativa-1.0.41/LICENSE` & `rpa_cooperativa-1.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.41/PKG-INFO` & `rpa_cooperativa-1.0.42/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.41
+Version: 1.0.42
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.41/README.md` & `rpa_cooperativa-1.0.42/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.41/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.42/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.41/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.42/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.41/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.42/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.41/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.42/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.41/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.42/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.41/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.42/rpa_coop/rpa_coop.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 class Dados:
     
 
     def __init__(self):
         self.ip_planning = str(os.getenv('ip_planning'))
         self.user_planning = str(os.getenv('user_planning'))
         self.pw_bd_planning = str(urllib.parse.quote_plus(os.getenv('pw_bd_planning'))) 
+        
         self.user_planning_controles = str(gerador_pwd('user_planning_controles', 'senha'))
         self.pw_planning_controles = str(gerador_pwd('pw_planning_controles', 'senha'))
         
         self.ip_grafana = str(gerador_pwd('grafana', 'ip_host'))
         self.user_grafana = str(gerador_pwd('grafana', 'usuario'))
         self.pw_bd_grafana = str(urllib.parse.quote_plus(gerador_pwd('grafana', 'senha')))
         
@@ -108,14 +109,17 @@
         self.user_sistema_senhas = str(gerador_pwd('sistema_senhas', 'usuario'))
         self.database_sistema_senhas = str(gerador_pwd('sistema_senhas', 'db_name'))
         self.pw_bd_sistema_senhas = str(urllib.parse.quote_plus(gerador_pwd('sistema_senhas', 'senha')))
         
         self.ip_denodo = str(gerador_pwd('denodo_web', 'ip_host'))
         self.user_denodo = str(gerador_pwd('denodo_web', 'usuario'))
         self.pw_denodo = str(urllib.parse.quote_plus(gerador_pwd('denodo_web', 'senha')))
+        
+        self.token_api_denodo = str(gerador_pwd('token_api_denodo', 'senha'))
+        self.url_api_denodo = str(gerador_pwd('token_api_denodo', 'ip_host'))
 
         
     def criar_engine(self, db:str, user_db='user_opcional', password_db='senha_opcional', ip_ou_host_db='ip_host_opcional', porta='3306', library_sql='mysqlconnector'):
         '''
         retorna conexao com db, db='parametro_obrigatorio' \n
         schema planinng: db = ('planning', 'fluid', 'cronos', 'controles_internos') \n
         schema sistema_senhas: db = 'sistema_senhas' \n
@@ -163,14 +167,42 @@
             conexao = create_engine(f'mysql+mysqlconnector://{self.user_sistema_senhas}:{self.pw_bd_sistema_senhas}@{self.ip_sistema_senhas}:3307/{banco}')
             # conexao = mysql.connect(host=self.ip_sistema_senhas, port=3307, database=banco, user=self.user_sistema_senhas, password=self.pw_bd_sistema_senhas)
         else:
             conexao = create_engine(f'mysql+{library_sql}://{user_db}:{password_db}@{ip_ou_host_db}:{porta}/{db}')
         return conexao
             
         
+        
+    def api_consulta_denodo(self, database:str, tabela:str, colunas:str, filtro_where="opcional"):
+        '''
+        filtro = "coluna2 eq 'SIM' and coluna3 eq 'Ativo'" \n
+        df = dados.api_consulta_denodo('ldw', 'nome_da_tabela', 'coluna1, coluna5', filtro) \n\n
+        
+        # operadores para filtro where: \n
+        eq = igual \n
+        lt = menor que \n
+        le = menor ou igual \n
+        ne = diferente \n
+        ge = maior ou igual \n
+        gt = maior que \n       
+        
+        '''
+        requests.packages.urllib3.disable_warnings()
+        if filtro_where == "opcional":
+            url = f"{self.url_api_denodo}/{database}/views/{tabela}?$select={colunas}"
+        else:
+            url = f"{self.url_api_denodo}/{database}/views/{tabela}?$select={colunas}&$filter={filtro_where}"
+        payload={}
+        headers = {'Accept': 'application/xhtml+xml;q=0.9,application/json', 'Authorization': self.token_api_denodo}
+        response = requests.request("GET", url, headers=headers, data=payload, verify=False)
+        rows = json.loads(response.content)
+        df = pd.DataFrame(rows['elements'])
+        return df   
+        
+        
     def consultar_banco_dados(self, conexao_engine, query_sql:str, retorna_DataFrame=True):
         '''
         retorna um DataFrame pandas \n
         exemplo de query: \n
         SELECT * FROM rpa_historico WHERE cod_rpa = "3000" \n
         '''
         if retorna_DataFrame:
@@ -232,14 +264,16 @@
         self.senha_fluid = str(gerador_pwd('usuario_fluid', 'senha'))
         
         self.ip_planning = str(os.getenv('ip_planning'))
         self.user_planning = str(os.getenv('user_planning'))
         self.pw_bd_planning = str(urllib.parse.quote_plus(os.getenv('pw_bd_planning'))) 
         
         
+        
+        
     def anexar_arquivo_fluid(self, cod_processo:str, path_file:str, tipo_arquivo:str):
         '''
             num_processo = '497305'\n
             path_file = 'C:\\Temp\\teste.xlsx'\n
             id_doc_fluid = '417'\n
             api_upload_anexo_fluid( num_processo, path_file, id_doc_fluid )
         '''
@@ -1219,16 +1253,15 @@
             df = self.dados.consultar_banco_dados(self.conexao, f"SELECT * FROM rpa_fila WHERE status_rpa='{tipo_status}'")
         df = df[['cod_rpa', 'executar_na_vm', 'status_rpa']]
         print(df)
         print()
         return df
     
             
-        
-         
+              
 class Escrever_por_extenso:  
             
     def __init__(self):
         self.url_api_escreve_por_extenso = str(gerador_pwd('por_extenso', 'senha'))
    
     
     def numero_por_extenso(self, valor:str):
```

### Comparing `rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.41
+Version: 1.0.42
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.41/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.41/setup.py` & `rpa_cooperativa-1.0.42/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.41",
+    version="1.0.42",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

