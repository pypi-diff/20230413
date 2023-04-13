# Comparing `tmp/rpa_cooperativa-1.0.42.tar.gz` & `tmp/rpa_cooperativa-1.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.42.tar", last modified: Thu Apr 13 13:19:23 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.43.tar", last modified: Thu Apr 13 17:54:51 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.42.tar` & `rpa_cooperativa-1.0.43.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 13:19:23.852287 rpa_cooperativa-1.0.42/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.42/LICENSE
--rw-rw-rw-   0        0        0     5578 2023-04-13 13:19:23.843387 rpa_cooperativa-1.0.42/PKG-INFO
--rw-rw-rw-   0        0        0     4429 2023-04-10 13:24:59.000000 rpa_cooperativa-1.0.42/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 13:19:23.567706 rpa_cooperativa-1.0.42/rpa_coop/
--rw-rw-rw-   0        0        0      528 2023-04-10 13:18:19.000000 rpa_cooperativa-1.0.42/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:19:23.702805 rpa_cooperativa-1.0.42/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.42/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.42/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.42/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.42/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.42/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.42/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      347 2023-02-28 19:51:44.000000 rpa_cooperativa-1.0.42/rpa_coop/img/siac_verde.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.42/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0      336 2023-02-28 19:52:19.000000 rpa_cooperativa-1.0.42/rpa_coop/img/siat_verde.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.42/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.42/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    66470 2023-04-13 13:16:12.000000 rpa_cooperativa-1.0.42/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:19:23.832158 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     5578 2023-04-13 13:19:22.000000 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-04-13 13:19:23.000000 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 13:19:22.000000 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 13:19:22.000000 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      544 2023-04-13 13:19:22.000000 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 13:19:22.000000 rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 13:19:23.854287 rpa_cooperativa-1.0.42/setup.cfg
--rw-rw-rw-   0        0        0     2305 2023-04-13 13:18:16.000000 rpa_cooperativa-1.0.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:54:51.305712 rpa_cooperativa-1.0.43/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.43/LICENSE
+-rw-rw-rw-   0        0        0     6237 2023-04-13 17:54:51.284915 rpa_cooperativa-1.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0     5088 2023-04-13 17:54:03.000000 rpa_cooperativa-1.0.43/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 17:54:50.954987 rpa_cooperativa-1.0.43/rpa_coop/
+-rw-rw-rw-   0        0        0      545 2023-04-13 14:56:13.000000 rpa_cooperativa-1.0.43/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:54:51.172010 rpa_cooperativa-1.0.43/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.43/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.43/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.43/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.43/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.43/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.43/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      347 2023-02-28 19:51:44.000000 rpa_cooperativa-1.0.43/rpa_coop/img/siac_verde.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.43/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0      336 2023-02-28 19:52:19.000000 rpa_cooperativa-1.0.43/rpa_coop/img/siat_verde.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.43/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.43/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    69808 2023-04-13 17:52:50.000000 rpa_cooperativa-1.0.43/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:54:51.268273 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6237 2023-04-13 17:54:49.000000 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-04-13 17:54:50.000000 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:54:49.000000 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-13 17:54:49.000000 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      559 2023-04-13 17:54:49.000000 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 17:54:49.000000 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 17:54:51.308832 rpa_cooperativa-1.0.43/setup.cfg
+-rw-rw-rw-   0        0        0     2323 2023-04-13 17:54:17.000000 rpa_cooperativa-1.0.43/setup.py
```

### Comparing `rpa_cooperativa-1.0.42/LICENSE` & `rpa_cooperativa-1.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.42/PKG-INFO` & `rpa_cooperativa-1.0.43/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: rpa_cooperativa
-Version: 1.0.42
-Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
-Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
-Author: Edenilson Fernandes dos Santos
-Author-email: santoeen@gmail.com
-License: MIT License
-Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
-Keywords: rpa cooperativa fluid api automação sql sqlalchemy
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Exemplos de utilizacao da bilioteca rpa_coop
 
 ```python
 # linha1: update pip 
 # linha2: install lib rpa-cooperativa via pip
 python -m pip install --trusted-host pypi.python.org --trusted-host files.pythonhosted.org --trusted-host pypi.org --upgrade pip
 pip install --trusted-host pypi.python.org --trusted-host files.pythonhosted.org --trusted-host pypi.org pip rpa-cooperativa
@@ -36,28 +11,46 @@
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
 ## - Add libs dependencia para todos projetos da VM
 ## - Add acesso gerador de senhas
 ## - Melhoria metodos da classe fluid, exceptions caso nao retorne 200
 ```
 
-## manipulacao selenium: automaÃ§Ã£o web
+## manipulacao selenium: automação web
 ```python
 from rpa_coop import selenium
 import time
 
 driver = selenium.driver_edge()
 url = 'http://www.google.com.br'
 
 time.sleep(1)
 driver.get(url)
 time.sleep(1)
 driver.maximize_window()
 ```
 
+## manipulacao de emails:
+```python
+from rpa_coop import mail
+
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg')
+
+lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']
+mail.enviar_email(lista_dest, 'teste titulo2', 'teste msg')
+
+anexos = ['notas.txt', 'README.md']
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos)
+
+anexos = ['notas.txt', 'README.md', 'imagem.PNG']
+html_text_img = '<html><body><h1>Teste img + texto</h1><img src="cid:imagem.PNG"></body></html>'
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos, html_text_img)
+        
+```
+
 
 ## manipulacao da ferramenta de fluxo de trabalho: fluid
 ```python
 ########################################################
 from rpa_coop import fluid
 
 # Variaveis
@@ -77,15 +70,15 @@
 cod_tipo_arquivo_fluid = '417' 
 fluid.anexar_arquivo_fluid(cod_processo, 'C:\\Temp\\teste.xlsx', cod_tipo_arquivo_fluid)
 
 # protocolar/enviar
 fluid.protocolar_processo_fluid(cod_processo, id_tipo_processo) # empresa 1 - padrao, proximo nodo padrao
 fluid.protocolar_processo_fluid(cod_processo, id_tipo_processo, filial_orig, filial_dest) # filiais, proximo nodo padrao
 fluid.protocolar_processo_fluid(cod_processo, id_tipo_processo, filial_orig, filial_dest, nome_do_nodo='Devolver a confeccao') 
-fluid.protocolar_processo_fluid(cod_processo, id_tipo_processo, nome_do_nodo='Devolver a confeccao') # nodo especÃ­fico pelo nome
+fluid.protocolar_processo_fluid(cod_processo, id_tipo_processo, nome_do_nodo='Devolver a confeccao') # nodo específico pelo nome
 
 # pegar processos aguardando na caixa do usuario
 df_processos = fluid.get_processos_fluid([id_tipo_processo]) # por padrao user do rpa no fluid, passar lista id_tipo_processo
 
 # pegar dados de processo especifico
 df_dados_processo = fluid.get_dados_processo(cod_processo)
 
@@ -118,15 +111,15 @@
 # sistema legado acclient
 ```python
 ########################################################
 
 from rpa_coop import acc 
 
 # abrir aplicativo acc 
-# obs. se transacional = False, clica na opÃ§Ã£o relatorios no menu inicial
+# obs. se transacional = False, clica na opção relatorios no menu inicial
 acc.open_acclient('siat', transacional=True)
 
 # verificar se existe texto na tela para decidir a proxima acao
 acc.exist_text('Retorna ao Sistema')
 acc.exist_text('Retorna ao Sistema', topo1=100, topo2=200, continua_seerro=True)
 
 # navegar ao menu, sequencia de letras, no caso C.B.C
```

### Comparing `rpa_cooperativa-1.0.42/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.43/rpa_coop/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,9 +11,10 @@
 monitorar = Monitorar()
 monitor_rpa = Monitorar()
 escrever_por_extenso = Escrever_por_extenso()
 numero_por_extenso = escrever_por_extenso.numero_por_extenso
 taxa_percentual_por_extenso = escrever_por_extenso.taxa_por_extenso
 gerador_de_codigo = Gerador_de_codigo()
 selenium = Selenium()
+mail = Emails()
```

### Comparing `rpa_cooperativa-1.0.42/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.43/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.42/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.43/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.42/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.43/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.42/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.43/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.42/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.43/rpa_coop/rpa_coop.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,19 @@
         credencial_atributos = {}
         df = df.drop(columns='id')
         valor = df.iloc[0,:].apply(str).values
         valor = str(valor[1])
         fernet = Fernet(hash_validador) 
         msg_encripted = valor
         msg = bytes(msg_encripted, "utf-8") 
-        valor = fernet.decrypt(msg).decode("utf-8")
-        df['senha'] = valor
+        try:
+            valor = fernet.decrypt(msg).decode("utf-8")
+            df['senha'] = valor
+        except:
+            pass
         credencial_atributos = df.to_dict(orient='records')
         credenciais = credencial_atributos[0]
         valor = credenciais.get(select_atributo)
         result = f'{select_atributo} : {valor}'
         if print_atributo: print(result)
         if retorna_atributo: return valor
         return credenciais
@@ -182,26 +185,32 @@
         lt = menor que \n
         le = menor ou igual \n
         ne = diferente \n
         ge = maior ou igual \n
         gt = maior que \n       
         
         '''
+        df = pd.DataFrame()
         requests.packages.urllib3.disable_warnings()
         if filtro_where == "opcional":
             url = f"{self.url_api_denodo}/{database}/views/{tabela}?$select={colunas}"
         else:
             url = f"{self.url_api_denodo}/{database}/views/{tabela}?$select={colunas}&$filter={filtro_where}"
         payload={}
         headers = {'Accept': 'application/xhtml+xml;q=0.9,application/json', 'Authorization': self.token_api_denodo}
         response = requests.request("GET", url, headers=headers, data=payload, verify=False)
+        # print(response.text.encode('utf8'))
         rows = json.loads(response.content)
-        df = pd.DataFrame(rows['elements'])
+        try:
+            df = pd.DataFrame(rows['elements'])
+        except:
+            print('erro ao converter para DataFrame, json retornou: \n', response.text.encode('utf8'))
         return df   
         
+    
         
     def consultar_banco_dados(self, conexao_engine, query_sql:str, retorna_DataFrame=True):
         '''
         retorna um DataFrame pandas \n
         exemplo de query: \n
         SELECT * FROM rpa_historico WHERE cod_rpa = "3000" \n
         '''
@@ -946,14 +955,85 @@
                 ]
             }
         response = requests.post(self.url_api_sms, headers=headers, json=body)
         cod_response  = response.status_code
         return cod_response
     
    
+   
+class Emails:
+    import smtplib
+    from email.mime.multipart import MIMEMultipart
+    from email.mime.text import MIMEText
+    from email.mime.application import MIMEApplication
+    
+    def __init__(self):
+        self.user_mail = gerador_pwd('api_email', 'usuario')
+        self.password_mail = gerador_pwd('api_email', 'sistema')
+        self.smtpsrv = gerador_pwd('api_email', 'ip_host')
+
+
+    def enviar_email(self, destinatarios, assunto: str, mensagem: str, anexo=None, html_text_img=None, com_copia=None):
+        '''
+        mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg') \n\n
+        
+        lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']\n
+        mail.enviar_email(lista_dest, 'teste titulo2', 'teste msg')\n\n
+        
+        anexos = ['notas.txt', 'README.md']\n
+        mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos)\n\n
+        
+        anexos = ['notas.txt', 'README.md', 'imagem.PNG']\n
+        html_text_img = '<html><body><h1>Teste img + texto</h1><img src="cid:imagem.PNG"></body></html>'\n
+        mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos, html_text_img)\n
+        '''
+        mail_content = mensagem
+        smtpserver = self.smtplib.SMTP(self.smtpsrv,587)
+        msg = self.MIMEMultipart('mixed')
+        msg = self.MIMEMultipart('alternative')
+        
+        msg['Subject'] = assunto
+        msg['From'] = self.user_mail 
+        msg['To'] = destinatarios if type(destinatarios) == str else ", ".join(destinatarios)
+
+        if com_copia: msg['Cc'] = com_copia
+        msg.attach(self.MIMEText(mail_content,'plain','utf8'))
+
+        msg.attach(self.MIMEText(html_text_img, 'html', 'utf-8'))
+        
+        if type(anexo) == str:
+            if anexo:
+                attachmentPath = anexo
+                try:
+                    with open(attachmentPath, "rb") as attachment:
+                        p = self.MIMEApplication(attachment.read(),_subtype="png")	
+                        p.add_header('Content-Disposition', "attachment; filename= %s" % attachmentPath) 
+                        msg.attach(p)
+                except Exception as e:
+                    print(str(e))
+        elif type(anexo) == list:
+            for attachmentPath in anexo:
+                try:
+                    with open(attachmentPath, "rb") as attachment:
+                        p = self.MIMEApplication(attachment.read(),_subtype="png")	
+                        p.add_header('Content-Disposition', "attachment; filename= %s" % attachmentPath) 
+                        msg.attach(p)
+                except Exception as e:
+                    print(str(e))
+            
+                
+
+        #Send the Email Message
+        smtpserver.ehlo()
+        smtpserver.starttls()
+        smtpserver.login(self.user_mail , self.password_mail)
+        smtpserver.send_message (msg, from_addr=self.user_mail, to_addrs=destinatarios)
+        smtpserver.close()
+
+
 
 class Acc:
     import pyautogui as p
     import subprocess
     import pyperclip
     
     
@@ -1458,14 +1538,11 @@
         return encontrou
         
         
 
     
     
     
-    
-
-
```

### Comparing `rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.43/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rpa-cooperativa
-Version: 1.0.42
+Name: rpa_cooperativa
+Version: 1.0.43
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
@@ -50,14 +50,32 @@
 
 time.sleep(1)
 driver.get(url)
 time.sleep(1)
 driver.maximize_window()
 ```
 
+## manipulacao de emails:
+```python
+from rpa_coop import mail
+
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg')
+
+lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']
+mail.enviar_email(lista_dest, 'teste titulo2', 'teste msg')
+
+anexos = ['notas.txt', 'README.md']
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos)
+
+anexos = ['notas.txt', 'README.md', 'imagem.PNG']
+html_text_img = '<html><body><h1>Teste img + texto</h1><img src="cid:imagem.PNG"></body></html>'
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos, html_text_img)
+        
+```
+
 
 ## manipulacao da ferramenta de fluxo de trabalho: fluid
 ```python
 ########################################################
 from rpa_coop import fluid
 
 # Variaveis
```

### Comparing `rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.42/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,7 +40,8 @@
 beautifulsoup4
 mechanize
 matplotlib
 Unidecode
 WMI
 tabulate
 python-dateutil==2.8.2
+secure-smtplib
```

### Comparing `rpa_cooperativa-1.0.42/setup.py` & `rpa_cooperativa-1.0.43/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.42",
+    version="1.0.43",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
@@ -37,9 +37,9 @@
     ],
     python_requires='>=3.8',
     install_requires=['wheel', 'pandas', 'openpyxl', 'cryptography', 'xlsxwriter', 'xlrd', 'openpyxl','selenium', 'webdriver_manager', 'easygui', 'pyperclip', 'mysql-connector-python==8.0.28',
                       'pymysql', 'pyodbc', 'sqlalchemy==1.4.37', 'psycopg2', 'psycopg2-binary', 'denodo-sqlalchemy', 'pillow', 'requests==2.28.1', 'urllib3==1.26.9', 
                       'certifi==2022.5.18.1', 'pyopenssl==22.0.0', 'idna==3.3', 'charset-normalizer==2.0.12', 'pyautogui',
                       'pyrect', 'pyscreeze', 'pytz', 'graypy', 'reportlab', 'psutil', 'requests-html', 'paramiko','opencv-python',
                       'pytesseract', 'xmltodict', 'pywin32', 'pywinauto', 'beautifulsoup4', 'mechanize', 'matplotlib', 
-                      'Unidecode', 'WMI', 'tabulate', 'python-dateutil==2.8.2']
+                      'Unidecode', 'WMI', 'tabulate', 'python-dateutil==2.8.2', 'secure-smtplib']
 )
```

