# Comparing `tmp/testing_package_exedoc-0.0.6.tar.gz` & `tmp/testing_package_exedoc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testing_package_exedoc-0.0.6.tar", last modified: Fri Mar 29 00:07:17 2024, max compression
+gzip compressed data, was "testing_package_exedoc-0.0.7.tar", last modified: Tue Apr  2 19:09:50 2024, max compression
```

## Comparing `testing_package_exedoc-0.0.6.tar` & `testing_package_exedoc-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 00:07:17.987132 testing_package_exedoc-0.0.6/
--rw-rw-rw-   0        0        0     1073 2024-03-20 07:11:42.000000 testing_package_exedoc-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      665 2024-03-29 00:07:17.986134 testing_package_exedoc-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      170 2024-03-20 07:11:09.000000 testing_package_exedoc-0.0.6/README.md
--rw-rw-rw-   0        0        0      568 2024-03-28 23:59:43.000000 testing_package_exedoc-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 00:07:17.987132 testing_package_exedoc-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-29 00:07:17.958130 testing_package_exedoc-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-03-29 00:07:17.969129 testing_package_exedoc-0.0.6/src/testing_package_exedoc/
--rw-rw-rw-   0        0        0        0 2024-03-20 07:04:46.000000 testing_package_exedoc-0.0.6/src/testing_package_exedoc/__init__.py
--rw-rw-rw-   0        0        0    21813 2024-03-29 00:02:25.000000 testing_package_exedoc-0.0.6/src/testing_package_exedoc/exedoc.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:07:17.985129 testing_package_exedoc-0.0.6/src/testing_package_exedoc.egg-info/
--rw-rw-rw-   0        0        0      665 2024-03-29 00:07:17.000000 testing_package_exedoc-0.0.6/src/testing_package_exedoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-03-29 00:07:17.000000 testing_package_exedoc-0.0.6/src/testing_package_exedoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 00:07:17.000000 testing_package_exedoc-0.0.6/src/testing_package_exedoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-03-29 00:07:17.000000 testing_package_exedoc-0.0.6/src/testing_package_exedoc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 19:09:50.801628 testing_package_exedoc-0.0.7/
+-rw-rw-rw-   0        0        0     1073 2024-03-20 07:11:42.000000 testing_package_exedoc-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      665 2024-04-02 19:09:50.799631 testing_package_exedoc-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2024-03-20 07:11:09.000000 testing_package_exedoc-0.0.7/README.md
+-rw-rw-rw-   0        0        0      568 2024-04-02 19:08:38.000000 testing_package_exedoc-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 19:09:50.801628 testing_package_exedoc-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 19:09:50.761630 testing_package_exedoc-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 19:09:50.780627 testing_package_exedoc-0.0.7/src/testing_package_exedoc/
+-rw-rw-rw-   0        0        0        0 2024-03-20 07:04:46.000000 testing_package_exedoc-0.0.7/src/testing_package_exedoc/__init__.py
+-rw-rw-rw-   0        0        0    20342 2024-04-02 19:08:07.000000 testing_package_exedoc-0.0.7/src/testing_package_exedoc/exedoc.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:09:50.798632 testing_package_exedoc-0.0.7/src/testing_package_exedoc.egg-info/
+-rw-rw-rw-   0        0        0      665 2024-04-02 19:09:50.000000 testing_package_exedoc-0.0.7/src/testing_package_exedoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-04-02 19:09:50.000000 testing_package_exedoc-0.0.7/src/testing_package_exedoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 19:09:50.000000 testing_package_exedoc-0.0.7/src/testing_package_exedoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-02 19:09:50.000000 testing_package_exedoc-0.0.7/src/testing_package_exedoc.egg-info/top_level.txt
```

### Comparing `testing_package_exedoc-0.0.6/LICENSE` & `testing_package_exedoc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `testing_package_exedoc-0.0.6/PKG-INFO` & `testing_package_exedoc-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testing_package_exedoc
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package for testing exedoc
 Author-email: Rompni <andresnavarrodev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `testing_package_exedoc-0.0.6/pyproject.toml` & `testing_package_exedoc-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "django==3.2.15"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "testing_package_exedoc"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Rompni", email="andresnavarrodev@gmail.com" },
 ]
 description = "A small example package for testing exedoc"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `testing_package_exedoc-0.0.6/src/testing_package_exedoc/exedoc.py` & `testing_package_exedoc-0.0.7/src/testing_package_exedoc/exedoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,277 +78,263 @@
     Retorno
     -------
     - ``data`` (dict) : diccionario con la respuesta de la llamada a EXEDOC
     - ``status`` (int) : el estado de la respuesta
     - ``URL_GDMTT`` (str|None) : la url de la llamada a EXEDOC
 
     """
-    try: 
-        print("Estoy en firma electronica avanzada")
-        log_sistema \
-            .add_params('ficha_id', ficha_id) \
-            .add_params('estado_evaluacion', estado_evaluacion) \
-            #.info('Inicia función de firma electrónica avanzada')
-            
-        print('ficha_id:', ficha_id, '- estado_evaluacion:', estado_evaluacion)
-        setLogSistema(log_sistema, 'Inicia función de firma electrónica avanzada', 'INFO', set_log_sistema)
+    print("Estoy en firma electronica avanzada")
+    log_sistema \
+        .add_params('ficha_id', ficha_id) \
+        .add_params('estado_evaluacion', estado_evaluacion) \
+        #.info('Inicia función de firma electrónica avanzada')
         
-        if not models.Ficha.objects.filter(id=ficha_id).exists():
-            print("Ficha no existe")
-            #log_sistema.error("La ficha no existe")
-            raise models.Ficha.DoesNotExist
-         
-        o_ficha = models.Ficha.objects.get(id=ficha_id)
-        log_sistema.add_params("o_ficha", o_ficha)
-
-        print(f'o_ficha.id: {o_ficha.id} - o_ficha.tipo_ficha: {o_ficha.tipo_ficha}')
-
-        if not models.Evaluacion_Imiv.objects.filter(imiv_id=o_ficha.id, vigente=True).exists():
-            print("La evaluacion no existe")
-            #log_sistema.error("La evaluacion no existe")
-            raise models.Evaluacion_Imiv.DoesNotExist
-
-        #print("Sali de los if de firma electrónica avanzada")
-        o_evaluacion = models.Evaluacion_Imiv.objects.get(imiv_id=o_ficha.id, vigente=True)
-        print(f'o_evaluacion.imiv.tipo_imiv_id: {o_evaluacion.imiv.tipo_imiv_id} ')
-        #log_sistema.info("firma_electronica_avanzada: se encontró la evaluacion")
-        setLogSistema(log_sistema, "firma_electronica_avanzada: se encontró la evaluacion", 'INFO', set_log_sistema)
-
-        tipo_documento_seim = None
-        if prorroga:
-            #print("Estoy en el if de prórroga")
-            tipo_documento_seim = models.TipoDocumentoSeim.RESPRORE
-            log_sistema \
-                .add_params("es_prorroga", True)
-
-        elif not models.EstadoEvaluacion.objects.filter(id=estado_evaluacion).exists():
-            print("El estado de evaluacion no existe")
-            #log_sistema.error("El estado de evaluacion no existe")
-            raise models.EstadoEvaluacion.DoesNotExist
+    print('ficha_id:', ficha_id, '- estado_evaluacion:', estado_evaluacion)
+    setLogSistema(log_sistema, 'Inicia función de firma electrónica avanzada', 'INFO', set_log_sistema)
     
-        else:
-            #print("Estoy en el if de estado evaluacion")
-            if estado_evaluacion == models.EstadoEvaluacion.RESOLUCION_OBSERVADO:
-                log_sistema.add_params("es_observado", True)
-                if o_evaluacion.imiv.tipo_imiv_id == models.TipoIMIV.TIPO_IMIV_INFORME_SUFICIENCIA:
-                    tipo_documento_seim = constants.DOCTO_SEIM_RESOLUCION_SUFICIENCIA_OBSERVA
-                else:
-                    tipo_documento_seim = models.TipoDocumentoSeim.RESEVAOBS if o_ficha.tipo_ficha == constants.TIPO_FICHA_SIMPLE else \
-                        models.TipoDocumentoSeim.RESEVAOBC
-            elif estado_evaluacion in [models.EstadoEvaluacion.RESOLUCION_APROBADO, models.EstadoEvaluacion.RESOLUCION_RECHAZADO]:
-                if o_evaluacion.imiv.tipo_imiv_id == models.TipoIMIV.TIPO_IMIV_INFORME_SUFICIENCIA:
-                    tipo_documento_seim = constants.DOCTO_SEIM_RESOLUCION_SUFICIENCIA_APRUEBA_RECHAZA
-                else:
-                    tipo_documento_seim = models.TipoDocumentoSeim.RESSEREVA if o_ficha.tipo_ficha == constants.TIPO_FICHA_SIMPLE else \
-                        models.TipoDocumentoSeim.RESEVAC
-            elif estado_evaluacion == models.EstadoEvaluacion.RESOLUCION_DESISTIDO:
-                tipo_documento_seim = models.TipoDocumentoSeim.RESDES
-            elif estado_evaluacion == models.EstadoEvaluacion.RECHAZADO_NO_CORRECCION:
-                tipo_documento_seim = models.TipoDocumentoSeim.RESNOCOS
-            else:
-                #log_sistema.error("Estado de evaluación no implementado para firma electrónica avanzada")
-                raise Exception("Estado de evaluación no implementado para firma electrónica avanzada")
-            
-        print(f"tipo documento seim es {tipo_documento_seim}")
-        log_sistema.add_params('tipo_documento_seim', tipo_documento_seim)
-        #.info(f'FEA: el documento es {tipo_documento_seim}')
-        setLogSistema(log_sistema, f'FEA: el documento es {tipo_documento_seim}', 'INFO', set_log_sistema)
+    if not models.Ficha.objects.filter(id=ficha_id).exists():
+        print("Ficha no existe")
+        #log_sistema.error("La ficha no existe")
+        raise models.Ficha.DoesNotExist
+        
+    o_ficha = models.Ficha.objects.get(id=ficha_id)
+    log_sistema.add_params("o_ficha", o_ficha)
 
-        if models.DocumentoEvaluacionImiv.objects.filter(
-            evaluacion_imiv=o_evaluacion,
-            tipo_documento_seim=models.TipoDocumentoSeim.get_id(tipo_documento_seim),
-            vigente=True
-        ).exists():
-            print("El documento evaluacion imiv existe")
-            #log_sistema.info('El documento evaluacion imiv existe')
-            setLogSistema(log_sistema, 'El documento evaluacion imiv existe', 'INFO', set_log_sistema)
-
-            o_documento_evaluacion_imiv = models.DocumentoEvaluacionImiv.objects.get(
-                evaluacion_imiv=o_evaluacion,
-                tipo_documento_seim=models.TipoDocumentoSeim.get_id(tipo_documento_seim),
-                vigente=True
-            )
-            o_archivo = o_documento_evaluacion_imiv.documento.file
-
-        elif borrador is not None:
-            log_sistema.add_params("es_borrador", True)
-            o_archivo = borrador.archivo
+    print(f'o_ficha.id: {o_ficha.id} - o_ficha.tipo_ficha: {o_ficha.tipo_ficha}')
 
-        else:
-            print("No existe documento para enviar a firmar")
-            #log_sistema.error("No existe documento para enviar a firmar")
-            raise models.DocumentoEvaluacionImiv.DoesNotExist
-        
-        print("firma_electronica_avanzada: se encontró el documento")
-        log_sistema.add_params("o_archivo", o_archivo)
-        #.info('firma_electronica_avanzada: se encontró el documento')
-        setLogSistema(log_sistema, 'firma_electronica_avanzada: se encontró el documento', 'INFO', set_log_sistema)
-
-        # Distribución externa
-        l_distribucion_externa = set([])
-
-        # Interesado
-        if o_ficha.tipo_ficha == constants.TIPO_FICHA_SIMPLE:
-            o_proyecto_ficha = models.Proyecto_Ficha.objects.filter(ficha_id=o_ficha).first()
-            print('firma_electronica_avanzada: es proyecto simple')
-            #log_sistema.info('firma_electronica_avanzada: es proyecto simple')
-            setLogSistema(log_sistema, 'firma_electronica_avanzada: es proyecto simple', 'INFO', set_log_sistema)
+    if not models.Evaluacion_Imiv.objects.filter(imiv_id=o_ficha.id, vigente=True).exists():
+        print("La evaluacion no existe")
+        #log_sistema.error("La evaluacion no existe")
+        raise models.Evaluacion_Imiv.DoesNotExist
+
+    #print("Sali de los if de firma electrónica avanzada")
+    o_evaluacion = models.Evaluacion_Imiv.objects.get(imiv_id=o_ficha.id, vigente=True)
+    print(f'o_evaluacion.imiv.tipo_imiv_id: {o_evaluacion.imiv.tipo_imiv_id} ')
+    #log_sistema.info("firma_electronica_avanzada: se encontró la evaluacion")
+    setLogSistema(log_sistema, "firma_electronica_avanzada: se encontró la evaluacion", 'INFO', set_log_sistema)
+
+    tipo_documento_seim = None
+    if prorroga:
+        #print("Estoy en el if de prórroga")
+        tipo_documento_seim = models.TipoDocumentoSeim.RESPRORE
+        log_sistema \
+            .add_params("es_prorroga", True)
 
+    elif not models.EstadoEvaluacion.objects.filter(id=estado_evaluacion).exists():
+        print("El estado de evaluacion no existe")
+        #log_sistema.error("El estado de evaluacion no existe")
+        raise models.EstadoEvaluacion.DoesNotExist
+
+    else:
+        #print("Estoy en el if de estado evaluacion")
+        if estado_evaluacion == models.EstadoEvaluacion.RESOLUCION_OBSERVADO:
+            log_sistema.add_params("es_observado", True)
+            if o_evaluacion.imiv.tipo_imiv_id == models.TipoIMIV.TIPO_IMIV_INFORME_SUFICIENCIA:
+                tipo_documento_seim = constants.DOCTO_SEIM_RESOLUCION_SUFICIENCIA_OBSERVA
+            else:
+                tipo_documento_seim = models.TipoDocumentoSeim.RESEVAOBS if o_ficha.tipo_ficha == constants.TIPO_FICHA_SIMPLE else \
+                    models.TipoDocumentoSeim.RESEVAOBC
+        elif estado_evaluacion in [models.EstadoEvaluacion.RESOLUCION_APROBADO, models.EstadoEvaluacion.RESOLUCION_RECHAZADO]:
+            if o_evaluacion.imiv.tipo_imiv_id == models.TipoIMIV.TIPO_IMIV_INFORME_SUFICIENCIA:
+                tipo_documento_seim = constants.DOCTO_SEIM_RESOLUCION_SUFICIENCIA_APRUEBA_RECHAZA
+            else:
+                tipo_documento_seim = models.TipoDocumentoSeim.RESSEREVA if o_ficha.tipo_ficha == constants.TIPO_FICHA_SIMPLE else \
+                    models.TipoDocumentoSeim.RESEVAC
+        elif estado_evaluacion == models.EstadoEvaluacion.RESOLUCION_DESISTIDO:
+            tipo_documento_seim = models.TipoDocumentoSeim.RESDES
+        elif estado_evaluacion == models.EstadoEvaluacion.RECHAZADO_NO_CORRECCION:
+            tipo_documento_seim = models.TipoDocumentoSeim.RESNOCOS
         else:
-            print('firma_electronica_avanzada: es proyecto conjunto')
-            o_proyecto_ficha = models.Proyecto_Ficha.objects.filter(ficha_id=o_ficha, proyecto_principal=True).first()
-            #log_sistema.info('firma_electronica_avanzada: es proyecto conjunto')
-            setLogSistema(log_sistema, 'firma_electronica_avanzada: es proyecto conjunto', 'INFO', set_log_sistema)
-
-        personas = obtiene_titular_representante_proyecto(o_proyecto_ficha.proyecto_id.rut_pertenece)
-        if personas['titular'] is not None:
-            print('firma_electronica_avanzada: El titular no es None')
-            l_distribucion_externa.add(personas['titular']['nombre_completo'])
-
-        if personas['responsable'] is not None:
-            print('firma_electronica_avanzada: El responsable no es None')
-            l_distribucion_externa.add(personas['responsable']['nombre_completo'])
-
-        # AOC
-        for aoc in models.Analista_Competente_Ficha.objects.filter(evaluacion_imiv=o_evaluacion).exclude(usuario_respuesta=None):
-            print(f'firma_electronica_avanzada: Se añade el AOC {aoc} a la lista de distribución')
-            l_distribucion_externa.add(aoc.usuario_respuesta.nombre_completo)
-
-        # AOE
-        o_analista_asignado = models.Analista_Asignado.objects.filter(evaluacion_imiv=o_evaluacion, vigente=True).first()
-        print(f'firma_electronica_avanzada: Se añade el AOE {o_analista_asignado} a la lista de distribución y la cadena de confianza')
-        l_distribucion_externa.add(o_analista_asignado.usuario.nombre_completo)
-        l_cadena_confianza_seim = o_analista_asignado.usuario.cadena_de_confianza
-
-        # revisor
-        # Solo seremi
-        revisor = models.Permiso.objects.filter(
-            acceso_id=constants.ACCESO_SEREMITT_SEREMI,
-            region_asignada=o_evaluacion.imiv.region_evaluador,
-            usuario__estado=True,
-            estado=True
-        ).first()
-
-        if models.Comuna.objects.filter(provincia__region=o_evaluacion.imiv.region_evaluador, es_capital_regional=True).exists():
-            
-            l_ciudad = models.Comuna.objects.filter(
-                provincia__region=o_evaluacion.imiv.region_evaluador, es_capital_regional=True
-            ).first().nombre
-        else:
-            l_ciudad = ""
+            #log_sistema.error("Estado de evaluación no implementado para firma electrónica avanzada")
+            raise Exception("Estado de evaluación no implementado para firma electrónica avanzada")
+        
+    print(f"tipo documento seim es {tipo_documento_seim}")
+    log_sistema.add_params('tipo_documento_seim', tipo_documento_seim)
+    #.info(f'FEA: el documento es {tipo_documento_seim}')
+    setLogSistema(log_sistema, f'FEA: el documento es {tipo_documento_seim}', 'INFO', set_log_sistema)
+
+    if models.DocumentoEvaluacionImiv.objects.filter(
+        evaluacion_imiv=o_evaluacion,
+        tipo_documento_seim=models.TipoDocumentoSeim.get_id(tipo_documento_seim),
+        vigente=True
+    ).exists():
+        print("El documento evaluacion imiv existe")
+        #log_sistema.info('El documento evaluacion imiv existe')
+        setLogSistema(log_sistema, 'El documento evaluacion imiv existe', 'INFO', set_log_sistema)
 
-        l_organizacion_seim = revisor.region_asignada.nombre_formal.upper()
-        l_tipo_materia = 107
+        o_documento_evaluacion_imiv = models.DocumentoEvaluacionImiv.objects.get(
+            evaluacion_imiv=o_evaluacion,
+            tipo_documento_seim=models.TipoDocumentoSeim.get_id(tipo_documento_seim),
+            vigente=True
+        )
+        o_archivo = o_documento_evaluacion_imiv.documento.file
 
-        l_distribucion_externa.add(revisor.usuario.nombre_completo)
+    elif borrador is not None:
+        log_sistema.add_params("es_borrador", True)
+        o_archivo = borrador.archivo
+
+    else:
+        print("No existe documento para enviar a firmar")
+        #log_sistema.error("No existe documento para enviar a firmar")
+        raise models.DocumentoEvaluacionImiv.DoesNotExist
+    
+    print("firma_electronica_avanzada: se encontró el documento")
+    log_sistema.add_params("o_archivo", o_archivo)
+    #.info('firma_electronica_avanzada: se encontró el documento')
+    setLogSistema(log_sistema, 'firma_electronica_avanzada: se encontró el documento', 'INFO', set_log_sistema)
+
+    # Distribución externa
+    l_distribucion_externa = set([])
+
+    # Interesado
+    if o_ficha.tipo_ficha == constants.TIPO_FICHA_SIMPLE:
+        o_proyecto_ficha = models.Proyecto_Ficha.objects.filter(ficha_id=o_ficha).first()
+        print('firma_electronica_avanzada: es proyecto simple')
+        #log_sistema.info('firma_electronica_avanzada: es proyecto simple')
+        setLogSistema(log_sistema, 'firma_electronica_avanzada: es proyecto simple', 'INFO', set_log_sistema)
+
+    else:
+        print('firma_electronica_avanzada: es proyecto conjunto')
+        o_proyecto_ficha = models.Proyecto_Ficha.objects.filter(ficha_id=o_ficha, proyecto_principal=True).first()
+        #log_sistema.info('firma_electronica_avanzada: es proyecto conjunto')
+        setLogSistema(log_sistema, 'firma_electronica_avanzada: es proyecto conjunto', 'INFO', set_log_sistema)
+
+    personas = obtiene_titular_representante_proyecto(o_proyecto_ficha.proyecto_id.rut_pertenece)
+    if personas['titular'] is not None:
+        print('firma_electronica_avanzada: El titular no es None')
+        l_distribucion_externa.add(personas['titular']['nombre_completo'])
+
+    if personas['responsable'] is not None:
+        print('firma_electronica_avanzada: El responsable no es None')
+        l_distribucion_externa.add(personas['responsable']['nombre_completo'])
+
+    # AOC
+    for aoc in models.Analista_Competente_Ficha.objects.filter(evaluacion_imiv=o_evaluacion).exclude(usuario_respuesta=None):
+        print(f'firma_electronica_avanzada: Se añade el AOC {aoc} a la lista de distribución')
+        l_distribucion_externa.add(aoc.usuario_respuesta.nombre_completo)
+
+    # AOE
+    o_analista_asignado = models.Analista_Asignado.objects.filter(evaluacion_imiv=o_evaluacion, vigente=True).first()
+    print(f'firma_electronica_avanzada: Se añade el AOE {o_analista_asignado} a la lista de distribución y la cadena de confianza')
+    l_distribucion_externa.add(o_analista_asignado.usuario.nombre_completo)
+    l_cadena_confianza_seim = o_analista_asignado.usuario.cadena_de_confianza
+
+    # revisor
+    # Solo seremi
+    revisor = models.Permiso.objects.filter(
+        acceso_id=constants.ACCESO_SEREMITT_SEREMI,
+        region_asignada=o_evaluacion.imiv.region_evaluador,
+        usuario__estado=True,
+        estado=True
+    ).first()
 
-        l_distribucion_externa.add("Biblioteca")
-        l_distribucion_externa.add("Gobierno Transparente")
-        l_distribucion_externa_str = ' \n'.join(str(e) for e in l_distribucion_externa)
-
-        l_emisor = settings.EMISOR_DOCUMENTO_EXEDOC
-
-        l_materia = models.TipoDocumentoSeim.get_name(tipo_documento_seim)
-        l_id = models.TipoDocumentoSeim.get_id(tipo_documento_seim)
-        fechas_plazo = get_fecha_vencimiento_evaluacion(o_evaluacion.id)
-        l_plazo_firma = date_to_str_local(fechas_plazo["fecha_plazo_AOE"], "%Y-%m-%d %H:%M:%S")
-
-        l_url_callback = f"{settings.URL_CALLBACK_EXEDOC}{l_id}/{o_archivo.id}/"
-        log_sistema.add_params('l_url_callback', l_url_callback)
-        #.info(f'FEA: el callback es {l_url_callback}')
-        setLogSistema(log_sistema, f'FEA: el callback es {l_url_callback}', 'INFO', set_log_sistema)
-
-        l_nombre_archivo = o_archivo.name
-
-        l_numero_expediente = o_evaluacion.imiv.ficha.expediente
-        log_sistema.add_params('l_numero_expediente', l_numero_expediente)
-        #.info(f'FEA: el nro de expediente es {l_numero_expediente}')
-        setLogSistema(log_sistema, f'FEA: el nro de expediente es {l_numero_expediente}', 'INFO', set_log_sistema)
-
-        l_version_doc = 1
-        # TODO  Versión de documento, en un inicio es 1
-
-        responsable = responsable_departamento_exedoc(o_evaluacion.imiv)
-        l_firmante = responsable["email"].split("@")[0]
-
-        l_firma_acotada = True if tipo_documento_seim not in [models.TipoDocumentoSeim.RESDES, models.TipoDocumentoSeim.RESNOCOM, models.TipoDocumentoSeim.RESNOCOS] else False
-
-        request_json = {
-            "emisor": "seim",
-            "documento": {
-                "autor": "seim",
-                "tipoDocumento": 104,
-                "tipoMateria": l_tipo_materia,
-                "reservado": False,
-                "actosEfectosTerceros": False,
-                "antecedentes": "Sin antecedentes",
-                "materia": l_materia,
-                "emisor": l_emisor,
-                "ciudad": l_ciudad,
-                "versionDoc": l_version_doc,
-                "plazoFirma": l_plazo_firma,
-                "firmaAcotada": l_firma_acotada,
-                "fechaTope": l_plazo_firma,
-                "urlCallbackSeim": l_url_callback,
-                "destinatario": ["Expediente IMIV"],
-                "dataArchivo": o_archivo.get_url(),
-                "nombreArchivo": l_nombre_archivo,
-                "contentType": "application/pdf",
-                "visadores": [],
-                "firmantes": [{
-                    "usuario": l_firmante,
-                    "esGrupo": False,
-                    "orden": "1"
-                }],
-                "distribucion": [],
-                "organizacionSeim": l_organizacion_seim,
-                "cadenaConfianzaSeim": l_cadena_confianza_seim,
-                "distribucionExterna": l_distribucion_externa_str
-            },
-            "destinatario": [{
+    if models.Comuna.objects.filter(provincia__region=o_evaluacion.imiv.region_evaluador, es_capital_regional=True).exists():
+        
+        l_ciudad = models.Comuna.objects.filter(
+            provincia__region=o_evaluacion.imiv.region_evaluador, es_capital_regional=True
+        ).first().nombre
+    else:
+        l_ciudad = ""
+
+    l_organizacion_seim = revisor.region_asignada.nombre_formal.upper()
+    l_tipo_materia = 107
+
+    l_distribucion_externa.add(revisor.usuario.nombre_completo)
+
+    l_distribucion_externa.add("Biblioteca")
+    l_distribucion_externa.add("Gobierno Transparente")
+    l_distribucion_externa_str = ' \n'.join(str(e) for e in l_distribucion_externa)
+
+    l_emisor = settings.EMISOR_DOCUMENTO_EXEDOC
+
+    l_materia = models.TipoDocumentoSeim.get_name(tipo_documento_seim)
+    l_id = models.TipoDocumentoSeim.get_id(tipo_documento_seim)
+    fechas_plazo = get_fecha_vencimiento_evaluacion(o_evaluacion.id)
+    l_plazo_firma = date_to_str_local(fechas_plazo["fecha_plazo_AOE"], "%Y-%m-%d %H:%M:%S")
+
+    l_url_callback = f"{settings.URL_CALLBACK_EXEDOC}{l_id}/{o_archivo.id}/"
+    log_sistema.add_params('l_url_callback', l_url_callback)
+    #.info(f'FEA: el callback es {l_url_callback}')
+    setLogSistema(log_sistema, f'FEA: el callback es {l_url_callback}', 'INFO', set_log_sistema)
+
+    l_nombre_archivo = o_archivo.name
+
+    l_numero_expediente = o_evaluacion.imiv.ficha.expediente
+    log_sistema.add_params('l_numero_expediente', l_numero_expediente)
+    #.info(f'FEA: el nro de expediente es {l_numero_expediente}')
+    setLogSistema(log_sistema, f'FEA: el nro de expediente es {l_numero_expediente}', 'INFO', set_log_sistema)
+
+    l_version_doc = 1
+    # TODO  Versión de documento, en un inicio es 1
+
+    responsable = responsable_departamento_exedoc(o_evaluacion.imiv)
+    l_firmante = responsable["email"].split("@")[0]
+
+    l_firma_acotada = True if tipo_documento_seim not in [models.TipoDocumentoSeim.RESDES, models.TipoDocumentoSeim.RESNOCOM, models.TipoDocumentoSeim.RESNOCOS] else False
+
+    request_json = {
+        "emisor": "seim",
+        "documento": {
+            "autor": "seim",
+            "tipoDocumento": 104,
+            "tipoMateria": l_tipo_materia,
+            "reservado": False,
+            "actosEfectosTerceros": False,
+            "antecedentes": "Sin antecedentes",
+            "materia": l_materia,
+            "emisor": l_emisor,
+            "ciudad": l_ciudad,
+            "versionDoc": l_version_doc,
+            "plazoFirma": l_plazo_firma,
+            "firmaAcotada": l_firma_acotada,
+            "fechaTope": l_plazo_firma,
+            "urlCallbackSeim": l_url_callback,
+            "destinatario": ["Expediente IMIV"],
+            "dataArchivo": o_archivo.get_url(),
+            "nombreArchivo": l_nombre_archivo,
+            "contentType": "application/pdf",
+            "visadores": [],
+            "firmantes": [{
                 "usuario": l_firmante,
-                "copia": False
+                "esGrupo": False,
+                "orden": "1"
             }],
-            "observacion": [{
-                "texto": "Sin observaciones",
-                "adjuntadoPor": "seim"
-            }]
-        }
-
-        if l_numero_expediente:
-            request_json["documento"].update(
-                {
-                    "numeroExpediente": l_numero_expediente
-                }
-            )
-
-        print('firma_electronica_avanzada: request enviado', request_json)
-        log_sistema.add_params('request_json', request_json)
-        #.info('FEA: Los parametros de la firma avanzada')
-        setLogSistema(log_sistema, 'FEA: Los parametros de la firma avanzada', 'INFO', set_log_sistema)
+            "distribucion": [],
+            "organizacionSeim": l_organizacion_seim,
+            "cadenaConfianzaSeim": l_cadena_confianza_seim,
+            "distribucionExterna": l_distribucion_externa_str
+        },
+        "destinatario": [{
+            "usuario": l_firmante,
+            "copia": False
+        }],
+        "observacion": [{
+            "texto": "Sin observaciones",
+            "adjuntadoPor": "seim"
+        }]
+    }
+
+    if l_numero_expediente:
+        request_json["documento"].update(
+            {
+                "numeroExpediente": l_numero_expediente
+            }
+        )
+
+    print('firma_electronica_avanzada: request enviado', request_json)
+    log_sistema.add_params('request_json', request_json)
+    #.info('FEA: Los parametros de la firma avanzada')
+    setLogSistema(log_sistema, 'FEA: Los parametros de la firma avanzada', 'INFO', set_log_sistema)
 
-        o_archivo.request_firma = request_json
-        o_archivo.save()
+    o_archivo.request_firma = request_json
+    o_archivo.save()
 
-        print(f'firma_electronica_avanzada: call inyectar_doc_exedoc({ficha_id}, {o_archivo}, {log_sistema.to_dict()})')
-        return inyectar_doc_exedoc(ficha_id,o_archivo,log_sistema,settings, set_log_sistema)
-    
+    print(f'firma_electronica_avanzada: call inyectar_doc_exedoc({ficha_id}, {o_archivo}, {log_sistema.to_dict()})')
+    return inyectar_doc_exedoc(ficha_id,o_archivo,log_sistema,settings, set_log_sistema)
 
-    except Exception as exception:
-        log = f'Error: {exception.__str__()}'
-        log_sistema \
-            .add_params("ficha_id", ficha_id) \
-            .add_params("estado_evaluacion", estado_evaluacion) \
-            .add_params("prorroga", prorroga) \
-            .add_params("borrador", borrador) \
-            .add_params('exception', exception.__str__()) \
-            .add_params('mensaje', log) \
-            .set_traceback('\n '.join(traceback.format_exc().splitlines()), ''.join(traceback.format_stack())) \
-        
-        setLogSistema(log_sistema, log, 'ERROR', set_log_sistema)
 
 
 def inyectar_doc_exedoc(
     ficha_id: str, # id de la ficha
     o_archivo,  # objeto de Archivo
     log_params, # objeto de SeimLogSistema
     settings, # objeto de settings
```

### Comparing `testing_package_exedoc-0.0.6/src/testing_package_exedoc.egg-info/PKG-INFO` & `testing_package_exedoc-0.0.7/src/testing_package_exedoc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testing_package_exedoc
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package for testing exedoc
 Author-email: Rompni <andresnavarrodev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

