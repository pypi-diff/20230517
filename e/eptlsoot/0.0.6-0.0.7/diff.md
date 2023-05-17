# Comparing `tmp/eptlsoot-0.0.6-cp39-cp39-win_amd64.whl.zip` & `tmp/eptlsoot-0.0.7-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 1713128 bytes, number of entries: 20
+Zip file size: 1713327 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat      513 b- defN 23-Apr-27 02:29 eptlsoot/__init__.py
 -rw-rw-rw-  2.0 fat  1465856 b- defN 23-Apr-05 21:26 eptlsoot/_eptlsoot.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     6093 b- defN 23-Apr-05 21:43 eptlsoot/cpfr.py
 -rw-rw-rw-  2.0 fat      679 b- defN 23-Apr-05 21:38 eptlsoot/eptlsoot.py
 -rw-rw-rw-  2.0 fat      644 b- defN 23-Apr-05 21:43 eptlsoot/psr.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-05 04:38 eptlsoot/apps/__init__.py
 -rw-rw-rw-  2.0 fat      882 b- defN 23-Apr-25 22:15 eptlsoot/apps/flame.py
 -rw-rw-rw-  2.0 fat     1843 b- defN 23-Apr-13 14:11 eptlsoot/apps/pahgrowth.py
--rw-rw-rw-  2.0 fat     6921 b- defN 23-Apr-27 04:40 eptlsoot/apps/reactors.py
+-rw-rw-rw-  2.0 fat     9348 b- defN 23-May-17 02:00 eptlsoot/apps/reactors.py
 -rw-rw-rw-  2.0 fat      265 b- defN 23-Apr-05 04:46 eptlsoot/apps/solutionarray.py
--rw-rw-rw-  2.0 fat     3145 b- defN 23-May-13 12:46 eptlsoot/apps/sootgas.py
+-rw-rw-rw-  2.0 fat     3447 b- defN 23-May-17 00:40 eptlsoot/apps/sootgas.py
 -rw-rw-rw-  2.0 fat      950 b- defN 23-Apr-05 21:55 eptlsoot/apps/sootmodels.py
 -rw-rw-rw-  2.0 fat     5993 b- defN 23-Apr-08 23:53 eptlsoot/apps/sootwrappers.py
 -rw-rw-rw-  2.0 fat      239 b- defN 23-Apr-05 21:52 eptlsoot/apps/surfacereactions.py
--rw-rw-rw-  2.0 fat  1717248 b- defN 23-May-16 23:48 eptlsoot/lib/_eptlsoot.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  1717248 b- defN 23-May-17 03:46 eptlsoot/lib/_eptlsoot.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat  1468928 b- defN 23-Apr-05 21:11 eptlsoot2/_eptlsoot2.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      734 b- defN 23-May-16 23:48 eptlsoot-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-16 23:48 eptlsoot-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-16 23:47 eptlsoot-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1641 b- defN 23-May-16 23:48 eptlsoot-0.0.6.dist-info/RECORD
-20 files, 4682683 bytes uncompressed, 1710464 bytes compressed:  63.5%
+-rw-rw-rw-  2.0 fat      734 b- defN 23-May-17 03:46 eptlsoot-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-17 03:46 eptlsoot-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-17 03:46 eptlsoot-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1641 b- defN 23-May-17 03:46 eptlsoot-0.0.7.dist-info/RECORD
+20 files, 4685412 bytes uncompressed, 1710663 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: eptlsoot/lib/_eptlsoot.cp39-win_amd64.pyd
 Comment: 
 
 Filename: eptlsoot2/_eptlsoot2.cp39-win_amd64.pyd
 Comment: 
 
-Filename: eptlsoot-0.0.6.dist-info/METADATA
+Filename: eptlsoot-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: eptlsoot-0.0.6.dist-info/WHEEL
+Filename: eptlsoot-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: eptlsoot-0.0.6.dist-info/top_level.txt
+Filename: eptlsoot-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: eptlsoot-0.0.6.dist-info/RECORD
+Filename: eptlsoot-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## eptlsoot/apps/reactors.py

```diff
@@ -55,24 +55,43 @@
             y0 = np.hstack((0.0, self.inlet.mdot, self.inlet.T, self.inlet.Y, self.inlet.soot));
             self.solver = integrate.LSODA(fun=self.derivatives, t0=0, y0=y0, t_bound=self.max_length,
                                         first_step=self.first_step, max_step = self.max_step);
             
 
     @property
     def total_carbon_flux(self) -> float:
-        carbon_mass = self.soot_gas.carbon_mass() + self.soot_wrapper.soot_model.carbon_mass();
+        carbon_mass = self.soot_gas.elemental_mass_fraction('C') + self.soot_wrapper.soot_model.carbon_mass();
         return carbon_mass * self.mdot;
     
     @property
     def gas_carbon_flux(self) -> float:
-        return self.soot_gas.carbon_mass() * self.mdot;
+        return self.soot_gas.elemental_mass_fraction('C') * self.mdot;
 
     @property
     def soot_carbon_flux(self) -> float:
-        return self.soot_wrapper.soot_model.carbon_mass() * self.mdot;
+        return self.soot_wrapper.soot_model.elemental_mass_fraction('C') * self.mdot;
+
+
+    @property
+    def total_hydrogen_flux(self) -> float:
+        hydrogen_mass = self.soot_gas.elemental_mass_fraction('H') + self.soot_wrapper.soot_model.hydrogen_mass();
+        return hydrogen_mass * self.mdot;
+    
+    @property
+    def gas_hydrogen_flux(self) -> float:
+        return self.soot_gas.elemental_mass_fraction('H') * self.mdot;
+
+    @property
+    def soot_hydrogen_flux(self) -> float:
+        return self.soot_wrapper.soot_model.elemental_mass_fraction('H') * self.mdot;
+
+    @property
+    def gas_elemental_flux(self, element_name) -> float:
+        return self.soot_gas.elemental_mass_fraction(element_name) * self.mdot;
+
 
 class Inlet:
     def __init__(self, reactor, mdot = 0, soot = "zero_soot"):
         self.reactor = reactor;
         self._Y = self.reactor.soot_gas.X;
         self._X = self.reactor.soot_gas.Y;
         self.T = self.reactor.soot_gas.T;
@@ -129,25 +148,41 @@
             y0 = np.hstack((self.soot_gas.rho, self.soot_gas.T, self.soot_gas.Y_array, self.initial_soot));
             self.solver = integrate.LSODA(fun=self.derivatives, t0=0, y0=y0, t_bound=self.max_time,
                                         first_step=self.first_step, max_step = self.max_step);
 
 
     @property
     def total_carbon_mass(self) -> float:
-        carbon_mass = self.soot_gas.carbon_mass() + self.soot_wrapper.soot_model.carbon_mass();
+        carbon_mass = self.soot_gas.elemental_mass_fraction('C') + self.soot_wrapper.soot_model.carbon_mass();
         return carbon_mass;
 
     @property
     def gas_carbon_mass(self) -> float:
-        return self.soot_gas.carbon_mass();
+        return self.soot_gas.elemental_mass_fraction('C');
 
     @property
     def soot_carbon_mass(self) -> float:
         return self.soot_wrapper.soot_model.carbon_mass();
 
+    @property
+    def total_hydrogen_mass(self) -> float:
+        hydrogen_mass = self.soot_gas.elemental_mass_fraction('H') + self.soot_wrapper.soot_model.hydrogen_mass();
+        return hydrogen_mass;
+
+    @property
+    def gas_hydrogen_mass(self) -> float:
+        return self.soot_gas.elemental_mass_fraction('H');
+
+    @property
+    def soot_hydrogen_mass(self) -> float:
+        return self.soot_wrapper.soot_model.hydrogen_mass();
+
+    @property
+    def gas_elemental_mass(self, element_name) -> float:
+        return self.soot_gas.elemental_mass_fraction(element_name);
 
 
 class PerfectlyStirredReactor(ReactorAbstract, CPSRSoot):
     def __init__(self, soot_gas):
         super().__init__(soot_gas);
         self.create_soot_wrapper();
         # Reactor pressure
@@ -189,24 +224,42 @@
             self.set_modt();
             y0 = np.hstack((self.soot_gas.rho, self.soot_gas.T, self.soot_gas.Y_array, self.initial_soot));
             self.solver = integrate.LSODA(fun=self.derivatives, t0=0, y0=y0, t_bound=self.max_time,
                                         first_step=self.first_step, max_step = self.max_step);
 
     @property
     def total_carbon_flux(self) -> float:
-        carbon_mass = self.soot_gas.carbon_mass() + self.soot_wrapper.soot_model.carbon_mass();
-        return carbon_mass * self.mdot;
+        carbon_mass = self.soot_gas.elemental_mass_fraction('C') + self.soot_wrapper.soot_model.carbon_mass();
+        return carbon_mass * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
     
     @property
     def gas_carbon_flux(self) -> float:
-        return self.soot_gas.carbon_mass() * self.mdot;
+        return self.soot_gas.elemental_mass_fraction('C') * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
 
     @property
     def soot_carbon_flux(self) -> float:
-        return self.soot_wrapper.soot_model.carbon_mass() * self.mdot;
+        return self.soot_wrapper.soot_model.elemental_mass_fraction('C') * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
+
+
+    @property
+    def total_hydrogen_flux(self) -> float:
+        hydrogen_mass = self.soot_gas.elemental_mass_fraction('H') + self.soot_wrapper.soot_model.hydrogen_mass();
+        return hydrogen_mass * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
+    
+    @property
+    def gas_hydrogen_flux(self) -> float:
+        return self.soot_gas.elemental_mass_fraction('H') * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
+
+    @property
+    def soot_hydrogen_flux(self) -> float:
+        return self.soot_wrapper.soot_model.elemental_mass_fraction('H') * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
+
+    @property
+    def gas_elemental_flux(self, element_name) -> float:
+        return self.soot_gas.elemental_mass_fraction(element_name) * self.mdot * (1.0-self.soot_wrapper.soot_model.volume_fraction());
 
 
     @property
     def residence_time(self) -> float:
         return self.phy_restime;
 
     @residence_time.setter
```

## eptlsoot/apps/sootgas.py

```diff
@@ -105,10 +105,18 @@
         #     sp_index = gas.species_names.index(sp);
         #     no_c = gas.n_atoms(sp, "C");
         #     total_c_mass += gas.X[sp_index]*no_c*MW_C;
 
         # total_c_mass = total_c_mass / gas.mean_molecular_weight; #[kg C/kg gas]
         #return total_c_mass
         return gas.elemental_mass_fraction('C')
+    
+    def elemental_mass_fraction(self, element_name):
+        gas = self.cantera_gas;
+        return gas.elemental_mass_fraction(element_name)
+    
+    def elemental_mole_fraction(self, element_name):
+        gas = self.cantera_gas;
+        return gas.elemental_mole_fraction(element_name)
```

## Comparing `eptlsoot-0.0.6.dist-info/METADATA` & `eptlsoot-0.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptlsoot
-Version: 0.0.6
+Version: 0.0.7
 Summary: Soot model from EPTL group
 Author-email: Mo Adib <moademic@gmail.com>
 Project-URL: Homepage, https://carleton.ca/eptl/people/336/
 Keywords: computational,soot
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

## Comparing `eptlsoot-0.0.6.dist-info/RECORD` & `eptlsoot-0.0.7.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 eptlsoot/_eptlsoot.cp39-win_amd64.pyd,sha256=n0qfhcvFyEQjpv7117acr92mBBCgo8dYZGJuVLbOa3Y,1465856
 eptlsoot/cpfr.py,sha256=INVeWGJNn6P_0GgLszuYd4T3ACnSRBngK_myE55eJ00,6093
 eptlsoot/eptlsoot.py,sha256=BykhVsFVrodoBTmpyPljYZdOtqaAyWJ0mj__3-_YWy8,679
 eptlsoot/psr.py,sha256=bOhT9fzCENuIAuZSD4-xNu_bvam7Q5bp3x7Q1XnicME,644
 eptlsoot/apps/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 eptlsoot/apps/flame.py,sha256=F1jPh51a3oQzRlc1dUEpr3UM6RFRsN-JSL6OsoRhdH0,882
 eptlsoot/apps/pahgrowth.py,sha256=Bv_iD3piHX9JDj1x57t5gtbUye3AWtAJIghGDM9jASQ,1843
-eptlsoot/apps/reactors.py,sha256=4R3fEei2sJ9v3XnmI1jsFekg444PW2oslTrMGeGlBo8,6921
+eptlsoot/apps/reactors.py,sha256=8HcA8DZyTuk1XQxQQz5Ax1gwBr7OTV0xUPCRNItr8uo,9348
 eptlsoot/apps/solutionarray.py,sha256=gGyAu8LnGNU3CuDvae8rXD3TrEnAanYeWOa1QErsV8U,265
-eptlsoot/apps/sootgas.py,sha256=2Zrb9vqIbgCR0GAcAn1KMYE1Jfj92-TAgP9EvEF3uw4,3145
+eptlsoot/apps/sootgas.py,sha256=AqpSsu6_Tuk3L0wlekNs3ZalMGhsZDtB4Yg54lIruuA,3447
 eptlsoot/apps/sootmodels.py,sha256=7ricACNZm1dQCstx6oYCBR26FheBwrrCYqkSe1KcqYA,950
 eptlsoot/apps/sootwrappers.py,sha256=oIW4uTcTtjvPkTuGRrICE5owx3T6R8fmDCAuVx-ZMhU,5993
 eptlsoot/apps/surfacereactions.py,sha256=pJmeJNx1MY9mEnNaDxdcsAy6bm1d_rBtJUt-mkZqiJk,239
-eptlsoot/lib/_eptlsoot.cp39-win_amd64.pyd,sha256=65oRCVDApxjbI1BNdHc_qyr6qPyyJrWP21o7QZt515s,1717248
+eptlsoot/lib/_eptlsoot.cp39-win_amd64.pyd,sha256=Oi8pw46_37lavissYG9MTG_0kToTv_f779ktWdjmf4s,1717248
 eptlsoot2/_eptlsoot2.cp39-win_amd64.pyd,sha256=_ZuT4TUsgcE1q80t6Dpxopn37BhJUZsMZcqBhaRKFiM,1468928
-eptlsoot-0.0.6.dist-info/METADATA,sha256=RBbEo7_BBCVkYFzZky5oqOkAWaeVJrFL1EsTBc_byMA,734
-eptlsoot-0.0.6.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-eptlsoot-0.0.6.dist-info/top_level.txt,sha256=DwjN4tmB8aSbrdDOeaZUoty0uZdWl5j18VgGc2qzU_U,9
-eptlsoot-0.0.6.dist-info/RECORD,,
+eptlsoot-0.0.7.dist-info/METADATA,sha256=TiXzWyvDuSyBcEnfvW-HpTwCaAYuGUqT4ragHDv0JVo,734
+eptlsoot-0.0.7.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+eptlsoot-0.0.7.dist-info/top_level.txt,sha256=DwjN4tmB8aSbrdDOeaZUoty0uZdWl5j18VgGc2qzU_U,9
+eptlsoot-0.0.7.dist-info/RECORD,,
```

