# Comparing `tmp/panda3d-gltf-0.8.tar.gz` & `tmp/panda3d-gltf-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/panda3d-gltf-0.8.tar", last modified: Sat Sep  5 17:42:16 2020, max compression
+gzip compressed data, was "dist/panda3d-gltf-0.9.tar", last modified: Sat Sep 19 18:24:46 2020, max compression
```

## Comparing `panda3d-gltf-0.8.tar` & `panda3d-gltf-0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-05 17:42:16.000000 panda3d-gltf-0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1515 2020-09-05 17:41:45.000000 panda3d-gltf-0.8/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2020-09-05 17:41:45.000000 panda3d-gltf-0.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4307 2020-09-05 17:42:16.000000 panda3d-gltf-0.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3013 2020-09-05 17:41:45.000000 panda3d-gltf-0.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-05 17:42:16.000000 panda3d-gltf-0.8/gltf/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1408 2020-09-05 17:41:45.000000 panda3d-gltf-0.8/gltf/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1761 2020-09-05 17:41:45.000000 panda3d-gltf-0.8/gltf/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70790 2020-09-05 17:41:45.000000 panda3d-gltf-0.8/gltf/converter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      535 2020-09-05 17:41:45.000000 panda3d-gltf-0.8/gltf/loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2020-09-05 17:41:45.000000 panda3d-gltf-0.8/gltf/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3463 2020-09-05 17:41:45.000000 panda3d-gltf-0.8/gltf/viewer.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-05 17:42:16.000000 panda3d-gltf-0.8/panda3d_gltf.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4307 2020-09-05 17:42:16.000000 panda3d-gltf-0.8/panda3d_gltf.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      363 2020-09-05 17:42:16.000000 panda3d-gltf-0.8/panda3d_gltf.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-05 17:42:16.000000 panda3d-gltf-0.8/panda3d_gltf.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      168 2020-09-05 17:42:16.000000 panda3d-gltf-0.8/panda3d_gltf.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       31 2020-09-05 17:42:16.000000 panda3d-gltf-0.8/panda3d_gltf.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2020-09-05 17:42:16.000000 panda3d-gltf-0.8/panda3d_gltf.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      729 2020-09-05 17:42:16.000000 panda3d-gltf-0.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      764 2020-09-05 17:41:45.000000 panda3d-gltf-0.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-19 18:24:46.000000 panda3d-gltf-0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1515 2020-09-19 18:24:18.000000 panda3d-gltf-0.9/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2020-09-19 18:24:18.000000 panda3d-gltf-0.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4307 2020-09-19 18:24:46.000000 panda3d-gltf-0.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3013 2020-09-19 18:24:18.000000 panda3d-gltf-0.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-19 18:24:46.000000 panda3d-gltf-0.9/gltf/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1408 2020-09-19 18:24:18.000000 panda3d-gltf-0.9/gltf/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1966 2020-09-19 18:24:18.000000 panda3d-gltf-0.9/gltf/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    72158 2020-09-19 18:24:18.000000 panda3d-gltf-0.9/gltf/converter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      535 2020-09-19 18:24:18.000000 panda3d-gltf-0.9/gltf/loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       20 2020-09-19 18:24:18.000000 panda3d-gltf-0.9/gltf/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3463 2020-09-19 18:24:18.000000 panda3d-gltf-0.9/gltf/viewer.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-19 18:24:46.000000 panda3d-gltf-0.9/panda3d_gltf.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4307 2020-09-19 18:24:46.000000 panda3d-gltf-0.9/panda3d_gltf.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      363 2020-09-19 18:24:46.000000 panda3d-gltf-0.9/panda3d_gltf.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-19 18:24:46.000000 panda3d-gltf-0.9/panda3d_gltf.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      168 2020-09-19 18:24:46.000000 panda3d-gltf-0.9/panda3d_gltf.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       31 2020-09-19 18:24:46.000000 panda3d-gltf-0.9/panda3d_gltf.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2020-09-19 18:24:46.000000 panda3d-gltf-0.9/panda3d_gltf.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      729 2020-09-19 18:24:46.000000 panda3d-gltf-0.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      764 2020-09-19 18:24:18.000000 panda3d-gltf-0.9/setup.py
```

### Comparing `panda3d-gltf-0.8/LICENSE.txt` & `panda3d-gltf-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda3d-gltf-0.8/PKG-INFO` & `panda3d-gltf-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda3d-gltf
-Version: 0.8
+Version: 0.9
 Summary: glTF utilities for Panda3D
 Home-page: https://github.com/Moguri/panda3d-gltf
 Author: Mitchell Stokes
 License: MIT
 Description: [![Build Status](https://travis-ci.org/Moguri/panda3d-gltf.svg?branch=master)](https://travis-ci.org/Moguri/panda3d-gltf)
         [![](https://img.shields.io/pypi/pyversions/panda3d_gltf.svg)](https://pypi.org/project/panda3d-gltf/)
         [![Panda3D Versions](https://img.shields.io/badge/panda3d-1.10%2C%201.11-blue.svg)](https://www.panda3d.org/)
```

### Comparing `panda3d-gltf-0.8/README.md` & `panda3d-gltf-0.9/README.md`

 * *Files identical despite different names*

### Comparing `panda3d-gltf-0.8/gltf/__init__.py` & `panda3d-gltf-0.9/gltf/__init__.py`

 * *Files identical despite different names*

### Comparing `panda3d-gltf-0.8/gltf/cli.py` & `panda3d-gltf-0.9/gltf/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -52,22 +52,29 @@
             'ref',
             'copy',
         ],
         default='ref',
         help='control what to do with external textures (embedded textures will remain embedded)'
     )
 
+    parser.add_argument(
+        '--legacy-materials',
+        action='store_true',
+        help='convert imported PBR materials to legacy materials'
+    )
+
     args = parser.parse_args()
 
     settings = gltf.GltfSettings(
         physics_engine=args.physics_engine,
         print_scene=args.print_scene,
         skip_axis_conversion=args.skip_axis_conversion,
         no_srgb=args.no_srgb,
         textures=args.textures,
+        legacy_materials=args.legacy_materials,
     )
 
     gltf.converter.convert(args.src, args.dst, settings)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `panda3d-gltf-0.8/gltf/converter.py` & `panda3d-gltf-0.9/gltf/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,21 +31,23 @@
 
 GltfSettings = collections.namedtuple('GltfSettings', (
     'physics_engine',
     'print_scene',
     'skip_axis_conversion',
     'no_srgb',
     'textures',
+    'legacy_materials',
 ))
 GltfSettings.__new__.__defaults__ = (
     'builtin', # physics engine
     False, # print_scene
     False, # skip_axis_conversion
     False, # do not load textures as sRGB
     'ref', # reference external textures
+    False, # use PBR materials
 )
 
 
 class Converter():
     _COMPONENT_TYPE_MAP = {
         5120: GeomEnums.NT_int8,
         5121: GeomEnums.NT_uint8,
@@ -575,63 +577,76 @@
 
         pmat = Material(matname)
         pbr_fallback = {'index': '__pbr-fallback', 'texCoord': 0}
         emission_fallback = {'index': '__emission-fallback', 'texCoord': 0}
         normal_fallback = {'index': '__normal-fallback', 'texCoord': 0}
         texinfos = []
 
-        if 'extensions' in gltf_mat and 'BP_materials_legacy' in gltf_mat['extensions']:
-            matsettings = gltf_mat['extensions']['BP_materials_legacy']['bpLegacy']
-            pmat.set_shininess(matsettings['shininessFactor'])
-            pmat.set_ambient(LColor(*matsettings['ambientFactor']))
-
-            if 'diffuseTexture' in matsettings:
-                texinfo = matsettings['diffuseTexture']
-                texinfos.append(texinfo)
-                if matsettings['diffuseTextureSrgb'] and texinfo['index'] in self.textures:
-                    self.make_texture_srgb(self.textures[texinfo['index']])
-            else:
-                pmat.set_diffuse(LColor(*matsettings['diffuseFactor']))
+        if self.settings.legacy_materials:
+            if 'pbrMetallicRoughness' in gltf_mat:
+                pbrsettings = gltf_mat['pbrMetallicRoughness']
+
+                pmat.set_diffuse(LColor(*pbrsettings.get('baseColorFactor', [1.0, 1.0, 1.0, 1.0])))
+                texinfos.append(pbrsettings.get('baseColorTexture', pbr_fallback))
+                if texinfos[-1]['index'] in self.textures:
+                    self.make_texture_srgb(self.textures[texinfos[-1]['index']])
 
-            if 'emissionTexture' in matsettings:
-                texinfo = matsettings['emissionTexture']
-                texinfos.append(texinfo)
-                if matsettings['emissionTextureSrgb'] and texinfo['index'] in self.textures:
-                    self.make_texture_srgb(self.textures[texinfo['index']])
-            else:
-                pmat.set_emission(LColor(*matsettings['emissionFactor']))
+            texinfos.append(gltf_mat.get('normalTexture', normal_fallback))
+            texinfos[-1]['mode'] = TextureStage.M_normal
+        else:
+            if 'extensions' in gltf_mat and 'BP_materials_legacy' in gltf_mat['extensions']:
+                matsettings = gltf_mat['extensions']['BP_materials_legacy']['bpLegacy']
+                pmat.set_shininess(matsettings['shininessFactor'])
+                pmat.set_ambient(LColor(*matsettings['ambientFactor']))
+
+                if 'diffuseTexture' in matsettings:
+                    texinfo = matsettings['diffuseTexture']
+                    texinfos.append(texinfo)
+                    if matsettings['diffuseTextureSrgb'] and texinfo['index'] in self.textures:
+                        self.make_texture_srgb(self.textures[texinfo['index']])
+                else:
+                    pmat.set_diffuse(LColor(*matsettings['diffuseFactor']))
 
-            if 'specularTexture' in matsettings:
-                texinfo = matsettings['specularTexture']
-                texinfos.append(texinfo)
-                if matsettings['specularTextureSrgb'] and texinfo['index'] in self.textures:
-                    self.make_texture_srgb(self.textures[texinfo['index']])
-            else:
-                pmat.set_specular(LColor(*matsettings['specularFactor']))
-        elif 'pbrMetallicRoughness' in gltf_mat:
-            pbrsettings = gltf_mat['pbrMetallicRoughness']
+                if 'emissionTexture' in matsettings:
+                    texinfo = matsettings['emissionTexture']
+                    texinfos.append(texinfo)
+                    if matsettings['emissionTextureSrgb'] and texinfo['index'] in self.textures:
+                        self.make_texture_srgb(self.textures[texinfo['index']])
+                else:
+                    pmat.set_emission(LColor(*matsettings['emissionFactor']))
 
-            pmat.set_base_color(LColor(*pbrsettings.get('baseColorFactor', [1.0, 1.0, 1.0, 1.0])))
-            texinfos.append(pbrsettings.get('baseColorTexture', pbr_fallback))
+                if 'specularTexture' in matsettings:
+                    texinfo = matsettings['specularTexture']
+                    texinfos.append(texinfo)
+                    if matsettings['specularTextureSrgb'] and texinfo['index'] in self.textures:
+                        self.make_texture_srgb(self.textures[texinfo['index']])
+                else:
+                    pmat.set_specular(LColor(*matsettings['specularFactor']))
+            elif 'pbrMetallicRoughness' in gltf_mat:
+                pbrsettings = gltf_mat['pbrMetallicRoughness']
+
+                pmat.set_base_color(LColor(*pbrsettings.get('baseColorFactor', [1.0, 1.0, 1.0, 1.0])))
+                texinfos.append(pbrsettings.get('baseColorTexture', pbr_fallback))
+                if texinfos[-1]['index'] in self.textures:
+                    self.make_texture_srgb(self.textures[texinfos[-1]['index']])
+
+                pmat.set_metallic(pbrsettings.get('metallicFactor', 1.0))
+                pmat.set_roughness(pbrsettings.get('roughnessFactor', 1.0))
+                texinfos.append(pbrsettings.get('metallicRoughnessTexture', pbr_fallback))
+
+            # Normal map
+            texinfos.append(gltf_mat.get('normalTexture', normal_fallback))
+            texinfos[-1]['mode'] = TextureStage.M_normal
+
+            # Emission map
+            pmat.set_emission(LColor(*gltf_mat.get('emissiveFactor', [0.0, 0.0, 0.0]), w=0.0))
+            texinfos.append(gltf_mat.get('emissiveTexture', emission_fallback))
             if texinfos[-1]['index'] in self.textures:
                 self.make_texture_srgb(self.textures[texinfos[-1]['index']])
 
-            pmat.set_metallic(pbrsettings.get('metallicFactor', 1.0))
-            pmat.set_roughness(pbrsettings.get('roughnessFactor', 1.0))
-            texinfos.append(pbrsettings.get('metallicRoughnessTexture', pbr_fallback))
-
-        # Normal map
-        texinfos.append(gltf_mat.get('normalTexture', normal_fallback))
-
-        #Emission map
-        pmat.set_emission(LColor(*gltf_mat.get('emissiveFactor', [0.0, 0.0, 0.0]), w=0.0))
-        texinfos.append(gltf_mat.get('emissiveTexture', emission_fallback))
-        if texinfos[-1]['index'] in self.textures:
-            self.make_texture_srgb(self.textures[texinfos[-1]['index']])
-
         pmat.set_twoside(gltf_mat.get('doubleSided', False))
 
         state = state.set_attrib(MaterialAttrib.make(pmat))
 
         # Setup textures
         tex_attrib = TextureAttrib.make()
         for i, texinfo in enumerate(texinfos):
@@ -639,14 +654,15 @@
             if texdata is None:
                 print("Could not find texture for key: {}".format(texinfo['index']))
                 continue
 
             texstage = TextureStage(str(i))
             texstage.set_sort(i)
             texstage.set_texcoord_name(InternalName.get_texcoord_name(str(texinfo.get('texCoord', 0))))
+            texstage.set_mode(texinfo.get('mode', TextureStage.M_modulate))
             tex_attrib = tex_attrib.add_on_stage(texstage, texdata)
 
         state = state.set_attrib(tex_attrib)
 
         # Setup Alpha mode
         alpha_mode = gltf_mat.get('alphaMode', 'OPAQUE')
         if alpha_mode == 'MASK':
@@ -891,21 +907,27 @@
         # Assign a material
         matid = gltf_primitive.get('material', None)
         if matid is None:
             print(
                 "Warning: mesh {} has a primitive with no material, using an empty RenderState"
                 .format(geom_node.name)
             )
-            mat = RenderState.make_empty()
+            pmat = Material('fallback material')
+            matattrib = MaterialAttrib.make(pmat)
+            texattrib = TextureAttrib.make(self.textures.get('__pbr-fallback'))
+            mat = RenderState.make(matattrib, texattrib)
         elif matid not in self.mat_states:
             print(
                 "Warning: material with name {} has no associated mat state, using an empty RenderState"
                 .format(matid)
             )
-            mat = RenderState.make_empty()
+            pmat = Material('fallback material')
+            matattrib = MaterialAttrib.make(pmat)
+            texattrib = TextureAttrib.make(self.textures.get('__pbr-fallback'))
+            mat = RenderState.make(matattrib, texattrib)
         else:
             mat = self.mat_states[gltf_primitive['material']]
             self.mat_mesh_map[gltf_primitive['material']].append((geom_node.name, primitiveid))
 
         # Add this primitive back to the geom node
         #ss = StringStream()
         #vdata.write(ss)
```

### Comparing `panda3d-gltf-0.8/gltf/loader.py` & `panda3d-gltf-0.9/gltf/loader.py`

 * *Files identical despite different names*

### Comparing `panda3d-gltf-0.8/gltf/viewer.py` & `panda3d-gltf-0.9/gltf/viewer.py`

 * *Files identical despite different names*

### Comparing `panda3d-gltf-0.8/panda3d_gltf.egg-info/PKG-INFO` & `panda3d-gltf-0.9/panda3d_gltf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda3d-gltf
-Version: 0.8
+Version: 0.9
 Summary: glTF utilities for Panda3D
 Home-page: https://github.com/Moguri/panda3d-gltf
 Author: Mitchell Stokes
 License: MIT
 Description: [![Build Status](https://travis-ci.org/Moguri/panda3d-gltf.svg?branch=master)](https://travis-ci.org/Moguri/panda3d-gltf)
         [![](https://img.shields.io/pypi/pyversions/panda3d_gltf.svg)](https://pypi.org/project/panda3d-gltf/)
         [![Panda3D Versions](https://img.shields.io/badge/panda3d-1.10%2C%201.11-blue.svg)](https://www.panda3d.org/)
```

### Comparing `panda3d-gltf-0.8/setup.cfg` & `panda3d-gltf-0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `panda3d-gltf-0.8/setup.py` & `panda3d-gltf-0.9/setup.py`

 * *Files identical despite different names*

