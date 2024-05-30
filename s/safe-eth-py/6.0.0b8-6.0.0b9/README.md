# Comparing `tmp/safe-eth-py-6.0.0b8.tar.gz` & `tmp/safe-eth-py-6.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe-eth-py-6.0.0b8.tar", last modified: Thu Nov 23 09:39:37 2023, max compression
+gzip compressed data, was "safe-eth-py-6.0.0b9.tar", last modified: Tue Dec 12 12:28:48 2023, max compression
```

## Comparing `safe-eth-py-6.0.0b8.tar` & `safe-eth-py-6.0.0b9.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.171278 safe-eth-py-6.0.0b8/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2023-11-23 09:39:37.171278 safe-eth-py-6.0.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.135278 safe-eth-py-6.0.0b8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.135278 safe-eth-py-6.0.0b8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/gnosis.eth.clients.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/gnosis.eth.contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/gnosis.eth.django.rst
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/gnosis.eth.eip712.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/gnosis.eth.oracles.abis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/gnosis.eth.oracles.rst
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/gnosis.eth.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/gnosis.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/gnosis.safe.rst
--rw-r--r--   0 runner    (1001) docker     (127)      896 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.135278 safe-eth-py-6.0.0b8/gnosis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.139278 safe-eth-py-6.0.0b8/gnosis/eth/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.139278 safe-eth-py-6.0.0b8/gnosis/eth/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/clients/blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/clients/contract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     9769 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/clients/etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/clients/sourcify.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.139278 safe-eth-py-6.0.0b8/gnosis/eth/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)    10109 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.151278 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/
--rw-r--r--   0 runner    (1001) docker     (127)   328664 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/CPKFactory.json
--rw-r--r--   0 runner    (1001) docker     (127)    28908 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)    29485 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json
--rw-r--r--   0 runner    (1001) docker     (127)    26897 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/DelegateConstructorProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    29068 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ERC1155.json
--rw-r--r--   0 runner    (1001) docker     (127)    54748 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ERC20.json
--rw-r--r--   0 runner    (1001) docker     (127)    89890 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ERC20TestToken.json
--rw-r--r--   0 runner    (1001) docker     (127)   622260 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ERC721.json
--rw-r--r--   0 runner    (1001) docker     (127)   983403 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json
--rw-r--r--   0 runner    (1001) docker     (127)  1158944 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (127)  1347363 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (127)   119875 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)    19886 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/MultiSend.json
--rw-r--r--   0 runner    (1001) docker     (127)    78793 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/PayingProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   136946 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (127)   288861 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (127)    18975 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)    15538 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json
--rw-r--r--   0 runner    (1001) docker     (127)    32495 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/Proxy_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (127)    39032 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/Proxy_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/Proxy_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/Proxy_V1_4_1.json
--rw-r--r--   0 runner    (1001) docker     (127)   121611 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/Safe_V1_4_1.json
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/kyber_network_proxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    19012 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)    17165 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/uniswap_exchange.json
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/uniswap_factory.json
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/uniswap_v2_factory.json
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/uniswap_v2_pair.json
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/uniswap_v2_router.json
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/contracts/contract_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.151278 safe-eth-py-6.0.0b8/gnosis/eth/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8445 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.155278 safe-eth-py-6.0.0b8/gnosis/eth/django/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/django/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.155278 safe-eth-py-6.0.0b8/gnosis/eth/eip712/
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    80662 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21119 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/ethereum_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/multicall.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.155278 safe-eth-py-6.0.0b8/gnosis/eth/oracles/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.155278 safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15986 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/aave_abis.py
--rw-r--r--   0 runner    (1001) docker     (127)    30036 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/balancer_abis.py
--rw-r--r--   0 runner    (1001) docker     (127)    29731 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/cream_abis.py
--rw-r--r--   0 runner    (1001) docker     (127)    27567 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/curve_abis.py
--rw-r--r--   0 runner    (1001) docker     (127)    25872 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-r--r--   0 runner    (1001) docker     (127)    45208 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    36257 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/yearn_abis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/zerion_abis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/cowswap.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.155278 safe-eth-py-6.0.0b8/gnosis/eth/oracles/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/kyber.py
--rw-r--r--   0 runner    (1001) docker     (127)    32246 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/oracles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/superfluid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/oracles/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.159278 safe-eth-py-6.0.0b8/gnosis/eth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.159278 safe-eth-py-6.0.0b8/gnosis/eth/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   107388 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/clients/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/clients/test_sourcify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.159278 safe-eth-py-6.0.0b8/gnosis/eth/tests/eip712/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13315 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/eip712/test_eip712.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/ethereum_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.163278 safe-eth-py-6.0.0b8/gnosis/eth/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31306 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-r--r--   0 runner    (1001) docker     (127)   792720 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    92795 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)   171076 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.163278 safe-eth-py-6.0.0b8/gnosis/eth/tests/oracles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/oracles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/oracles/test_cowswap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/oracles/test_kyber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/oracles/test_superfluid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    61105 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/test_ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/test_multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)    21137 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/test_oracles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/eth/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.163278 safe-eth-py-6.0.0b8/gnosis/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9510 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/protocol/gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/protocol/order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.163278 safe-eth-py-6.0.0b8/gnosis/protocol/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/protocol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/protocol/tests/test_gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.167278 safe-eth-py-6.0.0b8/gnosis/safe/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44751 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.167278 safe-eth-py-6.0.0b8/gnosis/safe/api/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/api/base_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/api/relay_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/api/transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11447 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/multi_send.py
--rw-r--r--   0 runner    (1001) docker     (127)    10479 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    36883 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/safe.py
--rw-r--r--   0 runner    (1001) docker     (127)    11873 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/safe_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)   101026 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/safe_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)     9885 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.167278 safe-eth-py-6.0.0b8/gnosis/safe/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.167278 safe-eth-py-6.0.0b8/gnosis/safe/tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17981 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/safe_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_multi_send.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.171278 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_proxy_factory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_proxy_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7510 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    32455 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_safe.py
--rw-r--r--   0 runner    (1001) docker     (127)    16674 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (127)    14117 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)    12995 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_safe_v1_0_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_safe_v1_3_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/test_signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/safe/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.171278 safe-eth-py-6.0.0b8/gnosis/util/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/gnosis/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 09:39:37.171278 safe-eth-py-6.0.0b8/safe_eth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2023-11-23 09:39:37.000000 safe-eth-py-6.0.0b8/safe_eth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2023-11-23 09:39:37.000000 safe-eth-py-6.0.0b8/safe_eth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 09:39:37.000000 safe-eth-py-6.0.0b8/safe_eth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-11-23 09:39:37.000000 safe-eth-py-6.0.0b8/safe_eth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-23 09:39:37.000000 safe-eth-py-6.0.0b8/safe_eth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2023-11-23 09:39:37.171278 safe-eth-py-6.0.0b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-23 09:39:24.000000 safe-eth-py-6.0.0b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.354859 safe-eth-py-6.0.0b9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2023-12-12 12:28:48.354859 safe-eth-py-6.0.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.318858 safe-eth-py-6.0.0b9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.322859 safe-eth-py-6.0.0b9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/gnosis.eth.clients.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/gnosis.eth.contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/gnosis.eth.django.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/gnosis.eth.eip712.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/gnosis.eth.oracles.abis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/gnosis.eth.oracles.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/gnosis.eth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/gnosis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/gnosis.safe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.322859 safe-eth-py-6.0.0b9/gnosis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.322859 safe-eth-py-6.0.0b9/gnosis/eth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.322859 safe-eth-py-6.0.0b9/gnosis/eth/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/clients/blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/clients/contract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9769 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/clients/etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/clients/sourcify_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.322859 safe-eth-py-6.0.0b9/gnosis/eth/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)    10109 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.334859 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/
+-rw-r--r--   0 runner    (1001) docker     (127)   328664 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/CPKFactory.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28908 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    29485 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26897 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/DelegateConstructorProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    29068 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ERC1155.json
+-rw-r--r--   0 runner    (1001) docker     (127)    54748 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ERC20.json
+-rw-r--r--   0 runner    (1001) docker     (127)    89890 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ERC20TestToken.json
+-rw-r--r--   0 runner    (1001) docker     (127)   622260 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ERC721.json
+-rw-r--r--   0 runner    (1001) docker     (127)   983403 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1158944 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1347363 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   119875 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19886 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/MultiSend.json
+-rw-r--r--   0 runner    (1001) docker     (127)    78793 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/PayingProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   136946 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)   288861 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18975 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15538 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32495 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/Proxy_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39032 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/Proxy_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/Proxy_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/Proxy_V1_4_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   121611 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/Safe_V1_4_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/kyber_network_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19012 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17165 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/uniswap_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/uniswap_factory.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/uniswap_v2_factory.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/uniswap_v2_pair.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/uniswap_v2_router.json
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/contracts/contract_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.338859 safe-eth-py-6.0.0b9/gnosis/eth/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8445 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.338859 safe-eth-py-6.0.0b9/gnosis/eth/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/django/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.338859 safe-eth-py-6.0.0b9/gnosis/eth/eip712/
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80662 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21193 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/ethereum_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.338859 safe-eth-py-6.0.0b9/gnosis/eth/oracles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.342859 safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15986 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/aave_abis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30036 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29731 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/cream_abis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27567 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/curve_abis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25872 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45208 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36257 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.342859 safe-eth-py-6.0.0b9/gnosis/eth/oracles/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/kyber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32246 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/oracles/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.342859 safe-eth-py-6.0.0b9/gnosis/eth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.342859 safe-eth-py-6.0.0b9/gnosis/eth/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107388 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/clients/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/clients/test_sourcify_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.342859 safe-eth-py-6.0.0b9/gnosis/eth/tests/eip712/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13315 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/eip712/test_eip712.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/ethereum_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.346859 safe-eth-py-6.0.0b9/gnosis/eth/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31306 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10570 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (127)   792720 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92795 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)   171076 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.346859 safe-eth-py-6.0.0b9/gnosis/eth/tests/oracles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/oracles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/oracles/test_kyber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61105 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/test_ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/test_multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21137 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/test_oracles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/eth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.346859 safe-eth-py-6.0.0b9/gnosis/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/protocol/gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/protocol/order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.346859 safe-eth-py-6.0.0b9/gnosis/protocol/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/protocol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/protocol/tests/test_gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.350859 safe-eth-py-6.0.0b9/gnosis/safe/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45909 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.350859 safe-eth-py-6.0.0b9/gnosis/safe/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/api/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/api/relay_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/api/transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11447 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10479 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36883 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/safe_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101026 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/safe_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9885 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.354859 safe-eth-py-6.0.0b9/gnosis/safe/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.354859 safe-eth-py-6.0.0b9/gnosis/safe/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17981 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/safe_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_multi_send.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.354859 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_proxy_factory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_proxy_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7510 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32455 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16674 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14117 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12995 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_safe_v1_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_safe_v1_3_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/test_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/safe/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.354859 safe-eth-py-6.0.0b9/gnosis/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/gnosis/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 12:28:48.354859 safe-eth-py-6.0.0b9/safe_eth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2023-12-12 12:28:48.000000 safe-eth-py-6.0.0b9/safe_eth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2023-12-12 12:28:48.000000 safe-eth-py-6.0.0b9/safe_eth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 12:28:48.000000 safe-eth-py-6.0.0b9/safe_eth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-12 12:28:48.000000 safe-eth-py-6.0.0b9/safe_eth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-12 12:28:48.000000 safe-eth-py-6.0.0b9/safe_eth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2023-12-12 12:28:48.354859 safe-eth-py-6.0.0b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-12 12:28:36.000000 safe-eth-py-6.0.0b9/setup.py
```

### Comparing `safe-eth-py-6.0.0b8/LICENSE` & `safe-eth-py-6.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/PKG-INFO` & `safe-eth-py-6.0.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-eth-py
-Version: 6.0.0b8
+Version: 6.0.0b9
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `safe-eth-py-6.0.0b8/README.rst` & `safe-eth-py-6.0.0b9/README.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/docs/Makefile` & `safe-eth-py-6.0.0b9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/docs/make.bat` & `safe-eth-py-6.0.0b9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/docs/source/conf.py` & `safe-eth-py-6.0.0b9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/docs/source/gnosis.eth.clients.rst` & `safe-eth-py-6.0.0b9/docs/source/gnosis.eth.clients.rst`

 * *Files 11% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 -------------------------------------------
 
 .. automodule:: gnosis.eth.clients.etherscan_client
    :members:
    :undoc-members:
    :show-inheritance:
 
-gnosis.eth.clients.sourcify module
+gnosis.eth.clients.sourcify_client module
 ----------------------------------
 
-.. automodule:: gnosis.eth.clients.sourcify
+.. automodule:: gnosis.eth.clients.sourcify_client
    :members:
    :undoc-members:
    :show-inheritance:
 
 Module contents
 ---------------
```

### Comparing `safe-eth-py-6.0.0b8/docs/source/gnosis.eth.django.rst` & `safe-eth-py-6.0.0b9/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/docs/source/gnosis.eth.oracles.abis.rst` & `safe-eth-py-6.0.0b9/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/docs/source/gnosis.eth.rst` & `safe-eth-py-6.0.0b9/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/docs/source/gnosis.safe.rst` & `safe-eth-py-6.0.0b9/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/docs/source/index.rst` & `safe-eth-py-6.0.0b9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/docs/source/quickstart.rst` & `safe-eth-py-6.0.0b9/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/__init__.py` & `safe-eth-py-6.0.0b9/gnosis/eth/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/clients/blockscout_client.py` & `safe-eth-py-6.0.0b9/gnosis/eth/clients/blockscout_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,17 @@
         EthereumNetwork.TENET: "https://tenetscan.io/graphiql",
         EthereumNetwork.TENET_TESTNET: "https://testnet.tenetscan.io/graphiql",
         EthereumNetwork.VELAS_EVM_MAINNET: "https://evmexplorer.velas.com/graphiql",
         EthereumNetwork.CRONOS_MAINNET_BETA: "https://cronos.org/explorer/graphiql",
         EthereumNetwork.CRONOS_TESTNET: "https://cronos.org/explorer/testnet3/graphiql",
         EthereumNetwork.THUNDERCORE_MAINNET: "https://explorer-mainnet.thundercore.com/graphiql",
         EthereumNetwork.THUNDERCORE_TESTNET: "https://explorer-testnet.thundercore.com/graphiql",
+        EthereumNetwork.PGN_MAINNET: "https://explorer.publicgoods.network/graphiql",
+        EthereumNetwork.PGN_TESTNET: "https://explorer.sepolia.publicgoods.network/graphiql",
+        EthereumNetwork.ARTHERA_TESTNET: "https://explorer-test.arthera.net/graphiql",
     }
 
     def __init__(self, network: EthereumNetwork):
         self.network = network
         self.grahpql_url = self.NETWORK_WITH_URL.get(network)
         if self.grahpql_url is None:
             raise BlockScoutConfigurationProblem(
```

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/clients/etherscan_client.py` & `safe-eth-py-6.0.0b9/gnosis/eth/clients/etherscan_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/clients/sourcify.py` & `safe-eth-py-6.0.0b9/gnosis/eth/clients/sourcify_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,57 @@
 from typing import Any, Dict, List, Optional
 from urllib.parse import urljoin
 
 import requests
 
+from gnosis.util import cache
+
 from .. import EthereumNetwork
 from ..utils import fast_is_checksum_address
 from .contract_metadata import ContractMetadata
 
 
-class Sourcify:
+class SourcifyClientException(Exception):
+    pass
+
+
+class SourcifyClientConfigurationProblem(Exception):
+    pass
+
+
+class SourcifyClient:
     """
     Get contract metadata from Sourcify. Matches can be full or partial:
 
       - Full: Both the source files as well as the meta data files were an exact match between the deployed bytecode
         and the published files.
       - Partial: Source code compiles to the same bytecode and thus the contract behaves in the same way,
         but the source code can be different: Variables can have misleading names,
         comments can be different and especially the NatSpec comments could have been modified.
 
     """
 
     def __init__(
         self,
         network: EthereumNetwork = EthereumNetwork.MAINNET,
-        base_url: str = "https://repo.sourcify.dev/",
+        base_url_api: str = "https://sourcify.dev",
+        base_url_repo: str = "https://repo.sourcify.dev/",
         request_timeout: int = 10,
     ):
         self.network = network
-        self.base_url = base_url
+        self.base_url_api = base_url_api
+        self.base_url_repo = base_url_repo
         self.http_session = self._prepare_http_session()
         self.request_timeout = request_timeout
 
+        if not self.is_chain_supported(network.value):
+            raise SourcifyClientConfigurationProblem(
+                f"Network {network.name} - {network.value} not supported"
+            )
+
     def _prepare_http_session(self) -> requests.Session:
         """
         Prepare http session with custom pooling. See:
         https://urllib3.readthedocs.io/en/stable/advanced-usage.html
         https://docs.python-requests.org/en/v1.2.3/api/#requests.adapters.HTTPAdapter
         https://web3py.readthedocs.io/en/stable/providers.html#httpprovider
         """
@@ -59,24 +76,32 @@
     def _do_request(self, url: str) -> Optional[Dict[str, Any]]:
         response = self.http_session.get(url, timeout=self.request_timeout)
         if not response.ok:
             return None
 
         return response.json()
 
+    def is_chain_supported(self, chain_id: int) -> bool:
+        return chain_id in (int(chain["chainId"]) for chain in self.get_chains())
+
+    @cache
+    def get_chains(self) -> Dict[str, Any]:
+        url = urljoin(self.base_url_api, "/server/chains")
+        return self._do_request(url)
+
     def get_contract_metadata(
         self, contract_address: str
     ) -> Optional[ContractMetadata]:
         assert fast_is_checksum_address(
             contract_address
         ), "Expecting a checksummed address"
 
         for match_type in ("full_match", "partial_match"):
             url = urljoin(
-                self.base_url,
+                self.base_url_repo,
                 f"/contracts/{match_type}/{self.network.value}/{contract_address}/metadata.json",
             )
             metadata = self._do_request(url)
             if metadata:
                 abi = self._get_abi_from_metadata(metadata)
                 name = self._get_name_from_metadata(metadata)
                 return ContractMetadata(name, abi, match_type == "partial_match")
```

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/constants.py` & `safe-eth-py-6.0.0b9/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/__init__.py` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/CPKFactory.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/DelegateConstructorProxy.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ERC1155.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ERC1155.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ERC20.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ERC20.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ERC20TestToken.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ERC721.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ERC721.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/MultiSend.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/MultiSend.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/PayingProxy.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/Proxy_V1_0_0.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/Proxy_V1_1_1.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/Proxy_V1_3_0.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/Proxy_V1_4_1.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/Proxy_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/Safe_V1_4_1.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/Safe_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/kyber_network_proxy.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/multicall.py` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/uniswap_exchange.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/uniswap_factory.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/uniswap_v2_factory.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/uniswap_v2_pair.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/abis/uniswap_v2_router.json` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/abis/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/contracts/contract_base.py` & `safe-eth-py-6.0.0b9/gnosis/eth/contracts/contract_base.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/django/admin.py` & `safe-eth-py-6.0.0b9/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/django/forms.py` & `safe-eth-py-6.0.0b9/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/django/models.py` & `safe-eth-py-6.0.0b9/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/django/serializers.py` & `safe-eth-py-6.0.0b9/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/django/tests/models.py` & `safe-eth-py-6.0.0b9/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/django/tests/test_forms.py` & `safe-eth-py-6.0.0b9/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/django/tests/test_models.py` & `safe-eth-py-6.0.0b9/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/django/tests/test_serializers.py` & `safe-eth-py-6.0.0b9/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/eip712/__init__.py` & `safe-eth-py-6.0.0b9/gnosis/eth/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/ethereum_client.py` & `safe-eth-py-6.0.0b9/gnosis/eth/ethereum_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/ethereum_network.py` & `safe-eth-py-6.0.0b9/gnosis/eth/ethereum_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,14 +182,15 @@
     THETA_AMBER_TESTNET = 364
     THETA_TESTNET = 365
     PULSECHAIN_MAINNET = 369
     LISINSKI = 385
     HYPERONCHAIN_TESTNET = 400
     SX_NETWORK_MAINNET = 416
     OPTIMISM_GOERLI_TESTNET = 420
+    PGN_MAINNET = 424
     ZEETH_CHAIN = 427
     RUPAYA = 499
     CAMINO_C_CHAIN = 500
     COLUMBUS_TEST_NETWORK = 501
     DOUBLE_A_CHAIN_MAINNET = 512
     DOUBLE_A_CHAIN_TESTNET = 513
     GEAR_ZERO_NETWORK_MAINNET = 516
@@ -472,14 +473,15 @@
     SMART_BITCOIN_CASH = 10000
     SMART_BITCOIN_CASH_TESTNET = 10001
     GON_CHAIN = 10024
     JAPAN_OPEN_CHAIN_TESTNET = 10081
     SJATSH = 10086
     BLOCKCHAIN_GENESIS_MAINNET = 10101
     CHIADO_TESTNET = 10200
+    ARTHERA_TESTNET = 10243
     _0XTADE = 10248
     NUMBERS_MAINNET = 10507
     NUMBERS_TESTNET = 10508
     CRYPTOCOINPAY = 10823
     QUADRANS_BLOCKCHAIN = 10946
     QUADRANS_BLOCKCHAIN_TESTNET = 10947
     ASTRA = 11110
@@ -557,14 +559,15 @@
     GTON_TESTNET = 50021
     SARDIS_MAINNET = 51712
     DFK_CHAIN = 53935
     HAQQ_CHAIN_TESTNET = 54211
     REI_CHAIN_MAINNET = 55555
     REI_CHAIN_TESTNET = 55556
     BOBA_BNB_MAINNET = 56288
+    PGN_TESTNET = 58008
     LINEA_TESTNET = 59140
     LINEA = 59144
     THINKIUM_TESTNET_CHAIN_0 = 60000
     THINKIUM_TESTNET_CHAIN_1 = 60001
     THINKIUM_TESTNET_CHAIN_2 = 60002
     THINKIUM_TESTNET_CHAIN_103 = 60103
     ETICA_MAINNET = 61803
```

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/exceptions.py` & `safe-eth-py-6.0.0b9/gnosis/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/multicall.py` & `safe-eth-py-6.0.0b9/gnosis/eth/multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/__init__.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/aave_abis.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/balancer_abis.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/cream_abis.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/curve_abis.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/mooniswap_abis.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/uniswap_v3.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/yearn_abis.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/abis/zerion_abis.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/cowswap.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/cowswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/kyber.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/oracles.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/oracles.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/superfluid.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/sushiswap.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/uniswap_v3.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/oracles/utils.py` & `safe-eth-py-6.0.0b9/gnosis/eth/oracles/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/clients/mocks.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/clients/test_blockscout_client.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/clients/test_etherscan_client.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/eip712/test_eip712.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/eip712/test_eip712.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/ethereum_test_case.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/ethereum_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/mocks/mock_internal_txs.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/mocks/mock_log_receipts.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/mocks/mock_trace_block.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/mocks/mock_trace_block.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/mocks/mock_trace_filter.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/oracles/test_cowswap.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/oracles/test_kyber.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/oracles/test_superfluid.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/oracles/test_sushiswap.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/test_ethereum_client.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/test_ethereum_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/test_multicall.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/test_oracles.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/test_utils.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/tests/utils.py` & `safe-eth-py-6.0.0b9/gnosis/eth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/eth/utils.py` & `safe-eth-py-6.0.0b9/gnosis/eth/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,14 @@
     """
     return fast_to_checksum_address(generate_contract_address(HexBytes(address), nonce))
 
 
 def mk_contract_address_2(
     from_: Union[str, bytes], salt: Union[str, bytes], init_code: Union[str, bytes]
 ) -> ChecksumAddress:
-
     """
     Generate expected contract address when using EVM CREATE2.
 
     :param from_: The address which is creating this new address (need to be 20 bytes)
     :param salt: A salt (32 bytes)
     :param init_code: A init code of the contract being created
     :return: Address of the new contract
```

### Comparing `safe-eth-py-6.0.0b8/gnosis/protocol/gnosis_protocol_api.py` & `safe-eth-py-6.0.0b9/gnosis/protocol/gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/protocol/order.py` & `safe-eth-py-6.0.0b9/gnosis/protocol/order.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/protocol/tests/test_gnosis_protocol_api.py` & `safe-eth-py-6.0.0b9/gnosis/protocol/tests/test_gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/__init__.py` & `safe-eth-py-6.0.0b9/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/addresses.py` & `safe-eth-py-6.0.0b9/gnosis/safe/addresses.py`

 * *Files 1% similar despite different names*

```diff
@@ -633,14 +633,28 @@
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 237435759, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 237435774, "1.3.0"),
     ],
     EthereumNetwork.TELOS_EVM_TESTNET: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 194005796, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 194005824, "1.3.0"),
     ],
+    EthereumNetwork.PGN_MAINNET: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 344345, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 344348, "1.3.0"),
+    ],
+    EthereumNetwork.PGN_TESTNET: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 1774114, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 1774116, "1.3.0"),
+    ],
+    EthereumNetwork.ARTHERA_TESTNET: [
+        ("0x29fcB43b46531BcA003ddC8FCB67FFE91900C762", 4186405, "1.4.1+L2"),
+        ("0x41675C099F32341bf84BFc5382aF534df5C7461a", 4186415, "1.4.1"),
+        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 119967, "1.3.0+L2"),
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 119968, "1.3.0"),
+    ],
 }
 
 PROXY_FACTORIES: Dict[EthereumNetwork, List[Tuple[str, int]]] = {
     EthereumNetwork.MAINNET: [
         ("0x4e1DCf7AD4e460CfD30791CCC4F9c8a4f820ec67", 17440707),  # v1.4.1
         (
             "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
@@ -1056,8 +1070,18 @@
     ],
     EthereumNetwork.TELOS_EVM_MAINNET: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 237435678),  # v1.3.0
     ],
     EthereumNetwork.TELOS_EVM_TESTNET: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 194005709),  # v1.3.0
     ],
+    EthereumNetwork.PGN_MAINNET: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 344314),  # v1.3.0
+    ],
+    EthereumNetwork.PGN_TESTNET: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 1774097),  # v1.3.0
+    ],
+    EthereumNetwork.ARTHERA_TESTNET: [
+        ("0x4e1DCf7AD4e460CfD30791CCC4F9c8a4f820ec67", 4186337),  # v1.4.1
+        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 119959),  # v1.3.0
+    ],
 }
```

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/api/base_api.py` & `safe-eth-py-6.0.0b9/gnosis/safe/api/base_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/api/relay_service_api.py` & `safe-eth-py-6.0.0b9/gnosis/safe/api/relay_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/api/transaction_service_api.py` & `safe-eth-py-6.0.0b9/gnosis/safe/api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/exceptions.py` & `safe-eth-py-6.0.0b9/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/multi_send.py` & `safe-eth-py-6.0.0b9/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/proxy_factory.py` & `safe-eth-py-6.0.0b9/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/safe.py` & `safe-eth-py-6.0.0b9/gnosis/safe/safe.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/safe_create2_tx.py` & `safe-eth-py-6.0.0b9/gnosis/safe/safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/safe_creator.py` & `safe-eth-py-6.0.0b9/gnosis/safe/safe_creator.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/safe_deployments.py` & `safe-eth-py-6.0.0b9/gnosis/safe/safe_deployments.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/safe_signature.py` & `safe-eth-py-6.0.0b9/gnosis/safe/safe_signature.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/safe_tx.py` & `safe-eth-py-6.0.0b9/gnosis/safe/safe_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/serializers.py` & `safe-eth-py-6.0.0b9/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/signatures.py` & `safe-eth-py-6.0.0b9/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/api/test_transaction_service_api.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/safe_test_case.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/test_addresses.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/test_addresses.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/test_multi_send.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/test_safe.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/test_safe_create2_tx.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/test_safe_signature.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/test_safe_signature.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/test_safe_tx.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/test_safe_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/test_safe_v1_0_0.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/test_safe_v1_0_0.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/test_safe_v1_3_0.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/test_safe_v1_3_0.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/test_serializers.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/gnosis/safe/tests/test_signatures.py` & `safe-eth-py-6.0.0b9/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-6.0.0b8/safe_eth_py.egg-info/PKG-INFO` & `safe-eth-py-6.0.0b9/safe_eth_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-eth-py
-Version: 6.0.0b8
+Version: 6.0.0b9
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `safe-eth-py-6.0.0b8/safe_eth_py.egg-info/SOURCES.txt` & `safe-eth-py-6.0.0b9/safe_eth_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 gnosis/eth/multicall.py
 gnosis/eth/typing.py
 gnosis/eth/utils.py
 gnosis/eth/clients/__init__.py
 gnosis/eth/clients/blockscout_client.py
 gnosis/eth/clients/contract_metadata.py
 gnosis/eth/clients/etherscan_client.py
-gnosis/eth/clients/sourcify.py
+gnosis/eth/clients/sourcify_client.py
 gnosis/eth/contracts/__init__.py
 gnosis/eth/contracts/contract_base.py
 gnosis/eth/contracts/abis/CPKFactory.json
 gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json
 gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json
 gnosis/eth/contracts/abis/DelegateConstructorProxy.json
 gnosis/eth/contracts/abis/ERC1155.json
@@ -109,15 +109,15 @@
 gnosis/eth/tests/test_oracles.py
 gnosis/eth/tests/test_utils.py
 gnosis/eth/tests/utils.py
 gnosis/eth/tests/clients/__init__.py
 gnosis/eth/tests/clients/mocks.py
 gnosis/eth/tests/clients/test_blockscout_client.py
 gnosis/eth/tests/clients/test_etherscan_client.py
-gnosis/eth/tests/clients/test_sourcify.py
+gnosis/eth/tests/clients/test_sourcify_client.py
 gnosis/eth/tests/eip712/__init__.py
 gnosis/eth/tests/eip712/test_eip712.py
 gnosis/eth/tests/mocks/__init__.py
 gnosis/eth/tests/mocks/mock_internal_txs.py
 gnosis/eth/tests/mocks/mock_log_receipts.py
 gnosis/eth/tests/mocks/mock_trace_block.py
 gnosis/eth/tests/mocks/mock_trace_filter.py
```

### Comparing `safe-eth-py-6.0.0b8/setup.cfg` & `safe-eth-py-6.0.0b9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = safe-eth-py
-version = 6.0.0b8
+version = 6.0.0b9
 description = Safe Ecosystem Foundation utilities for Ethereum projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
```

