# Comparing `tmp/EthTx-0.3.8.tar.gz` & `tmp/EthTx-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EthTx-0.3.8.tar", last modified: Fri Jan 14 12:23:38 2022, max compression
+gzip compressed data, was "EthTx-0.3.9.tar", last modified: Mon Feb  7 11:47:04 2022, max compression
```

## Comparing `EthTx-0.3.8.tar` & `EthTx-0.3.9.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)     7828 2022-01-14 12:21:54.000000 EthTx-0.3.8/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.545425 EthTx-0.3.8/EthTx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6479 2022-01-14 12:23:38.000000 EthTx-0.3.8/EthTx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3542 2022-01-14 12:23:38.000000 EthTx-0.3.8/EthTx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-14 12:23:38.000000 EthTx-0.3.8/EthTx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-01-14 12:23:38.000000 EthTx-0.3.8/EthTx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-01-14 12:23:38.000000 EthTx-0.3.8/EthTx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10141 2022-01-14 12:21:54.000000 EthTx-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-01-14 12:21:54.000000 EthTx-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6479 2022-01-14 12:23:38.553425 EthTx-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5945 2022-01-14 12:21:54.000000 EthTx-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.545425 EthTx-0.3.8/ethtx/
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.545425 EthTx-0.3.8/ethtx/decoders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.545425 EthTx-0.3.8/ethtx/decoders/abi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/abi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/abi/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/abi/balances.py
--rw-r--r--   0 runner    (1001) docker     (121)     9357 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/abi/calls.py
--rw-r--r--   0 runner    (1001) docker     (121)     6736 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/abi/decoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     5618 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/abi/events.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.549425 EthTx-0.3.8/ethtx/decoders/abi/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/abi/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4407 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/abi/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4567 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/abi/transfers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6022 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/decoder_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.549425 EthTx-0.3.8/ethtx/decoders/decoders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14343 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/decoders/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     3706 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/decoders/semantics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.549425 EthTx-0.3.8/ethtx/decoders/semantic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/semantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/semantic/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/semantic/balances.py
--rw-r--r--   0 runner    (1001) docker     (121)     6106 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/semantic/calls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4447 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/semantic/decoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6820 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/semantic/events.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.549425 EthTx-0.3.8/ethtx/decoders/semantic/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/semantic/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6798 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/semantic/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/semantic/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/decoders/semantic/transfers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5436 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/ethtx.py
--rw-r--r--   0 runner    (1001) docker     (121)     2261 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.549425 EthTx-0.3.8/ethtx/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/models/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2901 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/models/decoded_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3587 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/models/objects_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6417 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/models/semantics_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5501 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/models/w3_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.549425 EthTx-0.3.8/ethtx/providers/
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/ens_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.549425 EthTx-0.3.8/ethtx/providers/etherscan/
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/etherscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/etherscan/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     6497 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/etherscan/contracts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/etherscan/etherscan_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.549425 EthTx-0.3.8/ethtx/providers/node/
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/node/connection_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/node/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.549425 EthTx-0.3.8/ethtx/providers/semantic_providers/
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/semantic_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/semantic_providers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/semantic_providers/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     3899 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/semantic_providers/database.py
--rw-r--r--   0 runner    (1001) docker     (121)    17384 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/semantic_providers/repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     4771 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/signature_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.549425 EthTx-0.3.8/ethtx/providers/static/
--rw-r--r--   0 runner    (1001) docker     (121)     8794 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/static/tracer.js
--rw-r--r--   0 runner    (1001) docker     (121)    18922 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/providers/web3_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/ethtx/semantics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/ethtx/semantics/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5802 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols/anonymous.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/ethtx/semantics/protocols/maker/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols/maker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1939 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols/maker/cdp_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols/maker/dai.py
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols/maker/dai_join.py
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols/maker/ds_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols/maker/gem_join.py
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols/maker/jug.py
--rw-r--r--   0 runner    (1001) docker     (121)     3772 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols/maker/vat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/ethtx/semantics/protocols/wrappers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols/wrappers/weth.py
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/protocols_router.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/ethtx/semantics/rollups/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/rollups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3670 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/rollups/aztec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/router.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/ethtx/semantics/solidity/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/solidity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3548 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/solidity/precompiles.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/ethtx/semantics/standards/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/standards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/standards/eip1969.py
--rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/standards/erc20.py
--rw-r--r--   0 runner    (1001) docker     (121)     8722 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/standards/erc721.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/ethtx/semantics/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/semantics/utilities/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/ethtx/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/utils/attr_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/utils/measurable.py
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-01-14 12:21:54.000000 EthTx-0.3.8/ethtx/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-01-14 12:21:54.000000 EthTx-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-01-14 12:23:38.557425 EthTx-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-01-14 12:21:54.000000 EthTx-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.545425 EthTx-0.3.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3816 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/mocks/web3provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/tests/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6874 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/models/decoded_model_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/models/mock.py
--rw-r--r--   0 runner    (1001) docker     (121)     4125 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/models/objects_model_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3191 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/models/semantics_model_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5735 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/models/w3_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/tests/providers/node/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/providers/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/providers/node/connection_base_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/providers/node/pool_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 12:23:38.553425 EthTx-0.3.8/tests/providers/semantic_providers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/providers/semantic_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2670 2022-01-14 12:21:54.000000 EthTx-0.3.8/tests/providers/semantic_providers/semantics_database_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.268194 EthTx-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     8517 2022-02-07 11:44:41.000000 EthTx-0.3.9/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.256194 EthTx-0.3.9/EthTx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6606 2022-02-07 11:47:04.000000 EthTx-0.3.9/EthTx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3533 2022-02-07 11:47:04.000000 EthTx-0.3.9/EthTx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 11:47:04.000000 EthTx-0.3.9/EthTx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-02-07 11:47:04.000000 EthTx-0.3.9/EthTx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-07 11:47:04.000000 EthTx-0.3.9/EthTx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10141 2022-02-07 11:44:41.000000 EthTx-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-02-07 11:44:41.000000 EthTx-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6606 2022-02-07 11:47:04.268194 EthTx-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2022-02-07 11:44:41.000000 EthTx-0.3.9/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (121)     6072 2022-02-07 11:44:41.000000 EthTx-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.256194 EthTx-0.3.9/ethtx/
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.256194 EthTx-0.3.9/ethtx/decoders/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.260194 EthTx-0.3.9/ethtx/decoders/abi/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/abi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/abi/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/abi/balances.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9357 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/abi/calls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6736 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/abi/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5618 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/abi/events.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.260194 EthTx-0.3.9/ethtx/decoders/abi/helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/abi/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4407 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/abi/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4567 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/abi/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6022 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/decoder_service.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.260194 EthTx-0.3.9/ethtx/decoders/decoders/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14343 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/decoders/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3706 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/decoders/semantics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.260194 EthTx-0.3.9/ethtx/decoders/semantic/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/semantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2536 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/semantic/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/semantic/balances.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6017 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/semantic/calls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4447 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/semantic/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6820 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/semantic/events.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.260194 EthTx-0.3.9/ethtx/decoders/semantic/helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/semantic/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6798 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/semantic/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/semantic/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/decoders/semantic/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5436 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/ethtx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2261 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.260194 EthTx-0.3.9/ethtx/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/models/_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/models/decoded_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3597 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/models/objects_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6417 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/models/semantics_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5501 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/models/w3_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.260194 EthTx-0.3.9/ethtx/providers/
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/ens_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.264194 EthTx-0.3.9/ethtx/providers/etherscan/
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/etherscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/etherscan/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6497 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/etherscan/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/etherscan/etherscan_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.264194 EthTx-0.3.9/ethtx/providers/node/
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/node/connection_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/node/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.264194 EthTx-0.3.9/ethtx/providers/semantic_providers/
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/semantic_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/semantic_providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/semantic_providers/const.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3899 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/semantic_providers/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17146 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/semantic_providers/repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4771 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/signature_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.264194 EthTx-0.3.9/ethtx/providers/static/
+-rw-r--r--   0 runner    (1001) docker     (121)     8794 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/static/tracer.js
+-rw-r--r--   0 runner    (1001) docker     (121)    19007 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/providers/web3_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.264194 EthTx-0.3.9/ethtx/semantics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.264194 EthTx-0.3.9/ethtx/semantics/protocols/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5802 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols/anonymous.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.264194 EthTx-0.3.9/ethtx/semantics/protocols/maker/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols/maker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1939 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols/maker/cdp_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols/maker/dai.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols/maker/dai_join.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols/maker/ds_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols/maker/gem_join.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols/maker/jug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3772 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols/maker/vat.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.264194 EthTx-0.3.9/ethtx/semantics/protocols/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols/wrappers/weth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/protocols_router.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.264194 EthTx-0.3.9/ethtx/semantics/rollups/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/rollups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3670 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/rollups/aztec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/router.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.264194 EthTx-0.3.9/ethtx/semantics/solidity/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/solidity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3548 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/solidity/precompiles.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.268194 EthTx-0.3.9/ethtx/semantics/standards/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/standards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/standards/eip1969.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/standards/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8722 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/standards/erc721.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.268194 EthTx-0.3.9/ethtx/semantics/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/semantics/utilities/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.268194 EthTx-0.3.9/ethtx/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/utils/attr_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/utils/measurable.py
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-02-07 11:44:41.000000 EthTx-0.3.9/ethtx/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-02-07 11:47:04.268194 EthTx-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3553 2022-02-07 11:44:41.000000 EthTx-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.256194 EthTx-0.3.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.268194 EthTx-0.3.9/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3816 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/mocks/web3provider.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.268194 EthTx-0.3.9/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6874 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/models/decoded_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/models/mock.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4125 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/models/objects_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3191 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/models/semantics_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5735 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/models/w3_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.268194 EthTx-0.3.9/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.268194 EthTx-0.3.9/tests/providers/node/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/providers/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/providers/node/connection_base_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/providers/node/pool_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:47:04.268194 EthTx-0.3.9/tests/providers/semantic_providers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/providers/semantic_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2670 2022-02-07 11:44:41.000000 EthTx-0.3.9/tests/providers/semantic_providers/semantics_database_test.py
```

### Comparing `EthTx-0.3.8/CHANGELOG.md` & `EthTx-0.3.9/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
+## 0.3.9 - 2022-02-02
+
+### Added
+- Add some static types and LRU caches for proxy guessing and web3 [#112](https://github.com/EthTx/ethtx/pull/112)
+
+### Changed
+- Updated old ***Features*** section in `README.md` [#114](https://github.com/EthTx/ethtx/pull/114)
+- Removed *requirements.txt* file. Builds will use Pipfile from now on [#114](https://github.com/EthTx/ethtx/pull/114)
+
+### Fixed
+- `to_address` field in Call/DecodedCall is optional now [#111](https://github.com/EthTx/ethtx/pull/111)
+- Fixed `web3` dependencies [#114](https://github.com/EthTx/ethtx/pull/114)
+- Delete bunch of invalid if conditions when checking for semantic [#113](https://github.com/EthTx/ethtx/pull/113)
+
+
 ## 0.3.8 - 2022-01-14
 ### Added
 - Added option to disable refreshing of addresses in ENS for existing semantics [#106](https://github.com/EthTx/ethtx/pull/106)
 - Increased and added more lru_caches in different providers [#105](https://github.com/EthTx/ethtx/pull/105)
 
 ### Changed
 - Python version bumped to 3.9 [#103](https://github.com/EthTx/ethtx/pull/103)
```

### Comparing `EthTx-0.3.8/EthTx.egg-info/PKG-INFO` & `EthTx-0.3.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: EthTx
-Version: 0.3.8
-Summary: EthTx transaction decoder.
-Home-page: https://github.com/EthTx/ethtx
-Author: Karol Chojnowski, Tomasz Mierzwa, Piotr Rudnik
-Author-email: karol@tfi.team, tomek@tfi.team, piotr.rudnik@tfi.team
-License: Apache-2.0 License
-Platform: UNKNOWN
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 <h1 align='center' style='border-bottom: none'>
   <p>EthTx - Ethereum transactions decoder </p>
 </h1>
 
 <p align="center">
 <a target="_blank">
     <img src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg" alt="Python">
@@ -62,23 +45,23 @@
 
 ```python
 from ethtx import EthTx, EthTxConfig
 from ethtx.models.decoded_model import DecodedTransaction
 
 ethtx_config = EthTxConfig(
     mongo_connection_string="mongomock://localhost/ethtx",  ##MongoDB connection string,
-    etherscan_api_key = "",  ##Etherscan API key,
-    web3nodes = {
-                "mainnet": {
-                    "hook": "_Geth_archive_node_URL_", # multiple nodes supported, separate them with comma
-                    "poa": _POA_chain_indicator_  # represented by bool value
-                }
-            },
-            default_chain = "mainnet",
-            etherscan_urls = {"mainnet": "https://api.etherscan.io/api",},
+    etherscan_api_key="",  ##Etherscan API key,
+    web3nodes={
+        "mainnet": {
+            "hook": "_Geth_archive_node_URL_",  # multiple nodes supported, separate them with comma
+            "poa": _POA_chain_indicator_  # represented by bool value
+        }
+    },
+    default_chain="mainnet",
+    etherscan_urls={"mainnet": "https://api.etherscan.io/api", },
 )
 
 ethtx = EthTx.initialize(ethtx_config)
 transaction: DecodedTransaction = ethtx.decoders.decode_transaction(
     '0x50051e0a6f216ab9484c2080001c7e12d5138250acee1f4b7c725b8fb6bb922d')
 ```
 
@@ -95,62 +78,92 @@
 from ethtx.models.w3_model import W3Transaction, W3Block, W3Receipt, W3CallTree
 
 # read raw transaction data directly from the node
 w3transaction: W3Transaction = web3provider.get_transaction(
     '0x50051e0a6f216ab9484c2080001c7e12d5138250acee1f4b7c725b8fb6bb922d')
 w3block: W3Block = web3provider.get_block(w3transaction.blockNumber)
 w3receipt: W3Receipt = web3provider.get_receipt(w3transaction.hash.hex())
-w3calls: W3CallTree = web3provider.get_calls(w3transaction.hash.hex()
+w3calls: W3CallTree = web3provider.get_calls(w3transaction.hash.hex())
 ```
 
 2. ABI decoding:
 
 ```python
-from ethtx.models.objects_model import Transaction, Event, Call
-from ethtx.models.decoded_model import DecodedEvent, DecodedCall, DecodedTransfer, DecodedBalance
+from ethtx.models.decoded_model import (
+    DecodedTransfer,
+    DecodedBalance,
+    DecodedEvent, DecodedCall,
+)
+from ethtx.models.objects_model import Transaction, Event, Block, Call
 
 # read the raw transaction from the node
 transaction: Transaction = web3provider.get_full_transaction(
     '0x50051e0a6f216ab9484c2080001c7e12d5138250acee1f4b7c725b8fb6bb922d')
 
+# get proxies used in the transaction
+proxies = ethtx.decoders.get_proxies(transaction.root_call, 'mainnet')
+
+block: Block = Block.from_raw(
+    w3block=web3provider.get_block(
+        transaction.metadata.block_number
+    ),
+    chain_id='mainnet',
+)
+
 # decode transaction components
-abi_decoded_events: List[Event] = ethtx.decoders.abi_decoder.decode_events(transaction.events, transaction.metadata)
-abi_decoded_calls: DecodedCall = ethtx.decoders.abi_decoder.decode_calls(transaction.root_call, transaction.metadata)
-abi_decoded_transfers: List[DecodedTransfer] = ethtx.decoders.abi_decoder.decode_transfers(abi_decoded_calls,
-                                                                                           abi_decoded_events)
-abi_decoded_balances: List[DecodedBalance] = ethtx.decoders.abi_decoder.decode_balances(abi_decoded_transfers)
+abi_decoded_events: List[Event] = ethtx.decoders.abi_decoder.decode_events(
+    transaction.events, block.metadata, transaction.metadata
+)
+abi_decoded_calls: DecodedCall = ethtx.decoders.abi_decoder.decode_calls(transaction.root_call, block.metadata,
+                                                                         transaction.metadata, proxies)
+abi_decoded_transfers: List[
+    DecodedTransfer
+] = ethtx.decoders.abi_decoder.decode_transfers(abi_decoded_calls, abi_decoded_events)
+abi_decoded_balances: List[DecodedBalance] = ethtx.decoders.abi_decoder.decode_balances(
+    abi_decoded_transfers
+)
 
 # decode a single event
 raw_event: Event = transaction.events[3]
-abi_decoded_event: DecodedEvent = ethtx.decoders.abi_decoder.decode_event(raw_event, transaction.metadata)
+abi_decoded_event: DecodedEvent = ethtx.decoders.abi_decoder.decode_event(raw_event, block.metadata,
+                                                                          transaction.metadata)
 
 # decode a single call
-raw_call: Call = transaction.root_call.subcalls[3].subcalls[2]
-abi_decoded_call: DecodedCall = ethtx.decoders.abi_decoder.decode_call(raw_call, transaction.metadata)
+raw_call: Call = transaction.root_call.subcalls[0]
+abi_decoded_call: DecodedCall = ethtx.decoders.abi_decoder.decode_call(raw_call, block.metadata, transaction.metadata,
+                                                                       proxies)
 ```
 
 3. Semantic decoding:
 
 ```python
 from ethtx.models.decoded_model import DecodedTransactionMetadata
 
-# get proxies used in the transaction
-proxies = ethtx.decoders.get_proxies(transaction.root_call, chain_id)
-
 # semantically decode transaction components
-decoded_metadata: DecodedTransactionMetadata = ethtx.decoders.semantic_decoder.decode_metadata(block.metadata,
-                                                                                               transaction.metadata,
-                                                                                               chain_id)
-decoded_events: List[DecodedEvent] = ethtx.decoders.semantic_decoder.decode_events(abi_decoded_events, decoded_metadata,
-                                                                                   proxies)
+decoded_metadata: DecodedTransactionMetadata = (
+    ethtx.decoders.semantic_decoder.decode_metadata(
+        block.metadata, transaction.metadata, 'mainnet'
+    )
+)
+decoded_events: List[DecodedEvent] = ethtx.decoders.semantic_decoder.decode_events(
+    abi_decoded_events, decoded_metadata, proxies
+)
+
 decoded_calls: Call = ethtx.decoders.semantic_decoder.decode_calls(abi_decoded_calls, decoded_metadata, proxies)
-decoded_transfers: List[DecodedTransfer] = ethtx.decoders.semantic_decoder.decode_transfers(abi_decoded_transfers)
-decoded_balances: List[DecodedBalance] = ethtx.decoders.semantic_decoder.decode_balances(abi_decoded_balances)
+decoded_transfers: List[
+    DecodedTransfer
+] = ethtx.decoders.semantic_decoder.decode_transfers(
+    abi_decoded_transfers, decoded_metadata
+)
+decoded_balances: List[
+    DecodedBalance
+] = ethtx.decoders.semantic_decoder.decode_balances(
+    abi_decoded_balances, decoded_metadata
+)
 
 # semantically decode a single event
 decoded_event: DecodedEvent = ethtx.decoders.semantic_decoder.decode_event(abi_decoded_events[0], decoded_metadata,
                                                                            proxies)
 # semantically decode a single call
-decoded_call: Call = ethtx.decoders.semantic_decoder.decode_call(abi_decoded_calls.subcalls[2].subcalls[0],
+decoded_call: Call = ethtx.decoders.semantic_decoder.decode_call(abi_decoded_calls.subcalls[0],
                                                                  decoded_metadata, proxies)
-```
-
+```
```

### Comparing `EthTx-0.3.8/EthTx.egg-info/SOURCES.txt` & `EthTx-0.3.9/EthTx.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
+Pipfile
 README.md
-requirements.txt
 setup.cfg
 setup.py
 EthTx.egg-info/PKG-INFO
 EthTx.egg-info/SOURCES.txt
 EthTx.egg-info/dependency_links.txt
 EthTx.egg-info/requires.txt
 EthTx.egg-info/top_level.txt
```

### Comparing `EthTx-0.3.8/LICENSE` & `EthTx-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/PKG-INFO` & `EthTx-0.3.9/EthTx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: EthTx
-Version: 0.3.8
+Version: 0.3.9
 Summary: EthTx transaction decoder.
 Home-page: https://github.com/EthTx/ethtx
 Author: Karol Chojnowski, Tomasz Mierzwa, Piotr Rudnik
 Author-email: karol@tfi.team, tomek@tfi.team, piotr.rudnik@tfi.team
 License: Apache-2.0 License
 Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <h1 align='center' style='border-bottom: none'>
   <p>EthTx - Ethereum transactions decoder </p>
@@ -62,23 +62,23 @@
 
 ```python
 from ethtx import EthTx, EthTxConfig
 from ethtx.models.decoded_model import DecodedTransaction
 
 ethtx_config = EthTxConfig(
     mongo_connection_string="mongomock://localhost/ethtx",  ##MongoDB connection string,
-    etherscan_api_key = "",  ##Etherscan API key,
-    web3nodes = {
-                "mainnet": {
-                    "hook": "_Geth_archive_node_URL_", # multiple nodes supported, separate them with comma
-                    "poa": _POA_chain_indicator_  # represented by bool value
-                }
-            },
-            default_chain = "mainnet",
-            etherscan_urls = {"mainnet": "https://api.etherscan.io/api",},
+    etherscan_api_key="",  ##Etherscan API key,
+    web3nodes={
+        "mainnet": {
+            "hook": "_Geth_archive_node_URL_",  # multiple nodes supported, separate them with comma
+            "poa": _POA_chain_indicator_  # represented by bool value
+        }
+    },
+    default_chain="mainnet",
+    etherscan_urls={"mainnet": "https://api.etherscan.io/api", },
 )
 
 ethtx = EthTx.initialize(ethtx_config)
 transaction: DecodedTransaction = ethtx.decoders.decode_transaction(
     '0x50051e0a6f216ab9484c2080001c7e12d5138250acee1f4b7c725b8fb6bb922d')
 ```
 
@@ -95,62 +95,93 @@
 from ethtx.models.w3_model import W3Transaction, W3Block, W3Receipt, W3CallTree
 
 # read raw transaction data directly from the node
 w3transaction: W3Transaction = web3provider.get_transaction(
     '0x50051e0a6f216ab9484c2080001c7e12d5138250acee1f4b7c725b8fb6bb922d')
 w3block: W3Block = web3provider.get_block(w3transaction.blockNumber)
 w3receipt: W3Receipt = web3provider.get_receipt(w3transaction.hash.hex())
-w3calls: W3CallTree = web3provider.get_calls(w3transaction.hash.hex()
+w3calls: W3CallTree = web3provider.get_calls(w3transaction.hash.hex())
 ```
 
 2. ABI decoding:
 
 ```python
-from ethtx.models.objects_model import Transaction, Event, Call
-from ethtx.models.decoded_model import DecodedEvent, DecodedCall, DecodedTransfer, DecodedBalance
+from ethtx.models.decoded_model import (
+    DecodedTransfer,
+    DecodedBalance,
+    DecodedEvent, DecodedCall,
+)
+from ethtx.models.objects_model import Transaction, Event, Block, Call
 
 # read the raw transaction from the node
 transaction: Transaction = web3provider.get_full_transaction(
     '0x50051e0a6f216ab9484c2080001c7e12d5138250acee1f4b7c725b8fb6bb922d')
 
+# get proxies used in the transaction
+proxies = ethtx.decoders.get_proxies(transaction.root_call, 'mainnet')
+
+block: Block = Block.from_raw(
+    w3block=web3provider.get_block(
+        transaction.metadata.block_number
+    ),
+    chain_id='mainnet',
+)
+
 # decode transaction components
-abi_decoded_events: List[Event] = ethtx.decoders.abi_decoder.decode_events(transaction.events, transaction.metadata)
-abi_decoded_calls: DecodedCall = ethtx.decoders.abi_decoder.decode_calls(transaction.root_call, transaction.metadata)
-abi_decoded_transfers: List[DecodedTransfer] = ethtx.decoders.abi_decoder.decode_transfers(abi_decoded_calls,
-                                                                                           abi_decoded_events)
-abi_decoded_balances: List[DecodedBalance] = ethtx.decoders.abi_decoder.decode_balances(abi_decoded_transfers)
+abi_decoded_events: List[Event] = ethtx.decoders.abi_decoder.decode_events(
+    transaction.events, block.metadata, transaction.metadata
+)
+abi_decoded_calls: DecodedCall = ethtx.decoders.abi_decoder.decode_calls(transaction.root_call, block.metadata,
+                                                                         transaction.metadata, proxies)
+abi_decoded_transfers: List[
+    DecodedTransfer
+] = ethtx.decoders.abi_decoder.decode_transfers(abi_decoded_calls, abi_decoded_events)
+abi_decoded_balances: List[DecodedBalance] = ethtx.decoders.abi_decoder.decode_balances(
+    abi_decoded_transfers
+)
 
 # decode a single event
 raw_event: Event = transaction.events[3]
-abi_decoded_event: DecodedEvent = ethtx.decoders.abi_decoder.decode_event(raw_event, transaction.metadata)
+abi_decoded_event: DecodedEvent = ethtx.decoders.abi_decoder.decode_event(raw_event, block.metadata,
+                                                                          transaction.metadata)
 
 # decode a single call
-raw_call: Call = transaction.root_call.subcalls[3].subcalls[2]
-abi_decoded_call: DecodedCall = ethtx.decoders.abi_decoder.decode_call(raw_call, transaction.metadata)
+raw_call: Call = transaction.root_call.subcalls[0]
+abi_decoded_call: DecodedCall = ethtx.decoders.abi_decoder.decode_call(raw_call, block.metadata, transaction.metadata,
+                                                                       proxies)
 ```
 
 3. Semantic decoding:
 
 ```python
 from ethtx.models.decoded_model import DecodedTransactionMetadata
 
-# get proxies used in the transaction
-proxies = ethtx.decoders.get_proxies(transaction.root_call, chain_id)
-
 # semantically decode transaction components
-decoded_metadata: DecodedTransactionMetadata = ethtx.decoders.semantic_decoder.decode_metadata(block.metadata,
-                                                                                               transaction.metadata,
-                                                                                               chain_id)
-decoded_events: List[DecodedEvent] = ethtx.decoders.semantic_decoder.decode_events(abi_decoded_events, decoded_metadata,
-                                                                                   proxies)
+decoded_metadata: DecodedTransactionMetadata = (
+    ethtx.decoders.semantic_decoder.decode_metadata(
+        block.metadata, transaction.metadata, 'mainnet'
+    )
+)
+decoded_events: List[DecodedEvent] = ethtx.decoders.semantic_decoder.decode_events(
+    abi_decoded_events, decoded_metadata, proxies
+)
+
 decoded_calls: Call = ethtx.decoders.semantic_decoder.decode_calls(abi_decoded_calls, decoded_metadata, proxies)
-decoded_transfers: List[DecodedTransfer] = ethtx.decoders.semantic_decoder.decode_transfers(abi_decoded_transfers)
-decoded_balances: List[DecodedBalance] = ethtx.decoders.semantic_decoder.decode_balances(abi_decoded_balances)
+decoded_transfers: List[
+    DecodedTransfer
+] = ethtx.decoders.semantic_decoder.decode_transfers(
+    abi_decoded_transfers, decoded_metadata
+)
+decoded_balances: List[
+    DecodedBalance
+] = ethtx.decoders.semantic_decoder.decode_balances(
+    abi_decoded_balances, decoded_metadata
+)
 
 # semantically decode a single event
 decoded_event: DecodedEvent = ethtx.decoders.semantic_decoder.decode_event(abi_decoded_events[0], decoded_metadata,
                                                                            proxies)
 # semantically decode a single call
-decoded_call: Call = ethtx.decoders.semantic_decoder.decode_call(abi_decoded_calls.subcalls[2].subcalls[0],
+decoded_call: Call = ethtx.decoders.semantic_decoder.decode_call(abi_decoded_calls.subcalls[0],
                                                                  decoded_metadata, proxies)
 ```
```

### Comparing `EthTx-0.3.8/README.md` & `EthTx-0.3.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: EthTx
+Version: 0.3.9
+Summary: EthTx transaction decoder.
+Home-page: https://github.com/EthTx/ethtx
+Author: Karol Chojnowski, Tomasz Mierzwa, Piotr Rudnik
+Author-email: karol@tfi.team, tomek@tfi.team, piotr.rudnik@tfi.team
+License: Apache-2.0 License
+Platform: UNKNOWN
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 <h1 align='center' style='border-bottom: none'>
   <p>EthTx - Ethereum transactions decoder </p>
 </h1>
 
 <p align="center">
 <a target="_blank">
     <img src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg" alt="Python">
@@ -45,23 +62,23 @@
 
 ```python
 from ethtx import EthTx, EthTxConfig
 from ethtx.models.decoded_model import DecodedTransaction
 
 ethtx_config = EthTxConfig(
     mongo_connection_string="mongomock://localhost/ethtx",  ##MongoDB connection string,
-    etherscan_api_key = "",  ##Etherscan API key,
-    web3nodes = {
-                "mainnet": {
-                    "hook": "_Geth_archive_node_URL_", # multiple nodes supported, separate them with comma
-                    "poa": _POA_chain_indicator_  # represented by bool value
-                }
-            },
-            default_chain = "mainnet",
-            etherscan_urls = {"mainnet": "https://api.etherscan.io/api",},
+    etherscan_api_key="",  ##Etherscan API key,
+    web3nodes={
+        "mainnet": {
+            "hook": "_Geth_archive_node_URL_",  # multiple nodes supported, separate them with comma
+            "poa": _POA_chain_indicator_  # represented by bool value
+        }
+    },
+    default_chain="mainnet",
+    etherscan_urls={"mainnet": "https://api.etherscan.io/api", },
 )
 
 ethtx = EthTx.initialize(ethtx_config)
 transaction: DecodedTransaction = ethtx.decoders.decode_transaction(
     '0x50051e0a6f216ab9484c2080001c7e12d5138250acee1f4b7c725b8fb6bb922d')
 ```
 
@@ -78,61 +95,93 @@
 from ethtx.models.w3_model import W3Transaction, W3Block, W3Receipt, W3CallTree
 
 # read raw transaction data directly from the node
 w3transaction: W3Transaction = web3provider.get_transaction(
     '0x50051e0a6f216ab9484c2080001c7e12d5138250acee1f4b7c725b8fb6bb922d')
 w3block: W3Block = web3provider.get_block(w3transaction.blockNumber)
 w3receipt: W3Receipt = web3provider.get_receipt(w3transaction.hash.hex())
-w3calls: W3CallTree = web3provider.get_calls(w3transaction.hash.hex()
+w3calls: W3CallTree = web3provider.get_calls(w3transaction.hash.hex())
 ```
 
 2. ABI decoding:
 
 ```python
-from ethtx.models.objects_model import Transaction, Event, Call
-from ethtx.models.decoded_model import DecodedEvent, DecodedCall, DecodedTransfer, DecodedBalance
+from ethtx.models.decoded_model import (
+    DecodedTransfer,
+    DecodedBalance,
+    DecodedEvent, DecodedCall,
+)
+from ethtx.models.objects_model import Transaction, Event, Block, Call
 
 # read the raw transaction from the node
 transaction: Transaction = web3provider.get_full_transaction(
     '0x50051e0a6f216ab9484c2080001c7e12d5138250acee1f4b7c725b8fb6bb922d')
 
+# get proxies used in the transaction
+proxies = ethtx.decoders.get_proxies(transaction.root_call, 'mainnet')
+
+block: Block = Block.from_raw(
+    w3block=web3provider.get_block(
+        transaction.metadata.block_number
+    ),
+    chain_id='mainnet',
+)
+
 # decode transaction components
-abi_decoded_events: List[Event] = ethtx.decoders.abi_decoder.decode_events(transaction.events, transaction.metadata)
-abi_decoded_calls: DecodedCall = ethtx.decoders.abi_decoder.decode_calls(transaction.root_call, transaction.metadata)
-abi_decoded_transfers: List[DecodedTransfer] = ethtx.decoders.abi_decoder.decode_transfers(abi_decoded_calls,
-                                                                                           abi_decoded_events)
-abi_decoded_balances: List[DecodedBalance] = ethtx.decoders.abi_decoder.decode_balances(abi_decoded_transfers)
+abi_decoded_events: List[Event] = ethtx.decoders.abi_decoder.decode_events(
+    transaction.events, block.metadata, transaction.metadata
+)
+abi_decoded_calls: DecodedCall = ethtx.decoders.abi_decoder.decode_calls(transaction.root_call, block.metadata,
+                                                                         transaction.metadata, proxies)
+abi_decoded_transfers: List[
+    DecodedTransfer
+] = ethtx.decoders.abi_decoder.decode_transfers(abi_decoded_calls, abi_decoded_events)
+abi_decoded_balances: List[DecodedBalance] = ethtx.decoders.abi_decoder.decode_balances(
+    abi_decoded_transfers
+)
 
 # decode a single event
 raw_event: Event = transaction.events[3]
-abi_decoded_event: DecodedEvent = ethtx.decoders.abi_decoder.decode_event(raw_event, transaction.metadata)
+abi_decoded_event: DecodedEvent = ethtx.decoders.abi_decoder.decode_event(raw_event, block.metadata,
+                                                                          transaction.metadata)
 
 # decode a single call
-raw_call: Call = transaction.root_call.subcalls[3].subcalls[2]
-abi_decoded_call: DecodedCall = ethtx.decoders.abi_decoder.decode_call(raw_call, transaction.metadata)
+raw_call: Call = transaction.root_call.subcalls[0]
+abi_decoded_call: DecodedCall = ethtx.decoders.abi_decoder.decode_call(raw_call, block.metadata, transaction.metadata,
+                                                                       proxies)
 ```
 
 3. Semantic decoding:
 
 ```python
 from ethtx.models.decoded_model import DecodedTransactionMetadata
 
-# get proxies used in the transaction
-proxies = ethtx.decoders.get_proxies(transaction.root_call, chain_id)
-
 # semantically decode transaction components
-decoded_metadata: DecodedTransactionMetadata = ethtx.decoders.semantic_decoder.decode_metadata(block.metadata,
-                                                                                               transaction.metadata,
-                                                                                               chain_id)
-decoded_events: List[DecodedEvent] = ethtx.decoders.semantic_decoder.decode_events(abi_decoded_events, decoded_metadata,
-                                                                                   proxies)
+decoded_metadata: DecodedTransactionMetadata = (
+    ethtx.decoders.semantic_decoder.decode_metadata(
+        block.metadata, transaction.metadata, 'mainnet'
+    )
+)
+decoded_events: List[DecodedEvent] = ethtx.decoders.semantic_decoder.decode_events(
+    abi_decoded_events, decoded_metadata, proxies
+)
+
 decoded_calls: Call = ethtx.decoders.semantic_decoder.decode_calls(abi_decoded_calls, decoded_metadata, proxies)
-decoded_transfers: List[DecodedTransfer] = ethtx.decoders.semantic_decoder.decode_transfers(abi_decoded_transfers)
-decoded_balances: List[DecodedBalance] = ethtx.decoders.semantic_decoder.decode_balances(abi_decoded_balances)
+decoded_transfers: List[
+    DecodedTransfer
+] = ethtx.decoders.semantic_decoder.decode_transfers(
+    abi_decoded_transfers, decoded_metadata
+)
+decoded_balances: List[
+    DecodedBalance
+] = ethtx.decoders.semantic_decoder.decode_balances(
+    abi_decoded_balances, decoded_metadata
+)
 
 # semantically decode a single event
 decoded_event: DecodedEvent = ethtx.decoders.semantic_decoder.decode_event(abi_decoded_events[0], decoded_metadata,
                                                                            proxies)
 # semantically decode a single call
-decoded_call: Call = ethtx.decoders.semantic_decoder.decode_call(abi_decoded_calls.subcalls[2].subcalls[0],
+decoded_call: Call = ethtx.decoders.semantic_decoder.decode_call(abi_decoded_calls.subcalls[0],
                                                                  decoded_metadata, proxies)
-```
+```
+
```

### Comparing `EthTx-0.3.8/ethtx/__init__.py` & `EthTx-0.3.9/ethtx/__init__.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/abi/abc.py` & `EthTx-0.3.9/ethtx/decoders/abi/abc.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/abi/balances.py` & `EthTx-0.3.9/ethtx/decoders/abi/balances.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/abi/calls.py` & `EthTx-0.3.9/ethtx/decoders/abi/calls.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/abi/decoder.py` & `EthTx-0.3.9/ethtx/decoders/abi/decoder.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/abi/events.py` & `EthTx-0.3.9/ethtx/decoders/abi/events.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/abi/helpers/utils.py` & `EthTx-0.3.9/ethtx/decoders/abi/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/abi/transfers.py` & `EthTx-0.3.9/ethtx/decoders/abi/transfers.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/decoder_service.py` & `EthTx-0.3.9/ethtx/decoders/decoder_service.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/decoders/parameters.py` & `EthTx-0.3.9/ethtx/decoders/decoders/parameters.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/decoders/semantics.py` & `EthTx-0.3.9/ethtx/decoders/decoders/semantics.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/semantic/abc.py` & `EthTx-0.3.9/ethtx/decoders/semantic/abc.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/semantic/balances.py` & `EthTx-0.3.9/ethtx/decoders/semantic/balances.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/semantic/calls.py` & `EthTx-0.3.9/ethtx/decoders/semantic/calls.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         self,
         call: DecodedCall,
         tx_metadata: DecodedTransactionMetadata,
         proxies: Dict[str, Proxy],
     ) -> DecodedCall:
 
         standard = self.repository.get_standard(call.chain_id, call.to_address.address)
-
         function_transformations = self.repository.get_transformations(
             call.chain_id, call.to_address.address, call.function_signature
         )
 
         if function_transformations:
             call.function_name = (
                 function_transformations.get("name") or call.function_name
@@ -53,15 +52,14 @@
         context = create_transformation_context(
             call.to_address.address,
             call.arguments,
             call.outputs,
             tx_metadata,
             self.repository,
         )
-        standard = self.repository.get_standard(call.chain_id, call.to_address.address)
 
         # perform parameters transformations
         for i, parameter in enumerate(call.arguments):
             semantically_decode_parameter(
                 self.repository,
                 parameter,
                 f"__input{i}__",
```

### Comparing `EthTx-0.3.8/ethtx/decoders/semantic/decoder.py` & `EthTx-0.3.9/ethtx/decoders/semantic/decoder.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/semantic/events.py` & `EthTx-0.3.9/ethtx/decoders/semantic/events.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/semantic/helpers/utils.py` & `EthTx-0.3.9/ethtx/decoders/semantic/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/semantic/metadata.py` & `EthTx-0.3.9/ethtx/decoders/semantic/metadata.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/decoders/semantic/transfers.py` & `EthTx-0.3.9/ethtx/decoders/semantic/transfers.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/ethtx.py` & `EthTx-0.3.9/ethtx/ethtx.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/exceptions.py` & `EthTx-0.3.9/ethtx/exceptions.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/models/_types.py` & `EthTx-0.3.9/ethtx/models/_types.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/models/base_model.py` & `EthTx-0.3.9/ethtx/models/base_model.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/models/decoded_model.py` & `EthTx-0.3.9/ethtx/models/decoded_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class DecodedCall(BaseModel):
     chain_id: str
     timestamp: datetime
     tx_hash: str
     call_id: Optional[str]
     call_type: str
     from_address: AddressInfo
-    to_address: AddressInfo
+    to_address: Optional[AddressInfo]
     value: float
     function_signature: str
     function_name: str
     arguments: List[Argument]
     outputs: List[Argument]
     gas_used: Optional[int]
     error: Optional[str]
```

### Comparing `EthTx-0.3.8/ethtx/models/objects_model.py` & `EthTx-0.3.9/ethtx/models/objects_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         return w3log.to_object()
 
 
 class Call(BaseModel):
     call_type: str
     call_gas: Optional[int]
     from_address: str
-    to_address: str
+    to_address: Optional[str]
     call_value: int
     call_data: str
     return_value: str
     gas_used: Optional[int]
     status: bool
     error: Optional[str]
     subcalls: List[Call] = Field(default_factory=list)
```

### Comparing `EthTx-0.3.8/ethtx/models/semantics_model.py` & `EthTx-0.3.9/ethtx/models/semantics_model.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/models/w3_model.py` & `EthTx-0.3.9/ethtx/models/w3_model.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/__init__.py` & `EthTx-0.3.9/ethtx/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/ens_provider.py` & `EthTx-0.3.9/ethtx/providers/ens_provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,39 +32,31 @@
     def address(self, provider: Type[T], name: Any):
         ...
 
 
 class Web3ENSProvider(ENSProviderBase):
     ns: ENS
 
-    @lru_cache(maxsize=1024)
     def name(self, provider: Web3, address: str) -> str:
         ns = self._set_provider(provider)
         check_sum_address = Web3.toChecksumAddress(address)
         name = ns.name(address=check_sum_address)
 
         if name:
             log.info("ENS resolved an address: %s to name: %s", address, name)
 
         return name if name else address
 
-    @lru_cache(maxsize=1024)
     def address(self, provider: Web3, name: str) -> str:
         ns = self._set_provider(provider)
         address = ns.address(name=name)
 
         if address:
             log.info("ENS resolved name: %s to address: %s", name, address)
 
         return address if address else name
 
-    @staticmethod
-    def _set_provider(provider: Web3) -> ENS:
-        ns = ENS.fromWeb3(provider)
-
-        # ENS.fromWeb3 not copying middleware #1657
-        ns.web3.middleware_onion.inject(geth_poa_middleware, layer=0)
-
-        return ns
+    def _set_provider(self, provider: Web3) -> ENS:
+        return ENS.fromWeb3(provider)
 
 
 ENSProvider = Web3ENSProvider()
```

### Comparing `EthTx-0.3.8/ethtx/providers/etherscan/__init__.py` & `EthTx-0.3.9/ethtx/providers/etherscan/__init__.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/etherscan/client.py` & `EthTx-0.3.9/ethtx/providers/etherscan/client.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/etherscan/contracts.py` & `EthTx-0.3.9/ethtx/providers/etherscan/contracts.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/etherscan/etherscan_provider.py` & `EthTx-0.3.9/ethtx/providers/etherscan/etherscan_provider.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/node/__init__.py` & `EthTx-0.3.9/ethtx/providers/node/__init__.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/node/connection_base.py` & `EthTx-0.3.9/ethtx/providers/node/connection_base.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/node/pool.py` & `EthTx-0.3.9/ethtx/providers/node/pool.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/semantic_providers/__init__.py` & `EthTx-0.3.9/ethtx/providers/semantic_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/semantic_providers/base.py` & `EthTx-0.3.9/ethtx/providers/semantic_providers/base.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/semantic_providers/const.py` & `EthTx-0.3.9/ethtx/providers/semantic_providers/const.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/semantic_providers/database.py` & `EthTx-0.3.9/ethtx/providers/semantic_providers/database.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/semantic_providers/repository.py` & `EthTx-0.3.9/ethtx/providers/semantic_providers/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,26 +23,27 @@
     FunctionSemantics,
     EventSemantics,
     Signature,
     SignatureArg,
 )
 from ethtx.providers import EtherscanProvider, Web3Provider, ENSProvider
 from ethtx.providers.semantic_providers.database import ISemanticsDatabase
+from ethtx.providers.web3_provider import NodeDataProvider
 from ethtx.semantics.protocols_router import amend_contract_semantics
 from ethtx.semantics.solidity.precompiles import precompiles
 from ethtx.semantics.standards.erc20 import ERC20_FUNCTIONS, ERC20_EVENTS
 from ethtx.semantics.standards.erc721 import ERC721_FUNCTIONS, ERC721_EVENTS
 
 
 class SemanticsRepository:
     def __init__(
             self,
             database_connection: ISemanticsDatabase,
             etherscan_provider: EtherscanProvider,
-            web3provider: Web3Provider,
+            web3provider: NodeDataProvider,
             ens_provider: ENSProvider,
             refresh_ens: bool = True
     ):
         self.database = database_connection
         self.etherscan = etherscan_provider
         self._web3provider = web3provider
         self._ens_provider = ens_provider
@@ -190,15 +191,15 @@
 
         if self._records is not None:
             self._records.append(address)
 
         return address_semantics
 
     def _decode_standard_semantics(
-            self, address, name, events, functions
+            self, address, name, events, functions: Dict[str, FunctionSemantics]
     ) -> Tuple[Optional[str], Optional[ERC20Semantics]]:
         standard = None
         standard_semantics = None
 
         if not address:
             return standard, standard_semantics
 
@@ -227,93 +228,87 @@
     @lru_cache(maxsize=1024)
     def get_event_abi(self, chain_id, address, signature) -> Optional[EventSemantics]:
 
         if not address:
             return None
 
         semantics = self.get_semantics(chain_id, address)
-        event_semantics = (
-            semantics.contract.events.get(signature) if semantics else None
-        )
+        event_semantics = semantics.contract.events.get(signature)
+
 
         return event_semantics
 
     @lru_cache(maxsize=1024)
     def get_transformations(
             self, chain_id, address, signature
     ) -> Optional[Dict[str, TransformationSemantics]]:
 
         if not address:
             return None
 
         semantics = self.get_semantics(chain_id, address)
-        if semantics:
-            transformations = semantics.contract.transformations.get(signature)
-        else:
-            transformations = None
+        transformations = semantics.contract.transformations.get(signature)
 
         return transformations
 
     @lru_cache(maxsize=1024)
     def get_anonymous_event_abi(self, chain_id, address) -> Optional[EventSemantics]:
 
         if not address:
             return None
 
         semantics = self.get_semantics(chain_id, address)
         event_semantics = None
-        if semantics:
-            anonymous_events = {
-                signature
-                for signature, event in semantics.contract.events.items()
-                if event.anonymous
-            }
-            if len(anonymous_events) == 1:
-                event_signature = anonymous_events.pop()
-                event_semantics = semantics.contract.events[event_signature]
+
+        anonymous_events = {
+            signature
+            for signature, event in semantics.contract.events.items()
+            if event.anonymous
+        }
+        if len(anonymous_events) == 1:
+            event_signature = anonymous_events.pop()
+            event_semantics = semantics.contract.events[event_signature]
 
         return event_semantics
 
     @lru_cache(maxsize=1024)
     def get_function_abi(
             self, chain_id, address, signature
     ) -> Optional[FunctionSemantics]:
 
         if not address:
             return None
 
         semantics = self.get_semantics(chain_id, address)
-        function_semantics = (
-            semantics.contract.functions.get(signature) if semantics else None
-        )
+        function_semantics = semantics.contract.functions.get(signature)
 
         return function_semantics
 
     @lru_cache(maxsize=1024)
     def get_constructor_abi(self, chain_id, address) -> Optional[FunctionSemantics]:
 
         if not address:
             return None
 
         semantics = self.get_semantics(chain_id, address)
-        constructor_semantics = (
-            semantics.contract.functions.get("constructor") if semantics else None
-        )
+        constructor_semantics = semantics.contract.functions.get("constructor")
+
         if constructor_semantics:
             constructor_semantics.outputs.append(
                 ParameterSemantics(
                     parameter_name="__create_output__",
                     parameter_type="ignore",
                     indexed=False,
                     dynamic=True,
                 )
             )
 
         return constructor_semantics
 
+    # do not cache with lru - uses unhashable arguments
     def get_address_label(self, chain_id, address, proxies=None) -> str:
 
         if not address:
             return ""
 
         if int(address, 16) in precompiles:
             contract_label = "Precompiled"
@@ -344,35 +339,33 @@
     @lru_cache(maxsize=1024)
     def get_standard(self, chain_id, address) -> Optional[str]:
 
         if not address:
             return None
 
         semantics = self.get_semantics(chain_id, address)
-        standard = semantics.standard if semantics is not None else None
-
-        return standard
+        return semantics.standard
 
     def get_token_data(
             self, chain_id, address, proxies=None
     ) -> Tuple[Optional[str], Optional[str], Optional[int], Optional[str]]:
 
         if not address:
             return None, None, None, None
 
         semantics = self.get_semantics(chain_id, address)
-        if semantics and semantics.erc20:
+        if semantics.erc20:
             token_name = (
-                semantics.erc20.name if semantics and semantics.erc20 else address
+                semantics.erc20.name if semantics.erc20 else address
             )
             token_symbol = (
-                semantics.erc20.symbol if semantics and semantics.erc20 else "Unknown"
+                semantics.erc20.symbol if semantics.erc20 else "Unknown"
             )
             token_decimals = (
-                semantics.erc20.decimals if semantics and semantics.erc20 else 18
+                semantics.erc20.decimals if semantics.erc20 else 18
             )
         elif proxies and address in proxies and proxies[address].token:
             token_name = proxies[address].token.name
             token_symbol = proxies[address].token.symbol
             token_decimals = proxies[address].token.decimals
         else:
             token_name = address
```

### Comparing `EthTx-0.3.8/ethtx/providers/signature_provider.py` & `EthTx-0.3.9/ethtx/providers/signature_provider.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/static/tracer.js` & `EthTx-0.3.9/ethtx/providers/static/tracer.js`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/providers/web3_provider.py` & `EthTx-0.3.9/ethtx/providers/web3_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from web3.datastructures import AttributeDict
 from web3.middleware import geth_poa_middleware
 from web3.types import BlockData, TxData, TxReceipt, HexStr
 
 from .node import NodeConnectionPool
 from ..exceptions import NodeConnectionException, ProcessingException
 from ..models.objects_model import Transaction, BlockMetadata, TransactionMetadata, Call
+from ..models.semantics_model import FunctionSemantics
 from ..models.w3_model import W3Block, W3Transaction, W3Receipt, W3CallTree, W3Log
 from ..semantics.standards import erc20
 
 log = logging.getLogger(__name__)
 
 
 def connect_chain(
@@ -268,15 +269,15 @@
 
     # get the erc20 token data from the node
     @lru_cache(maxsize=1024)
     def get_erc20_token(
         self,
         token_address: str,
         contract_name: str,
-        functions,
+        functions: Dict[str, FunctionSemantics],
         chain_id: Optional[str] = None,
     ):
 
         name_abi = symbol_abi = decimals_abi = ""
 
         if functions:
             for function in functions.values():
```

### Comparing `EthTx-0.3.8/ethtx/semantics/base.py` & `EthTx-0.3.9/ethtx/semantics/base.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/protocols/anonymous.py` & `EthTx-0.3.9/ethtx/semantics/protocols/anonymous.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/protocols/maker/cdp_manager.py` & `EthTx-0.3.9/ethtx/semantics/protocols/maker/cdp_manager.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/protocols/maker/dai.py` & `EthTx-0.3.9/ethtx/semantics/protocols/maker/dai.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/protocols/maker/dai_join.py` & `EthTx-0.3.9/ethtx/semantics/protocols/maker/dai_join.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/protocols/maker/ds_proxy.py` & `EthTx-0.3.9/ethtx/semantics/protocols/maker/ds_proxy.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/protocols/maker/gem_join.py` & `EthTx-0.3.9/ethtx/semantics/protocols/maker/gem_join.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/protocols/maker/jug.py` & `EthTx-0.3.9/ethtx/semantics/protocols/maker/jug.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/protocols/maker/vat.py` & `EthTx-0.3.9/ethtx/semantics/protocols/maker/vat.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/protocols/wrappers/weth.py` & `EthTx-0.3.9/ethtx/semantics/protocols/wrappers/weth.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/protocols_router.py` & `EthTx-0.3.9/ethtx/semantics/protocols_router.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/rollups/aztec.py` & `EthTx-0.3.9/ethtx/semantics/rollups/aztec.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/router.py` & `EthTx-0.3.9/ethtx/semantics/router.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/solidity/precompiles.py` & `EthTx-0.3.9/ethtx/semantics/solidity/precompiles.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/standards/eip1969.py` & `EthTx-0.3.9/ethtx/semantics/standards/eip1969.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from functools import lru_cache
+
 from web3 import Web3
 
 
+@lru_cache(maxsize=1024)
 def is_eip1969_proxy(chain, delegator, delegate):
     implementation_slot = hex(
         int(Web3.keccak(text="eip1967.proxy.implementation").hex(), 16) - 1
     )
     try:
         implementation = (
             "0x"
@@ -13,14 +16,15 @@
             ).hex()[-40:]
         )
         return implementation == delegate
     except:
         return False
 
 
+@lru_cache(maxsize=1024)
 def is_eip1969_beacon_proxy(chain, delegator, delegate):
     ibeacon_abi = """[
                         {
                             "inputs": [],
                             "name": "implementation",
                             "outputs": [
                                 {
```

### Comparing `EthTx-0.3.8/ethtx/semantics/standards/erc20.py` & `EthTx-0.3.9/ethtx/semantics/standards/erc20.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/standards/erc721.py` & `EthTx-0.3.9/ethtx/semantics/standards/erc721.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/semantics/utilities/functions.py` & `EthTx-0.3.9/ethtx/semantics/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/utils/attr_dict.py` & `EthTx-0.3.9/ethtx/utils/attr_dict.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/utils/decorators.py` & `EthTx-0.3.9/ethtx/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/utils/measurable.py` & `EthTx-0.3.9/ethtx/utils/measurable.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/ethtx/utils/validators.py` & `EthTx-0.3.9/ethtx/utils/validators.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/setup.py` & `EthTx-0.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import io
 import os
 import subprocess
 import sys
 from shutil import rmtree
 
+import toml
 from setuptools import find_packages, setup, Command
 
 # root dir
 root = os.path.abspath(os.path.dirname(__file__))
 
 # Package meta-data.
 NAME = "EthTx"
@@ -43,16 +44,27 @@
         long_description = "\n" + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 
 def load_requirements(fname):
     """Load requirements from file."""
-    with open(fname) as file:
-        return file.read().splitlines()
+    try:
+        with open(fname, "r") as fh:
+            pipfile = fh.read()
+        pipfile_toml = toml.loads(pipfile)
+    except FileNotFoundError:
+        return []
+
+    try:
+        required_packages = pipfile_toml["packages"].items()
+    except KeyError:
+        return []
+
+    return [f"{pkg}{ver}" if ver != "*" else pkg for pkg, ver in required_packages]
 
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
     description = "Build and publish the package."
     user_options = []
@@ -78,15 +90,15 @@
         self.status("Building Source and Wheel (universal) distribution…")
         os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
 
         self.status("Uploading the package to PyPI via Twine…")
         os.system("twine upload dist/*")
 
         self.status("Pushing git tags…")
-        os.system("git tag v{0}".format(about["__version__"]))
+        os.system("git tag {0}".format(about["__version__"]))
         os.system("git push --tags")
 
         sys.exit()
 
 
 # *************** INSTALL *****************
 setup(
@@ -97,18 +109,18 @@
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     license="Apache-2.0 License",
     packages=find_packages(exclude=["tests"]),
-    install_requires=load_requirements("requirements.txt"),
+    install_requires=load_requirements("Pipfile"),
     include_package_data=True,
     test_suite="tests",
     classifiers=[
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
     # $ setup.py publish support.
     cmdclass={"upload": UploadCommand},
 )
```

### Comparing `EthTx-0.3.8/tests/mocks/web3provider.py` & `EthTx-0.3.9/tests/mocks/web3provider.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/tests/models/decoded_model_test.py` & `EthTx-0.3.9/tests/models/decoded_model_test.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/tests/models/mock.py` & `EthTx-0.3.9/tests/models/mock.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/tests/models/objects_model_test.py` & `EthTx-0.3.9/tests/models/objects_model_test.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/tests/models/semantics_model_test.py` & `EthTx-0.3.9/tests/models/semantics_model_test.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/tests/models/w3_model_test.py` & `EthTx-0.3.9/tests/models/w3_model_test.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/tests/providers/node/connection_base_test.py` & `EthTx-0.3.9/tests/providers/node/connection_base_test.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/tests/providers/node/pool_test.py` & `EthTx-0.3.9/tests/providers/node/pool_test.py`

 * *Files identical despite different names*

### Comparing `EthTx-0.3.8/tests/providers/semantic_providers/semantics_database_test.py` & `EthTx-0.3.9/tests/providers/semantic_providers/semantics_database_test.py`

 * *Files identical despite different names*

