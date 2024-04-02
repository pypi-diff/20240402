# Comparing `tmp/tanx-connector-2.0.1.tar.gz` & `tmp/tanx-connector-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ubuntu/code/tanx-connector-python/dist/.tmp-qruslb0c/tanx-connector-2.0.1.tar", last modified: Sat Mar 23 03:10:13 2024, max compression
+gzip compressed data, was "tanx-connector-2.0.2.tar", last modified: Tue Apr  2 07:55:02 2024, max compression
```

## Comparing `tanx-connector-2.0.1.tar` & `tanx-connector-2.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-23 03:10:13.353998 tanx-connector-2.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1063 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20246 2024-03-23 03:10:13.353998 tanx-connector-2.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17816 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1526 2024-03-23 03:08:29.000000 tanx-connector-2.0.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-23 03:10:13.353998 tanx-connector-2.0.1/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-23 03:10:13.345998 tanx-connector-2.0.1/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-23 03:10:13.353998 tanx-connector-2.0.1/src/tanx_connector.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20246 2024-03-23 03:10:13.000000 tanx-connector-2.0.1/src/tanx_connector.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2024-03-23 03:10:13.000000 tanx-connector-2.0.1/src/tanx_connector.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-23 03:10:13.000000 tanx-connector-2.0.1/src/tanx_connector.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      146 2024-03-23 03:10:13.000000 tanx-connector-2.0.1/src/tanx_connector.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-03-23 03:10:13.000000 tanx-connector-2.0.1/src/tanx_connector.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-23 03:10:13.349998 tanx-connector-2.0.1/src/tanxconnector/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2024-03-23 03:08:29.000000 tanx-connector-2.0.1/src/tanxconnector/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-23 03:10:13.353998 tanx-connector-2.0.1/src/tanxconnector/bin/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/bin/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      577 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/bin/blockchain_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4840 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/bin/erc20_abi.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1693 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/bin/math_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   102707 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/bin/pedersen_params.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7553 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/bin/polygon_deposit.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5278 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/bin/signature.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    64164 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/bin/starkex_abi_main.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    61398 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/bin/starkex_abi_test.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28194 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1043 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1044 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/exception.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1135 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/session.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4006 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/typings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4768 2024-03-23 02:56:06.000000 tanx-connector-2.0.1/src/tanxconnector/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2766 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/src/tanxconnector/wsclient.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-23 03:10:13.353998 tanx-connector-2.0.1/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30174 2024-03-22 13:14:02.000000 tanx-connector-2.0.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22820 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20390 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:55:02.550124 tanx-connector-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/src/tanx_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22820 2024-04-02 07:55:02.000000 tanx-connector-2.0.2/src/tanx_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-02 07:55:02.000000 tanx-connector-2.0.2/src/tanx_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:55:02.000000 tanx-connector-2.0.2/src/tanx_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 07:55:02.000000 tanx-connector-2.0.2/src/tanx_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 07:55:02.000000 tanx-connector-2.0.2/src/tanx_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/src/tanxconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/src/tanxconnector/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/blockchain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/erc20_abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102707 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/pedersen_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/polygon_deposit.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64164 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/starkex_abi_main.json
+-rw-r--r--   0 runner    (1001) docker     (127)    61398 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/bin/starkex_abi_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28194 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/src/tanxconnector/wsclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:55:02.554124 tanx-connector-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    30174 2024-04-02 07:54:58.000000 tanx-connector-2.0.2/tests/test_client.py
```

### Comparing `tanx-connector-2.0.1/LICENSE` & `tanx-connector-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/PKG-INFO` & `tanx-connector-2.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanx-connector
-Version: 2.0.1
+Version: 2.0.2
 Summary: The official Python connector for Tanx's API
 Author: tanX
 License: MIT License
         
         Copyright (c) 2023 Tanx Fi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -108,37 +108,38 @@
   - [WebSocket Client](#websocket-client)
     - [Connect](#connect)
     - [Subscribe](#subscribe)
     - [Unsubscribe](#unsubscribe)
     - [Disconnect](#disconnect)
     - [Usage](#usage)
   - [Error Handling](#error-handling)
-  - [Internal Transfer](#internal-transfer)
   - [Deposit](#deposit)
-    - [Ethereum Network Deposit](#ehtereum-network-deposit)
+    - [Ethereum Network Deposit](#ethereum-network-deposit)
     - [Polygon Network Deposit](#polygon-network-deposit)
     - [List Deposits](#list-deposits)
   - [Withdrawal](#withdrawal)
-    - [Normal Withdrawal](#normal-withdrawal)
+    - [Normal Withdrawal](#normal-withdrawal-only-for-ethereum-network)
     - [Fast Withdrawal](#fast-withdrawal)
+  - [Internal Transfer](#internal-transfer)
+    - [Available Methods](#available-methods)
 
 ## Installation
 
 First go to the [tanX Website](https://www.tanx.fi/) and create an account with your wallet.
 
 Install the package using pip.
 
 ```python
 pip install tanx-connector
 ```
 
 ## Quickstart
 
 Make sure that tanxconnector is [installed](#installation) and up-to-date.
-Also make sure you have an account on the [mainnet](https://www.tanx.fi/) or [testnet](https://api-testnet.tanx.fi) website.
+Also make sure you have an account on the [mainnet](https://trade.tanx.fi/) or [testnet](https://testnet.tanx.fi/) website.
 
 To get quickly started, try running the simple example for creating and fetching the order once logged in.
 
 ```python
 from tanxconnector import Client
 
 ETH_ADDRESS = "(your eth wallet address)"
@@ -173,15 +174,15 @@
 ### L2 Key Pair
 
 L2 Key Pair generation isn't currently available in the TanX Python SDK. 
 
 To get the L2 Key Pair, follow any of the two steps:
 
 1. Get the Key Pair from the [TanX official website](https://trade.tanx.fi/)'s Account Settings Tab once wallet is connected. Refer to the image below for more reference. Click on `Settings -> tanX key -> Show Keys` and Sign the request to get the keys. Copy these keys and store it securely.
-<img src="images/tanx-key.png">
+<img src="https://raw.githubusercontent.com/tanx-libs/tanx-connector-python/main/images/tanx-key.png">
 
 2. Generate the L2 key pair using the [TanX Nodejs SDK](https://github.com/tanx-libs/tanx-connector-nodejs). For generation using the Node SDK, refer to [this section](https://github.com/tanx-libs/tanx-connector-nodejs#create-l2-key-pair) in the documentation of the Nodejs SDK.
 
 ### Rest Client
 
 Import the REST Client
 
@@ -190,16 +191,16 @@
 ```
 
 Create a new instance
 
 ```python
 client = Client()
 # or
-client = Client() 
-# default is mainnet
+client = Client('testnet')
+# default is mainnet, can pass explicitly as well
 ```
 
 ### General Endpoints
 
 #### Test connectivity
 
 `GET /sapi/v1/health/`
@@ -472,80 +473,54 @@
     # call methods
 except tanxconnector.exception.AuthenticationError as exc:
     print(exc)
 except requests.exceptions.HTTPError as exc:
     print(exc.response.json())
 ```
 
-### Internal Transfer
-
-Users will be able to seamlessly transfer assets from their CEXs or other chains with minimal fees.
-
-To get started with the feature, follow these two steps:
-
-1. Reach out to tanX (support@tanx.fi) to get the organization key and API key.
-
-2. Generate the L2 key pair with your private key
+### Deposit
 
-#### Available methods:
+#### Ethereum Network Deposit
 
-1. To process the internal transfer, call the `intiate_and_process_internal_transfers` method and pass the necessary arguments:
+This method involves using a custom provider and signer, which can be created using the web3.py library. The `stark_public_key` mentioned in the code should be obtained using the steps described in the [L2 Key Pair](#l2-key-pair) section of the documentation. Here's the code snippet for this method:
 
 ```python
-key_pair = {
-  'stark_public_key': '(your stark public key here)'
-  'stark_private_key': '(your stark private key here)'
-}
+# Note: Please use web3>=6.0.0, <7.0.0
+from web3 import Web3, Account
 
-ETH_ADDRESS_2 = '(destination Eth wallet address here)'
+provider = Web3(Web3.HTTPProvider(RPC_PROVIDER))
+signer = Account.from_key(PRIVATE_KEY)
 
-internal_transfer_response = client.intiate_and_process_internal_transfers(
-  key_pair=key_pair,
-  organization_key=TANX_ORGANIZATION_KEY,
-  api_key=TANX_API_KEY,
-  currency='usdc',
-  amount=1,
-  destination_address=ETH_ADDRESS_2,
-  client_reference_id=1
+deposit_res_with_stark_keys = client.deposit_from_ethereum_network_with_stark_key(
+  signer,
+  provider,
+  f'0x{stark_public_key}',
+  0.0001,
+  'eth'
 )
 ```
 
-2. Retrieve a list of transfers initiated by the authenticated user:
+For any `ERC20` token (which is not native for the network, like usdc), first allow unlimited allowance for that token using the `approve_unlimited_allowance_ethereum_network` method.
 
 ```python
-internal_trasnfers_list = client.list_internal_transfers({
-  'limit': 10,
-  'offset': 10
-})
-```
-
-3. Retrieve an internal transfer using its client reference id:
-
-```python
-internal_transfer_by_id = client.get_internal_transfer_by_client_id(client_reference_id)
-```
+# Note: Please use web3>=6.0.0, <7.0.0
+from web3 import Web3, Account
 
-4. Check if a user exists by their destination address.
+provider = Web3(Web3.HTTPProvider(RPC_PROVIDER))
+signer = Account.from_key(PRIVATE_KEY)
 
-```python
-check_user_res = client.check_internal_transfer_user_exists(
-  TANX_ORGANIZATION_KEY,
-  TANX_API_KEY,
-  destination_address,
-)
+# approval for unlimited allowance for ERC20 contracts
+allowance = client.approve_unlimited_allowance_ethereum_network('usdc', signer, provider)
+print(allowance) # prints the hash for the allowance transaction, check this on the etherscan/sepoliascan for success.
 ```
 
-### Deposit
-
-#### Ethereum Network Deposit
-
-This method involves using a custom provider and signer, which can be created using the web3.py library. The `stark_public_key` mentioned in the code should be obtained using the steps described in the [L2 Key Pair](#l2-key-pair) section of the documentation. Here's the code snippet for this method:
+Once the allowance is success, transactions can be made for `ERC20` token on ETH network.
 
 ```python
-# Note: Please use web3 version 5.25.0
+# Note: Please use web3>=6.0.0, <7.0.0
 from web3 import Web3, Account
 
 provider = Web3(Web3.HTTPProvider(RPC_PROVIDER))
 signer = Account.from_key(PRIVATE_KEY)
 
 deposit_res_with_stark_keys = client.deposit_from_ethereum_network_with_stark_key(
   signer,
@@ -570,16 +545,54 @@
   'matic',  # Coin Symbol
   0.00001 # Amount to be deposited
 )
 ```
 
 2. Using Custom Provider and Signer:
 <br>This method involves using a custom provider and signer, which can be created using the web3.py library. Also, its important to inject a middleware at the 0th layer of the middleware onion for the provider ([See Reference](https://web3py.readthedocs.io/en/stable/middleware.html#proof-of-authority)). Here's the code snippet for this method:
+
+```python
+# Note: Please use web3>=6.0.0, <7.0.0
+from web3 import Web3, Account
+from web3.middleware.geth_poa import geth_poa_middleware
+
+provider = Web3(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON))
+provider.middleware_onion.inject(geth_poa_middleware, layer=0)
+
+signer = Account.from_key(PRIVATE_KEY)
+
+polygon_deposit_res = client.deposit_from_polygon_network_with_signer(
+  signer, # Signer Created above
+  provider, # Provider created above
+  'matic',  # Enter the coin symbol
+  0.0001, # Amount to be deposited
+)
+```
+
+For any `ERC20` token (which is not native for the network, like btc), first allow unlimited allowance for that token using the `approve_unlimited_allowance_polygon_network` method.
+
+```python
+# Note: Please use web3>=6.0.0, <7.0.0
+from web3 import Web3, Account
+from web3.middleware.geth_poa import geth_poa_middleware
+
+provider = Web3(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON))
+provider.middleware_onion.inject(geth_poa_middleware, layer=0)
+
+signer = Account.from_key(PRIVATE_KEY)
+
+# approval for unlimited allowance for ERC20 contracts
+allowance = client.approve_unlimited_allowance_polygon_network(coin='btc', signer=signer, w3=provider)
+print(allowance)  # prints the hash for the allowance, check on polygon scan for success
+```
+
+Once the allowance is success, transactions can be made for `ERC20` token on POLYGON network.
+
 ```python
-# Note: Please use ethers version 5.25.0.
+# Note: Please use web3>=6.0.0, <7.0.0
 from web3 import Web3, Account
 from web3.middleware.geth_poa import geth_poa_middleware
 
 provider = Web3(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON))
 provider.middleware_onion.inject(geth_poa_middleware, layer=0)
 
 signer = Account.from_key(PRIVATE_KEY)
@@ -636,22 +649,22 @@
 # 2. WAIT for up to 24 hours.
 # 3. Check whether the withdrawn balance is pending by calling the "getPendingNormalWithdrawalAmountByCoin" function with the required parameters.
 pending_balance = client.get_pending_normal_withdrawal_amount_by_coin(
   'eth', # Enter the coin symbol
   eth_address, # User public eth address
   signer, # The signer created above
   provider, # The provider created above
-  gas_price, # max gas price for the transaction
 )
 # 4. In the final step, if you find the balance is more than 0, you can use the "completeNormalWithdrawal" function to withdraw the cumulative amount to your ETH wallet.
 complete_normal_withdrawal_res = client.complete_normal_withdrawal(
   'eth', # Enter the coin symbol
   ethAddress, # User public eth address
   signer, # The signer created above
   provider, # The provider created above
+  gas_price, # max gas price for the transaction
 )
 
 #Get a list of withdrawals
 withdrawals_list = client.list_normal_withdrawals({
   page: 2, # This is an optional field
 })
 ```
@@ -690,7 +703,65 @@
 3. Get a list of fast withdrawals
 ```python
 fast_withdrawals_list = client.list_fast_withdrawals({
   'page': 2, # This is an optional field
   'network': 'POLYGON'  # This is an optional field
 })
 ```
+
+### Internal Transfer
+
+Users will be able to seamlessly transfer assets from their CEXs or other chains with minimal fees.
+
+To get started with the feature, follow these two steps:
+
+1. Reach out to tanX (support@tanx.fi) to get the organization key and API key.
+
+2. Generate the L2 key pair with your private key
+
+#### Available methods:
+
+1. To process the internal transfer, call the `intiate_and_process_internal_transfers` method and pass the necessary arguments:
+
+```python
+key_pair = {
+  'stark_public_key': '(your stark public key here)'
+  'stark_private_key': '(your stark private key here)'
+}
+
+ETH_ADDRESS_2 = '(destination Eth wallet address here)'
+
+internal_transfer_response = client.intiate_and_process_internal_transfers(
+  key_pair=key_pair,
+  organization_key=TANX_ORGANIZATION_KEY,
+  api_key=TANX_API_KEY,
+  currency='usdc',
+  amount=1,
+  destination_address=ETH_ADDRESS_2,
+  client_reference_id=1
+)
+```
+
+2. Retrieve a list of transfers initiated by the authenticated user:
+
+```python
+internal_trasnfers_list = client.list_internal_transfers({
+  'limit': 10,
+  'offset': 10
+})
+```
+
+3. Retrieve an internal transfer using its client reference id:
+
+```python
+internal_transfer_by_id = client.get_internal_transfer_by_client_id(client_reference_id)
+```
+
+4. Check if a user exists by their destination address.
+
+```python
+check_user_res = client.check_internal_transfer_user_exists(
+  TANX_ORGANIZATION_KEY,
+  TANX_API_KEY,
+  destination_address,
+)
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tanx-connector Version: 2.0.1 Summary: The official
+Metadata-Version: 2.1 Name: tanx-connector Version: 2.0.2 Summary: The official
 Python connector for Tanx's API Author: tanX License: MIT License Copyright (c)
 2023 Tanx Fi Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
@@ -47,24 +47,25 @@
 (#balance-details-private-) - [Profit and Loss Details (Private ð)](#profit-
 and-loss-details-private-) - [Create order (Private ð)](#create-order-
 private-) - [Get Order (Private ð)](#get-order-private-) - [List Orders
 (Private ð)](#list-orders-) - [Cancel Order (Private ð)](#cancel-order-
 private-) - [List Trades (Private ð)](#list-trades-private-) - [WebSocket
 Client](#websocket-client) - [Connect](#connect) - [Subscribe](#subscribe) -
 [Unsubscribe](#unsubscribe) - [Disconnect](#disconnect) - [Usage](#usage) -
-[Error Handling](#error-handling) - [Internal Transfer](#internal-transfer) -
-[Deposit](#deposit) - [Ethereum Network Deposit](#ehtereum-network-deposit) -
-[Polygon Network Deposit](#polygon-network-deposit) - [List Deposits](#list-
-deposits) - [Withdrawal](#withdrawal) - [Normal Withdrawal](#normal-withdrawal)
-- [Fast Withdrawal](#fast-withdrawal) ## Installation First go to the [tanX
+[Error Handling](#error-handling) - [Deposit](#deposit) - [Ethereum Network
+Deposit](#ethereum-network-deposit) - [Polygon Network Deposit](#polygon-
+network-deposit) - [List Deposits](#list-deposits) - [Withdrawal](#withdrawal)
+- [Normal Withdrawal](#normal-withdrawal-only-for-ethereum-network) - [Fast
+Withdrawal](#fast-withdrawal) - [Internal Transfer](#internal-transfer) -
+[Available Methods](#available-methods) ## Installation First go to the [tanX
 Website](https://www.tanx.fi/) and create an account with your wallet. Install
 the package using pip. ```python pip install tanx-connector ``` ## Quickstart
 Make sure that tanxconnector is [installed](#installation) and up-to-date. Also
-make sure you have an account on the [mainnet](https://www.tanx.fi/) or
-[testnet](https://api-testnet.tanx.fi) website. To get quickly started, try
+make sure you have an account on the [mainnet](https://trade.tanx.fi/) or
+[testnet](https://testnet.tanx.fi/) website. To get quickly started, try
 running the simple example for creating and fetching the order once logged in.
 ```python from tanxconnector import Client ETH_ADDRESS = "(your eth wallet
 address)" PRIVATE_KEY = "(your wallet's private key)" client = Client() # login
 to the network login = client.complete_login(ETH_ADDRESS, PRIVATE_KEY) # create
 an order nonce nonce: CreateOrderNonceBody = {'market': 'ethusdc', 'ord_type':
 'market', 'price': 29580.51, 'side': 'sell', 'volume': 0.0005} # create the
 order order = client.create_complete_order(nonce, stark_private_key) print
@@ -76,57 +77,58 @@
 REST apis, WebSockets are handled by Client, WsClient classes respectively. ###
 Workflow Check out the [example files](./example) to see an example workflow.
 ### L2 Key Pair L2 Key Pair generation isn't currently available in the TanX
 Python SDK. To get the L2 Key Pair, follow any of the two steps: 1. Get the Key
 Pair from the [TanX official website](https://trade.tanx.fi/)'s Account
 Settings Tab once wallet is connected. Refer to the image below for more
 reference. Click on `Settings -> tanX key -> Show Keys` and Sign the request to
-get the keys. Copy these keys and store it securely. [images/tanx-key.png]2.
-Generate the L2 key pair using the [TanX Nodejs SDK](https://github.com/tanx-
-libs/tanx-connector-nodejs). For generation using the Node SDK, refer to [this
-section](https://github.com/tanx-libs/tanx-connector-nodejs#create-l2-key-pair)
-in the documentation of the Nodejs SDK. ### Rest Client Import the REST Client
-```py from tanxconnector import Client ``` Create a new instance ```python
-client = Client() # or client = Client() # default is mainnet ``` ### General
-Endpoints #### Test connectivity `GET /sapi/v1/health/` ```python
-client.test_connection() ``` #### 24hr Price `GET /sapi/v1/market/tickers/
-` ```python client.get_24h_price('btcusdt') ``` #### Kline/Candlestick Data
-`GET /sapi/v1/market/kline/` ```python client.get_candlestick('btcusdt') ```
-#### Order Book `GET /sapi/v1/market/orderbook/` ```python client.get_orderbook
-('btcusdt') ``` #### Recent trades `GET /sapi/v1/market/trades/` ```python
-client.get_recent_trades('btcusdt') ``` #### Login Both login() and
-complete_Login() sets tokens internally. Optionally, set_access_token() and
-set_refresh_token() can be used to set tokens directly. getNonce: `POST /sapi/
-v1/auth/nonce/` login: `POST /sapi/v1/auth/login/` ```python from tanxconnector
-import sign_msg, Client client = Client() client.complete_login(ETH_ADDRESS,
-PRIVATE_KEY) # calls below functions internally, use this for ease # or nonce =
-client.get_nonce(ETH_ADDRESS) user_signature = sign_msg(nonce['payload'],
-PRIVATE_KEY) login = client.login(ETH_ADDRESS, user_signature) # or
-client.set_access_token(access_token) client.set_refresh_token(refresh_token) #
-these functions are called internally when you use login or complete_login ```
-#### Refresh Token `POST /sapi/v1/auth/token/refresh/` If refresh token is set
-(manually or by using login functions), the refresh endpoint is called
-automatically when access token expires. Optionally, you can call
-`refresh_tokens` manually by passing in refresh_token (passing it is optional,
-it'll work if has been set before). ```python res = client.refresh_tokens
-(refresh_token) ``` #### Logout Sets tokens to null ```python client.logout()
-``` #### Profile Information (Private ð) `GET /sapi/v1/user/profile/
-` ```python client.get_profile_info() ``` #### Balance details (Private ð)
-`GET /sapi/v1/user/balance/` ```python client.get_balance() ``` #### Profit and
-Loss Details (Private ð) `GET /sapi/v1/user/pnl/` ```python
-client.get_profit_and_loss() ``` #### Create order (Private ð) Order is
-created in 2 steps: 1. Create the order nonce body 2. Process the order nonce
-body with the stark private key to create the order Create Nonce Body ```py
-from tanxconnector.typings import CreateOrderNonceBody nonce:
-CreateOrderNonceBody = {'market': 'btcusdt', 'ord_type': 'market', 'price':
-29580.51, 'side': 'buy', 'volume': 0.0001} ``` Create Order create_order_nonce:
-`POST /sapi/v1/orders/nonce/` create_new_order: `POST /sapi/v1/orders/create/
-` For getting the L2 Key Pairs (Stark Keys) refer to the above [section](#l2-
-key-pair) in the documentation. ```python stark_private_key = '(Your Stark
-Private Key Here)' order = client.create_complete_order(nonce,
+get the keys. Copy these keys and store it securely. [https://
+raw.githubusercontent.com/tanx-libs/tanx-connector-python/main/images/tanx-
+key.png]2. Generate the L2 key pair using the [TanX Nodejs SDK](https://
+github.com/tanx-libs/tanx-connector-nodejs). For generation using the Node SDK,
+refer to [this section](https://github.com/tanx-libs/tanx-connector-
+nodejs#create-l2-key-pair) in the documentation of the Nodejs SDK. ### Rest
+Client Import the REST Client ```py from tanxconnector import Client ``` Create
+a new instance ```python client = Client() # or client = Client('testnet') #
+default is mainnet, can pass explicitly as well ``` ### General Endpoints ####
+Test connectivity `GET /sapi/v1/health/` ```python client.test_connection() ```
+#### 24hr Price `GET /sapi/v1/market/tickers/` ```python client.get_24h_price
+('btcusdt') ``` #### Kline/Candlestick Data `GET /sapi/v1/market/kline/
+` ```python client.get_candlestick('btcusdt') ``` #### Order Book `GET /sapi/
+v1/market/orderbook/` ```python client.get_orderbook('btcusdt') ``` #### Recent
+trades `GET /sapi/v1/market/trades/` ```python client.get_recent_trades
+('btcusdt') ``` #### Login Both login() and complete_Login() sets tokens
+internally. Optionally, set_access_token() and set_refresh_token() can be used
+to set tokens directly. getNonce: `POST /sapi/v1/auth/nonce/` login: `POST /
+sapi/v1/auth/login/` ```python from tanxconnector import sign_msg, Client
+client = Client() client.complete_login(ETH_ADDRESS, PRIVATE_KEY) # calls below
+functions internally, use this for ease # or nonce = client.get_nonce
+(ETH_ADDRESS) user_signature = sign_msg(nonce['payload'], PRIVATE_KEY) login =
+client.login(ETH_ADDRESS, user_signature) # or client.set_access_token
+(access_token) client.set_refresh_token(refresh_token) # these functions are
+called internally when you use login or complete_login ``` #### Refresh Token
+`POST /sapi/v1/auth/token/refresh/` If refresh token is set (manually or by
+using login functions), the refresh endpoint is called automatically when
+access token expires. Optionally, you can call `refresh_tokens` manually by
+passing in refresh_token (passing it is optional, it'll work if has been set
+before). ```python res = client.refresh_tokens(refresh_token) ``` #### Logout
+Sets tokens to null ```python client.logout() ``` #### Profile Information
+(Private ð) `GET /sapi/v1/user/profile/` ```python client.get_profile_info()
+``` #### Balance details (Private ð) `GET /sapi/v1/user/balance/` ```python
+client.get_balance() ``` #### Profit and Loss Details (Private ð) `GET /
+sapi/v1/user/pnl/` ```python client.get_profit_and_loss() ``` #### Create order
+(Private ð) Order is created in 2 steps: 1. Create the order nonce body 2.
+Process the order nonce body with the stark private key to create the order
+Create Nonce Body ```py from tanxconnector.typings import CreateOrderNonceBody
+nonce: CreateOrderNonceBody = {'market': 'btcusdt', 'ord_type': 'market',
+'price': 29580.51, 'side': 'buy', 'volume': 0.0001} ``` Create Order
+create_order_nonce: `POST /sapi/v1/orders/nonce/` create_new_order: `POST /
+sapi/v1/orders/create/` For getting the L2 Key Pairs (Stark Keys) refer to the
+above [section](#l2-key-pair) in the documentation. ```python stark_private_key
+= '(Your Stark Private Key Here)' order = client.create_complete_order(nonce,
 stark_private_key) # calls below functions internally, we recommend using
 createCompleteOrder for ease of use # or from tanxconnector import
 sign_order_with_stark_private_key nonce_res = client.create_order_nonce(nonce)
 msg_hash = sign_order_with_stark_private_key(stark_private_key, nonce_res
 ['payload']) order = client.create_new_order(msg_hash) ``` #### Get Order
 (Private ð) `GET /sapi/v1/orders/{order_id}/` ```python client.get_order
 (order_id) ``` #### List Orders (Private ð) `GET /sapi/v1/orders/` ```python
@@ -150,41 +152,36 @@
 ws_client.disconnect() ``` #### Usage WsClient includes a member called
 websocket which is initialized with websockets.connect(). You may use it to
 handle WebSocket operations. ```py async for message in ws_client.websocket:
 print(message) ``` ### Error Handling Errors thrown are of types
 `AuthenticationError or requests.exceptions.HTTPError`. Example ```py try: #
 call methods except tanxconnector.exception.AuthenticationError as exc: print
 (exc) except requests.exceptions.HTTPError as exc: print(exc.response.json())
-``` ### Internal Transfer Users will be able to seamlessly transfer assets from
-their CEXs or other chains with minimal fees. To get started with the feature,
-follow these two steps: 1. Reach out to tanX (support@tanx.fi) to get the
-organization key and API key. 2. Generate the L2 key pair with your private key
-#### Available methods: 1. To process the internal transfer, call the
-`intiate_and_process_internal_transfers` method and pass the necessary
-arguments: ```python key_pair = { 'stark_public_key': '(your stark public key
-here)' 'stark_private_key': '(your stark private key here)' } ETH_ADDRESS_2 = '
-(destination Eth wallet address here)' internal_transfer_response =
-client.intiate_and_process_internal_transfers( key_pair=key_pair,
-organization_key=TANX_ORGANIZATION_KEY, api_key=TANX_API_KEY, currency='usdc',
-amount=1, destination_address=ETH_ADDRESS_2, client_reference_id=1 ) ``` 2.
-Retrieve a list of transfers initiated by the authenticated user: ```python
-internal_trasnfers_list = client.list_internal_transfers({ 'limit': 10,
-'offset': 10 }) ``` 3. Retrieve an internal transfer using its client reference
-id: ```python internal_transfer_by_id =
-client.get_internal_transfer_by_client_id(client_reference_id) ``` 4. Check if
-a user exists by their destination address. ```python check_user_res =
-client.check_internal_transfer_user_exists( TANX_ORGANIZATION_KEY,
-TANX_API_KEY, destination_address, ) ``` ### Deposit #### Ethereum Network
-Deposit This method involves using a custom provider and signer, which can be
-created using the web3.py library. The `stark_public_key` mentioned in the code
-should be obtained using the steps described in the [L2 Key Pair](#l2-key-pair)
-section of the documentation. Here's the code snippet for this method:
-```python # Note: Please use web3 version 5.25.0 from web3 import Web3, Account
+``` ### Deposit #### Ethereum Network Deposit This method involves using a
+custom provider and signer, which can be created using the web3.py library. The
+`stark_public_key` mentioned in the code should be obtained using the steps
+described in the [L2 Key Pair](#l2-key-pair) section of the documentation.
+Here's the code snippet for this method: ```python # Note: Please use
+web3>=6.0.0, <7.0.0 from web3 import Web3, Account provider = Web3
+(Web3.HTTPProvider(RPC_PROVIDER)) signer = Account.from_key(PRIVATE_KEY)
+deposit_res_with_stark_keys =
+client.deposit_from_ethereum_network_with_stark_key( signer, provider, f'0x
+{stark_public_key}', 0.0001, 'eth' ) ``` For any `ERC20` token (which is not
+native for the network, like usdc), first allow unlimited allowance for that
+token using the `approve_unlimited_allowance_ethereum_network` method.
+```python # Note: Please use web3>=6.0.0, <7.0.0 from web3 import Web3, Account
 provider = Web3(Web3.HTTPProvider(RPC_PROVIDER)) signer = Account.from_key
-(PRIVATE_KEY) deposit_res_with_stark_keys =
+(PRIVATE_KEY) # approval for unlimited allowance for ERC20 contracts allowance
+= client.approve_unlimited_allowance_ethereum_network('usdc', signer, provider)
+print(allowance) # prints the hash for the allowance transaction, check this on
+the etherscan/sepoliascan for success. ``` Once the allowance is success,
+transactions can be made for `ERC20` token on ETH network. ```python # Note:
+Please use web3>=6.0.0, <7.0.0 from web3 import Web3, Account provider = Web3
+(Web3.HTTPProvider(RPC_PROVIDER)) signer = Account.from_key(PRIVATE_KEY)
+deposit_res_with_stark_keys =
 client.deposit_from_ethereum_network_with_stark_key( signer, provider, f'0x
 {stark_public_key}', 0.0001, 'usdc' ) ``` #### Polygon Network Deposit There
 are two ways to make a deposit on the Polygon network: 1. Using ETH Private Key
 and RPC URL:
 In this method, you will use an ETH private key and an RPC URL to execute a
 Polygon deposit. You'll also need to create an RPC URL using services like
 Infura, Alchemy, etc. Here's the code snippet for this method: ```python
@@ -192,20 +189,38 @@
 Use 'Polygon Mumbai' for the testnet and 'Polygon mainnet' for the mainnet.
 PRIVATE_KEY, # ETH Private Key 'matic', # Coin Symbol 0.00001 # Amount to be
 deposited ) ``` 2. Using Custom Provider and Signer:
 This method involves using a custom provider and signer, which can be created
 using the web3.py library. Also, its important to inject a middleware at the
 0th layer of the middleware onion for the provider ([See Reference](https://
 web3py.readthedocs.io/en/stable/middleware.html#proof-of-authority)). Here's
-the code snippet for this method: ```python # Note: Please use ethers version
-5.25.0. from web3 import Web3, Account from web3.middleware.geth_poa import
+the code snippet for this method: ```python # Note: Please use web3>=6.0.0,
+<7.0.0 from web3 import Web3, Account from web3.middleware.geth_poa import
 geth_poa_middleware provider = Web3(Web3.HTTPProvider
 (RPC_PROVIDER_FOR_POLYGON)) provider.middleware_onion.inject
 (geth_poa_middleware, layer=0) signer = Account.from_key(PRIVATE_KEY)
 polygon_deposit_res = client.deposit_from_polygon_network_with_signer( signer,
+# Signer Created above provider, # Provider created above 'matic', # Enter the
+coin symbol 0.0001, # Amount to be deposited ) ``` For any `ERC20` token (which
+is not native for the network, like btc), first allow unlimited allowance for
+that token using the `approve_unlimited_allowance_polygon_network` method.
+```python # Note: Please use web3>=6.0.0, <7.0.0 from web3 import Web3, Account
+from web3.middleware.geth_poa import geth_poa_middleware provider = Web3
+(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON)) provider.middleware_onion.inject
+(geth_poa_middleware, layer=0) signer = Account.from_key(PRIVATE_KEY) #
+approval for unlimited allowance for ERC20 contracts allowance =
+client.approve_unlimited_allowance_polygon_network(coin='btc', signer=signer,
+w3=provider) print(allowance) # prints the hash for the allowance, check on
+polygon scan for success ``` Once the allowance is success, transactions can be
+made for `ERC20` token on POLYGON network. ```python # Note: Please use
+web3>=6.0.0, <7.0.0 from web3 import Web3, Account from
+web3.middleware.geth_poa import geth_poa_middleware provider = Web3
+(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON)) provider.middleware_onion.inject
+(geth_poa_middleware, layer=0) signer = Account.from_key(PRIVATE_KEY)
+polygon_deposit_res = client.deposit_from_polygon_network_with_signer( signer,
 # Signer Created above provider, # Provider created above 'btc', # Enter the
 coin symbol 0.0001, # Amount to be deposited ) ``` #### List Deposits To get
 the deposit history, you can use the following code: ```python deposit_list =
 client.list_deposits({ 'page': 1, # This field is optional 'limit': 1, # This
 field is optional 'network': 'ETHEREUM' # Network for which you want to list
 the deposit history. Allowed networks are ETHEREUM & POLYGON }) ``` ###
 Withdrawal Generally, we have two modes of withdrawal: Normal Withdrawal and
@@ -224,22 +239,22 @@
 function. withdrawal_res = client.initiate_normal_withdrawal( key_pair, # The
 keyPair created for stark keys 0.0001, # Enter the amount you want to deposit
 'usdc', # Enter the coin symbol ) # 2. WAIT for up to 24 hours. # 3. Check
 whether the withdrawn balance is pending by calling the
 "getPendingNormalWithdrawalAmountByCoin" function with the required parameters.
 pending_balance = client.get_pending_normal_withdrawal_amount_by_coin( 'eth', #
 Enter the coin symbol eth_address, # User public eth address signer, # The
-signer created above provider, # The provider created above gas_price, # max
-gas price for the transaction ) # 4. In the final step, if you find the balance
-is more than 0, you can use the "completeNormalWithdrawal" function to withdraw
-the cumulative amount to your ETH wallet. complete_normal_withdrawal_res =
-client.complete_normal_withdrawal( 'eth', # Enter the coin symbol ethAddress, #
-User public eth address signer, # The signer created above provider, # The
-provider created above ) #Get a list of withdrawals withdrawals_list =
-client.list_normal_withdrawals({ page: 2, # This is an optional field }) ```
+signer created above provider, # The provider created above ) # 4. In the final
+step, if you find the balance is more than 0, you can use the
+"completeNormalWithdrawal" function to withdraw the cumulative amount to your
+ETH wallet. complete_normal_withdrawal_res = client.complete_normal_withdrawal
+( 'eth', # Enter the coin symbol ethAddress, # User public eth address signer,
+# The signer created above provider, # The provider created above gas_price, #
+max gas price for the transaction ) #Get a list of withdrawals withdrawals_list
+= client.list_normal_withdrawals({ page: 2, # This is an optional field }) ```
 #### Fast Withdrawal With Fast Withdrawal, your funds will be processed in an
 expedited timeframe, often within a few minutes. This mode is ideal for users
 who require immediate access to their funds and are comfortable with paying a
 fee. The `stark keys (L2 Key Pair)` can be generated with the help of [this
 section](#l2-key-pair) of the documentation. 1. Ethereum Network ```python
 key_pair = { 'stark_public_key': stark_public_key, 'stark_private_key':
 stark_private_key } fast_withdrawal_res = client.fast_withdrawal( key_pair, #
@@ -247,8 +262,27 @@
 'usdc', # Enter the coin symbol 'ETHEREUM', # Allowed networks are POLYGON &
 ETHEREUM ) ``` 2. Polygon network ```python const fastWithdrawalRes = await
 client.fastWithdrawal( key_pair, # The keyPair created above 0.001, # Enter the
 amount you want to deposit 'btc', # Enter the coin symbol 'POLYGON', # Allowed
 networks are POLYGON & ETHEREUM ) ``` 3. Get a list of fast withdrawals
 ```python fast_withdrawals_list = client.list_fast_withdrawals({ 'page': 2, #
 This is an optional field 'network': 'POLYGON' # This is an optional field })
-```
+``` ### Internal Transfer Users will be able to seamlessly transfer assets from
+their CEXs or other chains with minimal fees. To get started with the feature,
+follow these two steps: 1. Reach out to tanX (support@tanx.fi) to get the
+organization key and API key. 2. Generate the L2 key pair with your private key
+#### Available methods: 1. To process the internal transfer, call the
+`intiate_and_process_internal_transfers` method and pass the necessary
+arguments: ```python key_pair = { 'stark_public_key': '(your stark public key
+here)' 'stark_private_key': '(your stark private key here)' } ETH_ADDRESS_2 = '
+(destination Eth wallet address here)' internal_transfer_response =
+client.intiate_and_process_internal_transfers( key_pair=key_pair,
+organization_key=TANX_ORGANIZATION_KEY, api_key=TANX_API_KEY, currency='usdc',
+amount=1, destination_address=ETH_ADDRESS_2, client_reference_id=1 ) ``` 2.
+Retrieve a list of transfers initiated by the authenticated user: ```python
+internal_trasnfers_list = client.list_internal_transfers({ 'limit': 10,
+'offset': 10 }) ``` 3. Retrieve an internal transfer using its client reference
+id: ```python internal_transfer_by_id =
+client.get_internal_transfer_by_client_id(client_reference_id) ``` 4. Check if
+a user exists by their destination address. ```python check_user_res =
+client.check_internal_transfer_user_exists( TANX_ORGANIZATION_KEY,
+TANX_API_KEY, destination_address, ) ```
```

### Comparing `tanx-connector-2.0.1/README.md` & `tanx-connector-2.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -54,37 +54,38 @@
   - [WebSocket Client](#websocket-client)
     - [Connect](#connect)
     - [Subscribe](#subscribe)
     - [Unsubscribe](#unsubscribe)
     - [Disconnect](#disconnect)
     - [Usage](#usage)
   - [Error Handling](#error-handling)
-  - [Internal Transfer](#internal-transfer)
   - [Deposit](#deposit)
-    - [Ethereum Network Deposit](#ehtereum-network-deposit)
+    - [Ethereum Network Deposit](#ethereum-network-deposit)
     - [Polygon Network Deposit](#polygon-network-deposit)
     - [List Deposits](#list-deposits)
   - [Withdrawal](#withdrawal)
-    - [Normal Withdrawal](#normal-withdrawal)
+    - [Normal Withdrawal](#normal-withdrawal-only-for-ethereum-network)
     - [Fast Withdrawal](#fast-withdrawal)
+  - [Internal Transfer](#internal-transfer)
+    - [Available Methods](#available-methods)
 
 ## Installation
 
 First go to the [tanX Website](https://www.tanx.fi/) and create an account with your wallet.
 
 Install the package using pip.
 
 ```python
 pip install tanx-connector
 ```
 
 ## Quickstart
 
 Make sure that tanxconnector is [installed](#installation) and up-to-date.
-Also make sure you have an account on the [mainnet](https://www.tanx.fi/) or [testnet](https://api-testnet.tanx.fi) website.
+Also make sure you have an account on the [mainnet](https://trade.tanx.fi/) or [testnet](https://testnet.tanx.fi/) website.
 
 To get quickly started, try running the simple example for creating and fetching the order once logged in.
 
 ```python
 from tanxconnector import Client
 
 ETH_ADDRESS = "(your eth wallet address)"
@@ -119,15 +120,15 @@
 ### L2 Key Pair
 
 L2 Key Pair generation isn't currently available in the TanX Python SDK. 
 
 To get the L2 Key Pair, follow any of the two steps:
 
 1. Get the Key Pair from the [TanX official website](https://trade.tanx.fi/)'s Account Settings Tab once wallet is connected. Refer to the image below for more reference. Click on `Settings -> tanX key -> Show Keys` and Sign the request to get the keys. Copy these keys and store it securely.
-<img src="images/tanx-key.png">
+<img src="https://raw.githubusercontent.com/tanx-libs/tanx-connector-python/main/images/tanx-key.png">
 
 2. Generate the L2 key pair using the [TanX Nodejs SDK](https://github.com/tanx-libs/tanx-connector-nodejs). For generation using the Node SDK, refer to [this section](https://github.com/tanx-libs/tanx-connector-nodejs#create-l2-key-pair) in the documentation of the Nodejs SDK.
 
 ### Rest Client
 
 Import the REST Client
 
@@ -136,16 +137,16 @@
 ```
 
 Create a new instance
 
 ```python
 client = Client()
 # or
-client = Client() 
-# default is mainnet
+client = Client('testnet')
+# default is mainnet, can pass explicitly as well
 ```
 
 ### General Endpoints
 
 #### Test connectivity
 
 `GET /sapi/v1/health/`
@@ -418,80 +419,54 @@
     # call methods
 except tanxconnector.exception.AuthenticationError as exc:
     print(exc)
 except requests.exceptions.HTTPError as exc:
     print(exc.response.json())
 ```
 
-### Internal Transfer
-
-Users will be able to seamlessly transfer assets from their CEXs or other chains with minimal fees.
-
-To get started with the feature, follow these two steps:
-
-1. Reach out to tanX (support@tanx.fi) to get the organization key and API key.
-
-2. Generate the L2 key pair with your private key
+### Deposit
 
-#### Available methods:
+#### Ethereum Network Deposit
 
-1. To process the internal transfer, call the `intiate_and_process_internal_transfers` method and pass the necessary arguments:
+This method involves using a custom provider and signer, which can be created using the web3.py library. The `stark_public_key` mentioned in the code should be obtained using the steps described in the [L2 Key Pair](#l2-key-pair) section of the documentation. Here's the code snippet for this method:
 
 ```python
-key_pair = {
-  'stark_public_key': '(your stark public key here)'
-  'stark_private_key': '(your stark private key here)'
-}
+# Note: Please use web3>=6.0.0, <7.0.0
+from web3 import Web3, Account
 
-ETH_ADDRESS_2 = '(destination Eth wallet address here)'
+provider = Web3(Web3.HTTPProvider(RPC_PROVIDER))
+signer = Account.from_key(PRIVATE_KEY)
 
-internal_transfer_response = client.intiate_and_process_internal_transfers(
-  key_pair=key_pair,
-  organization_key=TANX_ORGANIZATION_KEY,
-  api_key=TANX_API_KEY,
-  currency='usdc',
-  amount=1,
-  destination_address=ETH_ADDRESS_2,
-  client_reference_id=1
+deposit_res_with_stark_keys = client.deposit_from_ethereum_network_with_stark_key(
+  signer,
+  provider,
+  f'0x{stark_public_key}',
+  0.0001,
+  'eth'
 )
 ```
 
-2. Retrieve a list of transfers initiated by the authenticated user:
+For any `ERC20` token (which is not native for the network, like usdc), first allow unlimited allowance for that token using the `approve_unlimited_allowance_ethereum_network` method.
 
 ```python
-internal_trasnfers_list = client.list_internal_transfers({
-  'limit': 10,
-  'offset': 10
-})
-```
-
-3. Retrieve an internal transfer using its client reference id:
-
-```python
-internal_transfer_by_id = client.get_internal_transfer_by_client_id(client_reference_id)
-```
+# Note: Please use web3>=6.0.0, <7.0.0
+from web3 import Web3, Account
 
-4. Check if a user exists by their destination address.
+provider = Web3(Web3.HTTPProvider(RPC_PROVIDER))
+signer = Account.from_key(PRIVATE_KEY)
 
-```python
-check_user_res = client.check_internal_transfer_user_exists(
-  TANX_ORGANIZATION_KEY,
-  TANX_API_KEY,
-  destination_address,
-)
+# approval for unlimited allowance for ERC20 contracts
+allowance = client.approve_unlimited_allowance_ethereum_network('usdc', signer, provider)
+print(allowance) # prints the hash for the allowance transaction, check this on the etherscan/sepoliascan for success.
 ```
 
-### Deposit
-
-#### Ethereum Network Deposit
-
-This method involves using a custom provider and signer, which can be created using the web3.py library. The `stark_public_key` mentioned in the code should be obtained using the steps described in the [L2 Key Pair](#l2-key-pair) section of the documentation. Here's the code snippet for this method:
+Once the allowance is success, transactions can be made for `ERC20` token on ETH network.
 
 ```python
-# Note: Please use web3 version 5.25.0
+# Note: Please use web3>=6.0.0, <7.0.0
 from web3 import Web3, Account
 
 provider = Web3(Web3.HTTPProvider(RPC_PROVIDER))
 signer = Account.from_key(PRIVATE_KEY)
 
 deposit_res_with_stark_keys = client.deposit_from_ethereum_network_with_stark_key(
   signer,
@@ -516,16 +491,54 @@
   'matic',  # Coin Symbol
   0.00001 # Amount to be deposited
 )
 ```
 
 2. Using Custom Provider and Signer:
 <br>This method involves using a custom provider and signer, which can be created using the web3.py library. Also, its important to inject a middleware at the 0th layer of the middleware onion for the provider ([See Reference](https://web3py.readthedocs.io/en/stable/middleware.html#proof-of-authority)). Here's the code snippet for this method:
+
+```python
+# Note: Please use web3>=6.0.0, <7.0.0
+from web3 import Web3, Account
+from web3.middleware.geth_poa import geth_poa_middleware
+
+provider = Web3(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON))
+provider.middleware_onion.inject(geth_poa_middleware, layer=0)
+
+signer = Account.from_key(PRIVATE_KEY)
+
+polygon_deposit_res = client.deposit_from_polygon_network_with_signer(
+  signer, # Signer Created above
+  provider, # Provider created above
+  'matic',  # Enter the coin symbol
+  0.0001, # Amount to be deposited
+)
+```
+
+For any `ERC20` token (which is not native for the network, like btc), first allow unlimited allowance for that token using the `approve_unlimited_allowance_polygon_network` method.
+
+```python
+# Note: Please use web3>=6.0.0, <7.0.0
+from web3 import Web3, Account
+from web3.middleware.geth_poa import geth_poa_middleware
+
+provider = Web3(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON))
+provider.middleware_onion.inject(geth_poa_middleware, layer=0)
+
+signer = Account.from_key(PRIVATE_KEY)
+
+# approval for unlimited allowance for ERC20 contracts
+allowance = client.approve_unlimited_allowance_polygon_network(coin='btc', signer=signer, w3=provider)
+print(allowance)  # prints the hash for the allowance, check on polygon scan for success
+```
+
+Once the allowance is success, transactions can be made for `ERC20` token on POLYGON network.
+
 ```python
-# Note: Please use ethers version 5.25.0.
+# Note: Please use web3>=6.0.0, <7.0.0
 from web3 import Web3, Account
 from web3.middleware.geth_poa import geth_poa_middleware
 
 provider = Web3(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON))
 provider.middleware_onion.inject(geth_poa_middleware, layer=0)
 
 signer = Account.from_key(PRIVATE_KEY)
@@ -582,22 +595,22 @@
 # 2. WAIT for up to 24 hours.
 # 3. Check whether the withdrawn balance is pending by calling the "getPendingNormalWithdrawalAmountByCoin" function with the required parameters.
 pending_balance = client.get_pending_normal_withdrawal_amount_by_coin(
   'eth', # Enter the coin symbol
   eth_address, # User public eth address
   signer, # The signer created above
   provider, # The provider created above
-  gas_price, # max gas price for the transaction
 )
 # 4. In the final step, if you find the balance is more than 0, you can use the "completeNormalWithdrawal" function to withdraw the cumulative amount to your ETH wallet.
 complete_normal_withdrawal_res = client.complete_normal_withdrawal(
   'eth', # Enter the coin symbol
   ethAddress, # User public eth address
   signer, # The signer created above
   provider, # The provider created above
+  gas_price, # max gas price for the transaction
 )
 
 #Get a list of withdrawals
 withdrawals_list = client.list_normal_withdrawals({
   page: 2, # This is an optional field
 })
 ```
@@ -636,7 +649,65 @@
 3. Get a list of fast withdrawals
 ```python
 fast_withdrawals_list = client.list_fast_withdrawals({
   'page': 2, # This is an optional field
   'network': 'POLYGON'  # This is an optional field
 })
 ```
+
+### Internal Transfer
+
+Users will be able to seamlessly transfer assets from their CEXs or other chains with minimal fees.
+
+To get started with the feature, follow these two steps:
+
+1. Reach out to tanX (support@tanx.fi) to get the organization key and API key.
+
+2. Generate the L2 key pair with your private key
+
+#### Available methods:
+
+1. To process the internal transfer, call the `intiate_and_process_internal_transfers` method and pass the necessary arguments:
+
+```python
+key_pair = {
+  'stark_public_key': '(your stark public key here)'
+  'stark_private_key': '(your stark private key here)'
+}
+
+ETH_ADDRESS_2 = '(destination Eth wallet address here)'
+
+internal_transfer_response = client.intiate_and_process_internal_transfers(
+  key_pair=key_pair,
+  organization_key=TANX_ORGANIZATION_KEY,
+  api_key=TANX_API_KEY,
+  currency='usdc',
+  amount=1,
+  destination_address=ETH_ADDRESS_2,
+  client_reference_id=1
+)
+```
+
+2. Retrieve a list of transfers initiated by the authenticated user:
+
+```python
+internal_trasnfers_list = client.list_internal_transfers({
+  'limit': 10,
+  'offset': 10
+})
+```
+
+3. Retrieve an internal transfer using its client reference id:
+
+```python
+internal_transfer_by_id = client.get_internal_transfer_by_client_id(client_reference_id)
+```
+
+4. Check if a user exists by their destination address.
+
+```python
+check_user_res = client.check_internal_transfer_user_exists(
+  TANX_ORGANIZATION_KEY,
+  TANX_API_KEY,
+  destination_address,
+)
+```
```

#### html2text {}

```diff
@@ -17,24 +17,25 @@
 (#balance-details-private-) - [Profit and Loss Details (Private ð)](#profit-
 and-loss-details-private-) - [Create order (Private ð)](#create-order-
 private-) - [Get Order (Private ð)](#get-order-private-) - [List Orders
 (Private ð)](#list-orders-) - [Cancel Order (Private ð)](#cancel-order-
 private-) - [List Trades (Private ð)](#list-trades-private-) - [WebSocket
 Client](#websocket-client) - [Connect](#connect) - [Subscribe](#subscribe) -
 [Unsubscribe](#unsubscribe) - [Disconnect](#disconnect) - [Usage](#usage) -
-[Error Handling](#error-handling) - [Internal Transfer](#internal-transfer) -
-[Deposit](#deposit) - [Ethereum Network Deposit](#ehtereum-network-deposit) -
-[Polygon Network Deposit](#polygon-network-deposit) - [List Deposits](#list-
-deposits) - [Withdrawal](#withdrawal) - [Normal Withdrawal](#normal-withdrawal)
-- [Fast Withdrawal](#fast-withdrawal) ## Installation First go to the [tanX
+[Error Handling](#error-handling) - [Deposit](#deposit) - [Ethereum Network
+Deposit](#ethereum-network-deposit) - [Polygon Network Deposit](#polygon-
+network-deposit) - [List Deposits](#list-deposits) - [Withdrawal](#withdrawal)
+- [Normal Withdrawal](#normal-withdrawal-only-for-ethereum-network) - [Fast
+Withdrawal](#fast-withdrawal) - [Internal Transfer](#internal-transfer) -
+[Available Methods](#available-methods) ## Installation First go to the [tanX
 Website](https://www.tanx.fi/) and create an account with your wallet. Install
 the package using pip. ```python pip install tanx-connector ``` ## Quickstart
 Make sure that tanxconnector is [installed](#installation) and up-to-date. Also
-make sure you have an account on the [mainnet](https://www.tanx.fi/) or
-[testnet](https://api-testnet.tanx.fi) website. To get quickly started, try
+make sure you have an account on the [mainnet](https://trade.tanx.fi/) or
+[testnet](https://testnet.tanx.fi/) website. To get quickly started, try
 running the simple example for creating and fetching the order once logged in.
 ```python from tanxconnector import Client ETH_ADDRESS = "(your eth wallet
 address)" PRIVATE_KEY = "(your wallet's private key)" client = Client() # login
 to the network login = client.complete_login(ETH_ADDRESS, PRIVATE_KEY) # create
 an order nonce nonce: CreateOrderNonceBody = {'market': 'ethusdc', 'ord_type':
 'market', 'price': 29580.51, 'side': 'sell', 'volume': 0.0005} # create the
 order order = client.create_complete_order(nonce, stark_private_key) print
@@ -46,57 +47,58 @@
 REST apis, WebSockets are handled by Client, WsClient classes respectively. ###
 Workflow Check out the [example files](./example) to see an example workflow.
 ### L2 Key Pair L2 Key Pair generation isn't currently available in the TanX
 Python SDK. To get the L2 Key Pair, follow any of the two steps: 1. Get the Key
 Pair from the [TanX official website](https://trade.tanx.fi/)'s Account
 Settings Tab once wallet is connected. Refer to the image below for more
 reference. Click on `Settings -> tanX key -> Show Keys` and Sign the request to
-get the keys. Copy these keys and store it securely. [images/tanx-key.png]2.
-Generate the L2 key pair using the [TanX Nodejs SDK](https://github.com/tanx-
-libs/tanx-connector-nodejs). For generation using the Node SDK, refer to [this
-section](https://github.com/tanx-libs/tanx-connector-nodejs#create-l2-key-pair)
-in the documentation of the Nodejs SDK. ### Rest Client Import the REST Client
-```py from tanxconnector import Client ``` Create a new instance ```python
-client = Client() # or client = Client() # default is mainnet ``` ### General
-Endpoints #### Test connectivity `GET /sapi/v1/health/` ```python
-client.test_connection() ``` #### 24hr Price `GET /sapi/v1/market/tickers/
-` ```python client.get_24h_price('btcusdt') ``` #### Kline/Candlestick Data
-`GET /sapi/v1/market/kline/` ```python client.get_candlestick('btcusdt') ```
-#### Order Book `GET /sapi/v1/market/orderbook/` ```python client.get_orderbook
-('btcusdt') ``` #### Recent trades `GET /sapi/v1/market/trades/` ```python
-client.get_recent_trades('btcusdt') ``` #### Login Both login() and
-complete_Login() sets tokens internally. Optionally, set_access_token() and
-set_refresh_token() can be used to set tokens directly. getNonce: `POST /sapi/
-v1/auth/nonce/` login: `POST /sapi/v1/auth/login/` ```python from tanxconnector
-import sign_msg, Client client = Client() client.complete_login(ETH_ADDRESS,
-PRIVATE_KEY) # calls below functions internally, use this for ease # or nonce =
-client.get_nonce(ETH_ADDRESS) user_signature = sign_msg(nonce['payload'],
-PRIVATE_KEY) login = client.login(ETH_ADDRESS, user_signature) # or
-client.set_access_token(access_token) client.set_refresh_token(refresh_token) #
-these functions are called internally when you use login or complete_login ```
-#### Refresh Token `POST /sapi/v1/auth/token/refresh/` If refresh token is set
-(manually or by using login functions), the refresh endpoint is called
-automatically when access token expires. Optionally, you can call
-`refresh_tokens` manually by passing in refresh_token (passing it is optional,
-it'll work if has been set before). ```python res = client.refresh_tokens
-(refresh_token) ``` #### Logout Sets tokens to null ```python client.logout()
-``` #### Profile Information (Private ð) `GET /sapi/v1/user/profile/
-` ```python client.get_profile_info() ``` #### Balance details (Private ð)
-`GET /sapi/v1/user/balance/` ```python client.get_balance() ``` #### Profit and
-Loss Details (Private ð) `GET /sapi/v1/user/pnl/` ```python
-client.get_profit_and_loss() ``` #### Create order (Private ð) Order is
-created in 2 steps: 1. Create the order nonce body 2. Process the order nonce
-body with the stark private key to create the order Create Nonce Body ```py
-from tanxconnector.typings import CreateOrderNonceBody nonce:
-CreateOrderNonceBody = {'market': 'btcusdt', 'ord_type': 'market', 'price':
-29580.51, 'side': 'buy', 'volume': 0.0001} ``` Create Order create_order_nonce:
-`POST /sapi/v1/orders/nonce/` create_new_order: `POST /sapi/v1/orders/create/
-` For getting the L2 Key Pairs (Stark Keys) refer to the above [section](#l2-
-key-pair) in the documentation. ```python stark_private_key = '(Your Stark
-Private Key Here)' order = client.create_complete_order(nonce,
+get the keys. Copy these keys and store it securely. [https://
+raw.githubusercontent.com/tanx-libs/tanx-connector-python/main/images/tanx-
+key.png]2. Generate the L2 key pair using the [TanX Nodejs SDK](https://
+github.com/tanx-libs/tanx-connector-nodejs). For generation using the Node SDK,
+refer to [this section](https://github.com/tanx-libs/tanx-connector-
+nodejs#create-l2-key-pair) in the documentation of the Nodejs SDK. ### Rest
+Client Import the REST Client ```py from tanxconnector import Client ``` Create
+a new instance ```python client = Client() # or client = Client('testnet') #
+default is mainnet, can pass explicitly as well ``` ### General Endpoints ####
+Test connectivity `GET /sapi/v1/health/` ```python client.test_connection() ```
+#### 24hr Price `GET /sapi/v1/market/tickers/` ```python client.get_24h_price
+('btcusdt') ``` #### Kline/Candlestick Data `GET /sapi/v1/market/kline/
+` ```python client.get_candlestick('btcusdt') ``` #### Order Book `GET /sapi/
+v1/market/orderbook/` ```python client.get_orderbook('btcusdt') ``` #### Recent
+trades `GET /sapi/v1/market/trades/` ```python client.get_recent_trades
+('btcusdt') ``` #### Login Both login() and complete_Login() sets tokens
+internally. Optionally, set_access_token() and set_refresh_token() can be used
+to set tokens directly. getNonce: `POST /sapi/v1/auth/nonce/` login: `POST /
+sapi/v1/auth/login/` ```python from tanxconnector import sign_msg, Client
+client = Client() client.complete_login(ETH_ADDRESS, PRIVATE_KEY) # calls below
+functions internally, use this for ease # or nonce = client.get_nonce
+(ETH_ADDRESS) user_signature = sign_msg(nonce['payload'], PRIVATE_KEY) login =
+client.login(ETH_ADDRESS, user_signature) # or client.set_access_token
+(access_token) client.set_refresh_token(refresh_token) # these functions are
+called internally when you use login or complete_login ``` #### Refresh Token
+`POST /sapi/v1/auth/token/refresh/` If refresh token is set (manually or by
+using login functions), the refresh endpoint is called automatically when
+access token expires. Optionally, you can call `refresh_tokens` manually by
+passing in refresh_token (passing it is optional, it'll work if has been set
+before). ```python res = client.refresh_tokens(refresh_token) ``` #### Logout
+Sets tokens to null ```python client.logout() ``` #### Profile Information
+(Private ð) `GET /sapi/v1/user/profile/` ```python client.get_profile_info()
+``` #### Balance details (Private ð) `GET /sapi/v1/user/balance/` ```python
+client.get_balance() ``` #### Profit and Loss Details (Private ð) `GET /
+sapi/v1/user/pnl/` ```python client.get_profit_and_loss() ``` #### Create order
+(Private ð) Order is created in 2 steps: 1. Create the order nonce body 2.
+Process the order nonce body with the stark private key to create the order
+Create Nonce Body ```py from tanxconnector.typings import CreateOrderNonceBody
+nonce: CreateOrderNonceBody = {'market': 'btcusdt', 'ord_type': 'market',
+'price': 29580.51, 'side': 'buy', 'volume': 0.0001} ``` Create Order
+create_order_nonce: `POST /sapi/v1/orders/nonce/` create_new_order: `POST /
+sapi/v1/orders/create/` For getting the L2 Key Pairs (Stark Keys) refer to the
+above [section](#l2-key-pair) in the documentation. ```python stark_private_key
+= '(Your Stark Private Key Here)' order = client.create_complete_order(nonce,
 stark_private_key) # calls below functions internally, we recommend using
 createCompleteOrder for ease of use # or from tanxconnector import
 sign_order_with_stark_private_key nonce_res = client.create_order_nonce(nonce)
 msg_hash = sign_order_with_stark_private_key(stark_private_key, nonce_res
 ['payload']) order = client.create_new_order(msg_hash) ``` #### Get Order
 (Private ð) `GET /sapi/v1/orders/{order_id}/` ```python client.get_order
 (order_id) ``` #### List Orders (Private ð) `GET /sapi/v1/orders/` ```python
@@ -120,41 +122,36 @@
 ws_client.disconnect() ``` #### Usage WsClient includes a member called
 websocket which is initialized with websockets.connect(). You may use it to
 handle WebSocket operations. ```py async for message in ws_client.websocket:
 print(message) ``` ### Error Handling Errors thrown are of types
 `AuthenticationError or requests.exceptions.HTTPError`. Example ```py try: #
 call methods except tanxconnector.exception.AuthenticationError as exc: print
 (exc) except requests.exceptions.HTTPError as exc: print(exc.response.json())
-``` ### Internal Transfer Users will be able to seamlessly transfer assets from
-their CEXs or other chains with minimal fees. To get started with the feature,
-follow these two steps: 1. Reach out to tanX (support@tanx.fi) to get the
-organization key and API key. 2. Generate the L2 key pair with your private key
-#### Available methods: 1. To process the internal transfer, call the
-`intiate_and_process_internal_transfers` method and pass the necessary
-arguments: ```python key_pair = { 'stark_public_key': '(your stark public key
-here)' 'stark_private_key': '(your stark private key here)' } ETH_ADDRESS_2 = '
-(destination Eth wallet address here)' internal_transfer_response =
-client.intiate_and_process_internal_transfers( key_pair=key_pair,
-organization_key=TANX_ORGANIZATION_KEY, api_key=TANX_API_KEY, currency='usdc',
-amount=1, destination_address=ETH_ADDRESS_2, client_reference_id=1 ) ``` 2.
-Retrieve a list of transfers initiated by the authenticated user: ```python
-internal_trasnfers_list = client.list_internal_transfers({ 'limit': 10,
-'offset': 10 }) ``` 3. Retrieve an internal transfer using its client reference
-id: ```python internal_transfer_by_id =
-client.get_internal_transfer_by_client_id(client_reference_id) ``` 4. Check if
-a user exists by their destination address. ```python check_user_res =
-client.check_internal_transfer_user_exists( TANX_ORGANIZATION_KEY,
-TANX_API_KEY, destination_address, ) ``` ### Deposit #### Ethereum Network
-Deposit This method involves using a custom provider and signer, which can be
-created using the web3.py library. The `stark_public_key` mentioned in the code
-should be obtained using the steps described in the [L2 Key Pair](#l2-key-pair)
-section of the documentation. Here's the code snippet for this method:
-```python # Note: Please use web3 version 5.25.0 from web3 import Web3, Account
+``` ### Deposit #### Ethereum Network Deposit This method involves using a
+custom provider and signer, which can be created using the web3.py library. The
+`stark_public_key` mentioned in the code should be obtained using the steps
+described in the [L2 Key Pair](#l2-key-pair) section of the documentation.
+Here's the code snippet for this method: ```python # Note: Please use
+web3>=6.0.0, <7.0.0 from web3 import Web3, Account provider = Web3
+(Web3.HTTPProvider(RPC_PROVIDER)) signer = Account.from_key(PRIVATE_KEY)
+deposit_res_with_stark_keys =
+client.deposit_from_ethereum_network_with_stark_key( signer, provider, f'0x
+{stark_public_key}', 0.0001, 'eth' ) ``` For any `ERC20` token (which is not
+native for the network, like usdc), first allow unlimited allowance for that
+token using the `approve_unlimited_allowance_ethereum_network` method.
+```python # Note: Please use web3>=6.0.0, <7.0.0 from web3 import Web3, Account
 provider = Web3(Web3.HTTPProvider(RPC_PROVIDER)) signer = Account.from_key
-(PRIVATE_KEY) deposit_res_with_stark_keys =
+(PRIVATE_KEY) # approval for unlimited allowance for ERC20 contracts allowance
+= client.approve_unlimited_allowance_ethereum_network('usdc', signer, provider)
+print(allowance) # prints the hash for the allowance transaction, check this on
+the etherscan/sepoliascan for success. ``` Once the allowance is success,
+transactions can be made for `ERC20` token on ETH network. ```python # Note:
+Please use web3>=6.0.0, <7.0.0 from web3 import Web3, Account provider = Web3
+(Web3.HTTPProvider(RPC_PROVIDER)) signer = Account.from_key(PRIVATE_KEY)
+deposit_res_with_stark_keys =
 client.deposit_from_ethereum_network_with_stark_key( signer, provider, f'0x
 {stark_public_key}', 0.0001, 'usdc' ) ``` #### Polygon Network Deposit There
 are two ways to make a deposit on the Polygon network: 1. Using ETH Private Key
 and RPC URL:
 In this method, you will use an ETH private key and an RPC URL to execute a
 Polygon deposit. You'll also need to create an RPC URL using services like
 Infura, Alchemy, etc. Here's the code snippet for this method: ```python
@@ -162,20 +159,38 @@
 Use 'Polygon Mumbai' for the testnet and 'Polygon mainnet' for the mainnet.
 PRIVATE_KEY, # ETH Private Key 'matic', # Coin Symbol 0.00001 # Amount to be
 deposited ) ``` 2. Using Custom Provider and Signer:
 This method involves using a custom provider and signer, which can be created
 using the web3.py library. Also, its important to inject a middleware at the
 0th layer of the middleware onion for the provider ([See Reference](https://
 web3py.readthedocs.io/en/stable/middleware.html#proof-of-authority)). Here's
-the code snippet for this method: ```python # Note: Please use ethers version
-5.25.0. from web3 import Web3, Account from web3.middleware.geth_poa import
+the code snippet for this method: ```python # Note: Please use web3>=6.0.0,
+<7.0.0 from web3 import Web3, Account from web3.middleware.geth_poa import
 geth_poa_middleware provider = Web3(Web3.HTTPProvider
 (RPC_PROVIDER_FOR_POLYGON)) provider.middleware_onion.inject
 (geth_poa_middleware, layer=0) signer = Account.from_key(PRIVATE_KEY)
 polygon_deposit_res = client.deposit_from_polygon_network_with_signer( signer,
+# Signer Created above provider, # Provider created above 'matic', # Enter the
+coin symbol 0.0001, # Amount to be deposited ) ``` For any `ERC20` token (which
+is not native for the network, like btc), first allow unlimited allowance for
+that token using the `approve_unlimited_allowance_polygon_network` method.
+```python # Note: Please use web3>=6.0.0, <7.0.0 from web3 import Web3, Account
+from web3.middleware.geth_poa import geth_poa_middleware provider = Web3
+(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON)) provider.middleware_onion.inject
+(geth_poa_middleware, layer=0) signer = Account.from_key(PRIVATE_KEY) #
+approval for unlimited allowance for ERC20 contracts allowance =
+client.approve_unlimited_allowance_polygon_network(coin='btc', signer=signer,
+w3=provider) print(allowance) # prints the hash for the allowance, check on
+polygon scan for success ``` Once the allowance is success, transactions can be
+made for `ERC20` token on POLYGON network. ```python # Note: Please use
+web3>=6.0.0, <7.0.0 from web3 import Web3, Account from
+web3.middleware.geth_poa import geth_poa_middleware provider = Web3
+(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON)) provider.middleware_onion.inject
+(geth_poa_middleware, layer=0) signer = Account.from_key(PRIVATE_KEY)
+polygon_deposit_res = client.deposit_from_polygon_network_with_signer( signer,
 # Signer Created above provider, # Provider created above 'btc', # Enter the
 coin symbol 0.0001, # Amount to be deposited ) ``` #### List Deposits To get
 the deposit history, you can use the following code: ```python deposit_list =
 client.list_deposits({ 'page': 1, # This field is optional 'limit': 1, # This
 field is optional 'network': 'ETHEREUM' # Network for which you want to list
 the deposit history. Allowed networks are ETHEREUM & POLYGON }) ``` ###
 Withdrawal Generally, we have two modes of withdrawal: Normal Withdrawal and
@@ -194,22 +209,22 @@
 function. withdrawal_res = client.initiate_normal_withdrawal( key_pair, # The
 keyPair created for stark keys 0.0001, # Enter the amount you want to deposit
 'usdc', # Enter the coin symbol ) # 2. WAIT for up to 24 hours. # 3. Check
 whether the withdrawn balance is pending by calling the
 "getPendingNormalWithdrawalAmountByCoin" function with the required parameters.
 pending_balance = client.get_pending_normal_withdrawal_amount_by_coin( 'eth', #
 Enter the coin symbol eth_address, # User public eth address signer, # The
-signer created above provider, # The provider created above gas_price, # max
-gas price for the transaction ) # 4. In the final step, if you find the balance
-is more than 0, you can use the "completeNormalWithdrawal" function to withdraw
-the cumulative amount to your ETH wallet. complete_normal_withdrawal_res =
-client.complete_normal_withdrawal( 'eth', # Enter the coin symbol ethAddress, #
-User public eth address signer, # The signer created above provider, # The
-provider created above ) #Get a list of withdrawals withdrawals_list =
-client.list_normal_withdrawals({ page: 2, # This is an optional field }) ```
+signer created above provider, # The provider created above ) # 4. In the final
+step, if you find the balance is more than 0, you can use the
+"completeNormalWithdrawal" function to withdraw the cumulative amount to your
+ETH wallet. complete_normal_withdrawal_res = client.complete_normal_withdrawal
+( 'eth', # Enter the coin symbol ethAddress, # User public eth address signer,
+# The signer created above provider, # The provider created above gas_price, #
+max gas price for the transaction ) #Get a list of withdrawals withdrawals_list
+= client.list_normal_withdrawals({ page: 2, # This is an optional field }) ```
 #### Fast Withdrawal With Fast Withdrawal, your funds will be processed in an
 expedited timeframe, often within a few minutes. This mode is ideal for users
 who require immediate access to their funds and are comfortable with paying a
 fee. The `stark keys (L2 Key Pair)` can be generated with the help of [this
 section](#l2-key-pair) of the documentation. 1. Ethereum Network ```python
 key_pair = { 'stark_public_key': stark_public_key, 'stark_private_key':
 stark_private_key } fast_withdrawal_res = client.fast_withdrawal( key_pair, #
@@ -217,8 +232,27 @@
 'usdc', # Enter the coin symbol 'ETHEREUM', # Allowed networks are POLYGON &
 ETHEREUM ) ``` 2. Polygon network ```python const fastWithdrawalRes = await
 client.fastWithdrawal( key_pair, # The keyPair created above 0.001, # Enter the
 amount you want to deposit 'btc', # Enter the coin symbol 'POLYGON', # Allowed
 networks are POLYGON & ETHEREUM ) ``` 3. Get a list of fast withdrawals
 ```python fast_withdrawals_list = client.list_fast_withdrawals({ 'page': 2, #
 This is an optional field 'network': 'POLYGON' # This is an optional field })
-```
+``` ### Internal Transfer Users will be able to seamlessly transfer assets from
+their CEXs or other chains with minimal fees. To get started with the feature,
+follow these two steps: 1. Reach out to tanX (support@tanx.fi) to get the
+organization key and API key. 2. Generate the L2 key pair with your private key
+#### Available methods: 1. To process the internal transfer, call the
+`intiate_and_process_internal_transfers` method and pass the necessary
+arguments: ```python key_pair = { 'stark_public_key': '(your stark public key
+here)' 'stark_private_key': '(your stark private key here)' } ETH_ADDRESS_2 = '
+(destination Eth wallet address here)' internal_transfer_response =
+client.intiate_and_process_internal_transfers( key_pair=key_pair,
+organization_key=TANX_ORGANIZATION_KEY, api_key=TANX_API_KEY, currency='usdc',
+amount=1, destination_address=ETH_ADDRESS_2, client_reference_id=1 ) ``` 2.
+Retrieve a list of transfers initiated by the authenticated user: ```python
+internal_trasnfers_list = client.list_internal_transfers({ 'limit': 10,
+'offset': 10 }) ``` 3. Retrieve an internal transfer using its client reference
+id: ```python internal_transfer_by_id =
+client.get_internal_transfer_by_client_id(client_reference_id) ``` 4. Check if
+a user exists by their destination address. ```python check_user_res =
+client.check_internal_transfer_user_exists( TANX_ORGANIZATION_KEY,
+TANX_API_KEY, destination_address, ) ```
```

### Comparing `tanx-connector-2.0.1/pyproject.toml` & `tanx-connector-2.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -46,18 +46,18 @@
     "bumpver",
     "build",
     "twine",
     "python-dotenv"
 ]
 
 [tool.bumpver]
-current_version = "2.0.1"
+current_version = "2.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "update version: v{old_version} -> v{new_version}"
-commit = true
+commit = false
 push = false
 
 [tool.setuptools.dynamic]
 version = {attr = "tanxconnector.__version__"}
 
 [tool.bumpver.file_patterns]
 "src/tanxconnector/__init__.py" = [
```

### Comparing `tanx-connector-2.0.1/src/tanx_connector.egg-info/PKG-INFO` & `tanx-connector-2.0.2/src/tanx_connector.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanx-connector
-Version: 2.0.1
+Version: 2.0.2
 Summary: The official Python connector for Tanx's API
 Author: tanX
 License: MIT License
         
         Copyright (c) 2023 Tanx Fi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -108,37 +108,38 @@
   - [WebSocket Client](#websocket-client)
     - [Connect](#connect)
     - [Subscribe](#subscribe)
     - [Unsubscribe](#unsubscribe)
     - [Disconnect](#disconnect)
     - [Usage](#usage)
   - [Error Handling](#error-handling)
-  - [Internal Transfer](#internal-transfer)
   - [Deposit](#deposit)
-    - [Ethereum Network Deposit](#ehtereum-network-deposit)
+    - [Ethereum Network Deposit](#ethereum-network-deposit)
     - [Polygon Network Deposit](#polygon-network-deposit)
     - [List Deposits](#list-deposits)
   - [Withdrawal](#withdrawal)
-    - [Normal Withdrawal](#normal-withdrawal)
+    - [Normal Withdrawal](#normal-withdrawal-only-for-ethereum-network)
     - [Fast Withdrawal](#fast-withdrawal)
+  - [Internal Transfer](#internal-transfer)
+    - [Available Methods](#available-methods)
 
 ## Installation
 
 First go to the [tanX Website](https://www.tanx.fi/) and create an account with your wallet.
 
 Install the package using pip.
 
 ```python
 pip install tanx-connector
 ```
 
 ## Quickstart
 
 Make sure that tanxconnector is [installed](#installation) and up-to-date.
-Also make sure you have an account on the [mainnet](https://www.tanx.fi/) or [testnet](https://api-testnet.tanx.fi) website.
+Also make sure you have an account on the [mainnet](https://trade.tanx.fi/) or [testnet](https://testnet.tanx.fi/) website.
 
 To get quickly started, try running the simple example for creating and fetching the order once logged in.
 
 ```python
 from tanxconnector import Client
 
 ETH_ADDRESS = "(your eth wallet address)"
@@ -173,15 +174,15 @@
 ### L2 Key Pair
 
 L2 Key Pair generation isn't currently available in the TanX Python SDK. 
 
 To get the L2 Key Pair, follow any of the two steps:
 
 1. Get the Key Pair from the [TanX official website](https://trade.tanx.fi/)'s Account Settings Tab once wallet is connected. Refer to the image below for more reference. Click on `Settings -> tanX key -> Show Keys` and Sign the request to get the keys. Copy these keys and store it securely.
-<img src="images/tanx-key.png">
+<img src="https://raw.githubusercontent.com/tanx-libs/tanx-connector-python/main/images/tanx-key.png">
 
 2. Generate the L2 key pair using the [TanX Nodejs SDK](https://github.com/tanx-libs/tanx-connector-nodejs). For generation using the Node SDK, refer to [this section](https://github.com/tanx-libs/tanx-connector-nodejs#create-l2-key-pair) in the documentation of the Nodejs SDK.
 
 ### Rest Client
 
 Import the REST Client
 
@@ -190,16 +191,16 @@
 ```
 
 Create a new instance
 
 ```python
 client = Client()
 # or
-client = Client() 
-# default is mainnet
+client = Client('testnet')
+# default is mainnet, can pass explicitly as well
 ```
 
 ### General Endpoints
 
 #### Test connectivity
 
 `GET /sapi/v1/health/`
@@ -472,80 +473,54 @@
     # call methods
 except tanxconnector.exception.AuthenticationError as exc:
     print(exc)
 except requests.exceptions.HTTPError as exc:
     print(exc.response.json())
 ```
 
-### Internal Transfer
-
-Users will be able to seamlessly transfer assets from their CEXs or other chains with minimal fees.
-
-To get started with the feature, follow these two steps:
-
-1. Reach out to tanX (support@tanx.fi) to get the organization key and API key.
-
-2. Generate the L2 key pair with your private key
+### Deposit
 
-#### Available methods:
+#### Ethereum Network Deposit
 
-1. To process the internal transfer, call the `intiate_and_process_internal_transfers` method and pass the necessary arguments:
+This method involves using a custom provider and signer, which can be created using the web3.py library. The `stark_public_key` mentioned in the code should be obtained using the steps described in the [L2 Key Pair](#l2-key-pair) section of the documentation. Here's the code snippet for this method:
 
 ```python
-key_pair = {
-  'stark_public_key': '(your stark public key here)'
-  'stark_private_key': '(your stark private key here)'
-}
+# Note: Please use web3>=6.0.0, <7.0.0
+from web3 import Web3, Account
 
-ETH_ADDRESS_2 = '(destination Eth wallet address here)'
+provider = Web3(Web3.HTTPProvider(RPC_PROVIDER))
+signer = Account.from_key(PRIVATE_KEY)
 
-internal_transfer_response = client.intiate_and_process_internal_transfers(
-  key_pair=key_pair,
-  organization_key=TANX_ORGANIZATION_KEY,
-  api_key=TANX_API_KEY,
-  currency='usdc',
-  amount=1,
-  destination_address=ETH_ADDRESS_2,
-  client_reference_id=1
+deposit_res_with_stark_keys = client.deposit_from_ethereum_network_with_stark_key(
+  signer,
+  provider,
+  f'0x{stark_public_key}',
+  0.0001,
+  'eth'
 )
 ```
 
-2. Retrieve a list of transfers initiated by the authenticated user:
+For any `ERC20` token (which is not native for the network, like usdc), first allow unlimited allowance for that token using the `approve_unlimited_allowance_ethereum_network` method.
 
 ```python
-internal_trasnfers_list = client.list_internal_transfers({
-  'limit': 10,
-  'offset': 10
-})
-```
-
-3. Retrieve an internal transfer using its client reference id:
-
-```python
-internal_transfer_by_id = client.get_internal_transfer_by_client_id(client_reference_id)
-```
+# Note: Please use web3>=6.0.0, <7.0.0
+from web3 import Web3, Account
 
-4. Check if a user exists by their destination address.
+provider = Web3(Web3.HTTPProvider(RPC_PROVIDER))
+signer = Account.from_key(PRIVATE_KEY)
 
-```python
-check_user_res = client.check_internal_transfer_user_exists(
-  TANX_ORGANIZATION_KEY,
-  TANX_API_KEY,
-  destination_address,
-)
+# approval for unlimited allowance for ERC20 contracts
+allowance = client.approve_unlimited_allowance_ethereum_network('usdc', signer, provider)
+print(allowance) # prints the hash for the allowance transaction, check this on the etherscan/sepoliascan for success.
 ```
 
-### Deposit
-
-#### Ethereum Network Deposit
-
-This method involves using a custom provider and signer, which can be created using the web3.py library. The `stark_public_key` mentioned in the code should be obtained using the steps described in the [L2 Key Pair](#l2-key-pair) section of the documentation. Here's the code snippet for this method:
+Once the allowance is success, transactions can be made for `ERC20` token on ETH network.
 
 ```python
-# Note: Please use web3 version 5.25.0
+# Note: Please use web3>=6.0.0, <7.0.0
 from web3 import Web3, Account
 
 provider = Web3(Web3.HTTPProvider(RPC_PROVIDER))
 signer = Account.from_key(PRIVATE_KEY)
 
 deposit_res_with_stark_keys = client.deposit_from_ethereum_network_with_stark_key(
   signer,
@@ -570,16 +545,54 @@
   'matic',  # Coin Symbol
   0.00001 # Amount to be deposited
 )
 ```
 
 2. Using Custom Provider and Signer:
 <br>This method involves using a custom provider and signer, which can be created using the web3.py library. Also, its important to inject a middleware at the 0th layer of the middleware onion for the provider ([See Reference](https://web3py.readthedocs.io/en/stable/middleware.html#proof-of-authority)). Here's the code snippet for this method:
+
+```python
+# Note: Please use web3>=6.0.0, <7.0.0
+from web3 import Web3, Account
+from web3.middleware.geth_poa import geth_poa_middleware
+
+provider = Web3(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON))
+provider.middleware_onion.inject(geth_poa_middleware, layer=0)
+
+signer = Account.from_key(PRIVATE_KEY)
+
+polygon_deposit_res = client.deposit_from_polygon_network_with_signer(
+  signer, # Signer Created above
+  provider, # Provider created above
+  'matic',  # Enter the coin symbol
+  0.0001, # Amount to be deposited
+)
+```
+
+For any `ERC20` token (which is not native for the network, like btc), first allow unlimited allowance for that token using the `approve_unlimited_allowance_polygon_network` method.
+
+```python
+# Note: Please use web3>=6.0.0, <7.0.0
+from web3 import Web3, Account
+from web3.middleware.geth_poa import geth_poa_middleware
+
+provider = Web3(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON))
+provider.middleware_onion.inject(geth_poa_middleware, layer=0)
+
+signer = Account.from_key(PRIVATE_KEY)
+
+# approval for unlimited allowance for ERC20 contracts
+allowance = client.approve_unlimited_allowance_polygon_network(coin='btc', signer=signer, w3=provider)
+print(allowance)  # prints the hash for the allowance, check on polygon scan for success
+```
+
+Once the allowance is success, transactions can be made for `ERC20` token on POLYGON network.
+
 ```python
-# Note: Please use ethers version 5.25.0.
+# Note: Please use web3>=6.0.0, <7.0.0
 from web3 import Web3, Account
 from web3.middleware.geth_poa import geth_poa_middleware
 
 provider = Web3(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON))
 provider.middleware_onion.inject(geth_poa_middleware, layer=0)
 
 signer = Account.from_key(PRIVATE_KEY)
@@ -636,22 +649,22 @@
 # 2. WAIT for up to 24 hours.
 # 3. Check whether the withdrawn balance is pending by calling the "getPendingNormalWithdrawalAmountByCoin" function with the required parameters.
 pending_balance = client.get_pending_normal_withdrawal_amount_by_coin(
   'eth', # Enter the coin symbol
   eth_address, # User public eth address
   signer, # The signer created above
   provider, # The provider created above
-  gas_price, # max gas price for the transaction
 )
 # 4. In the final step, if you find the balance is more than 0, you can use the "completeNormalWithdrawal" function to withdraw the cumulative amount to your ETH wallet.
 complete_normal_withdrawal_res = client.complete_normal_withdrawal(
   'eth', # Enter the coin symbol
   ethAddress, # User public eth address
   signer, # The signer created above
   provider, # The provider created above
+  gas_price, # max gas price for the transaction
 )
 
 #Get a list of withdrawals
 withdrawals_list = client.list_normal_withdrawals({
   page: 2, # This is an optional field
 })
 ```
@@ -690,7 +703,65 @@
 3. Get a list of fast withdrawals
 ```python
 fast_withdrawals_list = client.list_fast_withdrawals({
   'page': 2, # This is an optional field
   'network': 'POLYGON'  # This is an optional field
 })
 ```
+
+### Internal Transfer
+
+Users will be able to seamlessly transfer assets from their CEXs or other chains with minimal fees.
+
+To get started with the feature, follow these two steps:
+
+1. Reach out to tanX (support@tanx.fi) to get the organization key and API key.
+
+2. Generate the L2 key pair with your private key
+
+#### Available methods:
+
+1. To process the internal transfer, call the `intiate_and_process_internal_transfers` method and pass the necessary arguments:
+
+```python
+key_pair = {
+  'stark_public_key': '(your stark public key here)'
+  'stark_private_key': '(your stark private key here)'
+}
+
+ETH_ADDRESS_2 = '(destination Eth wallet address here)'
+
+internal_transfer_response = client.intiate_and_process_internal_transfers(
+  key_pair=key_pair,
+  organization_key=TANX_ORGANIZATION_KEY,
+  api_key=TANX_API_KEY,
+  currency='usdc',
+  amount=1,
+  destination_address=ETH_ADDRESS_2,
+  client_reference_id=1
+)
+```
+
+2. Retrieve a list of transfers initiated by the authenticated user:
+
+```python
+internal_trasnfers_list = client.list_internal_transfers({
+  'limit': 10,
+  'offset': 10
+})
+```
+
+3. Retrieve an internal transfer using its client reference id:
+
+```python
+internal_transfer_by_id = client.get_internal_transfer_by_client_id(client_reference_id)
+```
+
+4. Check if a user exists by their destination address.
+
+```python
+check_user_res = client.check_internal_transfer_user_exists(
+  TANX_ORGANIZATION_KEY,
+  TANX_API_KEY,
+  destination_address,
+)
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tanx-connector Version: 2.0.1 Summary: The official
+Metadata-Version: 2.1 Name: tanx-connector Version: 2.0.2 Summary: The official
 Python connector for Tanx's API Author: tanX License: MIT License Copyright (c)
 2023 Tanx Fi Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
@@ -47,24 +47,25 @@
 (#balance-details-private-) - [Profit and Loss Details (Private ð)](#profit-
 and-loss-details-private-) - [Create order (Private ð)](#create-order-
 private-) - [Get Order (Private ð)](#get-order-private-) - [List Orders
 (Private ð)](#list-orders-) - [Cancel Order (Private ð)](#cancel-order-
 private-) - [List Trades (Private ð)](#list-trades-private-) - [WebSocket
 Client](#websocket-client) - [Connect](#connect) - [Subscribe](#subscribe) -
 [Unsubscribe](#unsubscribe) - [Disconnect](#disconnect) - [Usage](#usage) -
-[Error Handling](#error-handling) - [Internal Transfer](#internal-transfer) -
-[Deposit](#deposit) - [Ethereum Network Deposit](#ehtereum-network-deposit) -
-[Polygon Network Deposit](#polygon-network-deposit) - [List Deposits](#list-
-deposits) - [Withdrawal](#withdrawal) - [Normal Withdrawal](#normal-withdrawal)
-- [Fast Withdrawal](#fast-withdrawal) ## Installation First go to the [tanX
+[Error Handling](#error-handling) - [Deposit](#deposit) - [Ethereum Network
+Deposit](#ethereum-network-deposit) - [Polygon Network Deposit](#polygon-
+network-deposit) - [List Deposits](#list-deposits) - [Withdrawal](#withdrawal)
+- [Normal Withdrawal](#normal-withdrawal-only-for-ethereum-network) - [Fast
+Withdrawal](#fast-withdrawal) - [Internal Transfer](#internal-transfer) -
+[Available Methods](#available-methods) ## Installation First go to the [tanX
 Website](https://www.tanx.fi/) and create an account with your wallet. Install
 the package using pip. ```python pip install tanx-connector ``` ## Quickstart
 Make sure that tanxconnector is [installed](#installation) and up-to-date. Also
-make sure you have an account on the [mainnet](https://www.tanx.fi/) or
-[testnet](https://api-testnet.tanx.fi) website. To get quickly started, try
+make sure you have an account on the [mainnet](https://trade.tanx.fi/) or
+[testnet](https://testnet.tanx.fi/) website. To get quickly started, try
 running the simple example for creating and fetching the order once logged in.
 ```python from tanxconnector import Client ETH_ADDRESS = "(your eth wallet
 address)" PRIVATE_KEY = "(your wallet's private key)" client = Client() # login
 to the network login = client.complete_login(ETH_ADDRESS, PRIVATE_KEY) # create
 an order nonce nonce: CreateOrderNonceBody = {'market': 'ethusdc', 'ord_type':
 'market', 'price': 29580.51, 'side': 'sell', 'volume': 0.0005} # create the
 order order = client.create_complete_order(nonce, stark_private_key) print
@@ -76,57 +77,58 @@
 REST apis, WebSockets are handled by Client, WsClient classes respectively. ###
 Workflow Check out the [example files](./example) to see an example workflow.
 ### L2 Key Pair L2 Key Pair generation isn't currently available in the TanX
 Python SDK. To get the L2 Key Pair, follow any of the two steps: 1. Get the Key
 Pair from the [TanX official website](https://trade.tanx.fi/)'s Account
 Settings Tab once wallet is connected. Refer to the image below for more
 reference. Click on `Settings -> tanX key -> Show Keys` and Sign the request to
-get the keys. Copy these keys and store it securely. [images/tanx-key.png]2.
-Generate the L2 key pair using the [TanX Nodejs SDK](https://github.com/tanx-
-libs/tanx-connector-nodejs). For generation using the Node SDK, refer to [this
-section](https://github.com/tanx-libs/tanx-connector-nodejs#create-l2-key-pair)
-in the documentation of the Nodejs SDK. ### Rest Client Import the REST Client
-```py from tanxconnector import Client ``` Create a new instance ```python
-client = Client() # or client = Client() # default is mainnet ``` ### General
-Endpoints #### Test connectivity `GET /sapi/v1/health/` ```python
-client.test_connection() ``` #### 24hr Price `GET /sapi/v1/market/tickers/
-` ```python client.get_24h_price('btcusdt') ``` #### Kline/Candlestick Data
-`GET /sapi/v1/market/kline/` ```python client.get_candlestick('btcusdt') ```
-#### Order Book `GET /sapi/v1/market/orderbook/` ```python client.get_orderbook
-('btcusdt') ``` #### Recent trades `GET /sapi/v1/market/trades/` ```python
-client.get_recent_trades('btcusdt') ``` #### Login Both login() and
-complete_Login() sets tokens internally. Optionally, set_access_token() and
-set_refresh_token() can be used to set tokens directly. getNonce: `POST /sapi/
-v1/auth/nonce/` login: `POST /sapi/v1/auth/login/` ```python from tanxconnector
-import sign_msg, Client client = Client() client.complete_login(ETH_ADDRESS,
-PRIVATE_KEY) # calls below functions internally, use this for ease # or nonce =
-client.get_nonce(ETH_ADDRESS) user_signature = sign_msg(nonce['payload'],
-PRIVATE_KEY) login = client.login(ETH_ADDRESS, user_signature) # or
-client.set_access_token(access_token) client.set_refresh_token(refresh_token) #
-these functions are called internally when you use login or complete_login ```
-#### Refresh Token `POST /sapi/v1/auth/token/refresh/` If refresh token is set
-(manually or by using login functions), the refresh endpoint is called
-automatically when access token expires. Optionally, you can call
-`refresh_tokens` manually by passing in refresh_token (passing it is optional,
-it'll work if has been set before). ```python res = client.refresh_tokens
-(refresh_token) ``` #### Logout Sets tokens to null ```python client.logout()
-``` #### Profile Information (Private ð) `GET /sapi/v1/user/profile/
-` ```python client.get_profile_info() ``` #### Balance details (Private ð)
-`GET /sapi/v1/user/balance/` ```python client.get_balance() ``` #### Profit and
-Loss Details (Private ð) `GET /sapi/v1/user/pnl/` ```python
-client.get_profit_and_loss() ``` #### Create order (Private ð) Order is
-created in 2 steps: 1. Create the order nonce body 2. Process the order nonce
-body with the stark private key to create the order Create Nonce Body ```py
-from tanxconnector.typings import CreateOrderNonceBody nonce:
-CreateOrderNonceBody = {'market': 'btcusdt', 'ord_type': 'market', 'price':
-29580.51, 'side': 'buy', 'volume': 0.0001} ``` Create Order create_order_nonce:
-`POST /sapi/v1/orders/nonce/` create_new_order: `POST /sapi/v1/orders/create/
-` For getting the L2 Key Pairs (Stark Keys) refer to the above [section](#l2-
-key-pair) in the documentation. ```python stark_private_key = '(Your Stark
-Private Key Here)' order = client.create_complete_order(nonce,
+get the keys. Copy these keys and store it securely. [https://
+raw.githubusercontent.com/tanx-libs/tanx-connector-python/main/images/tanx-
+key.png]2. Generate the L2 key pair using the [TanX Nodejs SDK](https://
+github.com/tanx-libs/tanx-connector-nodejs). For generation using the Node SDK,
+refer to [this section](https://github.com/tanx-libs/tanx-connector-
+nodejs#create-l2-key-pair) in the documentation of the Nodejs SDK. ### Rest
+Client Import the REST Client ```py from tanxconnector import Client ``` Create
+a new instance ```python client = Client() # or client = Client('testnet') #
+default is mainnet, can pass explicitly as well ``` ### General Endpoints ####
+Test connectivity `GET /sapi/v1/health/` ```python client.test_connection() ```
+#### 24hr Price `GET /sapi/v1/market/tickers/` ```python client.get_24h_price
+('btcusdt') ``` #### Kline/Candlestick Data `GET /sapi/v1/market/kline/
+` ```python client.get_candlestick('btcusdt') ``` #### Order Book `GET /sapi/
+v1/market/orderbook/` ```python client.get_orderbook('btcusdt') ``` #### Recent
+trades `GET /sapi/v1/market/trades/` ```python client.get_recent_trades
+('btcusdt') ``` #### Login Both login() and complete_Login() sets tokens
+internally. Optionally, set_access_token() and set_refresh_token() can be used
+to set tokens directly. getNonce: `POST /sapi/v1/auth/nonce/` login: `POST /
+sapi/v1/auth/login/` ```python from tanxconnector import sign_msg, Client
+client = Client() client.complete_login(ETH_ADDRESS, PRIVATE_KEY) # calls below
+functions internally, use this for ease # or nonce = client.get_nonce
+(ETH_ADDRESS) user_signature = sign_msg(nonce['payload'], PRIVATE_KEY) login =
+client.login(ETH_ADDRESS, user_signature) # or client.set_access_token
+(access_token) client.set_refresh_token(refresh_token) # these functions are
+called internally when you use login or complete_login ``` #### Refresh Token
+`POST /sapi/v1/auth/token/refresh/` If refresh token is set (manually or by
+using login functions), the refresh endpoint is called automatically when
+access token expires. Optionally, you can call `refresh_tokens` manually by
+passing in refresh_token (passing it is optional, it'll work if has been set
+before). ```python res = client.refresh_tokens(refresh_token) ``` #### Logout
+Sets tokens to null ```python client.logout() ``` #### Profile Information
+(Private ð) `GET /sapi/v1/user/profile/` ```python client.get_profile_info()
+``` #### Balance details (Private ð) `GET /sapi/v1/user/balance/` ```python
+client.get_balance() ``` #### Profit and Loss Details (Private ð) `GET /
+sapi/v1/user/pnl/` ```python client.get_profit_and_loss() ``` #### Create order
+(Private ð) Order is created in 2 steps: 1. Create the order nonce body 2.
+Process the order nonce body with the stark private key to create the order
+Create Nonce Body ```py from tanxconnector.typings import CreateOrderNonceBody
+nonce: CreateOrderNonceBody = {'market': 'btcusdt', 'ord_type': 'market',
+'price': 29580.51, 'side': 'buy', 'volume': 0.0001} ``` Create Order
+create_order_nonce: `POST /sapi/v1/orders/nonce/` create_new_order: `POST /
+sapi/v1/orders/create/` For getting the L2 Key Pairs (Stark Keys) refer to the
+above [section](#l2-key-pair) in the documentation. ```python stark_private_key
+= '(Your Stark Private Key Here)' order = client.create_complete_order(nonce,
 stark_private_key) # calls below functions internally, we recommend using
 createCompleteOrder for ease of use # or from tanxconnector import
 sign_order_with_stark_private_key nonce_res = client.create_order_nonce(nonce)
 msg_hash = sign_order_with_stark_private_key(stark_private_key, nonce_res
 ['payload']) order = client.create_new_order(msg_hash) ``` #### Get Order
 (Private ð) `GET /sapi/v1/orders/{order_id}/` ```python client.get_order
 (order_id) ``` #### List Orders (Private ð) `GET /sapi/v1/orders/` ```python
@@ -150,41 +152,36 @@
 ws_client.disconnect() ``` #### Usage WsClient includes a member called
 websocket which is initialized with websockets.connect(). You may use it to
 handle WebSocket operations. ```py async for message in ws_client.websocket:
 print(message) ``` ### Error Handling Errors thrown are of types
 `AuthenticationError or requests.exceptions.HTTPError`. Example ```py try: #
 call methods except tanxconnector.exception.AuthenticationError as exc: print
 (exc) except requests.exceptions.HTTPError as exc: print(exc.response.json())
-``` ### Internal Transfer Users will be able to seamlessly transfer assets from
-their CEXs or other chains with minimal fees. To get started with the feature,
-follow these two steps: 1. Reach out to tanX (support@tanx.fi) to get the
-organization key and API key. 2. Generate the L2 key pair with your private key
-#### Available methods: 1. To process the internal transfer, call the
-`intiate_and_process_internal_transfers` method and pass the necessary
-arguments: ```python key_pair = { 'stark_public_key': '(your stark public key
-here)' 'stark_private_key': '(your stark private key here)' } ETH_ADDRESS_2 = '
-(destination Eth wallet address here)' internal_transfer_response =
-client.intiate_and_process_internal_transfers( key_pair=key_pair,
-organization_key=TANX_ORGANIZATION_KEY, api_key=TANX_API_KEY, currency='usdc',
-amount=1, destination_address=ETH_ADDRESS_2, client_reference_id=1 ) ``` 2.
-Retrieve a list of transfers initiated by the authenticated user: ```python
-internal_trasnfers_list = client.list_internal_transfers({ 'limit': 10,
-'offset': 10 }) ``` 3. Retrieve an internal transfer using its client reference
-id: ```python internal_transfer_by_id =
-client.get_internal_transfer_by_client_id(client_reference_id) ``` 4. Check if
-a user exists by their destination address. ```python check_user_res =
-client.check_internal_transfer_user_exists( TANX_ORGANIZATION_KEY,
-TANX_API_KEY, destination_address, ) ``` ### Deposit #### Ethereum Network
-Deposit This method involves using a custom provider and signer, which can be
-created using the web3.py library. The `stark_public_key` mentioned in the code
-should be obtained using the steps described in the [L2 Key Pair](#l2-key-pair)
-section of the documentation. Here's the code snippet for this method:
-```python # Note: Please use web3 version 5.25.0 from web3 import Web3, Account
+``` ### Deposit #### Ethereum Network Deposit This method involves using a
+custom provider and signer, which can be created using the web3.py library. The
+`stark_public_key` mentioned in the code should be obtained using the steps
+described in the [L2 Key Pair](#l2-key-pair) section of the documentation.
+Here's the code snippet for this method: ```python # Note: Please use
+web3>=6.0.0, <7.0.0 from web3 import Web3, Account provider = Web3
+(Web3.HTTPProvider(RPC_PROVIDER)) signer = Account.from_key(PRIVATE_KEY)
+deposit_res_with_stark_keys =
+client.deposit_from_ethereum_network_with_stark_key( signer, provider, f'0x
+{stark_public_key}', 0.0001, 'eth' ) ``` For any `ERC20` token (which is not
+native for the network, like usdc), first allow unlimited allowance for that
+token using the `approve_unlimited_allowance_ethereum_network` method.
+```python # Note: Please use web3>=6.0.0, <7.0.0 from web3 import Web3, Account
 provider = Web3(Web3.HTTPProvider(RPC_PROVIDER)) signer = Account.from_key
-(PRIVATE_KEY) deposit_res_with_stark_keys =
+(PRIVATE_KEY) # approval for unlimited allowance for ERC20 contracts allowance
+= client.approve_unlimited_allowance_ethereum_network('usdc', signer, provider)
+print(allowance) # prints the hash for the allowance transaction, check this on
+the etherscan/sepoliascan for success. ``` Once the allowance is success,
+transactions can be made for `ERC20` token on ETH network. ```python # Note:
+Please use web3>=6.0.0, <7.0.0 from web3 import Web3, Account provider = Web3
+(Web3.HTTPProvider(RPC_PROVIDER)) signer = Account.from_key(PRIVATE_KEY)
+deposit_res_with_stark_keys =
 client.deposit_from_ethereum_network_with_stark_key( signer, provider, f'0x
 {stark_public_key}', 0.0001, 'usdc' ) ``` #### Polygon Network Deposit There
 are two ways to make a deposit on the Polygon network: 1. Using ETH Private Key
 and RPC URL:
 In this method, you will use an ETH private key and an RPC URL to execute a
 Polygon deposit. You'll also need to create an RPC URL using services like
 Infura, Alchemy, etc. Here's the code snippet for this method: ```python
@@ -192,20 +189,38 @@
 Use 'Polygon Mumbai' for the testnet and 'Polygon mainnet' for the mainnet.
 PRIVATE_KEY, # ETH Private Key 'matic', # Coin Symbol 0.00001 # Amount to be
 deposited ) ``` 2. Using Custom Provider and Signer:
 This method involves using a custom provider and signer, which can be created
 using the web3.py library. Also, its important to inject a middleware at the
 0th layer of the middleware onion for the provider ([See Reference](https://
 web3py.readthedocs.io/en/stable/middleware.html#proof-of-authority)). Here's
-the code snippet for this method: ```python # Note: Please use ethers version
-5.25.0. from web3 import Web3, Account from web3.middleware.geth_poa import
+the code snippet for this method: ```python # Note: Please use web3>=6.0.0,
+<7.0.0 from web3 import Web3, Account from web3.middleware.geth_poa import
 geth_poa_middleware provider = Web3(Web3.HTTPProvider
 (RPC_PROVIDER_FOR_POLYGON)) provider.middleware_onion.inject
 (geth_poa_middleware, layer=0) signer = Account.from_key(PRIVATE_KEY)
 polygon_deposit_res = client.deposit_from_polygon_network_with_signer( signer,
+# Signer Created above provider, # Provider created above 'matic', # Enter the
+coin symbol 0.0001, # Amount to be deposited ) ``` For any `ERC20` token (which
+is not native for the network, like btc), first allow unlimited allowance for
+that token using the `approve_unlimited_allowance_polygon_network` method.
+```python # Note: Please use web3>=6.0.0, <7.0.0 from web3 import Web3, Account
+from web3.middleware.geth_poa import geth_poa_middleware provider = Web3
+(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON)) provider.middleware_onion.inject
+(geth_poa_middleware, layer=0) signer = Account.from_key(PRIVATE_KEY) #
+approval for unlimited allowance for ERC20 contracts allowance =
+client.approve_unlimited_allowance_polygon_network(coin='btc', signer=signer,
+w3=provider) print(allowance) # prints the hash for the allowance, check on
+polygon scan for success ``` Once the allowance is success, transactions can be
+made for `ERC20` token on POLYGON network. ```python # Note: Please use
+web3>=6.0.0, <7.0.0 from web3 import Web3, Account from
+web3.middleware.geth_poa import geth_poa_middleware provider = Web3
+(Web3.HTTPProvider(RPC_PROVIDER_FOR_POLYGON)) provider.middleware_onion.inject
+(geth_poa_middleware, layer=0) signer = Account.from_key(PRIVATE_KEY)
+polygon_deposit_res = client.deposit_from_polygon_network_with_signer( signer,
 # Signer Created above provider, # Provider created above 'btc', # Enter the
 coin symbol 0.0001, # Amount to be deposited ) ``` #### List Deposits To get
 the deposit history, you can use the following code: ```python deposit_list =
 client.list_deposits({ 'page': 1, # This field is optional 'limit': 1, # This
 field is optional 'network': 'ETHEREUM' # Network for which you want to list
 the deposit history. Allowed networks are ETHEREUM & POLYGON }) ``` ###
 Withdrawal Generally, we have two modes of withdrawal: Normal Withdrawal and
@@ -224,22 +239,22 @@
 function. withdrawal_res = client.initiate_normal_withdrawal( key_pair, # The
 keyPair created for stark keys 0.0001, # Enter the amount you want to deposit
 'usdc', # Enter the coin symbol ) # 2. WAIT for up to 24 hours. # 3. Check
 whether the withdrawn balance is pending by calling the
 "getPendingNormalWithdrawalAmountByCoin" function with the required parameters.
 pending_balance = client.get_pending_normal_withdrawal_amount_by_coin( 'eth', #
 Enter the coin symbol eth_address, # User public eth address signer, # The
-signer created above provider, # The provider created above gas_price, # max
-gas price for the transaction ) # 4. In the final step, if you find the balance
-is more than 0, you can use the "completeNormalWithdrawal" function to withdraw
-the cumulative amount to your ETH wallet. complete_normal_withdrawal_res =
-client.complete_normal_withdrawal( 'eth', # Enter the coin symbol ethAddress, #
-User public eth address signer, # The signer created above provider, # The
-provider created above ) #Get a list of withdrawals withdrawals_list =
-client.list_normal_withdrawals({ page: 2, # This is an optional field }) ```
+signer created above provider, # The provider created above ) # 4. In the final
+step, if you find the balance is more than 0, you can use the
+"completeNormalWithdrawal" function to withdraw the cumulative amount to your
+ETH wallet. complete_normal_withdrawal_res = client.complete_normal_withdrawal
+( 'eth', # Enter the coin symbol ethAddress, # User public eth address signer,
+# The signer created above provider, # The provider created above gas_price, #
+max gas price for the transaction ) #Get a list of withdrawals withdrawals_list
+= client.list_normal_withdrawals({ page: 2, # This is an optional field }) ```
 #### Fast Withdrawal With Fast Withdrawal, your funds will be processed in an
 expedited timeframe, often within a few minutes. This mode is ideal for users
 who require immediate access to their funds and are comfortable with paying a
 fee. The `stark keys (L2 Key Pair)` can be generated with the help of [this
 section](#l2-key-pair) of the documentation. 1. Ethereum Network ```python
 key_pair = { 'stark_public_key': stark_public_key, 'stark_private_key':
 stark_private_key } fast_withdrawal_res = client.fast_withdrawal( key_pair, #
@@ -247,8 +262,27 @@
 'usdc', # Enter the coin symbol 'ETHEREUM', # Allowed networks are POLYGON &
 ETHEREUM ) ``` 2. Polygon network ```python const fastWithdrawalRes = await
 client.fastWithdrawal( key_pair, # The keyPair created above 0.001, # Enter the
 amount you want to deposit 'btc', # Enter the coin symbol 'POLYGON', # Allowed
 networks are POLYGON & ETHEREUM ) ``` 3. Get a list of fast withdrawals
 ```python fast_withdrawals_list = client.list_fast_withdrawals({ 'page': 2, #
 This is an optional field 'network': 'POLYGON' # This is an optional field })
-```
+``` ### Internal Transfer Users will be able to seamlessly transfer assets from
+their CEXs or other chains with minimal fees. To get started with the feature,
+follow these two steps: 1. Reach out to tanX (support@tanx.fi) to get the
+organization key and API key. 2. Generate the L2 key pair with your private key
+#### Available methods: 1. To process the internal transfer, call the
+`intiate_and_process_internal_transfers` method and pass the necessary
+arguments: ```python key_pair = { 'stark_public_key': '(your stark public key
+here)' 'stark_private_key': '(your stark private key here)' } ETH_ADDRESS_2 = '
+(destination Eth wallet address here)' internal_transfer_response =
+client.intiate_and_process_internal_transfers( key_pair=key_pair,
+organization_key=TANX_ORGANIZATION_KEY, api_key=TANX_API_KEY, currency='usdc',
+amount=1, destination_address=ETH_ADDRESS_2, client_reference_id=1 ) ``` 2.
+Retrieve a list of transfers initiated by the authenticated user: ```python
+internal_trasnfers_list = client.list_internal_transfers({ 'limit': 10,
+'offset': 10 }) ``` 3. Retrieve an internal transfer using its client reference
+id: ```python internal_transfer_by_id =
+client.get_internal_transfer_by_client_id(client_reference_id) ``` 4. Check if
+a user exists by their destination address. ```python check_user_res =
+client.check_internal_transfer_user_exists( TANX_ORGANIZATION_KEY,
+TANX_API_KEY, destination_address, ) ```
```

### Comparing `tanx-connector-2.0.1/src/tanx_connector.egg-info/SOURCES.txt` & `tanx-connector-2.0.2/src/tanx_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/bin/blockchain_utils.py` & `tanx-connector-2.0.2/src/tanxconnector/bin/blockchain_utils.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/bin/erc20_abi.json` & `tanx-connector-2.0.2/src/tanxconnector/bin/erc20_abi.json`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/bin/math_utils.py` & `tanx-connector-2.0.2/src/tanxconnector/bin/math_utils.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/bin/pedersen_params.json` & `tanx-connector-2.0.2/src/tanxconnector/bin/pedersen_params.json`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/bin/polygon_deposit.json` & `tanx-connector-2.0.2/src/tanxconnector/bin/polygon_deposit.json`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/bin/signature.py` & `tanx-connector-2.0.2/src/tanxconnector/bin/signature.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/bin/starkex_abi_main.json` & `tanx-connector-2.0.2/src/tanxconnector/bin/starkex_abi_main.json`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/bin/starkex_abi_test.json` & `tanx-connector-2.0.2/src/tanxconnector/bin/starkex_abi_test.json`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/client.py` & `tanx-connector-2.0.2/src/tanxconnector/client.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/constants.py` & `tanx-connector-2.0.2/src/tanxconnector/constants.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/exception.py` & `tanx-connector-2.0.2/src/tanxconnector/exception.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/session.py` & `tanx-connector-2.0.2/src/tanxconnector/session.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/typings.py` & `tanx-connector-2.0.2/src/tanxconnector/typings.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/utils.py` & `tanx-connector-2.0.2/src/tanxconnector/utils.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/src/tanxconnector/wsclient.py` & `tanx-connector-2.0.2/src/tanxconnector/wsclient.py`

 * *Files identical despite different names*

### Comparing `tanx-connector-2.0.1/tests/test_client.py` & `tanx-connector-2.0.2/tests/test_client.py`

 * *Files identical despite different names*

