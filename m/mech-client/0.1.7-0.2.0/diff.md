# Comparing `tmp/mech_client-0.1.7.tar.gz` & `tmp/mech_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mech_client-0.1.7.tar", max compression
+gzip compressed data, was "mech_client-0.2.0.tar", max compression
```

## Comparing `mech_client-0.1.7.tar` & `mech_client-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,41 @@
--rw-r--r--   0        0        0    11339 2023-05-27 20:23:22.952168 mech_client-0.1.7/LICENSE
--rw-r--r--   0        0        0     2037 2023-05-30 10:09:38.116752 mech_client-0.1.7/README.md
--rw-r--r--   0        0        0       22 2023-06-03 09:13:28.534323 mech_client-0.1.7/mech_client/__init__.py
--rw-r--r--   0        0        0     1514 2023-06-01 18:17:24.000853 mech_client-0.1.7/mech_client/cli.py
--rw-r--r--   0        0        0     7617 2023-06-01 12:41:57.849598 mech_client-0.1.7/mech_client/interact.py
--rw-r--r--   0        0        0     1779 2023-05-31 14:33:42.502514 mech_client-0.1.7/mech_client/prompt_to_ipfs.py
--rw-r--r--   0        0        0     1659 2023-05-31 14:33:42.503191 mech_client-0.1.7/mech_client/push_to_ipfs.py
--rw-r--r--   0        0        0     1993 2023-06-01 18:17:24.001121 mech_client-0.1.7/mech_client/to_png.py
--rw-r--r--   0        0        0      581 2023-06-03 09:13:33.787570 mech_client-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 mech_client-0.1.7/setup.py
--rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 mech_client-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-06-24 06:13:48.183400 mech_client-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4049 2023-06-24 06:13:48.183400 mech_client-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/__init__.py
+-rw-r--r--   0        0        0     5090 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/acn.py
+-rw-r--r--   0        0        0     3359 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/cli.py
+-rw-r--r--   0        0        0     1027 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/helpers/__init__.py
+-rw-r--r--   0        0        0     1641 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/README.md
+-rw-r--r--   0        0        0     1143 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/__init__.py
+-rw-r--r--   0        0        0     1543 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/acn.proto
+-rw-r--r--   0        0        0     8325 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/acn_pb2.py
+-rw-r--r--   0        0        0     7982 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/custom_types.py
+-rw-r--r--   0        0        0     4443 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/dialogues.py
+-rw-r--r--   0        0        0    10256 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/message.py
+-rw-r--r--   0        0        0     1233 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/protocol.yaml
+-rw-r--r--   0        0        0     6405 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/serialization.py
+-rw-r--r--   0        0        0      847 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/tests/__init__.py
+-rw-r--r--   0        0        0     8965 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/tests/test_acn.py
+-rw-r--r--   0        0        0     1964 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/tests/test_acn_dialogues.py
+-rw-r--r--   0        0        0     4332 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/tests/test_acn_messages.py
+-rw-r--r--   0        0        0      577 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/README.md
+-rw-r--r--   0        0        0     1221 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/acn_data_share.proto
+-rw-r--r--   0        0        0     2349 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/acn_data_share_pb2.py
+-rw-r--r--   0        0        0     4078 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/dialogues.py
+-rw-r--r--   0        0        0     7726 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/message.py
+-rw-r--r--   0        0        0     1052 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/protocol.yaml
+-rw-r--r--   0        0        0     4450 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/serialization.py
+-rw-r--r--   0        0        0     1835 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py
+-rw-r--r--   0        0        0     2021 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py
+-rw-r--r--   0        0        0      631 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/p2p_libp2p_client/README.md
+-rw-r--r--   0        0        0      879 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/p2p_libp2p_client/__init__.py
+-rw-r--r--   0        0        0    27786 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/p2p_libp2p_client/connection.py
+-rw-r--r--   0        0        0     1763 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/p2p_libp2p_client/connection.yaml
+-rw-r--r--   0        0        0     9124 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/interact.py
+-rw-r--r--   0        0        0     1779 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/prompt_to_ipfs.py
+-rw-r--r--   0        0        0     1659 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/push_to_ipfs.py
+-rw-r--r--   0        0        0     1604 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/subgraph.py
+-rw-r--r--   0        0        0     1993 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/to_png.py
+-rw-r--r--   0        0        0     4901 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/wss.py
+-rw-r--r--   0        0        0     1424 2023-06-24 06:13:48.183400 mech_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4830 1970-01-01 00:00:00.000000 mech_client-0.2.0/PKG-INFO
```

### Comparing `mech_client-0.1.7/LICENSE` & `mech_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.7/mech_client/interact.py` & `mech_client-0.2.0/mech_client/interact.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,196 +21,252 @@
 This script allows sending a Request to an on-chain mech and waiting for the Deliver.
 
 Usage:
 
 python client.py <prompt> <tool>
 """
 
+import asyncio
 import json
 import os
-import time
 import warnings
-from typing import Any, Dict, Optional
+from enum import Enum
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Tuple
 
 import requests
 import websocket
-from aea.contracts.base import Contract
+from aea.crypto.base import Crypto
 from aea_ledger_ethereum import EthereumApi, EthereumCrypto
+from web3.contract import Contract as Web3Contract
 
+from mech_client.acn import (
+    watch_for_data_url_from_mech,
+    watch_for_data_url_from_mech_sync,
+)
 from mech_client.prompt_to_ipfs import push_metadata_to_ipfs
+from mech_client.subgraph import query_agent_address
+from mech_client.wss import (
+    register_event_handlers,
+    watch_for_data_url_from_wss,
+    watch_for_data_url_from_wss_sync,
+    watch_for_request_id,
+)
 
-CONTRACT_ADDRESS = "0xFf82123dFB52ab75C417195c5fDB87630145ae81"
-ETHEREUM_TESTNET_CONFIG = {
-    "address": "https://rpc.eu-central-2.gateway.fm/v4/gnosis/non-archival/mainnet",
+AGENT_REGISTRY_CONTRACT = "0xE49CB081e8d96920C38aA7AB90cb0294ab4Bc8EA"
+MECHX_CHAIN_RPC = os.environ.get(
+    "MECHX_CHAIN_RPC",
+    "https://rpc.eu-central-2.gateway.fm/v4/gnosis/non-archival/mainnet",
+)
+LEDGER_CONFIG = {
+    "address": MECHX_CHAIN_RPC,
     "chain_id": 100,
     "poa_chain": False,
     "default_gas_price_strategy": "eip1559",
 }
 PRIVATE_KEY_FILE_PATH = "ethereum_private_key.txt"
-EVENT_SIGNATURE_REQUEST = (
-    "0x4bda649efe6b98b0f9c1d5e859c29e20910f45c66dabfe6fad4a4881f7faf9cc"
-)
-EVENT_SIGNATURE_DELIVER = (
-    "0x3ec84da2cdc1ce60c063642b69ff2e65f3b69787a2b90443457ba274e51e7c72"
-)
+
 WSS_ENDPOINT = os.getenv(
     "WEBSOCKET_ENDPOINT",
     "wss://rpc.eu-central-2.gateway.fm/ws/v4/gnosis/non-archival/mainnet",
 )
+GNOSISSCAN_API_URL = "https://api.gnosisscan.io/api?module=contract&action=getabi&address={contract_address}"
 
 # Ignore a specific warning message
 warnings.filterwarnings("ignore", "The log with transaction hash.*")
 
 
-def check_for_tools(tool: str) -> Optional[int]:
-    """Checks if the tool is valid and for what agent."""
-    # TODO - replace hardcoded logic with on-chain check against agent mech registry
-    return (
-        3
-        if tool
-        in [
-            "openai-text-davinci-002",
-            "openai-text-davinci-003",
-            "openai-gpt-3.5-turbo",
-            "openai-gpt-4",
-            "stabilityai-stable-diffusion-v1-5",
-            "stabilityai-stable-diffusion-xl-beta-v2-2-2",
-            "stabilityai-stable-diffusion-512-v2-1",
-            "stabilityai-stable-diffusion-768-v2-1",
-        ]
-        else None
+class ConfirmationType(Enum):
+    """Verification type."""
+
+    ON_CHAIN = "on-chain"
+    OFF_CHAIN = "off-chain"
+    WAIT_FOR_BOTH = "wait-for-both"
+
+
+def get_contract(contract_address: str, ledger_api: EthereumApi) -> Web3Contract:
+    """Returns a contract instance."""
+    abi_request_url = GNOSISSCAN_API_URL.format(contract_address=contract_address)
+    response = requests.get(abi_request_url).json()
+    abi = json.loads(response["result"])
+    return ledger_api.get_contract_instance(
+        {"abi": abi, "bytecode": "0x"}, contract_address
     )
 
 
-def register_event_handlers(ethereum_crypto: EthereumCrypto) -> websocket.WebSocket:
-    """Register event handlers."""
-    wss = websocket.create_connection(WSS_ENDPOINT)
-    subscription_request = {
-        "jsonrpc": "2.0",
-        "id": 1,
-        "method": "eth_subscribe",
-        "params": [
-            "logs",
-            {
-                "address": CONTRACT_ADDRESS,
-                "topics": [
-                    EVENT_SIGNATURE_REQUEST,
-                    ["0x" + "0" * 24 + ethereum_crypto.address[2:]],
-                ],
-            },
-        ],
-    }
-    content = bytes(json.dumps(subscription_request), "utf-8")
-    wss.send(content)
-    # registration confirmation
-    msg = wss.recv()
-    subscription_deliver = {
-        "jsonrpc": "2.0",
-        "id": 1,
-        "method": "eth_subscribe",
-        "params": [
-            "logs",
-            {"address": CONTRACT_ADDRESS, "topics": [EVENT_SIGNATURE_DELIVER]},
-        ],
-    }
-    content = bytes(json.dumps(subscription_deliver), "utf-8")
-    wss.send(content)
-    # registration confirmation
-    msg = wss.recv()
-    return wss
+def _tool_selector_prompt(available_tools: List[str]) -> str:
+    """Tool selector prompt."""
+
+    tool_col_len = max(map(len, available_tools))
+    id_col_len = max(2, len(str(len(available_tools))))
+    table_len = tool_col_len + id_col_len + 5
+
+    separator = "|" + "-" * table_len + "|"
+    print("Select prompting tool")
+
+    def format_row(row: Tuple[str, str]) -> str:
+        _row = list(map(str, row))
+        row_str = "| "
+        row_str += _row[0]
+        row_str += " " * (id_col_len - len(_row[0]))
+        row_str += " | "
+        row_str += _row[1]
+        row_str += " " * (tool_col_len - len(_row[1]))
+        row_str += " |"
+        return row_str
+
+    while True:
+        print(separator)
+        print(format_row(("ID", "Tool")))
+        print(separator)
+        print("\n".join(map(format_row, enumerate(available_tools))))
+        print(separator)
+        try:
+            tool_id = int(input("Tool ID > "))
+            return available_tools[tool_id]
+        except (ValueError, TypeError, IndexError):
+            print("\nPlease enter valid tool ID.")
+
+
+def verify_or_retrieve_tool(
+    agent_id: int, ledger_api: EthereumApi, tool: Optional[str] = None
+) -> str:
+    """Checks if the tool is valid and for what agent."""
+    available_tools = fetch_tools(agent_id=agent_id, ledger_api=ledger_api)
+    if tool is not None and tool not in available_tools:
+        raise ValueError(
+            f"Provided tool `{tool}` not in the list of available tools; Available tools={available_tools}"
+        )
+    if tool is not None:
+        return tool
+    return _tool_selector_prompt(available_tools=available_tools)
+
+
+def fetch_tools(agent_id: int, ledger_api: EthereumApi) -> List[str]:
+    """Fetch tools for specified agent ID."""
+    mech_registry = get_contract(
+        contract_address=AGENT_REGISTRY_CONTRACT, ledger_api=ledger_api
+    )
+    token_uri = mech_registry.functions.tokenURI(agent_id).call()
+    response = requests.get(token_uri).json()
+    return response["tools"]
 
 
 def send_request(
-    ethereum_crypto: EthereumCrypto,
-    ethereum_ledger_api: EthereumApi,
+    crypto: EthereumCrypto,
+    ledger_api: EthereumApi,
+    mech_contract: Web3Contract,
     prompt: str,
     tool: str,
-    contract_address: str = CONTRACT_ADDRESS,
     price: int = 10_000_000_000_000_000,
-) -> Contract:
+) -> None:
     """Sends a request to the mech."""
-    mech = check_for_tools(tool)
-    if mech is None:
-        raise ValueError(f"Tool {tool} is not supported by any mech.")
     v1_file_hash_hex_truncated, v1_file_hash_hex = push_metadata_to_ipfs(prompt, tool)
     print(f"Prompt uploaded: https://gateway.autonolas.tech/ipfs/{v1_file_hash_hex}")
 
-    gnosisscan_api_url = f"https://api.gnosisscan.io/api?module=contract&action=getabi&address={contract_address}"
-    response = requests.get(gnosisscan_api_url)
-    abi = response.json()["result"]
-    abi = json.loads(abi)
-
-    contract_instance = ethereum_ledger_api.get_contract_instance(
-        {"abi": abi, "bytecode": "0x"}, contract_address
-    )
     method_name = "request"
-    methord_args = {
-        "data": v1_file_hash_hex_truncated
-    }  # bytes.fromhex(v1_file_hash_hex_truncated[2:])}
-    tx_args = {"sender_address": ethereum_crypto.address, "value": price}
-
-    raw_transaction = ethereum_ledger_api.build_transaction(
-        contract_instance=contract_instance,
+    methord_args = {"data": v1_file_hash_hex_truncated}
+    tx_args = {"sender_address": crypto.address, "value": price}
+    raw_transaction = ledger_api.build_transaction(
+        contract_instance=mech_contract,
         method_name=method_name,
         method_args=methord_args,
         tx_args=tx_args,
     )
     raw_transaction["gas"] = 50_000
-    # raw_transaction = ethereum_ledger_api.update_with_gas_estimate(raw_transaction)
-    signed_transaction = ethereum_crypto.sign_transaction(raw_transaction)
-    transaction_digest = ethereum_ledger_api.send_signed_transaction(signed_transaction)
+    signed_transaction = crypto.sign_transaction(raw_transaction)
+    transaction_digest = ledger_api.send_signed_transaction(signed_transaction)
     print(f"Transaction sent: https://gnosisscan.io/tx/{transaction_digest}")
-    return contract_instance
 
 
-def watch_for_events(
+def wait_for_data_url(
+    request_id: str,
     wss: websocket.WebSocket,
-    contract_instance: Contract,
-    ethereum_ledger_api: EthereumApi,
-    ethereum_crypto: EthereumCrypto,
+    mech_contract: Web3Contract,
+    ledger_api: EthereumApi,
+    crypto: Crypto,
+) -> Any:
+    """Wait for data from on-chain/off-chain"""
+    loop = asyncio.new_event_loop()
+    off_chain_task = loop.create_task(watch_for_data_url_from_mech(crypto=crypto))
+    on_chain_task = loop.create_task(
+        watch_for_data_url_from_wss(
+            request_id=request_id,
+            wss=wss,
+            mech_contract=mech_contract,
+            ledger_api=ledger_api,
+            loop=loop,
+        )
+    )
+
+    async def _wait_for_tasks() -> Any:
+        """Wait for tasks to finish."""
+        (finished, *_), unfinished = await asyncio.wait(
+            [off_chain_task, on_chain_task], return_when=asyncio.FIRST_COMPLETED
+        )
+        for task in unfinished:
+            task.cancel()
+        await asyncio.wait(unfinished)
+        return finished.result()
+
+    result = loop.run_until_complete(_wait_for_tasks())
+    return result
+
+
+def interact(
+    prompt: str,
+    agent_id: int,
+    tool: Optional[str] = None,
+    private_key_path: Optional[str] = None,
+    confirmation_type: ConfirmationType = ConfirmationType.WAIT_FOR_BOTH,
 ) -> Dict[str, Any]:
-    """Watches for events on mech."""
-    is_waiting = True
-    request_id = None
-    while is_waiting:
-        msg = wss.recv()
-        data = json.loads(msg)
-        tx_hash = data["params"]["result"]["transactionHash"]
-        no_receipt = True
-        while no_receipt:
-            try:
-                tx_receipt = ethereum_ledger_api._api.eth.get_transaction_receipt(
-                    tx_hash
-                )
-                no_receipt = False
-            except Exception:
-                time.sleep(1)
-        event_signature = tx_receipt["logs"][0]["topics"][0].hex()
-        if event_signature == EVENT_SIGNATURE_REQUEST:
-            rich_logs = contract_instance.events.Request().processReceipt(tx_receipt)
-            request_id = rich_logs[0]["args"]["requestId"]
-            print(f"Request on-chain with id: {request_id}")
-        if event_signature == EVENT_SIGNATURE_DELIVER:
-            rich_logs = contract_instance.events.Deliver().processReceipt(tx_receipt)
-            data = rich_logs[0]["args"]["data"]
-            request_id_ = rich_logs[0]["args"]["requestId"]
-            if request_id != request_id_:
-                continue
-            data_url = "https://gateway.autonolas.tech/ipfs/f01701220" + data.hex()
-            print(f"Data arrived: {data_url}")
-            is_waiting = False
-    response = requests.get(data_url + "/" + str(request_id))
-    response_json = response.json()
-    result = response_json["result"]
-    print(f"Data:\n{result}")
-    return response_json
-
-
-def interact(prompt: str, tool: str) -> Dict[str, Any]:
-    ethereum_crypto = EthereumCrypto(private_key_path=PRIVATE_KEY_FILE_PATH)
-    ethereum_ledger_api = EthereumApi(**ETHEREUM_TESTNET_CONFIG)
-    wss = register_event_handlers(ethereum_crypto)
-    contract_instance = send_request(ethereum_crypto, ethereum_ledger_api, prompt, tool)
-    response = watch_for_events(
-        wss, contract_instance, ethereum_ledger_api, ethereum_crypto
+    """Interact with agent mech contract."""
+    contract_address = query_agent_address(agent_id=agent_id)
+    if contract_address is None:
+        raise ValueError(f"Agent with ID {agent_id} does not exist!")
+
+    private_key_path = private_key_path or PRIVATE_KEY_FILE_PATH
+    if not Path(private_key_path).exists():
+        raise FileNotFoundError(
+            f"Private key file `{private_key_path}` does not exist!"
+        )
+
+    wss = websocket.create_connection(WSS_ENDPOINT)
+    crypto = EthereumCrypto(private_key_path=private_key_path)
+    ledger_api = EthereumApi(**LEDGER_CONFIG)
+
+    tool = verify_or_retrieve_tool(agent_id=agent_id, ledger_api=ledger_api, tool=tool)
+    mech_contract = get_contract(
+        contract_address=contract_address, ledger_api=ledger_api
+    )
+    register_event_handlers(wss=wss, contract_address=contract_address, crypto=crypto)
+    send_request(
+        crypto=crypto,
+        ledger_api=ledger_api,
+        mech_contract=mech_contract,
+        prompt=prompt,
+        tool=tool,
+    )
+    request_id = watch_for_request_id(
+        wss=wss, mech_contract=mech_contract, ledger_api=ledger_api
     )
-    return response
+    print(f"Created on-chain request with ID {request_id}")
+    if confirmation_type == ConfirmationType.OFF_CHAIN:
+        data_url = watch_for_data_url_from_mech_sync(crypto=crypto)
+    elif confirmation_type == ConfirmationType.ON_CHAIN:
+        data_url = watch_for_data_url_from_wss_sync(
+            request_id=request_id,
+            wss=wss,
+            mech_contract=mech_contract,
+            ledger_api=ledger_api,
+        )
+    else:
+        data_url = wait_for_data_url(
+            request_id=request_id,
+            wss=wss,
+            mech_contract=mech_contract,
+            ledger_api=ledger_api,
+            crypto=crypto,
+        )
+    print(f"Data arrived: {data_url}")
+    data = requests.get(f"{data_url}/{request_id}").json()
+    print(f"Data from agent: {data}")
```

### Comparing `mech_client-0.1.7/mech_client/prompt_to_ipfs.py` & `mech_client-0.2.0/mech_client/prompt_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.7/mech_client/push_to_ipfs.py` & `mech_client-0.2.0/mech_client/push_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.7/mech_client/to_png.py` & `mech_client-0.2.0/mech_client/to_png.py`

 * *Files identical despite different names*

