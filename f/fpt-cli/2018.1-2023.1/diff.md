# Comparing `tmp/fpt-cli-2018.1.tar.gz` & `tmp/fpt-cli-2023.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fpt-cli-2018.1.tar", last modified: Mon Jan 22 17:51:14 2018, max compression
+gzip compressed data, was "fpt-cli-2023.1.tar", last modified: Sat Jun 24 01:14:15 2023, max compression
```

## Comparing `fpt-cli-2018.1.tar` & `fpt-cli-2023.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 matiasb   (1000) matiasb   (1000)        0 2018-01-22 17:51:14.000000 fpt-cli-2018.1/
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     1142 2018-01-22 16:23:05.000000 fpt-cli-2018.1/README.rst
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)       27 2017-11-05 15:38:37.000000 fpt-cli-2018.1/MANIFEST.in
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     1555 2017-11-11 19:00:24.000000 fpt-cli-2018.1/setup.py
-drwxrwxr-x   0 matiasb   (1000) matiasb   (1000)        0 2018-01-22 17:51:14.000000 fpt-cli-2018.1/fpt/
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)       22 2018-01-22 16:23:33.000000 fpt-cli-2018.1/fpt/__version__.py
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)        0 2017-11-04 16:53:29.000000 fpt-cli-2018.1/fpt/__init__.py
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     5071 2018-01-22 16:23:05.000000 fpt-cli-2018.1/fpt/main.py
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     4603 2017-10-28 00:10:08.000000 fpt-cli-2018.1/fpt/api.py
-drwxrwxr-x   0 matiasb   (1000) matiasb   (1000)        0 2018-01-22 17:51:14.000000 fpt-cli-2018.1/fpt_cli.egg-info/
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)        1 2017-11-11 19:01:20.000000 fpt-cli-2018.1/fpt_cli.egg-info/not-zip-safe
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)       39 2018-01-22 17:51:14.000000 fpt-cli-2018.1/fpt_cli.egg-info/entry_points.txt
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)      325 2018-01-22 17:51:14.000000 fpt-cli-2018.1/fpt_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     2442 2018-01-22 17:51:14.000000 fpt-cli-2018.1/fpt_cli.egg-info/PKG-INFO
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)        4 2018-01-22 17:51:14.000000 fpt-cli-2018.1/fpt_cli.egg-info/top_level.txt
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)       41 2018-01-22 17:51:14.000000 fpt-cli-2018.1/fpt_cli.egg-info/requires.txt
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)        1 2018-01-22 17:51:14.000000 fpt-cli-2018.1/fpt_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     1063 2017-10-23 23:30:38.000000 fpt-cli-2018.1/LICENSE
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     2442 2018-01-22 17:51:14.000000 fpt-cli-2018.1/PKG-INFO
--rw-rw-r--   0 matiasb   (1000) matiasb   (1000)      102 2018-01-22 17:51:14.000000 fpt-cli-2018.1/setup.cfg
+drwxrwxr-x   0 matiasb   (1000) matiasb   (1000)        0 2023-06-24 01:14:15.395385 fpt-cli-2023.1/
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     1063 2023-05-23 19:48:13.000000 fpt-cli-2023.1/LICENSE
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)       27 2023-05-23 19:48:13.000000 fpt-cli-2023.1/MANIFEST.in
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     1743 2023-06-24 01:14:15.395385 fpt-cli-2023.1/PKG-INFO
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     1142 2023-05-23 19:48:13.000000 fpt-cli-2023.1/README.rst
+drwxrwxr-x   0 matiasb   (1000) matiasb   (1000)        0 2023-06-24 01:14:15.395385 fpt-cli-2023.1/fpt/
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)        0 2023-05-23 19:48:13.000000 fpt-cli-2023.1/fpt/__init__.py
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)       22 2023-06-24 01:04:39.000000 fpt-cli-2023.1/fpt/__version__.py
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     4573 2023-05-23 19:51:50.000000 fpt-cli-2023.1/fpt/api.py
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     5169 2023-06-24 01:14:12.000000 fpt-cli-2023.1/fpt/main.py
+drwxrwxr-x   0 matiasb   (1000) matiasb   (1000)        0 2023-06-24 01:14:15.395385 fpt-cli-2023.1/fpt_cli.egg-info/
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     1743 2023-06-24 01:14:15.000000 fpt-cli-2023.1/fpt_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)      325 2023-06-24 01:14:15.000000 fpt-cli-2023.1/fpt_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)        1 2023-06-24 01:14:15.000000 fpt-cli-2023.1/fpt_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)       38 2023-06-24 01:14:15.000000 fpt-cli-2023.1/fpt_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)        1 2023-06-24 01:07:10.000000 fpt-cli-2023.1/fpt_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)       41 2023-06-24 01:14:15.000000 fpt-cli-2023.1/fpt_cli.egg-info/requires.txt
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)        4 2023-06-24 01:14:15.000000 fpt-cli-2023.1/fpt_cli.egg-info/top_level.txt
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)      102 2023-06-24 01:14:15.395385 fpt-cli-2023.1/setup.cfg
+-rw-rw-r--   0 matiasb   (1000) matiasb   (1000)     1555 2023-05-23 19:48:13.000000 fpt-cli-2023.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fpt-cli-2018.1/README.rst` & `fpt-cli-2023.1/README.rst`

 * *Files identical despite different names*

### Comparing `fpt-cli-2018.1/setup.py` & `fpt-cli-2023.1/setup.py`

 * *Files identical despite different names*

### Comparing `fpt-cli-2018.1/fpt/main.py` & `fpt-cli-2023.1/fpt/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     click.secho(
         "%-3s %-25s %-5s %-3s %-10s" %
         ("POS", "EQUIPO", "  PTS", " PJ", "  PROMEDIO"))
     for i, r in enumerate(rows, start=1):
         team_str = ("{pos:<3} {row.team:<25} {row.pts:>5} "
                     "{row.p:>3} {row.average:>10}").format(pos=i, row=r)
         color = 'blue'
-        if (total - 4) < i <= total:
-            # 4 last
+        if (total - 1) < i <= total:
+            # last one
             color = 'red'
         click.secho(team_str, fg=color)
     click.echo()
     click.secho('En zona de descenso', fg='red')
 
 
 def show_standings():
@@ -42,24 +42,27 @@
          " GF", " GC", " DG")
     )
     for i, r in enumerate(rows, start=1):
         team_str = ("{pos:<3} {row.team:<25} {row.pts:>5} "
                     "{row.p:>3} {row.w:>3} {row.d:>3} {row.l:>3} "
                     "{row.f:>3} {row.a:>3} {row.gd:>3}").format(pos=i, row=r)
         color = 'blue'
-        if i <= 5:
+        if i <= 3:
             # libertadores
             color = 'green'
-        elif 5 < i <= 11:
+        elif 3 < i <= 9:
             # sudamericana
             color = 'yellow'
+        elif i == 28:
+            color = 'red'
         click.secho(team_str, fg=color)
     click.echo()
     click.secho('En zona de clasificación a Copa Libertadores', fg='green')
     click.secho('En zona de clasificación a Copa Sudamericana', fg='yellow')
+    click.secho('En zona de descenso', fg='red')
 
 
 def _show_matches(matches, enum=False):
     """Display given matches."""
     for i, m in enumerate(matches, start=1):
         home_color = away_color = 'yellow'
         if m.is_finished and m.home_goals > m.away_goals:
```

### Comparing `fpt-cli-2018.1/fpt/api.py` & `fpt-cli-2023.1/fpt/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -65,21 +65,21 @@
     def is_current(self):
         return 'show' in self._css_class
 
 
 class StandingsRow(demiurge.Item):
     team = demiurge.TextField(selector='td.team')
     pts = demiurge.TextField(selector='td.puntos')
-    p = demiurge.TextField(selector='td.hidden-xs:eq(0)')
-    w = demiurge.TextField(selector='td.hidden-xs:eq(1)')
-    d = demiurge.TextField(selector='td.hidden-xs:eq(2)')
-    l = demiurge.TextField(selector='td.hidden-xs:eq(3)')
-    f = demiurge.TextField(selector='td.hidden-xs:eq(4)')
-    a = demiurge.TextField(selector='td.hidden-xs:eq(5)')
-    gd = demiurge.TextField(selector='td.hidden-xs:eq(6)')
+    p = demiurge.TextField(selector='td.d-none:eq(0)')
+    w = demiurge.TextField(selector='td.d-none:eq(1)')
+    d = demiurge.TextField(selector='td.d-none:eq(2)')
+    l = demiurge.TextField(selector='td.d-none:eq(3)')
+    f = demiurge.TextField(selector='td.d-none:eq(4)')
+    a = demiurge.TextField(selector='td.d-none:eq(5)')
+    gd = demiurge.TextField(selector='td.d-none:eq(6)')
 
     class Meta:
         selector = 'tr.linea'
         encoding = 'utf-8'
 
 
 class Standings(demiurge.Item):
@@ -91,17 +91,17 @@
         base_url = BASE_URL + 'posiciones.html'
 
 
 class RelegationRow(demiurge.Item):
     team = demiurge.TextField(selector='td.team')
     average = demiurge.TextField(selector='td.promediodescenso')
 
-    before1 = demiurge.TextField(selector='td.hidden-xs:eq(0)')
-    before2 = demiurge.TextField(selector='td.hidden-xs:eq(1)')
-    before3 = demiurge.TextField(selector='td.hidden-xs:eq(2)')
+    before1 = demiurge.TextField(selector='td.d-none:eq(0)')
+    before2 = demiurge.TextField(selector='td.d-none:eq(1)')
+    before3 = demiurge.TextField(selector='td.d-none:eq(2)')
     current = demiurge.TextField(selector='td.puntosactual')
 
     pts = demiurge.TextField(selector='td.puntosdescenso')
     p = demiurge.TextField(selector='td.jugadosdescenso')
 
     class Meta:
         selector = 'tr.linea'
```

### Comparing `fpt-cli-2018.1/fpt_cli.egg-info/PKG-INFO` & `fpt-cli-2023.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,99 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fpt-cli
-Version: 2018.1
+Version: 2023.1
 Summary: Estadísticas de la primera división del fútbol argentino por línea de comandos.
 Home-page: https://github.com/el-ega/fpt-cli
 Author: Matias Bordese
 Author-email: mbordese@gmail.com
 License: MIT
-Description-Content-Type: UNKNOWN
-Description: FPT-cli
-        =======
-        
-        *Facilitame los Partidos del Torneo*
-        
-        Estadísticas de la primera división del fútbol argentino por línea de
-        comandos.
-        
-        Instalación
-        ===========
-        
-        Usando ``pip``
-        ~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ pip install fpt-cli
-        
-        Desde el source
-        ~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ git clone https://github.com/el-ega/fpt-cli.git
-            $ cd fpt-cli
-            $ python setup.py install
-        
-        Debería correr en Linux, Mac OS X, NetBSD, FreeBSD y Windows.
-        
-        Cómo se usa?
-        ============
-        
-        Ver posiciones del torneo
-        ~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ fpt --posiciones
-        
-        Ver tabla del descenso
-        ~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ fpt --descenso
-        
-        Ver fixture para un equipo particular
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ fpt --equipo=Boca
-        
-        Ver fecha actual
-        ~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ fpt --fecha-actual
-        
-        Ver resultados de partidos en juego
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ fpt --en-juego
-        
-        Ayuda
-        ~~~~~
-        
-        .. code:: bash
-        
-            $ fpt --help
-        
-        Licencia
-        ========
-        
-        Liberado bajo `MIT License`_
-        
-        *Inspirado en https://github.com/architv/soccer-cli*
-        
-        .. _MIT License: LICENSE
-        
 Keywords: fútbol,argentina,resultados,estadísticas
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
+License-File: LICENSE
+
+FPT-cli
+=======
+
+*Facilitame los Partidos del Torneo*
+
+Estadísticas de la primera división del fútbol argentino por línea de
+comandos.
+
+Instalación
+===========
+
+Usando ``pip``
+~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ pip install fpt-cli
+
+Desde el source
+~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ git clone https://github.com/el-ega/fpt-cli.git
+    $ cd fpt-cli
+    $ python setup.py install
+
+Debería correr en Linux, Mac OS X, NetBSD, FreeBSD y Windows.
+
+Cómo se usa?
+============
+
+Ver posiciones del torneo
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ fpt --posiciones
+
+Ver tabla del descenso
+~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ fpt --descenso
+
+Ver fixture para un equipo particular
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ fpt --equipo=Boca
+
+Ver fecha actual
+~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ fpt --fecha-actual
+
+Ver resultados de partidos en juego
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ fpt --en-juego
+
+Ayuda
+~~~~~
+
+.. code:: bash
+
+    $ fpt --help
+
+Licencia
+========
+
+Liberado bajo `MIT License`_
+
+*Inspirado en https://github.com/architv/soccer-cli*
+
+.. _MIT License: LICENSE
```

### Comparing `fpt-cli-2018.1/LICENSE` & `fpt-cli-2023.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fpt-cli-2018.1/PKG-INFO` & `fpt-cli-2023.1/fpt_cli.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,99 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fpt-cli
-Version: 2018.1
+Version: 2023.1
 Summary: Estadísticas de la primera división del fútbol argentino por línea de comandos.
 Home-page: https://github.com/el-ega/fpt-cli
 Author: Matias Bordese
 Author-email: mbordese@gmail.com
 License: MIT
-Description-Content-Type: UNKNOWN
-Description: FPT-cli
-        =======
-        
-        *Facilitame los Partidos del Torneo*
-        
-        Estadísticas de la primera división del fútbol argentino por línea de
-        comandos.
-        
-        Instalación
-        ===========
-        
-        Usando ``pip``
-        ~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ pip install fpt-cli
-        
-        Desde el source
-        ~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ git clone https://github.com/el-ega/fpt-cli.git
-            $ cd fpt-cli
-            $ python setup.py install
-        
-        Debería correr en Linux, Mac OS X, NetBSD, FreeBSD y Windows.
-        
-        Cómo se usa?
-        ============
-        
-        Ver posiciones del torneo
-        ~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ fpt --posiciones
-        
-        Ver tabla del descenso
-        ~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ fpt --descenso
-        
-        Ver fixture para un equipo particular
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ fpt --equipo=Boca
-        
-        Ver fecha actual
-        ~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ fpt --fecha-actual
-        
-        Ver resultados de partidos en juego
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            $ fpt --en-juego
-        
-        Ayuda
-        ~~~~~
-        
-        .. code:: bash
-        
-            $ fpt --help
-        
-        Licencia
-        ========
-        
-        Liberado bajo `MIT License`_
-        
-        *Inspirado en https://github.com/architv/soccer-cli*
-        
-        .. _MIT License: LICENSE
-        
 Keywords: fútbol,argentina,resultados,estadísticas
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
+License-File: LICENSE
+
+FPT-cli
+=======
+
+*Facilitame los Partidos del Torneo*
+
+Estadísticas de la primera división del fútbol argentino por línea de
+comandos.
+
+Instalación
+===========
+
+Usando ``pip``
+~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ pip install fpt-cli
+
+Desde el source
+~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ git clone https://github.com/el-ega/fpt-cli.git
+    $ cd fpt-cli
+    $ python setup.py install
+
+Debería correr en Linux, Mac OS X, NetBSD, FreeBSD y Windows.
+
+Cómo se usa?
+============
+
+Ver posiciones del torneo
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ fpt --posiciones
+
+Ver tabla del descenso
+~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ fpt --descenso
+
+Ver fixture para un equipo particular
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ fpt --equipo=Boca
+
+Ver fecha actual
+~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ fpt --fecha-actual
+
+Ver resultados de partidos en juego
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ fpt --en-juego
+
+Ayuda
+~~~~~
+
+.. code:: bash
+
+    $ fpt --help
+
+Licencia
+========
+
+Liberado bajo `MIT License`_
+
+*Inspirado en https://github.com/architv/soccer-cli*
+
+.. _MIT License: LICENSE
```

