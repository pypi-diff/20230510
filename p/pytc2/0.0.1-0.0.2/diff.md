# Comparing `tmp/pytc2-0.0.1.tar.gz` & `tmp/pytc2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytc2-0.0.1.tar", max compression
+gzip compressed data, was "pytc2-0.0.2.tar", max compression
```

## Comparing `pytc2-0.0.1.tar` & `pytc2-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rwxr-xr-x   0        0        0     1080 2023-03-09 11:48:58.092063 pytc2-0.0.1/LICENSE
--rw-r--r--   0        0        0      687 2023-03-09 11:48:58.100062 pytc2-0.0.1/README.md
--rw-r--r--   0        0        0      706 2023-03-09 11:48:58.108062 pytc2-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1858 2023-03-09 11:48:58.108062 pytc2-0.0.1/src/pytc2/__init__.py
--rw-r--r--   0        0        0    21222 2023-03-13 18:34:45.304006 pytc2-0.0.1/src/pytc2/cuadripolos.py
--rw-r--r--   0        0        0    27228 2023-03-09 13:23:00.725423 pytc2-0.0.1/src/pytc2/dibujar.py
--rw-r--r--   0        0        0     1847 2023-03-09 13:20:47.279045 pytc2-0.0.1/src/pytc2/general.py
--rw-r--r--   0        0        0     1682 2023-03-09 11:48:58.108062 pytc2-0.0.1/src/pytc2/imagen.py
--rw-r--r--   0        0        0     7210 2023-03-09 11:48:58.108062 pytc2-0.0.1/src/pytc2/ltspice.py
--rw-r--r--   0        0        0    15900 2023-03-09 13:24:20.606830 pytc2-0.0.1/src/pytc2/remociones.py
--rw-r--r--   0        0        0     6525 2023-03-09 13:24:44.423248 pytc2-0.0.1/src/pytc2/sintesis_dipolo.py
--rw-r--r--   0        0        0    48704 2023-03-13 18:30:33.778867 pytc2-0.0.1/src/pytc2/sistemas_lineales.py
--rw-r--r--   0        0        0     1436 1970-01-01 00:00:00.000000 pytc2-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1080 2023-04-18 22:36:19.453348 pytc2-0.0.2/LICENSE
+-rw-r--r--   0        0        0      859 2023-04-18 22:36:19.457348 pytc2-0.0.2/README.md
+-rw-r--r--   0        0        0      896 2023-05-09 22:54:14.724460 pytc2-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1858 2023-04-18 22:36:19.477348 pytc2-0.0.2/src/pytc2/__init__.py
+-rw-r--r--   0        0        0    21251 2023-05-09 22:25:00.708452 pytc2-0.0.2/src/pytc2/cuadripolos.py
+-rw-r--r--   0        0        0    32307 2023-05-09 22:25:00.708452 pytc2-0.0.2/src/pytc2/dibujar.py
+-rw-r--r--   0        0        0     1763 2023-04-20 20:45:17.511151 pytc2-0.0.2/src/pytc2/ej5.13 schaumann.py
+-rw-r--r--   0        0        0     4811 2023-05-09 22:25:00.708452 pytc2-0.0.2/src/pytc2/general.py
+-rw-r--r--   0        0        0     2376 2023-04-18 22:36:19.481348 pytc2-0.0.2/src/pytc2/imagen.py
+-rw-r--r--   0        0        0     8598 2023-04-18 22:36:19.481348 pytc2-0.0.2/src/pytc2/ltspice.py
+-rw-r--r--   0        0        0    16960 2023-04-19 14:59:38.942917 pytc2-0.0.2/src/pytc2/remociones.py
+-rw-r--r--   0        0        0     6525 2023-04-18 22:36:19.481348 pytc2-0.0.2/src/pytc2/sintesis_dipolo.py
+-rw-r--r--   0        0        0    56375 2023-04-19 15:02:51.214773 pytc2-0.0.2/src/pytc2/sistemas_lineales.py
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 pytc2-0.0.2/PKG-INFO
```

### Comparing `pytc2-0.0.1/LICENSE` & `pytc2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytc2-0.0.1/pyproject.toml` & `pytc2-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,39 @@
+
 [tool.poetry]
 name = "pytc2"
-version = "0.0.1"
+version = "0.0.2"
 description = "A circuit theory module for students at Universidad Tecnológica Nacional Regional Buen"
 authors = ["Mariano Llamedo Soria"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "<3.12, >=3.8"
+#prompt-toolkit = "^3.0.38"
+#jupyter-console = "^6.6.3"
+#ipython = "^7.34"
 sympy = "^1.11.1"
 schemdraw = "^0.15"
 jupyter = "^1.0.0"
 matplotlib = "^3.7.0"
-spyder = "^5.4.2"
-pyfda = "^0.7.1"
+#spyder = "^5.4.2"
+#pyfda = "^0.7.1"
+numpy = "^1.24.2"
+scipy = "^1.10.1"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 jupyter = "^1.0.0"
 myst-nb = {version = "^0.17.1", python = "^3.9"}
 sphinx-autoapi = "^2.0.1"
 sphinx-rtd-theme = "^1.2.0"
+sphinxcontrib-napoleon = "^0.7"
+pandas = "^2.0.0"
+spyder = "^5.4.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pytc2-0.0.1/src/pytc2/__init__.py` & `pytc2-0.0.2/src/pytc2/__init__.py`

 * *Files identical despite different names*

### Comparing `pytc2-0.0.1/src/pytc2/cuadripolos.py` & `pytc2-0.0.2/src/pytc2/cuadripolos.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,14 @@
     # C = 1/Z21
     Tpar[1,0] = sp.Rational('0') 
     # D = Z22/Z21
     Tpar[1,1] = sp.Rational('1')  
     
     return( Tpar ) 
 
-
 def TabcdY_s(Yexc):
     '''
     Implementa una matriz de transferencia ABCD (Tabcd) a partir de 
     un cuadripolo constituido únicamente por una Y en derivación.
 
     Parameters
     ----------
@@ -338,16 +337,15 @@
     # C = 1/Z21
     Tpar[1,0] = Yexc
     # D = Z22/Z21
     Tpar[1,1] = sp.Rational('1')  
     
     return( Tpar ) 
 
-
-def Y2T_s(YY):
+def Y2Tabcd_s(YY):
     """
     
     Parameters
     ----------
     tfa : TYPE
         DESCRIPTION.
     tfb : TYPE
@@ -371,15 +369,15 @@
     # C = -DY/Y21
     TT[1,0] = sp.simplify(sp.expand(-sp.Determinant(YY)/YY[1,0]))
     # D = Y11/Y21
     TT[1,1] = sp.simplify(sp.expand(-YY[1,1]/YY[1,0]))
     
     return(TT)
 
-def Z2T_s(ZZ):
+def Z2Tabcd_s(ZZ):
     '''
     Convierte la MAD en MAI luego de levantar de referencia.
 
     Parameters
     ----------
     Ymai : Symbolic Matrix
         Matriz admitancia indefinida.
@@ -402,15 +400,15 @@
     # C = 1/Z21
     TT[1,0] = sp.simplify(sp.expand(1/ZZ[1,0]))
     # D = Z22/Z21
     TT[1,1] = sp.simplify(sp.expand(ZZ[1,1]/ZZ[1,0]))
     
     return(TT)
 
-def T2Z_s(TT):
+def Tabcd2Z_s(TT):
     '''
     Convierte la MAD en MAI luego de levantar de referencia.
 
     Parameters
     ----------
     Ymai : Symbolic Matrix
         Matriz admitancia indefinida.
@@ -433,15 +431,15 @@
     # Z21 = 1/C
     ZZ[1,0] = sp.simplify(sp.expand(1/TT[1,0]))
     # Z22 = D/C
     ZZ[1,1] = sp.simplify(sp.expand(TT[1,1]/TT[1,0]))
     
     return(ZZ)
 
-def T2Y_s(TT):
+def Tabcd2Y_s(TT):
     '''
     Convierte la MAD en MAI luego de levantar de referencia.
 
     Parameters
     ----------
     Ymai : Symbolic Matrix
         Matriz admitancia indefinida.
@@ -464,15 +462,15 @@
     # Y21 = -1/B
     YY[1,0] = sp.simplify(sp.expand(-1/TT[0,1]))
     # Y22 = A/B
     YY[1,1] = sp.simplify(sp.expand(TT[0,0]/TT[0,1]))
     
     return(YY)
 
-def Y2T(YY):
+def Y2Tabcd(YY):
     """
     
     Parameters
     ----------
     tfa : TYPE
         DESCRIPTION.
     tfb : TYPE
@@ -496,15 +494,15 @@
     # C = -DY/Y21
     TT[1,0] = -np.linalg.det(YY)/YY[1,0]
     # D = Y11/Y21
     TT[1,1] = -YY[1,1]/YY[1,0]
     
     return(TT)
 
-def Z2T(ZZ):
+def Z2Tabcd(ZZ):
     '''
     Convierte la MAD en MAI luego de levantar de referencia.
 
     Parameters
     ----------
     Ymai : Symbolic Matrix
         Matriz admitancia indefinida.
@@ -527,15 +525,15 @@
     # C = 1/Z21
     TT[1,0] = 1/ZZ[1,0]
     # D = Z22/Z21
     TT[1,1] = ZZ[1,1]/ZZ[1,0]
     
     return(TT)
 
-def T2Z(TT):
+def Tabcd2Z(TT):
     '''
     Convierte la MAD en MAI luego de levantar de referencia.
 
     Parameters
     ----------
     Ymai : Symbolic Matrix
         Matriz admitancia indefinida.
@@ -558,15 +556,15 @@
     # Z21 = 1/C
     ZZ[1,0] = 1/TT[1,0]
     # Z22 = D/C
     ZZ[1,1] = TT[1,1]/TT[1,0]
     
     return(ZZ)
 
-def T2Y(TT):
+def Tabcd2Y(TT):
     '''
     Convierte la MAD en MAI luego de levantar de referencia.
 
     Parameters
     ----------
     Ymai : Symbolic Matrix
         Matriz admitancia indefinida.
@@ -885,15 +883,14 @@
     
         print_latex(r'[Y^{{ {:d}{:d} }}_{{ {:d}{:d} }} ] = '.format(mm,nn,mm,nn) + sp.latex(den) )
     
         print_latex(r'T^{{ {:d}{:d} }}_{{ {:d}{:d} }} = \frac{{ \underline{{Y}}^{{ {:d}{:d} }}_{{ {:d}{:d} }} }}{{ \underline{{Y}}^{{ {:d}{:d} }}_{{ {:d}{:d} }} }} = '.format(ii,jj,mm,nn,mm,nn,ii,jj,mm,nn,mm,nn) + r' -1^{{ {:d} }} '.format(sign_correction)  + r'\frac{{ ' + sp.latex(num_det) + r'}}{{' + sp.latex(den_det) + r'}} = ' + sp.latex(Av) )
     
     return(Av)
 
-
 def calc_MAI_impedance_ij(Ymai, ii=0, jj=1, verbose=False):
     """Calcula la transferencia de tensión V_ij / V_mn
     
     Parameters
     ----------
     tfa : TYPE
         DESCRIPTION.
```

### Comparing `pytc2-0.0.1/src/pytc2/dibujar.py` & `pytc2-0.0.2/src/pytc2/dibujar.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,43 +16,23 @@
 from schemdraw.elements import  Resistor, ResistorIEC, Capacitor, Inductor, Line, Dot, Gap, Arrow
 
 
 ##########################################
 #%% Variables para el análisis simbólico #
 ##########################################
 
-from .general import s
+from .general import s, to_latex, str_to_latex
 
 
-#########################
-#%% Funciones generales #
-#########################
-
-
-
-def to_latex( unsimbolo ):
-    '''
-    Convierte un símbolo en un string formateado para visualizarse en LaTex 
-    '''
-    
-    return('$'+ sp.latex(unsimbolo) + '$')
-
-def str_to_latex( unstr):
-    '''
-    Formatea un string para visualizarse en LaTex 
-    '''
-    
-    return('$'+ unstr + '$')
-
 
 ########################################
 #%% Funciones para dibujar cuadripolos #
 ########################################
 
-def dibujar_Tee(ZZ):
+def dibujar_Tee(ZZ, return_components = False):
     '''
     Dibuja una red Tee a partir de la matriz Z.
 
     Parameters
     ----------
     Ymai : Symbolic Matrix
         Matriz admitancia indefinida.
@@ -69,31 +49,39 @@
     # Dibujo la red Tee
     
     d = Drawing(unit=4)  # unit=2 makes elements have shorter than normal leads
     
     d = dibujar_puerto_entrada(d,
                                    port_name = 'In' )
     
-    Za = ZZ[0,0] - ZZ[0,1] 
-    Zb = ZZ[0,1] 
-    Zc = ZZ[1,1] - ZZ[0,1] 
-    
-    d = dibujar_elemento_serie(d, ResistorIEC, Za )
-    d = dibujar_elemento_derivacion(d, ResistorIEC, Zb )
-    d = dibujar_elemento_serie(d, ResistorIEC, Zc )
+    Za = sp.simplify(sp.expand(ZZ[0,0] - ZZ[0,1]))
+    Zb = sp.simplify(sp.expand(ZZ[0,1]))
+    Zc = sp.simplify(sp.expand(ZZ[1,1] - ZZ[0,1]))
+    
+    if( not Za.is_zero ):
+        d = dibujar_elemento_serie(d, ResistorIEC, Za )
+
+    if( not Zb.is_zero ):
+        d = dibujar_elemento_derivacion(d, ResistorIEC, Zb )
+    
+    if( not Zc.is_zero ):
+        d = dibujar_elemento_serie(d, ResistorIEC, Zc )
+        
     
     d = dibujar_puerto_salida(d, 
                                   port_name = 'Out')
 
     display(d)        
     
-    return([Za,Zb,Zc])
+    if(return_components):
+        return([Za,Zb,Zc])
+    
 
 
-def dibujar_Pi(YY):
+def dibujar_Pi(YY, return_components = False):
     '''
     Dibuja una red Pi a partir de la matriz Y.
 
     Parameters
     ----------
     Ymai : Symbolic Matrix
         Matriz admitancia indefinida.
@@ -110,40 +98,48 @@
     # Dibujo la red Tee
     
     d = Drawing(unit=4)  # unit=2 makes elements have shorter than normal leads
     
     d = dibujar_puerto_entrada(d,
                                    port_name = 'In')
     
-    Ya = YY[0,0] + YY[0,1]
-    Yb = -YY[0,1]
-    Yc = YY[1,1] + YY[0,1]
+    Ya = sp.simplify(sp.expand(YY[0,0] + YY[0,1]))
+    Yb = sp.simplify(sp.expand(-YY[0,1]))
+    Yc = sp.simplify(sp.expand(YY[1,1] + YY[0,1]))
+    
+    bSymbolic = isinstance(YY[0,0], sp.Basic)
     
-    if isinstance(YY[0,0], sp.Symbol):
+    if bSymbolic:
         
         Za = sp.simplify(sp.expand(1/Ya))
         Zb = sp.simplify(sp.expand(1/Yb))
         Zc = sp.simplify(sp.expand(1/Yc))
         
     else:
 
         Za = 1/(YY[0,0] + YY[0,1])
         Zb = 1/(-YY[0,1])
         Zc = 1/(YY[1,1] + YY[0,1])
     
-    d = dibujar_elemento_derivacion(d, ResistorIEC, Za )
-    d = dibujar_elemento_serie(d, ResistorIEC, Zb )
-    d = dibujar_elemento_derivacion(d, ResistorIEC, Zc )
+    if( bSymbolic and (not Ya.is_zero) or (not bSymbolic) and Ya != 0 ):
+        d = dibujar_elemento_derivacion(d, ResistorIEC, Za )
+
+    if( bSymbolic and (not Yb.is_zero) or (not bSymbolic) and Yb != 0 ):
+        d = dibujar_elemento_serie(d, ResistorIEC, Zb )
+
+    if( bSymbolic and (not Yc.is_zero) or (not bSymbolic) and Yc != 0 ):
+        d = dibujar_elemento_derivacion(d, ResistorIEC, Zc )
     
     d = dibujar_puerto_salida(d, 
                                   port_name = 'Out')
     
     display(d)        
-    
-    return([Ya, Yb, Yc])
+
+    if(return_components):
+        return([Ya, Yb, Yc])
 
 
 
 def dibujar_cauer_RC_RL(ki = None, y_exc = None, z_exc = None):
     '''
     Description
     -----------
@@ -546,16 +542,14 @@
 
 
         d += Line().right().length(d.unit*.25)
         d += Line().down()
         d += Line().left().length(d.unit*.25)
         
         display(d)
-        
-        return(d)
 
     else:    
         
         print('Nada para dibujar')
 
 
 
@@ -563,14 +557,29 @@
 
 ##################################################
 #%% Funciones para dibujar redes de forma bonita #
 ##################################################
 
 
 def dibujar_puerto_entrada(d, port_name = None, voltage_lbl = None, current_lbl = None):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
     d += Dot(open=True)
     
     if voltage_lbl is None:
         d += Gap().down().label( '' )
     else:
         d += Gap().down().label( voltage_lbl, fontsize=16)
@@ -594,14 +603,29 @@
         d += Arrow(reverse=True).left().label( current_lbl, fontsize=16).length(d.unit*.25)
     
     d.pop()
 
     return(d)
 
 def dibujar_puerto_salida(d, port_name = None, voltage_lbl = None, current_lbl = None):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
     if current_lbl is None:
         d += Line().right().length(d.unit*.5)
     else:
         d += Line().right().length(d.unit*.25)
         d += Arrow(reverse=True).right().label( current_lbl, fontsize=16).length(d.unit*.25)
     
@@ -626,14 +650,29 @@
 
     d.pop()
 
     return(d)
 
 
 def dibujar_espaciador( d ):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
 
     d += Line().right().length(d.unit*.5)
 
     d.push()
 
     d += Gap().down().label( '' )
 
@@ -641,15 +680,29 @@
 
     d.pop()
 
     return(d)
 
 
 def dibujar_funcion_exc_abajo(d, func_label, sym_func, k_gap_width=0.5, hacia_salida  = False, hacia_entrada  = False ):
-# ok
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
 
     half_width = d.unit*k_gap_width/2
     
     d += Line().right().length(half_width)
     d.push()
     d += Gap().down().label('')
     d.push()
@@ -684,14 +737,29 @@
     d += Line().right().length(half_width)
     d.pop()
     d += Line().right().length(half_width)
 
     return([d, lbl])
 
 def dibujar_funcion_exc_arriba(d, func_label, sym_func, k_gap_width=0.5, hacia_salida = False, hacia_entrada = False ):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
 
     half_width = d.unit*k_gap_width/2
     
     d += Line().right().length(half_width)
     d.push()
     
     if isinstance(sym_func, sp.Basic ):
@@ -728,16 +796,31 @@
     d += Line().right().length(half_width)
 
 
 
     return([d, lbl])
 
 def dibujar_elemento_serie(d, elemento, sym_label=''):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
-    if isinstance(sym_label, sp.Number ):
+    if isinstance(sym_label, sp.Basic ):
         sym_label = to_latex(sym_label)
     elif isinstance(sym_label, np.number):
         sym_label = str_to_latex('{:3.3f}'.format(sym_label))
     elif isinstance(sym_label, str):
         sym_label = str_to_latex(sym_label)
     else:
         sym_label = '$ ?? $'
@@ -748,26 +831,56 @@
     d += Gap().down().label( '' )
     d += Line().left()
     d.pop()
 
     return(d)
 
 def dibujar_espacio_derivacion(d):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
 
     d += Line().right().length(d.unit*.25)
     d.push()
     d += Gap().down().label( '' )
     d += Line().left().length(d.unit*.25)
     d.pop()
 
     return(d)
 
 def dibujar_elemento_derivacion(d, elemento, sym_label=''):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
-    if isinstance(sym_label, sp.Number ):
+    if isinstance(sym_label, sp.Basic ):
         sym_label = to_latex(sym_label)
     elif isinstance(sym_label, np.number):
         sym_label = str_to_latex('{:3.3f}'.format(sym_label))
     elif isinstance(sym_label, str):
         sym_label = str_to_latex(sym_label)
     else:
         sym_label = '$ ?? $'
@@ -778,21 +891,36 @@
     d += Dot()
     d.pop()
 
     return(d)
 
 
 def dibujar_tanque_RC_serie(d, sym_R_label='', capacitor_lbl=''):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
-    if isinstance(sym_R_label, sp.Number ):
+    if isinstance(sym_R_label, sp.Basic ):
         sym_R_label = to_latex(sym_R_label)
     else:
         sym_R_label = str_to_latex(sym_R_label)
     
-    if isinstance(capacitor_lbl, sp.Number ):
+    if isinstance(capacitor_lbl, sp.Basic ):
         capacitor_lbl = to_latex(capacitor_lbl)
     else:
         capacitor_lbl = str_to_latex(capacitor_lbl)
     
     d.push()
     d += Dot()
     d += Capacitor().right().label(capacitor_lbl, fontsize=16)
@@ -805,42 +933,72 @@
     d += Gap().down().label( '' )
     d += Line().left()
     d.pop()
 
     return(d)
 
 def dibujar_tanque_RC_derivacion(d, sym_R_label='', capacitor_lbl=''):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
-    if isinstance(sym_R_label, sp.Number ):
+    if isinstance(sym_R_label, sp.Basic ):
         sym_R_label = to_latex(sym_R_label)
     else:
         sym_R_label = str_to_latex(sym_R_label)
     
-    if isinstance(capacitor_lbl, sp.Number ):
+    if isinstance(capacitor_lbl, sp.Basic ):
         capacitor_lbl = to_latex(capacitor_lbl)
     else:
         capacitor_lbl = str_to_latex(capacitor_lbl)
     
     d.push()
     d += Dot()
     d += Capacitor().down().label(capacitor_lbl, fontsize=16).length(d.unit*.5)
     d += Resistor().down().label(sym_R_label, fontsize=16).length(d.unit*.5)
     d += Dot()
     d.pop()
 
     return(d)
 
 def dibujar_tanque_RL_serie(d, sym_R_label='', sym_ind_label=''):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
-    if isinstance(sym_R_label, sp.Number ):
+    if isinstance(sym_R_label, sp.Basic ):
         sym_R_label = to_latex(sym_R_label)
     else:
         sym_R_label = str_to_latex(sym_R_label)
     
-    if isinstance(sym_ind_label, sp.Number ):
+    if isinstance(sym_ind_label, sp.Basic ):
         sym_ind_label = to_latex(sym_ind_label)
     else:
         sym_ind_label = str_to_latex(sym_ind_label)
     
     d.push()
     d += Dot()
     d += Inductor().right().label(sym_ind_label, fontsize=16)
@@ -853,42 +1011,72 @@
     d += Gap().down().label( '' )
     d += Line().left()
     d.pop()
 
     return(d)
 
 def dibujar_tanque_RL_derivacion(d, sym_R_label='', sym_ind_label=''):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
-    if isinstance(sym_R_label, sp.Number ):
+    if isinstance(sym_R_label, sp.Basic ):
         sym_R_label = to_latex(sym_R_label)
     else:
         sym_R_label = str_to_latex(sym_R_label)
     
-    if isinstance(sym_ind_label, sp.Number ):
+    if isinstance(sym_ind_label, sp.Basic ):
         sym_ind_label = to_latex(sym_ind_label)
     else:
         sym_ind_label = str_to_latex(sym_ind_label)
     
     d.push()
     d += Dot()
     d += Inductor().down().label(sym_ind_label, fontsize=16).length(d.unit*.5)
     d += Resistor().down().label(sym_R_label, fontsize=16).length(d.unit*.5)
     d += Dot()
     d.pop()
 
     return(d)
 
 def dibujar_tanque_serie(d, sym_ind_label='', sym_cap_label=''):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
-    if isinstance(sym_cap_label, sp.Number ):
+    if isinstance(sym_cap_label, sp.Basic ):
         sym_cap_label = to_latex(sym_cap_label)
     else:
         sym_cap_label = str_to_latex(sym_cap_label)
     
-    if isinstance(sym_ind_label, sp.Number ):
+    if isinstance(sym_ind_label, sp.Basic ):
         sym_ind_label = to_latex(sym_ind_label)
     else:
         sym_ind_label = str_to_latex(sym_ind_label)
     
     d.push()
     d += Dot()
     d += Inductor().right().label(sym_ind_label, fontsize=16)
@@ -902,20 +1090,20 @@
     d += Line().left()
     d.pop()
 
     return(d)
 
 # def dibujar_tanque_RL_derivacion(d, sym_R_label='', inductor_lbl=''):
     
-#     if isinstance(sym_R_label, sp.Number ):
+#     if isinstance(sym_R_label, sp.Basic ):
 #         sym_R_label = to_latex(sym_R_label)
 #     else:
 #         sym_R_label = str_to_latex(sym_R_label)
     
-#     if isinstance(inductor_lbl, sp.Number ):
+#     if isinstance(inductor_lbl, sp.Basic ):
 #         inductor_lbl = to_latex(inductor_lbl)
 #     else:
 #         inductor_lbl = str_to_latex(inductor_lbl)
     
 #     d.push()
 #     d += Dot()
 #     d += Inductor().down().label(inductor_lbl, fontsize=16).length(d.unit*.5)
@@ -923,20 +1111,20 @@
 #     d += Dot()
 #     d.pop()
 
 #     return(d)
 
 # def dibujar_tanque_serie(d, inductor_lbl='', capacitor_lbl=''):
     
-#     if isinstance(inductor_lbl, sp.Number ):
+#     if isinstance(inductor_lbl, sp.Basic ):
 #         inductor_lbl = to_latex(inductor_lbl)
 #     else:
 #         inductor_lbl = str_to_latex(inductor_lbl)
     
-#     if isinstance(capacitor_lbl, sp.Number ):
+#     if isinstance(capacitor_lbl, sp.Basic ):
 #         capacitor_lbl = to_latex(capacitor_lbl)
 #     else:
 #         capacitor_lbl = str_to_latex(capacitor_lbl)
     
 #     d.push()
 #     d += Dot()
 #     d += Capacitor().right().label(capacitor_lbl, fontsize=16)
@@ -949,21 +1137,36 @@
 #     d += Gap().down().label( '' )
 #     d += Line().left()
 #     d.pop()
 
 #     return(d)
 
 def dibujar_tanque_derivacion(d, inductor_lbl='', capacitor_lbl=''):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
-    if isinstance(inductor_lbl, sp.Number ):
+    if isinstance(inductor_lbl, sp.Basic ):
         inductor_lbl = to_latex(inductor_lbl)
     else:
         inductor_lbl = str_to_latex(inductor_lbl)
     
-    if isinstance(capacitor_lbl, sp.Number ):
+    if isinstance(capacitor_lbl, sp.Basic ):
         capacitor_lbl = to_latex(capacitor_lbl)
     else:
         capacitor_lbl = str_to_latex(capacitor_lbl)
     
     d.push()
     d += Dot()
     d += Capacitor().down().label(capacitor_lbl, fontsize=16).length(d.unit*.5)
```

### Comparing `pytc2-0.0.1/src/pytc2/ltspice.py` & `pytc2-0.0.2/src/pytc2/ltspice.py`

 * *Files 17% similar despite different names*

```diff
@@ -97,14 +97,29 @@
 
 
 #############################################
 #%% Funciones para dibujar redes en LTspice #
 #############################################
 
 def ltsp_nuevo_circuito(circ_name=None):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
 
     global cap_num, res_num, ind_num, cur_x, cur_y
 
     if circ_name is None:
 
         timestr = time.strftime("%Y%m%d-%H%M%S")
         circ_name = 'NN-' + timestr
@@ -137,14 +152,29 @@
         
     else:
         print("No se encontró el archivo {}".format(src_fname))
     
     return(circ_hdl)
 
 def ltsp_capa_derivacion(circ_hdl, cap_value, cap_label=None):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
     global cap_der_str, cap_num
     
     if cap_label is None:
         
         cap_label = 'C{:d}'.format(cap_num)
         cap_num += 1
@@ -171,14 +201,29 @@
     circ_hdl.writelines(gnd_str)
     
     return()
 
 
 
 def ltsp_ind_serie(circ_hdl, ind_value, ind_label=None):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
     global ind_ser_str, cap_num, cur_x, cur_y
     
     if ind_label is None:
         
         ind_label = 'C{:d}'.format(cap_num)
         cap_num += 1
@@ -211,14 +256,29 @@
     circ_hdl.writelines(wire_str)
     circ_hdl.writelines(this_ind_str)
     
     return()
 
 
 def ltsp_etiquetar_nodo(circ_hdl, node_label=None):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
     global cap_der_str, node_num, cur_x, cur_y
     
     if node_label is None:
         
         node_label = 'v{:d}'.format(node_num)
         node_num += 1
```

### Comparing `pytc2-0.0.1/src/pytc2/remociones.py` & `pytc2-0.0.2/src/pytc2/remociones.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,31 +14,14 @@
 #%% Variables para el análisis simbólico #
 ##########################################
 
 from .general import s
 
 
 
-def simplify_n_monic(tt):
-    
-    num, den = sp.fraction(sp.simplify(sp.expand(tt)))
-    
-    num = sp.poly(num,s)
-    den = sp.poly(den,s)
-    
-    # lcnum = sp.LC(num)
-    # lcden = sp.LC(den)
-    
-    k = num.LC() / den.LC()
-    
-    num = num.monic()
-    den = den.monic()
-
-    return( sp.Mul(k,num/den, evaluate=False) )
-
 
 def tanque_z( doska, omegasq ):
     '''
     Calcula los valores de L y C que componen un tanque resonante LC 
     (tanque Z), a partir del valor del residuo ($ k $) y la omega al cuadrado 
     ($ \omega^2 $) de la expresión de impedancia dada por:
         
@@ -87,14 +70,29 @@
     '''
     
     return( [1/doska, doska/omegasq] )
 
 
 
 def trim_poly_s( this_poly, tol = 10**-6 ):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
 
     all_terms = this_poly.as_poly(s).all_terms()
     
     poly_acc = 0
     
     for this_pow, this_coeff in all_terms:
     
@@ -102,23 +100,53 @@
             
             poly_acc = poly_acc + this_coeff * s**this_pow[0]
 
 
     return(poly_acc)
 
 def trim_func_s( rat_func, tol = 10**-6 ):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
 
     num, den = rat_func.as_numer_denom()
     
     num = trim_poly_s(num, tol)
     den = trim_poly_s(den, tol)
     
     return(num/den)
 
 def modsq2mod_s( aa ):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
 
     num, den = sp.fraction(aa)
 
     k = sp.poly(num,s).LC() / sp.poly(den,s).LC()
     
     # roots_num = num.as_poly(s).all_roots()
     
@@ -180,14 +208,29 @@
 
     den = poly_acc
 
     return(sp.simplify(sp.expand(sp.sqrt(k) * num/den))) 
 
 
 def modsq2mod( aa ):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
     
     rr = np.roots(aa)
     bb = rr[np.real(rr) == 0]
     bb = bb[ :(bb.size//2)]
     bb = np.concatenate( [bb, rr[np.real(rr) < 0]])
     
     return np.flip(np.real(np.polynomial.polynomial.polyfromroots(bb)))
```

### Comparing `pytc2-0.0.1/src/pytc2/sintesis_dipolo.py` & `pytc2-0.0.2/src/pytc2/sintesis_dipolo.py`

 * *Files identical despite different names*

### Comparing `pytc2-0.0.1/src/pytc2/sistemas_lineales.py` & `pytc2-0.0.2/src/pytc2/sistemas_lineales.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,14 +23,47 @@
 #%% Variables para el análisis simbólico #
 ##########################################
 
 from .general import s
 
 
 
+def simplify_n_monic(tt):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
+    
+    num, den = sp.fraction(sp.simplify(sp.expand(tt)))
+    
+    num = sp.poly(num,s)
+    den = sp.poly(den,s)
+    
+    # lcnum = sp.LC(num)
+    # lcden = sp.LC(den)
+    
+    k = num.LC() / den.LC()
+    
+    num = num.monic()
+    den = den.monic()
+
+    return( sp.Mul(k,num/den, evaluate=False) )
+
+
 def parametrize_sos(num, den):
     '''
     Parameters
     ----------
     num : TYPE
         DESCRIPTION.
     den : TYPE
@@ -326,15 +359,14 @@
         # complete 2nd order, omega and Q parametrization
         num_str_aux = _build_omegayq_str(num)
     elif np.all(num[[0,2]] == 0) and num[1] > 0 :
         # bandpass style  s . k = s . H . omega/Q 
         num_str_aux = _build_omegayq_str(num, den = den)
     elif num[1] == 0 and np.all(num[[0,2]] > 0):
         # complex conj zeros style  s² + omega² 
-        num_str_aux = _build_omegayq_str(num)
         
         kk = num[0]
         if kk == 1.0:        
             omega = np.sqrt(num[2])
             num_str_aux = r's^2 + {:3.4g}^2'.format(omega)
         else:
             omega = np.sqrt(num[2]/kk)
@@ -409,30 +441,88 @@
 
     if displaystr:
         display(Math( r' ' + sos_str))
     else:
         return sos_str
 
 def analyze_sys( all_sys, sys_name = None, img_ext = 'none', same_figs=True, annotations = True, digital = False, fs = 2*np.pi):
-    """
+    """ Analyzes the behavior of a linear system in terms of:
+        
+          * Magnitude and phase response or Bode plot
+          * Pole-zero map
+          * Group delay
+          
+        The funcion admits the system to analyze (*all_sys*) as:
+            
+            * one or a list of TransferFunction objects
+            * a matrix defining several second order sections (SOSs).
+            
+        If *all_sys* is a SOS matrix, the function displays each of the SOS, 
+        and the system resulting frome the cascade of all SOS.
     
     Parameters
     ----------
-    tfa : TYPE
-        DESCRIPTION.
-    tfb : TYPE
-        DESCRIPTION.
-
+    all_sys : list or (Nx5) matrix
+        The linear system to analyze. Wether a list of [scipy.signal.TransferFuncion](https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.TransferFunction.html)
+        objects or a matrix defining a cascade of SOS.
+    sys_name : string or list.
+        The labels or system description. Default: None
+    img_ext : string  ['none', 'png', 'svg'].
+        When different from 'none' the function save plot results to a file with 
+        the indicated extension. Default: 'none'
+    same_figs : boolean
+        Use always the same figure numbers to plot results. When False, each call
+        produce a new group of figures in a separate plot container. Default: True
+    annotations : boolean
+        Add annotations to the PZmap plot. When True, each singularity will be 
+        acompanied of the value of omega (i.e. the radial distance to the origin)
+        and Q (i.e. measure of proximity to the jw axis). Default: True
+    digital : boolean
+        True to analyze the system as *digital*. Default: False
+    fs : real value.
+        The sampling frequency of the digital system. Valid only if digital is 
+        True. Default:  2*np.pi
+    
     Returns
     -------
     None.
 
     Example
     -------
 
+    Analyze a system with w0 = 1 rad/s and Q = sqrt(2)/2
+
+    >>> import numpy as np
+    >>> from scipy import signal as sig
+    >>> from pytc2.sistemas_lineales import analyze_sys, pretty_print_bicuad_omegayq
+    >>> Q = np.sqrt(2)/2
+    >>> w0 = 1
+    >>> # Cargamos la funcion transferencia como vectores de sus coeficientes.
+    >>> num = np.array([ w0**2 ])
+    >>> den = np.array([ 1., w0 / Q, w0**2 ])
+    >>> H1 = sig.TransferFunction( num, den )
+    >>> pretty_print_bicuad_omegayq(num,den)
+    >>> analyze_sys(H1, sys_name='mi ejemplo')
+
+    Compare the former system with two others with different Q values
+
+    >>> Q = 5
+    >>> w0 = 1
+    >>> num = np.array([ w0**2 ])
+    >>> den = np.array([ 1., w0 / Q, w0**2 ])
+    >>> H2 = sig.TransferFunction( num, den )
+    >>> analyze_sys([H1, H2], sys_name=['H1', 'H2'])
+
+    See Also
+    --------
+
+    :func:`pretty_print_bicuad_omegayq`
+    :func:`bodePlot`
+    :func:`pzmap`
+
     """
 
     valid_ext = ['none', 'png', 'svg']
     if img_ext not in valid_ext:
         raise ValueError('Image extension must be one of %s, not %s'
                          % (valid_ext, img_ext))
     
@@ -521,15 +611,15 @@
         fig_id = 'none'
     
     for ii in range(cant_sys):
         fig_id, axes_hdl = GroupDelay(all_sys[ii], fig_id, filter_description = sys_name[ii], digital = digital, fs = fs)
     
     # axes_hdl.legend(sys_name)
 
-    axes_hdl.set_ylim(bottom=0)
+    # axes_hdl.set_ylim(bottom=0)
 
     if img_ext != 'none':
         plt.savefig('_'.join(sys_name) + '_GroupDelay.'  + img_ext, format=img_ext)
 
 def pzmap(myFilter, annotations = False, filter_description = None, fig_id='none', axes_hdl='none', digital = False, fs = 2*np.pi):
     """
     
@@ -813,50 +903,87 @@
         phase = np.empty((npoints, cant_sos+1))
         sos_label = []
         
         for ii in range(cant_sos):
             
             num, den = _one_sos2tf(myFilter[ii,:])
             thisFilter = TransferFunction(num, den)
+
+            this_zzpp = np.abs(np.concatenate([thisFilter.zeros, thisFilter.poles]))
+            this_zzpp = this_zzpp[this_zzpp > 0]
             
             if digital:
-                w, _, phase[:,ii] = thisFilter.bode(np.linspace(10**-2, w_nyq, npoints))
+                w, _, phase[:,ii] = thisFilter.bode(np.linspace(np.floor(np.log10(np.min(this_zzpp)))-1, w_nyq, npoints))
             else:
-                w, _, phase[:,ii] = thisFilter.bode(np.logspace(-2,2,npoints))
+                w, _, phase[:,ii] = thisFilter.bode(np.logspace(np.floor(np.log10(np.min(this_zzpp)))-1, np.ceil(np.log10(np.max(this_zzpp))) + 1 ,npoints))
             
             sos_label += [filter_description + ' - SOS {:d}'.format(ii)]
         
         # whole filter
         thisFilter = sos2tf_analog(myFilter)
+
+        this_zzpp = np.abs(np.concatenate([thisFilter.zeros, thisFilter.poles]))
+        this_zzpp = this_zzpp[this_zzpp > 0]
         
         if digital:
-            w, _, phase[:,cant_sos] = thisFilter.bode(np.linspace(10**-2, w_nyq, npoints))
+            w, _, phase[:,cant_sos] = thisFilter.bode(np.linspace(np.floor(np.log10(np.min(this_zzpp)))-1, w_nyq, npoints))
         else:
-            w, _, phase[:,cant_sos] = thisFilter.bode(np.logspace(-2,2,npoints))
+            w, _, phase[:,cant_sos] = thisFilter.bode(np.logspace(np.floor(np.log10(np.min(this_zzpp)))-1, np.ceil(np.log10(np.max(this_zzpp))) + 1 ,npoints))
+        
+        # if digital:
+        #     w, _, phase[:,cant_sos] = thisFilter.bode(np.linspace(10**-2, w_nyq, npoints))
+        # else:
+        #     w, _, phase[:,cant_sos] = thisFilter.bode(np.logspace(-2,2,npoints))
         
         sos_label += [filter_description]
         
         filter_description = sos_label
+
+        phaseRad = phase * np.pi / 180.0
+    
+        phaseRad = phaseRad.reshape((npoints, 1+cant_sos))
+        
+        # filter gaps and jumps
+        all_jump_x, all_jump_y = (np.abs(np.diff(phaseRad, axis = 0)) > 4/5*np.pi).nonzero()
+
+        for this_jump_x, this_jump_y in zip(all_jump_x, all_jump_y ):
+            phaseRad[this_jump_x+1:, this_jump_y] = phaseRad[this_jump_x+1:, this_jump_y]  - np.pi
         
     else:
         # LTI object
         cant_sos = 0
         
-        if myFilter.dt is None:
-            w, _, phase = myFilter.bode(np.logspace(-2,2,npoints))
+        this_zzpp = np.abs(np.concatenate([myFilter.zeros, myFilter.poles]))
+        this_zzpp = this_zzpp[this_zzpp > 0]
+        
+        if digital:
+            w, _, phase = myFilter.bode(np.linspace(np.floor(np.log10(np.min(this_zzpp)))-1, w_nyq, npoints))
         else:
-            digital = True
-            w, _, phase = myFilter.bode(np.linspace(10**-2, w_nyq, npoints))
+            w, _, phase = myFilter.bode(np.logspace(np.floor(np.log10(np.min(this_zzpp)))-1, np.ceil(np.log10(np.max(this_zzpp))) + 1 ,npoints))
+
+        phaseRad = phase * np.pi / 180.0
+
+        phaseRad = phaseRad.reshape((npoints, 1))
+
+        # filter gaps and jumps
+        all_jump = np.where(np.abs(np.diff(phaseRad, axis = 0)) > 4/5*np.pi)[0]
+
+        for this_jump_x in all_jump:
+            phaseRad[this_jump_x+1:] = phaseRad[this_jump_x+1] - np.pi
+        
+        # if myFilter.dt is None:
+        #     w, _, phase = myFilter.bode(np.logspace(-2,2,npoints))
+        # else:
+        #     digital = True
+        #     w, _, phase = myFilter.bode(np.linspace(10**-2, w_nyq, npoints))
         
         # if isinstance(filter_description, str):
         #     filter_description = [filter_description]
-
-
-    phaseRad = phase * np.pi / 180.0
-    groupDelay = -np.diff(phaseRad.reshape((npoints, 1+cant_sos)), axis = 0)/np.diff(w).reshape((npoints-1,1))
+    
+    groupDelay = -np.diff(phaseRad, axis = 0) / np.diff(w).reshape((npoints-1,1))
 
     if fig_id == 'none':
         fig_hdl = plt.figure()
         fig_id = fig_hdl.number
     else:
         if plt.fignum_exists(fig_id):
             fig_hdl = plt.figure(fig_id)
@@ -924,42 +1051,67 @@
         phase = np.empty_like(mag)
         sos_label = []
         
         for ii in range(cant_sos):
             
             num, den = _one_sos2tf(myFilter[ii,:])
             thisFilter = TransferFunction(num, den)
+            
+            this_zzpp = np.abs(np.concatenate([thisFilter.zeros, thisFilter.poles]))
+            this_zzpp = this_zzpp[this_zzpp > 0]
+            
             if digital:
-                w, mag[:, ii], phase[:,ii] = thisFilter.bode(np.linspace(10**-2, w_nyq,npoints))
+                w, mag[:, ii], phase[:,ii] = thisFilter.bode(np.linspace(np.floor(np.log10(np.min(this_zzpp)))-1, w_nyq, npoints))
             else:
-                w, mag[:, ii], phase[:,ii] = thisFilter.bode(np.logspace(-2,2,npoints))
+                w, mag[:, ii], phase[:,ii] = thisFilter.bode(np.logspace(np.floor(np.log10(np.min(this_zzpp)))-1, np.ceil(np.log10(np.max(this_zzpp))) + 1 ,npoints))
+            
+            # if digital:
+            #     w, mag[:, ii], phase[:,ii] = thisFilter.bode(np.linspace(10**-2, w_nyq,npoints))
+            # else:
+            #     w, mag[:, ii], phase[:,ii] = thisFilter.bode(np.logspace(-2,2,npoints))
                 
             sos_label += [filter_description + ' - SOS {:d}'.format(ii)]
         
         # whole filter
         thisFilter = sos2tf_analog(myFilter)
 
+        this_zzpp = np.abs(np.concatenate([thisFilter.zeros, thisFilter.poles]))
+        this_zzpp = this_zzpp[this_zzpp > 0]
+        
         if digital:
-            w, mag[:, cant_sos], phase[:,cant_sos] = thisFilter.bode(np.linspace(10**-2, w_nyq, npoints))
+            w, mag[:, cant_sos], phase[:,cant_sos] = thisFilter.bode(np.linspace(np.floor(np.log10(np.min(this_zzpp)))-1, w_nyq, npoints))
         else:
-            w, mag[:, cant_sos], phase[:,cant_sos] = thisFilter.bode(np.logspace(-2,2,npoints))
+            w, mag[:, cant_sos], phase[:,cant_sos] = thisFilter.bode(np.logspace(np.floor(np.log10(np.min(this_zzpp)))-1, np.ceil(np.log10(np.max(this_zzpp))) + 1 ,npoints))
+
+        # if digital:
+        #     w, mag[:, cant_sos], phase[:,cant_sos] = thisFilter.bode(np.linspace(10**-2, w_nyq, npoints))
+        # else:
+        #     w, mag[:, cant_sos], phase[:,cant_sos] = thisFilter.bode(np.logspace(-2,2,npoints))
             
         sos_label += [filter_description]
         
         filter_description = sos_label
         
     else:
         # LTI object
         cant_sos = 0
         
-        if myFilter.dt is None:
-            # filtro analógico normalizado
-            w, mag, phase = myFilter.bode(np.logspace(-2,2,npoints))
+        this_zzpp = np.abs(np.concatenate([myFilter.zeros, myFilter.poles]))
+        this_zzpp = this_zzpp[this_zzpp > 0]
+        
+        if digital:
+            w, mag, phase = myFilter.bode(np.linspace(np.floor(np.log10(np.min(this_zzpp)))-1, w_nyq, npoints))
         else:
-            w, mag, phase = myFilter.bode(np.linspace(10**-2, w_nyq, npoints))
+            w, mag, phase = myFilter.bode(np.logspace(np.floor(np.log10(np.min(this_zzpp)))-1, np.ceil(np.log10(np.max(this_zzpp))) + 1 ,npoints))
+        
+        # if myFilter.dt is None:
+        #     # filtro analógico normalizado
+        #     w, mag, phase = myFilter.bode(np.logspace(-2,2,npoints))
+        # else:
+        #     w, mag, phase = myFilter.bode(np.linspace(10**-2, w_nyq, npoints))
         
         # if isinstance(filter_description, str):
         #     filter_description = [filter_description]
         
 
     if fig_id == 'none':
         fig_hdl, axes_hdl = plt.subplots(2, 1, sharex='col')
@@ -1218,15 +1370,15 @@
 
     z, p, k = tf2zpk(num, den)
     
     sos = zpk2sos_analog(z, p, k, pairing = pairing)
 
     return sos
         
-def zpk2sos_analog(z, p, k, pairing='nearest'):
+def zpk2sos_analog(zz, pp, kk, pairing='nearest'):
     """
     From scipy.signal, modified by marianux
     ----------------------------------------
     
     Return second-order sections from zeros, poles, and gain of a system
     
     Parameters
@@ -1260,26 +1412,26 @@
         2- order sections by increasing Q
         3- gains ordering to maximize dynamic range. See ch. 5.
 
   
     """
     
     # if empty filter then
-    if len(z) == len(p) == 0:
-        return np.array([[0., 0., k, 1., 0., 0.]])
+    if len(zz) == len(pp) == 0:
+        return np.array([[0., 0., kk, 1., 0., 0.]])
 
-    assert len(z) <= len(p), "Filter must have more poles than zeros"
+    assert len(zz) <= len(pp), "Filter must have more poles than zeros"
     
-    n_sections = ( len(p) + 1) // 2
+    n_sections = ( len(pp) + 1) // 2
     sos = np.zeros((n_sections, 6))
 
     # Ensure we have complex conjugate pairs
     # (note that _cplxreal only gives us one element of each complex pair):
-    z = np.concatenate(_cplxreal(z))
-    p = np.concatenate(_cplxreal(p))
+    z = np.concatenate(_cplxreal(zz))
+    p = np.concatenate(_cplxreal(pp))
 
     # calculate los omega_0 and Q for each pole
     # w0 = np.abs(p)
     qq = 1 / (2*np.cos(np.pi - np.angle(p)))
 
     p_sos = np.zeros((n_sections, 2), np.complex128)
     z_sos = np.zeros_like(p_sos)
@@ -1310,143 +1462,193 @@
                 z1_idx = _nearest_real_complex_idx(z, p1, 'real')
                 z1 = z[z1_idx]
                 z = np.delete(z, z1_idx)
                 
             p2 = z2 = np.nan
             
         else:
+            # SOS 
             
             if z.size == 0:
                 # no zero, just poles
                 z1 = np.nan
                 
             else:
                 # Pair the pole with the closest zero (real or complex)
                 z1_idx = np.argmin(np.abs(p1 - z))
                 z1 = z[z1_idx]
                 z = np.delete(z, z1_idx)
 
             # Now that we have p1 and z1, figure out what p2 and z2 need to be
             
-            if z.size == 0:
+            if np.isnan(z1):
                 # no zero, just poles
+                z2 = np.nan
+                
                 if np.isreal(p1):
                     # pick the next "worst" pole to use
                     idx = np.nonzero(np.isreal(p))[0]
                     assert len(idx) > 0
                     p2_idx = idx[np.argmax(qq)]
                     p2 = p[p2_idx]
-                    z2 = np.nan
                     p = np.delete(p, p2_idx)
 
                 else:
                     # complex pole
                     p2 = p1.conj()
-                    if np.isnan(z1):
-                        z2 = z1
-                    else:
-                        # complex zero (no more zeros)
-                        z2 = z1.conj()
+
                 
             else:
                 # there are zero/s for z2
                     
-                if not np.isreal(p1):
-                    p2 = p1.conj()
+                if np.isreal(p1):
                     
-                    if not np.isreal(z1):  # complex pole, complex zero
-                        z2 = z1.conj()
-                    else:  # complex pole, real zero
+                    if np.isreal(z1):  
+                        
+                        # real pole, real zero
+                        # pick the next "worst" pole to use
+                        idx = np.nonzero(np.isreal(p))[0]
+                        assert len(idx) > 0
+                        p2_idx = idx[np.argmin(np.abs(np.abs(p[idx]) - 1))]
+                        p2 = p[p2_idx]
+                        # find a real zero to match the added pole
+                        assert np.isreal(p2)
                         
                         if one_z_per_section:
                             # avoid picking double zero (high-pass)
                             # prefer picking band-pass sections (Schaumann 5.3.1)
                             z2 = np.nan
                         else:
-                            z2_idx = _nearest_real_complex_idx(z, p1, 'real')
+                            z2_idx = _nearest_real_complex_idx(z, p2, 'real')
                             z2 = z[z2_idx]
                             assert np.isreal(z2)
                             z = np.delete(z, z2_idx)
-                else:
-                    if not np.isreal(z1):  # real pole, complex zero
+                        
+                    else:  
+
+                        # real pole, complex zero
                         z2 = z1.conj()
                         p2_idx = _nearest_real_complex_idx(p, z1, 'real')
                         p2 = p[p2_idx]
                         assert np.isreal(p2)
-                    else:  # real pole, real zero
-                        # pick the next "worst" pole to use
-                        idx = np.nonzero(np.isreal(p))[0]
-                        assert len(idx) > 0
-                        p2_idx = idx[np.argmin(np.abs(np.abs(p[idx]) - 1))]
-                        p2 = p[p2_idx]
-                        # find a real zero to match the added pole
-                        assert np.isreal(p2)
+
+                    p = np.delete(p, p2_idx)
+                    
+                else:
+                    # complex pole
+
+                    p2 = p1.conj()
+                    
+                    if np.isreal(z1):  # complex pole, complex zero
+
+                        # complex pole, real zero -> possible bandpass
                         
-                        if one_z_per_section:
+                        if z1 == 0:
                             # avoid picking double zero (high-pass)
                             # prefer picking band-pass sections (Schaumann 5.3.1)
                             z2 = np.nan
                         else:
-                            z2_idx = _nearest_real_complex_idx(z, p2, 'real')
+                            # z1 over the \sigma axis
+                            z2_idx = _nearest_real_complex_idx(z, p1, 'real')
                             z2 = z[z2_idx]
                             assert np.isreal(z2)
                             z = np.delete(z, z2_idx)
-                    p = np.delete(p, p2_idx)
+
+                    else:  
+                        # complex pole, complex zero -> SOS
+                        
+                        z2 = z1.conj()
                     
         p_sos[si] = [p1, p2]
         z_sos[si] = [z1, z2]
         
     assert len(p) == 0  # we've consumed all poles and zeros
     del p, z
 
     # Construct the system, reversing order so the "worst" are last
     p_sos = np.reshape(p_sos[::-1], (n_sections, 2))
     z_sos = np.reshape(z_sos[::-1], (n_sections, 2))
     
-    maxima_tf = np.ones(n_sections)
-    gains = np.ones(n_sections, np.array(k).dtype)
-    # gains[0] = k # todo: distribute k along sections
+    # asignación de ganancias para cada SOS
+    mmi = np.ones(n_sections)
+    gains = np.ones(n_sections, np.array(kk).dtype)
+    
+    tf_j = TransferFunction(1.0, 1.0)
     
     for si in range(n_sections):
         
-        num, den = zpk2tf(z_sos[si, np.logical_not( np.isnan(z_sos[si])) ], p_sos[si, np.logical_not(np.isnan(p_sos[si]))], 1) # no gain
+        this_zz = z_sos[si, np.logical_not( np.isnan(z_sos[si])) ]
+        this_pp = p_sos[si, np.logical_not(np.isnan(p_sos[si]))]
+        
+        num, den = zpk2tf(this_zz, this_pp, 1) # no gain
         
-        # find maximum in transfer function
-        thisFilter = TransferFunction(num, den)
+        tf_j = tfcascade(tf_j, TransferFunction(num, den))
+
+        this_zzpp = np.abs(np.concatenate([this_zz, this_pp]))
+        this_zzpp = this_zzpp[this_zzpp > 0]
         
-        _, mag, _ = thisFilter.bode(np.logspace(-2,2,100))
+        _, mag, _ = tf_j.bode(np.logspace(np.floor(np.log10(np.min(this_zzpp)))-2, np.ceil(np.log10(np.max(this_zzpp)))+2, 100))
         
         # bode in dB
-        maxima_tf[si] = 10**(np.max(mag)/20)
+        mmi[si] = 10**(np.max(mag)/20) # M_i according to Schaumann eq 5.76
     
-    mmi = np.cumprod(maxima_tf) # M_i according to Schaumann eq 5.76
 
     # first gain to optimize dynamic range.
-    gains[0] = k * (mmi[-1]/mmi[0])
+    gains[0] = kk * (mmi[-1]/mmi[0])
 
     for si in range(n_sections):
 
         if si > 0:
             gains[si] = (mmi[si-1]/mmi[si])
 
         num, den = zpk2tf(z_sos[si, np.logical_not(np.isnan(z_sos[si])) ], p_sos[si, np.logical_not(np.isnan(p_sos[si]))], gains[si]) # now with gain
         
         num = np.concatenate((np.zeros(np.max(3 - len(num), 0)), num))
         den = np.concatenate((np.zeros(np.max(3 - len(den), 0)), den))
             
         sos[si] = np.concatenate((num,den))
         
+        
+    # verify the factorization
+    tf_verif = sos2tf_analog(sos)
+    z_v, p_v, k_v = tf2zpk(tf_verif.num, tf_verif.den)
+    
+    num_t, den_t = zpk2tf(zz, pp, kk)
+    
+    if np.std(num_t - tf_verif.num) > 1e-10:
+
+        raise ValueError('Incorrect factorization: Zeros does not match')
+
+    if np.std(den_t - tf_verif.den) > 1e-10:
+
+        raise ValueError('Incorrect factorization: Poles does not match')
+        
+        
     return sos
     
 ########################
 #%% Funciones internas #
 ########################
 
 def _nearest_real_complex_idx(fro, to, which):
-    """Get the next closest real or complex element based on distance"""
+    '''
+    Get the next closest real or complex element based on distance
+    
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
+    
     assert which in ('real', 'complex')
     order = np.argsort(np.abs(fro - to))
     mask = np.isreal(fro[order])
     if which == 'complex':
         mask = ~mask
     return order[np.nonzero(mask)[0][0]]
 
@@ -1656,17 +1858,21 @@
         hh = this_quad_poly[1] * qq / omega
         
         poly_str = r's\,{:3.4g}\,\frac{{{:3.4g}}}{{{:3.4g}}}'.format(hh, omega, qq )
     
     else:
         # all other complete quadratic polynomial
         omega = np.sqrt(this_quad_poly[2])
-        qq = omega / this_quad_poly[1]
         
-        poly_str = r's^2 + s \frac{{{:3.4g}}}{{{:3.4g}}} + {:3.4g}^2'.format(omega, qq, omega)
+        if this_quad_poly[1] == 0:
+            poly_str = r's^2 + {:3.4g}^2'.format(omega)
+        else:
+            qq = omega / this_quad_poly[1]
+            poly_str = r's^2 + s \frac{{{:3.4g}}}{{{:3.4g}}} + {:3.4g}^2'.format(omega, qq, omega)
+        
                 
     return poly_str
 
 def _complementaryColor(my_hex):
     """Returns complementary RGB color
 
     Example:
```

### Comparing `pytc2-0.0.1/PKG-INFO` & `pytc2-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 Metadata-Version: 2.1
 Name: pytc2
-Version: 0.0.1
+Version: 0.0.2
 Summary: A circuit theory module for students at Universidad Tecnológica Nacional Regional Buen
 License: MIT
 Author: Mariano Llamedo Soria
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
-Requires-Dist: pyfda (>=0.7.1,<0.8.0)
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: schemdraw (>=0.15,<0.16)
-Requires-Dist: spyder (>=5.4.2,<6.0.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: sympy (>=1.11.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # pytc2
 
-A circuit theory module for students at Universidad Tecnológica Nacional Regional Buen
+A circuit theory module for students at Universidad Tecnológica Nacional, en Buenos Aires, Argentina.
+
+* Free software: MIT license
+* [online Documentation](https://pytc2.readthedocs.io)
 
 ## Installation
 
 ```bash
 $ pip install pytc2
 ```
 
 ## Usage
 
-- TODO
+- Check the jupyter notebook examples in the documentation for fast starting.
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
 ## License
 
 `pytc2` was created by Mariano Llamedo Soria. It is licensed under the terms of the MIT license.
 
 ## Credits
 
 `pytc2` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
 
+
```

