# Comparing `tmp/liveboot-0.0.3.tar.gz` & `tmp/liveboot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveboot-0.0.3.tar", last modified: Mon Mar  6 18:10:15 2023, max compression
+gzip compressed data, was "liveboot-0.0.4.tar", last modified: Wed May 17 14:41:43 2023, max compression
```

## Comparing `liveboot-0.0.3.tar` & `liveboot-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-03-06 18:10:15.865274 liveboot-0.0.3/
--rw-r--r--   0 tparment (15010) diana    (200036)      568 2023-03-06 18:10:15.864968 liveboot-0.0.3/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)    10393 2023-03-06 16:56:57.000000 liveboot-0.0.3/README.md
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-03-06 18:10:15.859119 liveboot-0.0.3/cloud-init/
--rwxr-xr-x   0 tparment (15010) diana    (200036)     1149 2023-03-06 13:47:04.000000 liveboot-0.0.3/cloud-init/seed-cloud-init.sh
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-03-06 18:10:15.859397 liveboot-0.0.3/fedora/
--rwxr-xr-x   0 tparment (15010) diana    (200036)      853 2023-02-28 16:22:08.000000 liveboot-0.0.3/fedora/build-fedora-liveboot.sh
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-03-06 18:10:15.861842 liveboot-0.0.3/liveboot/
--rw-r--r--   0 tparment (15010) diana    (200036)     8450 2023-03-06 15:51:06.000000 liveboot-0.0.3/liveboot/cli.py
--rw-r--r--   0 tparment (15010) diana    (200036)     8442 2023-03-06 14:53:30.000000 liveboot-0.0.3/liveboot/cli2.py
--rw-r--r--   0 tparment (15010) diana    (200036)    18106 2023-03-06 13:47:04.000000 liveboot-0.0.3/liveboot/idrac.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-03-06 18:10:15.863871 liveboot-0.0.3/liveboot/templates/
--rw-r--r--   0 tparment (15010) diana    (200036)      935 2023-03-06 11:43:02.000000 liveboot-0.0.3/liveboot/templates/cloud-init-template.yaml.j2
--rw-r--r--   0 tparment (15010) diana    (200036)     1194 2023-03-04 15:18:14.000000 liveboot-0.0.3/liveboot/test_iso.py
--rw-r--r--   0 tparment (15010) diana    (200036)       47 2023-03-06 17:15:21.000000 liveboot-0.0.3/liveboot/version.py
--rw-r--r--   0 tparment (15010) diana    (200036)      836 2023-03-06 13:46:32.000000 liveboot-0.0.3/liveboot/waitloop.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-03-06 18:10:15.863579 liveboot-0.0.3/liveboot.egg-info/
--rw-r--r--   0 tparment (15010) diana    (200036)      568 2023-03-06 18:10:15.000000 liveboot-0.0.3/liveboot.egg-info/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)      463 2023-03-06 18:10:15.000000 liveboot-0.0.3/liveboot.egg-info/SOURCES.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2023-03-06 18:10:15.000000 liveboot-0.0.3/liveboot.egg-info/dependency_links.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       47 2023-03-06 18:10:15.000000 liveboot-0.0.3/liveboot.egg-info/entry_points.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       57 2023-03-06 18:10:15.000000 liveboot-0.0.3/liveboot.egg-info/requires.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        9 2023-03-06 18:10:15.000000 liveboot-0.0.3/liveboot.egg-info/top_level.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       38 2023-03-06 18:10:15.865377 liveboot-0.0.3/setup.cfg
--rwxr-xr-x   0 tparment (15010) diana    (200036)     1816 2023-03-06 15:49:13.000000 liveboot-0.0.3/setup.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-03-06 18:10:15.864571 liveboot-0.0.3/ubuntu/
--rwxr-xr-x   0 tparment (15010) diana    (200036)     2568 2023-02-28 16:22:08.000000 liveboot-0.0.3/ubuntu/patch-ubuntu-image.sh
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-05-17 14:41:43.745536 liveboot-0.0.4/
+-rw-r--r--   0 tparment (15010) diana    (200036)      568 2023-05-17 14:41:43.745266 liveboot-0.0.4/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)     7856 2023-05-17 14:20:11.000000 liveboot-0.0.4/README.md
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-05-17 14:41:43.737461 liveboot-0.0.4/cloud-init/
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     1149 2023-03-06 13:47:04.000000 liveboot-0.0.4/cloud-init/seed-cloud-init.sh
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-05-17 14:41:43.738124 liveboot-0.0.4/fedora/
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     2328 2023-05-17 13:01:50.000000 liveboot-0.0.4/fedora/build-rpm-liveboot.sh
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-05-17 14:41:43.741828 liveboot-0.0.4/liveboot/
+-rw-r--r--   0 tparment (15010) diana    (200036)     8609 2023-05-17 10:28:30.000000 liveboot-0.0.4/liveboot/cli.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     8442 2023-03-06 14:53:30.000000 liveboot-0.0.4/liveboot/cli2.py
+-rw-r--r--   0 tparment (15010) diana    (200036)    18106 2023-03-06 13:47:04.000000 liveboot-0.0.4/liveboot/idrac.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-05-17 14:41:43.744267 liveboot-0.0.4/liveboot/templates/
+-rw-r--r--   0 tparment (15010) diana    (200036)      935 2023-03-06 11:43:02.000000 liveboot-0.0.4/liveboot/templates/cloud-init-template.yaml.j2
+-rw-r--r--   0 tparment (15010) diana    (200036)     1194 2023-03-04 15:18:14.000000 liveboot-0.0.4/liveboot/test_iso.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       47 2023-05-17 14:41:23.000000 liveboot-0.0.4/liveboot/version.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      836 2023-03-06 13:46:32.000000 liveboot-0.0.4/liveboot/waitloop.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-05-17 14:41:43.743987 liveboot-0.0.4/liveboot.egg-info/
+-rw-r--r--   0 tparment (15010) diana    (200036)      568 2023-05-17 14:41:43.000000 liveboot-0.0.4/liveboot.egg-info/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)      460 2023-05-17 14:41:43.000000 liveboot-0.0.4/liveboot.egg-info/SOURCES.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2023-05-17 14:41:43.000000 liveboot-0.0.4/liveboot.egg-info/dependency_links.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       47 2023-05-17 14:41:43.000000 liveboot-0.0.4/liveboot.egg-info/entry_points.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       57 2023-05-17 14:41:43.000000 liveboot-0.0.4/liveboot.egg-info/requires.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        9 2023-05-17 14:41:43.000000 liveboot-0.0.4/liveboot.egg-info/top_level.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       38 2023-05-17 14:41:43.745611 liveboot-0.0.4/setup.cfg
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     1813 2023-05-17 14:04:28.000000 liveboot-0.0.4/setup.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-05-17 14:41:43.744917 liveboot-0.0.4/ubuntu/
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     3419 2023-05-17 14:36:03.000000 liveboot-0.0.4/ubuntu/patch-ubuntu-image.sh
```

### Comparing `liveboot-0.0.3/PKG-INFO` & `liveboot-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveboot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Testbed Management Framework for Sophia Node
 Author: Thierry Parmentelat
 Author-email: thierry.parmentelat@inria.fr
 License: CC BY-SA 4.0
 Project-URL: source, https://github.com/sopnode/liveboot/
 Keywords: Sophia Node,networking testbed
 Classifier: Development Status :: 4 - Beta
```

### Comparing `liveboot-0.0.3/README.md` & `liveboot-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # booting vanilla OSes live using redfish
 
 goal is for a user to be able to boot a sopnode with a live session of an OS of
 their choice; for starters we have ubuntu LTS 18 20 and 22, and fedora 36 and 37
 
 expected (stuff to test):
 
-* can enter ssh as root using our ssh keys
-* can reboot gracefully
-
-plus:
-
-* we don't care too much about the state of the console during that time
-* it's OK if the console is stuck at the installation program, as long as, of
-course, no installation takes places
-* in general we can easily open a shell from the console; that's OK too, and
-  actually useful esp. at the begining of this project as we often need to
-  inspect the current state, sometimes with no ssh available
+* can turn boxes on and off
+* can reboot on hard disk
+* can reboot on vanilla image for some pre-built OS's
+  * can then enter ssh as root using our ssh keys
+  * currently supports fedora and ubuntu
+* there is also support for dealing with the BIOS config, i.e. to schedule, prior to rebooting
+  * a complete reset of the BIOS settings
+  * and then specific changes
 
 ## a sample session
 
 run this on `sopnode-l1`
 
 ```bash
 # the plain command name is liveboot
@@ -59,14 +56,15 @@
 ```
 
 to see the list of available images, for now just do
 
 ```bash
 ls /srv/shares/bootable-images/
 ```
+
 where the short names like `u18` above are symlinks to real images
 
 see below about how to produce these images
 
 ### `wait`
 
 this is to wait for a node to be ssh-reachable
@@ -84,15 +82,15 @@
 
 to reboot the node under its "normal" OS - i.e. the one on its hard drive, do this
 
 ```bash
 lb diskboot w3
 ```
 
-### `biosget`: inspecting the BIOS settings
+### `biosget` : inspecting the BIOS settings
 
 you can see them all
 
 ```
 lb biosget w3
 BIOS settings captured on sopnode-w3-drac.inria.fr on 2023 03 06 @ 17:44:37
                   AcPwrRcvry: Last
@@ -107,15 +105,14 @@
 
 ```
 lb biosget w3 profile
 BIOS settings captured on sopnode-w3-drac.inria.fr on 2023 03 06 @ 17:46:02 with pattern=`profile`
      SysProfile: PerfPerWattOptimizedDapc
 WorkloadProfile: NotAvailable
 
-
 lb biosget w3 'profile|usb'
 BIOS settings captured on sopnode-w3-drac.inria.fr on 2023 03 06 @ 17:46:10 with pattern=`profile|usb`
 ControlledTurboMinusBin: 0
          GenericUsbBoot: Disabled
             InternalUsb: On
              SysProfile: PerfPerWattOptimizedDapc
          UsbManagedPort: On
@@ -141,142 +138,114 @@
 * as a corollary, inspecting the job queue in the DRAC  
   be aware that when you change a bios setting, it's not applied immediately (it
   makes sense) but kept in a job queue
 
 all this is maybe not quite entirely smooth at this point,
 so please start with using the simple features above
 
-#### note
+### devel / tmp notes
 
 there's a need to better understand the logic of how the drac and the BIOS are
 supposed to interact; see also
 
 <https://github.com/dell/iDRAC-Redfish-Scripting/issues/249>
 
-#### warning
+**WARNING**
 
-if you do try to mess with the BIOS settings this way, 
+if you do try to mess with the BIOS settings this way,
 and you hit a wall: trying to insert a virtual media complains about the server
 not having 1GB of RAM (sic): then do a biosreset, and reboot as many times as needed
 
 ## strategy
 
+### one-time
+
 * build a `cloud-init` capable live image for the target distribution
   * fedora: use `livecd-creator`
   * ubuntu: use the upstream public image and tweak its grub config
     **note** in theory there are other means to achieve that; in particular
     https://help.ubuntu.com/community/LiveCDCustomization, even if my first
     attempts seemed unrewarding, maybe this could use another look
-* build a cloud-init config that contains our ssh keys
-* expose these 2 ISOs using redfish virtual media, and boot from there
-* the HHD-installed fedora37 is totally untouched, so it can still be used if
-  needed
-* diskless ?
-  * in a first step, keep the live session totally diskless
-  * later on we can consider shrinking the disk exposed
-    to the current fedora installation, so that the live session
-    can store stuff on the disk and thus have more memory space
-
-## setup on sopnode-l1
-
-using this box as a gatekeeper for the sopnode-w* workers
-
-### setup nginx
-
-done manually - as opposed to using ansible - see `/etc/nginx/nginx.conf`
-expose folder `/srv/shares/bootable-images/` as <http://sopnode-l1.inria.fr/bootable-images/>
-
-### fetch some images
-
-as far as ubuntu, we start from the publicly available so-called live-server images
-
-```bash
-# on l1
-cd /srv/shares/bootable-images/public
-# see .url files
-```
-
-## on sopnode-w3 (setup)
-
-* enabled life cycle manager in the BIOS
-(not quite sure yet if that's mandatory, but it does feel that way)
 
-* iDrac firmware version was 5.10.50.00, upgraded to 6.x
-  (its other siblings are all upgraded as well)
+### each session
 
-## ubuntu
+* build a cloud-init config that contains our ssh keys (will depend on the slice)
+* expose these 2 ISOs using redfish virtual media, and boot from there
+* the HHD-installed OS (here fedora37) is totally untouched, so it can still be used if
+  needed (see `diskboot`)
 
-1st and foremost objective is to create an ssh-reachable admin user that we can later on use with ansible
+### diskless ?
 
-### cloud-init images
+* in a first step, keep the live session totally diskless
+* later on we can consider shrinking the disk exposed
+  to the current fedora installation, so that the live session
+  can store stuff on the disk and thus have more memory space
 
-based on <https://cloudinit.readthedocs.io/en/latest/reference/datasources/nocloud.html#creating-a-disk>
+## building images
 
-```shell
-# create an ISO image suitable for cloud-init
-seed-cloud-init.sh /srv/shares/bootable-images/cidata-seed.iso cloud-init-template.yaml
+```{warning}
+this is still WIP
 ```
 
-### liveboot image
+### ubuntu liveboot
 
 we patch the standard ubuntu image, e.g.
 
 ```shell
 # from https://releases.ubuntu.com/22.04/ubuntu-22.04.2-live-server-amd64.iso
 -rw-r--r-- 1 root root 1474873344 Feb 16 15:41 ubuntu-22.04.1-live-server-amd64.iso
 ```
 
 using our home-brewed tool like so
 
 ```shell
-./patch-ubuntu-image.sh /srv/shares/bootable-images/ubuntu-22.04.2-live-server-amd64.iso
+./patch-ubuntu-image.sh /srv/shares/bootable-images/public/ubuntu-22.04.2-live-server-amd64.iso
 ```
 
-### of interest for troubleshooting
+#### of interest for troubleshooting
 
 * use Alt-F2 to get a login shell without the password
 * https://cloudinit.readthedocs.io/en/latest/reference/datasources/nocloud.html
 * https://cloudinit.readthedocs.io/en/latest/howto/bugs.html#collect-logs
 
-### status
+#### status
 
 * 22: OK
 * 20: kind of OK
-  * the console is stuck at 'select your language' (harmless)
-  * **HOWEVER** when rebooting the system enters an endless loop of squashfs error
+  + the console is stuck at 'select your language' (harmless)
+  + **HOWEVER** when rebooting the system enters an endless loop of squashfs error
 * 18: OK as well
 
-### epilogue: `livefs-editor` ?
+#### epilogue: `livefs-editor` ?
 
 should we switch to using livefs-editor
 
 see also https://github.com/mwhudson/livefs-editor/issues/31
 
-## fedora
+### fedora liveboot
 
 here's what we need:
 
 https://docs.fedoraproject.org/en-US/quick-docs/creating-and-using-a-live-installation-image/#proc_creating-and-using-live-cd
 
 here again, working from sopnode-l1
 
-### prerequisites
+#### prerequisites
 
 ```shell
 dnf install livecd-tools fedora-kickstarts pykickstart
 ```
 
-### f37
+#### f37
 
 inspired from <https://www.spinics.net/linux/fedora/fedora-users/msg516742.html>
 
 ```bash
 cd fedora
-# xxx argument not yet used
-build-fedora-liveboot.sh 37
+build-rpm.sh f37
 ```
 
 the `-original.ks` file is kept in the repo for the record only; it is the output of
 
 ```bash
 ksflatten -c /usr/share/spin-kickstarts/fedora-liveboot.ks -o fedora-liveboot-original.ks
 ```
@@ -289,92 +258,33 @@
 
 the process if rather long, as it actually builds an image from scratch for us
 however it uses cloud-init at run time so we only need to do it once, and the ssh keys
 actually used will come from the `cidata` image
 
 see also <https://github.com/livecd-tools/livecd-tools>
 
-### status
+#### status
 
 * works with rawhide
 * scripting for fedora37
 * need to check alterative versions as well ?
 
+### rocky liveboot
 
-***
-***
-***
-
-## archive section
-
-### setup samba on sopnode-l1
-
-also done; however it is **no longer needed** since with idrac v6.x we can use
-both virtual media slots to expose the ISO **and** the cloud-init config **over http**
+very close to fedora, so the code is also in the `fedora/` folder
 
-so for the record only:
+* kickstart files can be found here
+  https://github.com/rocky-linux/kickstarts/tree/r9
+  
 
-using the ansible collection here
-<https://github.com/vladgh/ansible-collection-vladgh-samba>
-
-we create a samba service on the sopnode-l1 server, where we will
-store bootable images
-
-```bash
-ansible-playbook -i sopnodes-inventory -K setup-samba-playbook.yml
-```
-
-## basics of redfish
-
-leverage redfish Python scripts from here
-<https://github.com/dell/iDRAC-Redfish-Scripting>
-to redirect sopnode-w* to boot off these images
-
-```bash
-# this is where I run the stuff
-sopnode-l1@root ~/kube-redfish (master=) $
-# and this file contains helpful shortcuts
-source aliases
-# FYI Dell's repo is cloned into a separate repo, and the python scripts are here:
-# (cd iD*/*on; pwd)
-# /root/kube-redfish/iDRAC-Redfish-Scripting/Redfish Python
-```
-
-see aliases for the extended version - we use the aliases only here
-
-### `power` - `GetSetPowerStateREDFISH.py`
-
-```bash
-power3 --get
-power3 --set GracefulRestart
-power3 --set ForceRestart
-```
-
-### `media` - `InsertEjectVirtualMediaREDFISH.py`
+### cloud-init images
 
-it feels like only one of 'cd' and 'removabledisk' are available at the same time
-we try to use the removabledisk to inject the ignition config
+based on <https://cloudinit.readthedocs.io/en/latest/reference/datasources/nocloud.html#creating-a-disk>
 
 ```shell
-media3 --get
-# cleanup
-media3 --action eject --index 1
-media3 --action eject --index 2
-# for example
-media3 --action insert --index 1 --uripath  http://138.96.245.50/bootable-images/ubuntu-22.04.1-live-server-amd64-liveboot.iso
-media3 --action insert --index 2 --uripath  http://138.96.245.50/bootable-images/cidata-seed.iso
-```
-
-### `nextboot` - `SetNextOneTimeBootVirtualMediaDeviceOemREDFISH.py`
-
-```bash
-# works also without --reboot
-nextboot3 --device 1 --reboot
+# create an ISO image suitable for cloud-init
+seed-cloud-init.sh /srv/shares/bootable-images/cidata-seed.iso cloud-init-template.yaml
 ```
 
-### `nextbootdev` - `SetNextOneTimeBootDeviceREDFISH.py`
-
-```bash
-# same as above mostly
-nextbootdev --device Hdd --reboot
-```
+## issues
 
+please use https://github.com/sopnode/liveboot/issues
```

### Comparing `liveboot-0.0.3/cloud-init/seed-cloud-init.sh` & `liveboot-0.0.4/cloud-init/seed-cloud-init.sh`

 * *Files identical despite different names*

### Comparing `liveboot-0.0.3/liveboot/cli.py` & `liveboot-0.0.4/liveboot/cli2.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,17 +163,17 @@
     # check image can be found
     if (code := (requests.head(url1).status_code)) // 100 != 2:
         logging.error(f"got HHTP code {code} with {url1}")
         logging.error(f"this image does not seem to exist")
         return 1
 
     stem = args.stem
-    packaged_data = resources.files('liveboot')
+    packaged_data = resources.files('cloud-init')
     # generate the cloud-init seed
-    template = packaged_data / "templates/cloud-init-template.yaml.j2"
+    template = packaged_data / "cloud-init-template.yaml.j2"
     # xxx these should come from the slice
     # they are hard-wired for now
     keysfile = "/etc/sopnode/sopnode-keys.yaml"
     seed = f"cidata-seed-{stem}.iso"
     path_to_seed = f"{images_config['absolute-path']}/{seed}"
     command = f"seed-cloud-init.sh {stem} {keysfile} {template} {path_to_seed}"
     logging.info(f"running command {command}")
```

### Comparing `liveboot-0.0.3/liveboot/cli2.py` & `liveboot-0.0.4/liveboot/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # pylint: disable=missing-function-docstring
 
 import sys
 import os
 import time
 import logging
 from argparse import ArgumentParser
+from pathlib import Path
 from importlib import resources
 
 import requests
 import yaml
 
 from .idrac import Idrac
 from .version import __version__ as liveboot_version
@@ -153,27 +154,30 @@
 def liveboot(config, args):
     images_config = config['images']
     proto = images_config.get('proto', 'http')
     ip = images_config.get('ip')
     port = images_config.get('port', 80)
     path = images_config.get('path')
     image = args.image
+    # normalize path - allows to pass a path using bash completion
+    image_path = Path(image)
+    image = f"{image_path.stem}.iso"
     url_prefix = f"{proto}://{ip}:{port}/{path}"
     url1 = f"{url_prefix}/{image}"
 
     # check image can be found
     if (code := (requests.head(url1).status_code)) // 100 != 2:
         logging.error(f"got HHTP code {code} with {url1}")
         logging.error(f"this image does not seem to exist")
         return 1
 
     stem = args.stem
-    packaged_data = resources.files('cloud-init')
+    packaged_data = resources.files('liveboot')
     # generate the cloud-init seed
-    template = packaged_data / "cloud-init-template.yaml.j2"
+    template = packaged_data / "templates/cloud-init-template.yaml.j2"
     # xxx these should come from the slice
     # they are hard-wired for now
     keysfile = "/etc/sopnode/sopnode-keys.yaml"
     seed = f"cidata-seed-{stem}.iso"
     path_to_seed = f"{images_config['absolute-path']}/{seed}"
     command = f"seed-cloud-init.sh {stem} {keysfile} {template} {path_to_seed}"
     logging.info(f"running command {command}")
@@ -253,15 +257,15 @@
     parser.add_argument("stem")
 
 
 
 
 @subcommand
 def version(config, args):
-    print(f"sopnode v{liveboot_version}")
+    print(f"liveboot v{liveboot_version}")
 
 
 
 def main() -> int:
 
     parser = ArgumentParser()
     parser.add_argument("--config", default=CONFIG_FILENAME,
```

### Comparing `liveboot-0.0.3/liveboot/idrac.py` & `liveboot-0.0.4/liveboot/idrac.py`

 * *Files identical despite different names*

### Comparing `liveboot-0.0.3/liveboot/templates/cloud-init-template.yaml.j2` & `liveboot-0.0.4/liveboot/templates/cloud-init-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `liveboot-0.0.3/liveboot/test_iso.py` & `liveboot-0.0.4/liveboot/test_iso.py`

 * *Files identical despite different names*

### Comparing `liveboot-0.0.3/liveboot/waitloop.py` & `liveboot-0.0.4/liveboot/waitloop.py`

 * *Files identical despite different names*

### Comparing `liveboot-0.0.3/liveboot.egg-info/PKG-INFO` & `liveboot-0.0.4/liveboot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveboot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Testbed Management Framework for Sophia Node
 Author: Thierry Parmentelat
 Author-email: thierry.parmentelat@inria.fr
 License: CC BY-SA 4.0
 Project-URL: source, https://github.com/sopnode/liveboot/
 Keywords: Sophia Node,networking testbed
 Classifier: Development Status :: 4 - Beta
```

### Comparing `liveboot-0.0.3/setup.py` & `liveboot-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     packages=['liveboot'],
     version=__version__,
     python_requires=">=3.10",
 
     entry_points={ 'console_scripts': ['liveboot = liveboot.cli:main'] },
     scripts=[
         'cloud-init/seed-cloud-init.sh',
-        'fedora/build-fedora-liveboot.sh',
+        'fedora/build-rpm-liveboot.sh',
         'ubuntu/patch-ubuntu-image.sh',
     ],
     package_data={
         'liveboot': [
             'templates/cloud-init-template.yaml.j2',
         ],
     },
```

