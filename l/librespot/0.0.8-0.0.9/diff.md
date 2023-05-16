# Comparing `tmp/librespot-0.0.8.tar.gz` & `tmp/librespot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librespot-0.0.8.tar", last modified: Thu Apr 13 12:09:04 2023, max compression
+gzip compressed data, was "librespot-0.0.9.tar", last modified: Tue May 16 22:00:38 2023, max compression
```

## Comparing `librespot-0.0.8.tar` & `librespot-0.0.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.835367 librespot-0.0.8/
--rw-rw-rw-   0        0        0    11572 2023-04-12 21:59:13.000000 librespot-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     3988 2023-04-13 12:09:04.834296 librespot-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3561 2023-04-12 21:59:13.000000 librespot-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.721266 librespot-0.0.8/librespot/
--rw-rw-rw-   0        0        0     1168 2023-04-13 12:08:08.000000 librespot-0.0.8/librespot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.746770 librespot-0.0.8/librespot/audio/
--rw-rw-rw-   0        0        0    36315 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/audio/__init__.py
--rw-rw-rw-   0        0        0     2897 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/audio/decoders.py
--rw-rw-rw-   0        0        0     1714 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/audio/decrypt.py
--rw-rw-rw-   0        0        0     1160 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/audio/format.py
--rw-rw-rw-   0        0        0     5621 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/audio/storage.py
--rw-rw-rw-   0        0        0      378 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/cache.py
--rw-rw-rw-   0        0        0    73074 2023-04-12 22:00:44.000000 librespot-0.0.8/librespot/core.py
--rw-rw-rw-   0        0        0    13141 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/crypto.py
--rw-rw-rw-   0        0        0      390 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/dealer.py
--rw-rw-rw-   0        0        0    14068 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/mercury.py
--rw-rw-rw-   0        0        0     8711 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/metadata.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.807513 librespot-0.0.8/librespot/proto/
--rw-rw-rw-   0        0        0    69584 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Authentication_pb2.py
--rw-rw-rw-   0        0        0     2965 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/CanvazMeta_pb2.py
--rw-rw-rw-   0        0        0    19169 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Canvaz_pb2.py
--rw-rw-rw-   0        0        0     6425 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/ClientToken_pb2.py
--rw-rw-rw-   0        0        0    83348 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Connect_pb2.py
--rw-rw-rw-   0        0        0     3061 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Connectivity_pb2.py
--rw-rw-rw-   0        0        0     8152 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/ContextPage_pb2.py
--rw-rw-rw-   0        0        0     7395 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/ContextPlayerOptions_pb2.py
--rw-rw-rw-   0        0        0     7197 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/ContextTrack_pb2.py
--rw-rw-rw-   0        0        0     8845 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Context_pb2.py
--rw-rw-rw-   0        0        0     5095 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/ExplicitContentPubsub_pb2.py
--rw-rw-rw-   0        0        0    87983 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Keyexchange_pb2.py
--rw-rw-rw-   0        0        0    20962 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Mercury_pb2.py
--rw-rw-rw-   0        0        0   132205 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Metadata_pb2.py
--rw-rw-rw-   0        0        0     6729 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/PlayOrigin_pb2.py
--rw-rw-rw-   0        0        0     5556 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Playback_pb2.py
--rw-rw-rw-   0        0        0    67514 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Player_pb2.py
--rw-rw-rw-   0        0        0   108912 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Playlist4External_pb2.py
--rw-rw-rw-   0        0        0    16084 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/PlaylistAnnotate3_pb2.py
--rw-rw-rw-   0        0        0     3662 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Pubsub_pb2.py
--rw-rw-rw-   0        0        0     3413 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Queue_pb2.py
--rw-rw-rw-   0        0        0    17651 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Restrictions_pb2.py
--rw-rw-rw-   0        0        0     5352 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Session_pb2.py
--rw-rw-rw-   0        0        0     5527 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/StorageResolve_pb2.py
--rw-rw-rw-   0        0        0     6353 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/TransferState_pb2.py
--rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.809535 librespot-0.0.8/librespot/proto/spotify/
--rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.810677 librespot-0.0.8/librespot/proto/spotify/login5/
--rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.818124 librespot-0.0.8/librespot/proto/spotify/login5/v3/
--rw-rw-rw-   0        0        0     3230 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/ClientInfo_pb2.py
--rw-rw-rw-   0        0        0    35170 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/Login5_pb2.py
--rw-rw-rw-   0        0        0     8963 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/UserInfo_pb2.py
--rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.823603 librespot-0.0.8/librespot/proto/spotify/login5/v3/challenges/
--rw-rw-rw-   0        0        0     7597 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/challenges/Code_pb2.py
--rw-rw-rw-   0        0        0     6086 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/challenges/Hashcash_pb2.py
--rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/challenges/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.827207 librespot-0.0.8/librespot/proto/spotify/login5/v3/credentials/
--rw-rw-rw-   0        0        0    16339 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/credentials/Credentials_pb2.py
--rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/credentials/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.831175 librespot-0.0.8/librespot/proto/spotify/login5/v3/identifiers/
--rw-rw-rw-   0        0        0     4132 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/identifiers/Identifiers.py
--rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/identifiers/__init__.py
--rw-rw-rw-   0        0        0     2668 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/structure.py
--rw-rw-rw-   0        0        0     3876 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/util.py
--rw-rw-rw-   0        0        0    14135 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/zeroconf.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.735839 librespot-0.0.8/librespot.egg-info/
--rw-rw-rw-   0        0        0     3988 2023-04-13 12:09:04.000000 librespot-0.0.8/librespot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2156 2023-04-13 12:09:04.000000 librespot-0.0.8/librespot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 12:09:04.000000 librespot-0.0.8/librespot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2023-04-13 12:09:04.000000 librespot-0.0.8/librespot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-13 12:09:04.000000 librespot-0.0.8/librespot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.832256 librespot-0.0.8/librespot_player/
--rw-rw-rw-   0        0        0     7643 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot_player/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-13 12:09:04.835888 librespot-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      820 2023-04-13 12:08:08.000000 librespot-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:00:38.565857 librespot-0.0.9/
+-rw-rw-rw-   0        0        0    11572 2023-04-12 21:59:13.000000 librespot-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3988 2023-05-16 22:00:38.564430 librespot-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3561 2023-04-12 21:59:13.000000 librespot-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 22:00:38.471093 librespot-0.0.9/librespot/
+-rw-rw-rw-   0        0        0     1168 2023-05-16 21:58:25.000000 librespot-0.0.9/librespot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:00:38.490551 librespot-0.0.9/librespot/audio/
+-rw-rw-rw-   0        0        0    36315 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/audio/__init__.py
+-rw-rw-rw-   0        0        0     2897 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/audio/decoders.py
+-rw-rw-rw-   0        0        0     1714 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/audio/decrypt.py
+-rw-rw-rw-   0        0        0     1160 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/audio/format.py
+-rw-rw-rw-   0        0        0     5621 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/audio/storage.py
+-rw-rw-rw-   0        0        0      378 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/cache.py
+-rw-rw-rw-   0        0        0    73074 2023-04-12 22:00:44.000000 librespot-0.0.9/librespot/core.py
+-rw-rw-rw-   0        0        0    13141 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/crypto.py
+-rw-rw-rw-   0        0        0      390 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/dealer.py
+-rw-rw-rw-   0        0        0    14068 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/mercury.py
+-rw-rw-rw-   0        0        0     8711 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/metadata.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:00:38.541860 librespot-0.0.9/librespot/proto/
+-rw-rw-rw-   0        0        0    69584 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Authentication_pb2.py
+-rw-rw-rw-   0        0        0     2965 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/CanvazMeta_pb2.py
+-rw-rw-rw-   0        0        0    19169 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Canvaz_pb2.py
+-rw-rw-rw-   0        0        0     6425 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/ClientToken_pb2.py
+-rw-rw-rw-   0        0        0    83348 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Connect_pb2.py
+-rw-rw-rw-   0        0        0     3061 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Connectivity_pb2.py
+-rw-rw-rw-   0        0        0     8152 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/ContextPage_pb2.py
+-rw-rw-rw-   0        0        0     7395 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/ContextPlayerOptions_pb2.py
+-rw-rw-rw-   0        0        0     7197 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/ContextTrack_pb2.py
+-rw-rw-rw-   0        0        0     8845 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Context_pb2.py
+-rw-rw-rw-   0        0        0     5095 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/ExplicitContentPubsub_pb2.py
+-rw-rw-rw-   0        0        0    87983 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Keyexchange_pb2.py
+-rw-rw-rw-   0        0        0    20962 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Mercury_pb2.py
+-rw-rw-rw-   0        0        0   132205 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Metadata_pb2.py
+-rw-rw-rw-   0        0        0     6729 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/PlayOrigin_pb2.py
+-rw-rw-rw-   0        0        0     5556 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Playback_pb2.py
+-rw-rw-rw-   0        0        0    67514 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Player_pb2.py
+-rw-rw-rw-   0        0        0   108912 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Playlist4External_pb2.py
+-rw-rw-rw-   0        0        0    16084 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/PlaylistAnnotate3_pb2.py
+-rw-rw-rw-   0        0        0     3662 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Pubsub_pb2.py
+-rw-rw-rw-   0        0        0     3413 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Queue_pb2.py
+-rw-rw-rw-   0        0        0    17651 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Restrictions_pb2.py
+-rw-rw-rw-   0        0        0     5352 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/Session_pb2.py
+-rw-rw-rw-   0        0        0     5527 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/StorageResolve_pb2.py
+-rw-rw-rw-   0        0        0     6353 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/TransferState_pb2.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:00:38.543218 librespot-0.0.9/librespot/proto/spotify/
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:00:38.544394 librespot-0.0.9/librespot/proto/spotify/login5/
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/login5/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:00:38.550548 librespot-0.0.9/librespot/proto/spotify/login5/v3/
+-rw-rw-rw-   0        0        0     3230 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/login5/v3/ClientInfo_pb2.py
+-rw-rw-rw-   0        0        0    35170 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/login5/v3/Login5_pb2.py
+-rw-rw-rw-   0        0        0     8963 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/login5/v3/UserInfo_pb2.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/login5/v3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:00:38.555259 librespot-0.0.9/librespot/proto/spotify/login5/v3/challenges/
+-rw-rw-rw-   0        0        0     7597 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/login5/v3/challenges/Code_pb2.py
+-rw-rw-rw-   0        0        0     6086 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/login5/v3/challenges/Hashcash_pb2.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/login5/v3/challenges/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:00:38.558844 librespot-0.0.9/librespot/proto/spotify/login5/v3/credentials/
+-rw-rw-rw-   0        0        0    16339 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/login5/v3/credentials/Credentials_pb2.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/login5/v3/credentials/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:00:38.561752 librespot-0.0.9/librespot/proto/spotify/login5/v3/identifiers/
+-rw-rw-rw-   0        0        0     4132 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/login5/v3/identifiers/Identifiers.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/proto/spotify/login5/v3/identifiers/__init__.py
+-rw-rw-rw-   0        0        0     2668 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/structure.py
+-rw-rw-rw-   0        0        0     3876 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/util.py
+-rw-rw-rw-   0        0        0    14135 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot/zeroconf.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:00:38.481790 librespot-0.0.9/librespot.egg-info/
+-rw-rw-rw-   0        0        0     3988 2023-05-16 22:00:38.000000 librespot-0.0.9/librespot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2156 2023-05-16 22:00:38.000000 librespot-0.0.9/librespot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 22:00:38.000000 librespot-0.0.9/librespot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2023-05-16 22:00:38.000000 librespot-0.0.9/librespot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-16 22:00:38.000000 librespot-0.0.9/librespot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 22:00:38.562898 librespot-0.0.9/librespot_player/
+-rw-rw-rw-   0        0        0     7643 2023-04-12 21:59:13.000000 librespot-0.0.9/librespot_player/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-16 22:00:38.565857 librespot-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      820 2023-05-16 22:00:06.000000 librespot-0.0.9/setup.py
```

### Comparing `librespot-0.0.8/LICENSE.txt` & `librespot-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/PKG-INFO` & `librespot-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librespot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Open Source Spotify Client
 Home-page: https://github.com/kokarare1212/librespot-python
 Author: kokarare1212
 License: Apache-2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Multimedia :: Sound/Audio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: librespot Version: 0.0.8 Summary: Open Source
+Metadata-Version: 2.1 Name: librespot Version: 0.0.9 Summary: Open Source
 Spotify Client Home-page: https://github.com/kokarare1212/librespot-python
 Author: kokarare1212 License: Apache-2.0 Classifier: Development Status :: 1 -
 Planning Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Multimedia :: Sound/Audio Description-Content-Type: text/
 markdown License-File: LICENSE.txt ![License](https://img.shields.io/github/
 license/kokarare1212/librespot-python.svg) ![Stars](https://img.shields.io/
 github/stars/kokarare1212/librespot-python.svg) ![Forks](https://
```

### Comparing `librespot-0.0.8/README.md` & `librespot-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/__init__.py` & `librespot-0.0.9/librespot/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from librespot.crypto import DiffieHellman
 from librespot.proto.Keyexchange_pb2 import BuildInfo, Platform, Product, ProductFlags
 from librespot.structure import Closeable, Runnable
 import platform
 
 
 class Version:
-    version_name = "0.0.8"
+    version_name = "0.0.9"
 
     @staticmethod
     def platform() -> Platform:
         if platform.system() == "Windows":
             return Platform.PLATFORM_WIN32_X86
         if platform.system() == "Darwin":
             return Platform.PLATFORM_OSX_X86
@@ -27,8 +27,8 @@
                "; " + platform.system()
 
     @staticmethod
     def standard_build_info() -> BuildInfo:
         return BuildInfo(product=Product.PRODUCT_CLIENT,
                          product_flags=[ProductFlags.PRODUCT_FLAG_NONE],
                          platform=Version.platform(),
-                         version=112800721)
+                         version=117300517)
```

### Comparing `librespot-0.0.8/librespot/audio/__init__.py` & `librespot-0.0.9/librespot/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/audio/decoders.py` & `librespot-0.0.9/librespot/audio/decoders.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/audio/decrypt.py` & `librespot-0.0.9/librespot/audio/decrypt.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/audio/format.py` & `librespot-0.0.9/librespot/audio/format.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/audio/storage.py` & `librespot-0.0.9/librespot/audio/storage.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/core.py` & `librespot-0.0.9/librespot/core.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/crypto.py` & `librespot-0.0.9/librespot/crypto.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/mercury.py` & `librespot-0.0.9/librespot/mercury.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/metadata.py` & `librespot-0.0.9/librespot/metadata.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Authentication_pb2.py` & `librespot-0.0.9/librespot/proto/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/CanvazMeta_pb2.py` & `librespot-0.0.9/librespot/proto/CanvazMeta_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Canvaz_pb2.py` & `librespot-0.0.9/librespot/proto/Canvaz_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/ClientToken_pb2.py` & `librespot-0.0.9/librespot/proto/ClientToken_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Connect_pb2.py` & `librespot-0.0.9/librespot/proto/Connect_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Connectivity_pb2.py` & `librespot-0.0.9/librespot/proto/Connectivity_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/ContextPage_pb2.py` & `librespot-0.0.9/librespot/proto/ContextPage_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/ContextPlayerOptions_pb2.py` & `librespot-0.0.9/librespot/proto/ContextPlayerOptions_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/ContextTrack_pb2.py` & `librespot-0.0.9/librespot/proto/ContextTrack_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Context_pb2.py` & `librespot-0.0.9/librespot/proto/Context_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/ExplicitContentPubsub_pb2.py` & `librespot-0.0.9/librespot/proto/ExplicitContentPubsub_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Keyexchange_pb2.py` & `librespot-0.0.9/librespot/proto/Keyexchange_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Mercury_pb2.py` & `librespot-0.0.9/librespot/proto/Mercury_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Metadata_pb2.py` & `librespot-0.0.9/librespot/proto/Metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/PlayOrigin_pb2.py` & `librespot-0.0.9/librespot/proto/PlayOrigin_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Playback_pb2.py` & `librespot-0.0.9/librespot/proto/Playback_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Player_pb2.py` & `librespot-0.0.9/librespot/proto/Player_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Playlist4External_pb2.py` & `librespot-0.0.9/librespot/proto/Playlist4External_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/PlaylistAnnotate3_pb2.py` & `librespot-0.0.9/librespot/proto/PlaylistAnnotate3_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Pubsub_pb2.py` & `librespot-0.0.9/librespot/proto/Pubsub_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Queue_pb2.py` & `librespot-0.0.9/librespot/proto/Queue_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Restrictions_pb2.py` & `librespot-0.0.9/librespot/proto/Restrictions_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/Session_pb2.py` & `librespot-0.0.9/librespot/proto/Session_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/StorageResolve_pb2.py` & `librespot-0.0.9/librespot/proto/StorageResolve_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/TransferState_pb2.py` & `librespot-0.0.9/librespot/proto/TransferState_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/spotify/login5/v3/ClientInfo_pb2.py` & `librespot-0.0.9/librespot/proto/spotify/login5/v3/ClientInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/spotify/login5/v3/Login5_pb2.py` & `librespot-0.0.9/librespot/proto/spotify/login5/v3/Login5_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/spotify/login5/v3/UserInfo_pb2.py` & `librespot-0.0.9/librespot/proto/spotify/login5/v3/UserInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/spotify/login5/v3/challenges/Code_pb2.py` & `librespot-0.0.9/librespot/proto/spotify/login5/v3/challenges/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/spotify/login5/v3/challenges/Hashcash_pb2.py` & `librespot-0.0.9/librespot/proto/spotify/login5/v3/challenges/Hashcash_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/spotify/login5/v3/credentials/Credentials_pb2.py` & `librespot-0.0.9/librespot/proto/spotify/login5/v3/credentials/Credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/proto/spotify/login5/v3/identifiers/Identifiers.py` & `librespot-0.0.9/librespot/proto/spotify/login5/v3/identifiers/Identifiers.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/structure.py` & `librespot-0.0.9/librespot/structure.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/util.py` & `librespot-0.0.9/librespot/util.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot/zeroconf.py` & `librespot-0.0.9/librespot/zeroconf.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot.egg-info/PKG-INFO` & `librespot-0.0.9/librespot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librespot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Open Source Spotify Client
 Home-page: https://github.com/kokarare1212/librespot-python
 Author: kokarare1212
 License: Apache-2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Multimedia :: Sound/Audio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: librespot Version: 0.0.8 Summary: Open Source
+Metadata-Version: 2.1 Name: librespot Version: 0.0.9 Summary: Open Source
 Spotify Client Home-page: https://github.com/kokarare1212/librespot-python
 Author: kokarare1212 License: Apache-2.0 Classifier: Development Status :: 1 -
 Planning Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Multimedia :: Sound/Audio Description-Content-Type: text/
 markdown License-File: LICENSE.txt ![License](https://img.shields.io/github/
 license/kokarare1212/librespot-python.svg) ![Stars](https://img.shields.io/
 github/stars/kokarare1212/librespot-python.svg) ![Forks](https://
```

### Comparing `librespot-0.0.8/librespot.egg-info/SOURCES.txt` & `librespot-0.0.9/librespot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/librespot_player/__init__.py` & `librespot-0.0.9/librespot_player/__init__.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.8/setup.py` & `librespot-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name="librespot",
-                 version="0.0.8",
+                 version="0.0.9",
                  description="Open Source Spotify Client",
                  long_description=open("README.md").read(),
                  long_description_content_type="text/markdown",
                  author="kokarare1212",
                  url="https://github.com/kokarare1212/librespot-python",
                  license="Apache-2.0",
                  packages=setuptools.find_packages("."),
```

