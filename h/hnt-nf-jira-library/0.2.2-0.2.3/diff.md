# Comparing `tmp/hnt_nf_jira_library-0.2.2.tar.gz` & `tmp/hnt_nf_jira_library-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.2.2.tar", last modified: Fri Mar 22 18:29:58 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.2.3.tar", last modified: Tue Apr  2 19:41:36 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.2.2.tar` & `hnt_nf_jira_library-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 18:29:58.000091 hnt_nf_jira_library-0.2.2/
--rw-rw-rw-   0        0        0      286 2024-03-22 18:29:58.000091 hnt_nf_jira_library-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 18:29:58.000091 hnt_nf_jira_library-0.2.2/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-03-22 18:29:57.000000 hnt_nf_jira_library-0.2.2/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2024-03-22 18:29:57.000000 hnt_nf_jira_library-0.2.2/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 18:29:57.000000 hnt_nf_jira_library-0.2.2/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-03-22 18:29:57.000000 hnt_nf_jira_library-0.2.2/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-22 18:29:57.000000 hnt_nf_jira_library-0.2.2/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-22 18:29:57.957585 hnt_nf_jira_library-0.2.2/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.2/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 18:29:57.996507 hnt_nf_jira_library-0.2.2/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/chave_acesso.py
--rw-rw-rw-   0        0        0      132 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      145 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/dados_basicos.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      140 2024-03-15 19:20:34.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0       97 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      397 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      379 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.2/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    23248 2024-03-22 18:28:51.000000 hnt_nf_jira_library-0.2.2/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-03-22 18:29:58.005214 hnt_nf_jira_library-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      489 2024-03-22 18:29:26.000000 hnt_nf_jira_library-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:41:36.785987 hnt_nf_jira_library-0.2.3/
+-rw-rw-rw-   0        0        0      286 2024-04-02 19:41:36.781985 hnt_nf_jira_library-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 19:41:36.779986 hnt_nf_jira_library-0.2.3/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-02 19:41:36.000000 hnt_nf_jira_library-0.2.3/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2024-04-02 19:41:36.000000 hnt_nf_jira_library-0.2.3/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 19:41:36.000000 hnt_nf_jira_library-0.2.3/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-02 19:41:36.000000 hnt_nf_jira_library-0.2.3/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 19:41:36.000000 hnt_nf_jira_library-0.2.3/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 19:41:36.645285 hnt_nf_jira_library-0.2.3/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.3/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:41:36.776984 hnt_nf_jira_library-0.2.3/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/chave_acesso.py
+-rw-rw-rw-   0        0        0     1863 2024-04-02 19:41:07.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      145 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/dados_basicos.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      140 2024-03-15 19:20:34.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0       97 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      397 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      379 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.3/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    23461 2024-04-02 19:41:07.000000 hnt_nf_jira_library-0.2.3/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 19:41:36.786987 hnt_nf_jira_library-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      489 2024-04-02 19:41:12.000000 hnt_nf_jira_library-0.2.3/setup.py
```

### Comparing `hnt_nf_jira_library-0.2.2/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.2.3/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.2.2/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.2.3/nf_jira/wrapper_nf_jira.py`

 * *Files 13% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         if not issue["allocation_data"]:
 
             item = {
                 "centro": issue["domain_data"]["centro"]["centro"],
                 "centro_custo": f"{issue['domain_data']['centro']['centro']}210",
                 "cod_imposto": "C6",
-                "valor_bruto": str(issue["json_data"]["Valor"]).replace(".", ","),
+                "valor_bruto": str(issue["json_data"][VALOR_TOTAL_DA_FATURA]).replace(".", ","),
             }
 
             sintese_item = {
                 "categoria_cc": "K",
                 "quantidade": 1,
                 "cod_material": issue["domain_data"]["fornecedor"]["codigo_material"],
                 "item": item,
@@ -97,15 +97,15 @@
                 validTotalPercents += float(centro_issue["porcentagem"])
 
                 item = {
                     "centro": centro_issue["nome"].split("210")[0],
                     "centro_custo": centro_issue["nome"],
                     "cod_imposto": "C6",
                     "valor_bruto": "{:.2f}".format(
-                        issue["json_data"]["Valor"]
+                        issue["json_data"][VALOR_TOTAL_DA_FATURA]
                         * float(
                             centro_issue["porcentagem"].replace(
                                 ",",
                             )
                         )
                         / 100,
                         2,
@@ -143,74 +143,74 @@
         }
 
         return nota_pedido
 
     def _miro_factory(self, issue: dict):
 
         data_ref = (
-            datetime.strptime(issue["DataReferencia"], "%d/%m/%Y %H:%M:%S")
+            datetime.strptime(issue[DATA_DE_REFERÊNCIA], "%d/%m/%Y %H:%M:%S")
             .strftime("%b/%y")
             .upper()
         )
 
-        if issue["ComplementoAgua"] is not None:
+        if issue[COMPLEMENTO_DE_ÁGUA] is not None:
             leitura_anterior = (
                 datetime.strptime(
-                    issue["ComplementoAgua"]["DataLeituraAnterior"], "%Y-%m-%dT%H:%M:%S"
+                    issue[COMPLEMENTO_DE_ÁGUA]["DataLeituraAnterior"], "%Y-%m-%dT%H:%M:%S"
                 )
                 .strftime("%b/%y")
                 .upper()
             )
             leitura_atual = (
                 datetime.strptime(
-                    issue["ComplementoAgua"]["DataLeituraAtual"], "%Y-%m-%dT%H:%M:%S"
+                    issue[COMPLEMENTO_DE_ÁGUA]["DataLeituraAtual"], "%Y-%m-%dT%H:%M:%S"
                 )
                 .strftime("%b/%y")
                 .upper()
             )
-        elif issue["ComplementoEnergia"] is not None:
+        elif issue[COMPLEMENTO_DE_ENERGIA] is not None:
             leitura_anterior = (
                 datetime.strptime(
-                    issue["ComplementoEnergia"]["DataLeituraAnterior"],
+                    issue[COMPLEMENTO_DE_ENERGIA]["DataLeituraAnterior"],
                     "%Y-%m-%dT%H:%M:%S",
                 )
                 .strftime("%b/%y")
                 .upper()
             )
             leitura_atual = (
                 datetime.strptime(
-                    issue["ComplementoEnergia"]["DataLeituraAtual"], "%Y-%m-%dT%H:%M:%S"
+                    issue[COMPLEMENTO_DE_ENERGIA]["DataLeituraAtual"], "%Y-%m-%dT%H:%M:%S"
                 )
                 .strftime("%b/%y")
                 .upper()
             )
-        elif issue["ComplementoGas"] is not None:
+        elif issue[COMPLEMENTO_DE_GÁS] is not None:
             leitura_anterior = (
                 datetime.strptime(
-                    issue["ComplementoGas"]["DataLeituraAnterior"], "%Y-%m-%dT%H:%M:%S"
+                    issue[COMPLEMENTO_DE_GÁS]["DataLeituraAnterior"], "%Y-%m-%dT%H:%M:%S"
                 )
                 .strftime("%b/%y")
                 .upper()
             )
             leitura_atual = (
                 datetime.strptime(
-                    issue["ComplementoGas"]["DataLeituraAtual"], "%Y-%m-%dT%H:%M:%S"
+                    issue[COMPLEMENTO_DE_GÁS]["DataLeituraAtual"], "%Y-%m-%dT%H:%M:%S"
                 )
                 .strftime("%b/%y")
                 .upper()
             )
 
         texto = f"REF: {data_ref} PERIODO: {leitura_anterior} A {leitura_atual}"
 
         dados_basicos = {
             "data_da_fatura": datetime.strptime(
-                issue["DataEmissao"], "%Y-%m-%dT%H:%M:%S"
+                issue[DATA_DE_EMISSÃO], "%Y-%m-%dT%H:%M:%S"
             ).strftime("%d%m%Y"),
             "referencia": f"{issue['ChaveAcessoNotaFiscal'][25:34]}-{issue['ChaveAcessoNotaFiscal'][22:25]}",
-            "montante": str(issue["Valor"]).replace(".", ","),
+            "montante": str(issue[VALOR_TOTAL_DA_FATURA]).replace(".", ","),
             "texto": texto,
         }
 
         referencia_pedido = {"numero_pedido": issue["cod_sap"]}
 
         detalhe = {"ctg_nf": issue["domain_data"]["fornecedor"]["categoria_nf"]}
 
@@ -245,31 +245,31 @@
             issue_json = self._get_nf_jira(issue_id)
 
             attachment = issue_json["attachment"]
             jira_info = issue_json["jira_info"]
 
             ##### GET DOMAIN #####
             ## FORNECEDOR
-            cnpj_fornecedor = attachment.get("CnpjFornecedor")
+            cnpj_fornecedor = attachment.get(CNPJ_DO_FORNECEDOR)
             fornecedor = self._get_nf_domain("fornecedor", cnpj_fornecedor)
 
             ## CENTRO
-            cnpj_centro = attachment.get("CnpjCliente")
+            cnpj_centro = attachment.get(CNPJ_DO_CLIENTE)
             centro = self._get_nf_domain("centro", cnpj_centro)
 
             domain = {"fornecedor": fornecedor, "centro": centro}
 
             ##### GET PDF #####
-            pdf_data = self._download_pdf(attachment["Arquivos"][0])
+            pdf_data = self._download_pdf(attachment[ARQUIVOS_DA_FATURA][0])
 
             ##### GET ALLOCATION #####
             allocation = self._get_allocation(
-                attachment["CnpjFornecedor"],
-                attachment["CnpjCliente"],
-                attachment["Contrato"],
+                attachment[CNPJ_DO_FORNECEDOR],
+                attachment[CNPJ_DO_CLIENTE],
+                attachment[NÚMERO_DO_CONTRATO],
             )
 
             ##### FORMAT JSON #####
             issue = {
                 "issue_data": issue_json["issue_data"],
                 "json_data": attachment,
                 "domain_data": domain,
@@ -308,19 +308,19 @@
             issue_data["issue_data"]["fields"] = clean_fields
 
             attachment = issue_data["attachment"]
             attachment["cod_sap"] = cod_sap
 
             ##### GET DOMAIN #####
             ## FORNECEDOR
-            cnpj_fornecedor = attachment.get("CnpjFornecedor")
+            cnpj_fornecedor = attachment.get(CNPJ_DO_FORNECEDOR)
             fornecedor = self._get_nf_domain("fornecedor", cnpj_fornecedor)
 
             ## CENTRO
-            cnpj_centro = attachment.get("CnpjCliente")
+            cnpj_centro = attachment.get(CNPJ_DO_CLIENTE)
             centro = self._get_nf_domain("centro", cnpj_centro)
 
             attachment["domain_data"] = {"fornecedor": fornecedor, "centro": centro}
 
             miro_model = self._miro_factory(attachment)
 
             miro = Miro(**miro_model)
@@ -385,74 +385,79 @@
                 if attachment is not None:
                     attachment_data = attachment
 
             if "21" in form_data["state"]["answers"] is not None:
                 nf_type_id = form_data["state"]["answers"]["21"]["choices"][0]
 
                 if nf_type_id == "1":
-                    nf_type = "ComplementoAgua"
+                    nf_type = COMPLEMENTO_DE_ÁGUA
 
                 elif nf_type_id == "2":
-                    nf_type = "ComplementoEnergia"
+                    nf_type = COMPLEMENTO_DE_ENERGIA
 
                 elif nf_type_id == "3":
-                    nf_type = "ComplementoGas"
+                    nf_type = COMPLEMENTO_DE_GÁS
 
             else:
-                if attachment["ComplementoAgua"] is not None:
-                    nf_type = "ComplementoAgua"
-                elif attachment["ComplementoEnergia"] is not None:
-                    nf_type = "ComplementoEnergia"
-                elif attachment["ComplementoGas"] is not None:
-                    nf_type = "ComplementoGas"
+                if attachment[COMPLEMENTO_DE_ÁGUA] is not None:
+                    nf_type = COMPLEMENTO_DE_ÁGUA
+                elif attachment[COMPLEMENTO_DE_ENERGIA] is not None:
+                    nf_type = COMPLEMENTO_DE_ENERGIA
+                elif attachment[COMPLEMENTO_DE_GÁS] is not None:
+                    nf_type = COMPLEMENTO_DE_GÁS
 
-            attachment["CnpjFornecedor"] = (
+            attachment[CNPJ_DO_FORNECEDOR] = (
                 form_data["state"]["answers"]["3"]["text"]
                 if "3" in form_data["state"]["answers"]
-                else attachment.get("CnpjFornecedor")
+                else attachment.get(CNPJ_DO_FORNECEDOR)
             )
-            attachment["RazaoSocialFornecedor"] = (
+            attachment[RAZÃO_SOCIAL_DO_FORNECEDOR] = (
                 form_data["state"]["answers"]["4"]["text"]
                 if "4" in form_data["state"]["answers"]
-                else attachment.get("RazaoSocialFornecedor")
+                else attachment.get(RAZÃO_SOCIAL_DO_FORNECEDOR)
             )
-            attachment["CnpjCliente"] = (
+            attachment[CNPJ_DO_CLIENTE] = (
                 form_data["state"]["answers"]["5"]["text"]
                 if "5" in form_data["state"]["answers"]
-                else attachment.get("CnpjCliente")
+                else attachment.get(CNPJ_DO_CLIENTE)
             )
-            attachment["NotaFiscal"] = (
+            attachment[NÚMERO_DA_FATURA] = (
                 form_data["state"]["answers"]["7"]["text"]
                 if "7" in form_data["state"]["answers"]
-                else attachment.get("NotaFiscal")
+                else attachment.get(NÚMERO_DA_FATURA)
             )
-            attachment["NumeroFaturaFornecedor"] = (
+            attachment[NÚMERO_DA_FATURA_DO_FORNECEDOR] = (
                 form_data["state"]["answers"]["8"]["text"]
                 if "8" in form_data["state"]["answers"]
-                else attachment.get("NumeroFaturaFornecedor")
+                else attachment.get(NÚMERO_DA_FATURA_DO_FORNECEDOR)
             )
-            attachment["DataEmissao"] = (
+            attachment[DATA_DE_EMISSÃO] = (
                 form_data["state"]["answers"]["9"]["date"]
                 if "9" in form_data["state"]["answers"]
-                else attachment.get("DataEmissao")
+                else attachment.get(DATA_DE_EMISSÃO)
             )
-            attachment["DataVencimento"] = (
+            attachment[DATA_DE_VENCIMENTO] = (
                 form_data["state"]["answers"]["10"]["date"]
                 if "10" in form_data["state"]["answers"]
-                else attachment.get("DataVencimento")
+                else attachment.get(DATA_DE_VENCIMENTO)
             )
-            attachment["Valor"] = (
+            attachment[VALOR_TOTAL_DA_FATURA] = (
                 form_data["state"]["answers"]["11"]["text"]
                 if "11" in form_data["state"]["answers"]
-                else attachment.get("Valor")
+                else attachment.get(VALOR_TOTAL_DA_FATURA)
             )
-            attachment["ChaveAcessoNotaFiscal"] = (
+            attachment[CHAVE_DE_ACESSO_DA_FATURA] = (
                 form_data["state"]["answers"]["12"]["text"]
                 if "12" in form_data["state"]["answers"]
-                else attachment.get("ChaveAcessoNotaFiscal")
+                else attachment.get(CHAVE_DE_ACESSO_DA_FATURA)
+            )
+            attachment[DATA_DE_REFERÊNCIA] = (
+                form_data["state"]["answers"]["18"]["text"]
+                if "18" in form_data["state"]["answers"]
+                else attachment.get(DATA_DE_REFERÊNCIA)
             )
             attachment["numero_log"] = (
                 form_data["state"]["answers"]["13"]["text"]
                 if "13" in form_data["state"]["answers"]
                 else attachment.get("numero_log")
             )
             attachment["data_procmto"] = (
@@ -471,19 +476,14 @@
                 else attachment[nf_type].get("DataLeituraAnterior")
             )
             attachment[nf_type]["DataLeituraAtual"] = (
                 form_data["state"]["answers"]["17"]["date"]
                 if "17" in form_data["state"]["answers"]
                 else attachment[nf_type].get("DataLeituraAtual")
             )
-            attachment["DataReferencia"] = (
-                form_data["state"]["answers"]["18"]["text"]
-                if "18" in form_data["state"]["answers"]
-                else attachment.get("DataReferencia")
-            )
 
             jira_info = {"issue_id": issue_id, "form_id": automacao_form_id}
 
             nf_jira_json = {
                 "issue_data": issue_data,
                 "attachment": attachment_data,
                 "jira_info": jira_info,
```

