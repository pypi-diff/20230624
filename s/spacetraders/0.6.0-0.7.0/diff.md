# Comparing `tmp/spacetraders-0.6.0.tar.gz` & `tmp/spacetraders-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetraders-0.6.0.tar", max compression
+gzip compressed data, was "spacetraders-0.7.0.tar", max compression
```

## Comparing `spacetraders-0.6.0.tar` & `spacetraders-0.7.0.tar`

### file list

```diff
@@ -1,231 +1,232 @@
--rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.6.0/README.md
--rw-r--r--   0        0        0      664 2023-06-05 13:55:27.670386 spacetraders-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      250 2023-06-05 13:53:26.330387 spacetraders-0.6.0/spacetraders/__init__.py
--rw-r--r--   0        0        0       47 2023-06-05 13:53:25.790387 spacetraders-0.6.0/spacetraders/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 13:53:25.840387 spacetraders-0.6.0/spacetraders/api/agents/__init__.py
--rw-r--r--   0        0        0     4139 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/agents/get_my_agent.py
--rw-r--r--   0        0        0        0 2023-06-05 13:53:25.840387 spacetraders-0.6.0/spacetraders/api/contracts/__init__.py
--rw-r--r--   0        0        0     4425 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/contracts/accept_contract.py
--rw-r--r--   0        0        0     5022 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/contracts/deliver_contract.py
--rw-r--r--   0        0        0     4437 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/contracts/fulfill_contract.py
--rw-r--r--   0        0        0     4420 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/contracts/get_contract.py
--rw-r--r--   0        0        0     4900 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/contracts/get_contracts.py
--rw-r--r--   0        0        0        0 2023-06-05 13:53:25.800387 spacetraders-0.6.0/spacetraders/api/default/__init__.py
--rw-r--r--   0        0        0     4069 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/default/get_status.py
--rw-r--r--   0        0        0     6960 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/default/register.py
--rw-r--r--   0        0        0        0 2023-06-05 13:53:25.840387 spacetraders-0.6.0/spacetraders/api/factions/__init__.py
--rw-r--r--   0        0        0     4427 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/factions/get_faction.py
--rw-r--r--   0        0        0     4853 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/factions/get_factions.py
--rw-r--r--   0        0        0        0 2023-06-05 13:53:25.850387 spacetraders-0.6.0/spacetraders/api/fleet/__init__.py
--rw-r--r--   0        0        0     4900 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/create_chart.py
--rw-r--r--   0        0        0     4550 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/create_ship_ship_scan.py
--rw-r--r--   0        0        0     4587 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/create_ship_system_scan.py
--rw-r--r--   0        0        0     4615 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/create_ship_waypoint_scan.py
--rw-r--r--   0        0        0     5382 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/create_survey.py
--rw-r--r--   0        0        0     4961 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/dock_ship.py
--rw-r--r--   0        0        0     5217 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/extract_resources.py
--rw-r--r--   0        0        0     4462 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/get_mounts.py
--rw-r--r--   0        0        0     4373 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/get_my_ship.py
--rw-r--r--   0        0        0     4447 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/get_my_ship_cargo.py
--rw-r--r--   0        0        0     4871 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/get_my_ships.py
--rw-r--r--   0        0        0     5562 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/get_ship_cooldown.py
--rw-r--r--   0        0        0     4414 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/get_ship_nav.py
--rw-r--r--   0        0        0     5182 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/install_mount.py
--rw-r--r--   0        0        0     4905 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/jettison.py
--rw-r--r--   0        0        0     5343 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/jump_ship.py
--rw-r--r--   0        0        0     5893 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/navigate_ship.py
--rw-r--r--   0        0        0     4905 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/negotiate_contract.py
--rw-r--r--   0        0        0     4954 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/orbit_ship.py
--rw-r--r--   0        0        0     5001 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/patch_ship_nav.py
--rw-r--r--   0        0        0     5192 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/purchase_cargo.py
--rw-r--r--   0        0        0     4680 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/purchase_ship.py
--rw-r--r--   0        0        0     4419 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/refuel_ship.py
--rw-r--r--   0        0        0     5136 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/remove_mount.py
--rw-r--r--   0        0        0     5010 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/sell_cargo.py
--rw-r--r--   0        0        0     5244 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/ship_refine.py
--rw-r--r--   0        0        0     5215 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/transfer_cargo.py
--rw-r--r--   0        0        0     5569 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/warp_ship.py
--rw-r--r--   0        0        0        0 2023-06-05 13:53:25.840387 spacetraders-0.6.0/spacetraders/api/systems/__init__.py
--rw-r--r--   0        0        0     4735 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/systems/get_jump_gate.py
--rw-r--r--   0        0        0     5121 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/systems/get_market.py
--rw-r--r--   0        0        0     4951 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/systems/get_shipyard.py
--rw-r--r--   0        0        0     4469 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/systems/get_system.py
--rw-r--r--   0        0        0     5421 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/systems/get_system_waypoints.py
--rw-r--r--   0        0        0     4877 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/systems/get_systems.py
--rw-r--r--   0        0        0     4710 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/systems/get_waypoint.py
--rw-r--r--   0        0        0     4384 2023-06-05 13:53:26.670387 spacetraders-0.6.0/spacetraders/client.py
--rw-r--r--   0        0        0      470 2023-06-05 13:53:26.580387 spacetraders-0.6.0/spacetraders/errors.py
--rw-r--r--   0        0        0    15720 2023-06-05 13:53:26.830387 spacetraders-0.6.0/spacetraders/models/__init__.py
--rw-r--r--   0        0        0     1269 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/accept_contract_response_200.py
--rw-r--r--   0        0        0     1299 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/accept_contract_response_200_data.py
--rw-r--r--   0        0        0     1587 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/agent.py
--rw-r--r--   0        0        0     1532 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/chart.py
--rw-r--r--   0        0        0     1709 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/connected_system.py
--rw-r--r--   0        0        0     2160 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/contract.py
--rw-r--r--   0        0        0     1712 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/contract_deliver_good.py
--rw-r--r--   0        0        0     1340 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/contract_payment.py
--rw-r--r--   0        0        0     1567 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/contract_terms.py
--rw-r--r--   0        0        0      201 2023-06-05 13:53:25.970387 spacetraders-0.6.0/spacetraders/models/contract_type.py
--rw-r--r--   0        0        0     1744 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/cooldown.py
--rw-r--r--   0        0        0     1251 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/create_chart_response_201.py
--rw-r--r--   0        0        0     1469 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/create_chart_response_201_data.py
--rw-r--r--   0        0        0     1304 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/create_ship_ship_scan_response_201.py
--rw-r--r--   0        0        0     1425 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/create_ship_ship_scan_response_201_data.py
--rw-r--r--   0        0        0     1316 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/create_ship_system_scan_response_201.py
--rw-r--r--   0        0        0     1443 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/create_ship_system_scan_response_201_data.py
--rw-r--r--   0        0        0     1328 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/create_ship_waypoint_scan_response_201.py
--rw-r--r--   0        0        0     1461 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
--rw-r--r--   0        0        0     1257 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/create_survey_response_201.py
--rw-r--r--   0        0        0     1398 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/create_survey_response_201_data.py
--rw-r--r--   0        0        0     1284 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/deliver_contract_json_body.py
--rw-r--r--   0        0        0     1275 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/deliver_contract_response_200.py
--rw-r--r--   0        0        0     1318 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/deliver_contract_response_200_data.py
--rw-r--r--   0        0        0     1292 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/dock_ship_dock_ship_200_response.py
--rw-r--r--   0        0        0     1227 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py
--rw-r--r--   0        0        0     1368 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/extract_resources_json_body.py
--rw-r--r--   0        0        0     1281 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/extract_resources_response_201.py
--rw-r--r--   0        0        0     1532 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/extract_resources_response_201_data.py
--rw-r--r--   0        0        0     1261 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/extraction.py
--rw-r--r--   0        0        0     1250 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/extraction_yield.py
--rw-r--r--   0        0        0     1604 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/faction.py
--rw-r--r--   0        0        0     1421 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/faction_trait.py
--rw-r--r--   0        0        0     1869 2023-06-05 13:53:26.060387 spacetraders-0.6.0/spacetraders/models/faction_trait_symbol.py
--rw-r--r--   0        0        0     1275 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/fulfill_contract_response_200.py
--rw-r--r--   0        0        0     1301 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/fulfill_contract_response_200_data.py
--rw-r--r--   0        0        0     1175 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_contract_response_200.py
--rw-r--r--   0        0        0     1282 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_contracts_response_200.py
--rw-r--r--   0        0        0     1169 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_faction_response_200.py
--rw-r--r--   0        0        0     1276 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_factions_response_200.py
--rw-r--r--   0        0        0     1176 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_jump_gate_response_200.py
--rw-r--r--   0        0        0     1163 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_market_response_200.py
--rw-r--r--   0        0        0     1208 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_mounts_get_mounts_200_response.py
--rw-r--r--   0        0        0     1161 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_my_agent_response_200.py
--rw-r--r--   0        0        0     1186 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/get_my_ship_cargo_response_200.py
--rw-r--r--   0        0        0     1162 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_my_ship_response_200.py
--rw-r--r--   0        0        0     1262 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_my_ships_response_200.py
--rw-r--r--   0        0        0     1262 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_ship_cooldown_response_200.py
--rw-r--r--   0        0        0     1210 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/get_ship_nav_response_200.py
--rw-r--r--   0        0        0     1175 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_shipyard_response_200.py
--rw-r--r--   0        0        0     2640 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_status_response_200.py
--rw-r--r--   0        0        0     1213 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_announcements_item.py
--rw-r--r--   0        0        0     1807 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_leaderboards.py
--rw-r--r--   0        0        0     1264 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py
--rw-r--r--   0        0        0     1289 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py
--rw-r--r--   0        0        0     1191 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_links_item.py
--rw-r--r--   0        0        0     1314 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_server_resets.py
--rw-r--r--   0        0        0     1331 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_stats.py
--rw-r--r--   0        0        0     1163 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_system_response_200.py
--rw-r--r--   0        0        0     1294 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_system_waypoints_response_200.py
--rw-r--r--   0        0        0     1270 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_systems_response_200.py
--rw-r--r--   0        0        0     1266 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_waypoint_response_200.py
--rw-r--r--   0        0        0     1340 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/install_mount_install_mount_201_response.py
--rw-r--r--   0        0        0     1773 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/install_mount_install_mount_201_response_data.py
--rw-r--r--   0        0        0     1385 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/install_mount_install_mount_201_response_data_transaction.py
--rw-r--r--   0        0        0     1148 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/install_mount_install_mount_request.py
--rw-r--r--   0        0        0     1177 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/jettison_json_body.py
--rw-r--r--   0        0        0     1232 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/jettison_response_200.py
--rw-r--r--   0        0        0     1185 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/jettison_response_200_data.py
--rw-r--r--   0        0        0     1606 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/jump_gate.py
--rw-r--r--   0        0        0     1168 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/jump_ship_json_body.py
--rw-r--r--   0        0        0     1233 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/jump_ship_response_200.py
--rw-r--r--   0        0        0     1462 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/jump_ship_response_200_data.py
--rw-r--r--   0        0        0     2398 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/market.py
--rw-r--r--   0        0        0     1880 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/market_trade_good.py
--rw-r--r--   0        0        0      224 2023-06-05 13:53:25.980387 spacetraders-0.6.0/spacetraders/models/market_trade_good_supply.py
--rw-r--r--   0        0        0     2109 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/market_transaction.py
--rw-r--r--   0        0        0      170 2023-06-05 13:53:25.980387 spacetraders-0.6.0/spacetraders/models/market_transaction_type.py
--rw-r--r--   0        0        0     1206 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/meta.py
--rw-r--r--   0        0        0     1176 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/navigate_ship_json_body.py
--rw-r--r--   0        0        0     1257 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/navigate_ship_response_200.py
--rw-r--r--   0        0        0     1444 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/navigate_ship_response_200_data.py
--rw-r--r--   0        0        0     1400 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py
--rw-r--r--   0        0        0     1241 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py
--rw-r--r--   0        0        0     1304 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py
--rw-r--r--   0        0        0     1231 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
--rw-r--r--   0        0        0     1420 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/patch_ship_nav_json_body.py
--rw-r--r--   0        0        0     1214 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/patch_ship_nav_response_200.py
--rw-r--r--   0        0        0     1352 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
--rw-r--r--   0        0        0     1484 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
--rw-r--r--   0        0        0     1211 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py
--rw-r--r--   0        0        0     1333 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/purchase_ship_json_body.py
--rw-r--r--   0        0        0     1257 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/purchase_ship_response_201.py
--rw-r--r--   0        0        0     1447 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/purchase_ship_response_201_data.py
--rw-r--r--   0        0        0     1245 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/refuel_ship_response_200.py
--rw-r--r--   0        0        0     1562 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/refuel_ship_response_200_data.py
--rw-r--r--   0        0        0     1516 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/register_json_body.py
--rw-r--r--   0        0        0     1232 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/register_response_201.py
--rw-r--r--   0        0        0     1608 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/register_response_201_data.py
--rw-r--r--   0        0        0     1328 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/remove_mount_remove_mount_201_response.py
--rw-r--r--   0        0        0     1761 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/remove_mount_remove_mount_201_response_data.py
--rw-r--r--   0        0        0     1381 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/remove_mount_remove_mount_201_response_data_transaction.py
--rw-r--r--   0        0        0     1144 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/remove_mount_remove_mount_request.py
--rw-r--r--   0        0        0     2444 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/scanned_ship.py
--rw-r--r--   0        0        0     1144 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/scanned_ship_engine.py
--rw-r--r--   0        0        0     1141 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/scanned_ship_frame.py
--rw-r--r--   0        0        0     1149 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/scanned_ship_mounts_item.py
--rw-r--r--   0        0        0     1147 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/scanned_ship_reactor.py
--rw-r--r--   0        0        0     1492 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/scanned_system.py
--rw-r--r--   0        0        0     2293 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/scanned_waypoint.py
--rw-r--r--   0        0        0     1304 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py
--rw-r--r--   0        0        0     1468 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
--rw-r--r--   0        0        0     1195 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/sell_cargo_sell_cargo_request.py
--rw-r--r--   0        0        0     3140 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship.py
--rw-r--r--   0        0        0     1484 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_cargo.py
--rw-r--r--   0        0        0     1510 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/ship_cargo_item.py
--rw-r--r--   0        0        0     2248 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/ship_crew.py
--rw-r--r--   0        0        0      167 2023-06-05 13:53:25.940387 spacetraders-0.6.0/spacetraders/models/ship_crew_rotation.py
--rw-r--r--   0        0        0     1879 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_engine.py
--rw-r--r--   0        0        0      319 2023-06-05 13:53:26.040387 spacetraders-0.6.0/spacetraders/models/ship_engine_symbol.py
--rw-r--r--   0        0        0     2278 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship_frame.py
--rw-r--r--   0        0        0      694 2023-06-05 13:53:25.960387 spacetraders-0.6.0/spacetraders/models/ship_frame_symbol.py
--rw-r--r--   0        0        0     1586 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/ship_fuel.py
--rw-r--r--   0        0        0     1340 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/ship_fuel_consumed.py
--rw-r--r--   0        0        0     1965 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship_module.py
--rw-r--r--   0        0        0     1033 2023-06-05 13:53:25.990387 spacetraders-0.6.0/spacetraders/models/ship_module_symbol.py
--rw-r--r--   0        0        0     1947 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_mount.py
--rw-r--r--   0        0        0      572 2023-06-05 13:53:26.050387 spacetraders-0.6.0/spacetraders/models/ship_mount_deposits_item.py
--rw-r--r--   0        0        0      854 2023-06-05 13:53:26.050387 spacetraders-0.6.0/spacetraders/models/ship_mount_symbol.py
--rw-r--r--   0        0        0     2114 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_nav.py
--rw-r--r--   0        0        0      206 2023-06-05 13:53:25.960387 spacetraders-0.6.0/spacetraders/models/ship_nav_flight_mode.py
--rw-r--r--   0        0        0     1891 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship_nav_route.py
--rw-r--r--   0        0        0     1497 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship_nav_route_waypoint.py
--rw-r--r--   0        0        0      196 2023-06-05 13:53:25.980387 spacetraders-0.6.0/spacetraders/models/ship_nav_status.py
--rw-r--r--   0        0        0     1934 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_reactor.py
--rw-r--r--   0        0        0      344 2023-06-05 13:53:25.960387 spacetraders-0.6.0/spacetraders/models/ship_reactor_symbol.py
--rw-r--r--   0        0        0     1246 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/ship_refine_json_body.py
--rw-r--r--   0        0        0      330 2023-06-05 13:53:26.040387 spacetraders-0.6.0/spacetraders/models/ship_refine_json_body_produce.py
--rw-r--r--   0        0        0     1316 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response.py
--rw-r--r--   0        0        0     2047 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py
--rw-r--r--   0        0        0     1344 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
--rw-r--r--   0        0        0     1344 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
--rw-r--r--   0        0        0     1477 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship_registration.py
--rw-r--r--   0        0        0     1541 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship_requirements.py
--rw-r--r--   0        0        0      479 2023-06-05 13:53:26.030387 spacetraders-0.6.0/spacetraders/models/ship_role.py
--rw-r--r--   0        0        0      549 2023-06-05 13:53:25.950387 spacetraders-0.6.0/spacetraders/models/ship_type.py
--rw-r--r--   0        0        0     2009 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/shipyard.py
--rw-r--r--   0        0        0     2498 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/shipyard_ship.py
--rw-r--r--   0        0        0     1225 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/shipyard_ship_types_item.py
--rw-r--r--   0        0        0     1698 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/shipyard_transaction.py
--rw-r--r--   0        0        0     2228 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/survey.py
--rw-r--r--   0        0        0     1209 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/survey_deposit.py
--rw-r--r--   0        0        0      181 2023-06-05 13:53:25.970387 spacetraders-0.6.0/spacetraders/models/survey_size.py
--rw-r--r--   0        0        0     1725 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/system.py
--rw-r--r--   0        0        0     1112 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/system_faction.py
--rw-r--r--   0        0        0      405 2023-06-05 13:53:25.960387 spacetraders-0.6.0/spacetraders/models/system_type.py
--rw-r--r--   0        0        0     1352 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/system_waypoint.py
--rw-r--r--   0        0        0     1299 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/trade_good.py
--rw-r--r--   0        0        0     4422 2023-06-05 13:53:26.030387 spacetraders-0.6.0/spacetraders/models/trade_symbol.py
--rw-r--r--   0        0        0     1352 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
--rw-r--r--   0        0        0     1221 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
--rw-r--r--   0        0        0     1304 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py
--rw-r--r--   0        0        0     1168 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/warp_ship_json_body.py
--rw-r--r--   0        0        0     1233 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/warp_ship_response_200.py
--rw-r--r--   0        0        0     1436 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/warp_ship_response_200_data.py
--rw-r--r--   0        0        0     2279 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/waypoint.py
--rw-r--r--   0        0        0     1116 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/waypoint_faction.py
--rw-r--r--   0        0        0     1178 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/waypoint_orbital.py
--rw-r--r--   0        0        0     1427 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/waypoint_trait.py
--rw-r--r--   0        0        0     2200 2023-06-05 13:53:26.060387 spacetraders-0.6.0/spacetraders/models/waypoint_trait_symbol.py
--rw-r--r--   0        0        0      381 2023-06-05 13:53:25.970387 spacetraders-0.6.0/spacetraders/models/waypoint_type.py
--rw-r--r--   0        0        0     1341 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/types.py
--rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 spacetraders-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3472 2023-06-24 20:27:51.914738 spacetraders-0.7.0/README.md
+-rw-r--r--   0        0        0      664 2023-06-24 20:46:22.094297 spacetraders-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      250 2023-06-24 20:29:35.619679 spacetraders-0.7.0/spacetraders/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-24 20:29:32.919850 spacetraders-0.7.0/spacetraders/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:29:32.999539 spacetraders-0.7.0/spacetraders/api/agents/__init__.py
+-rw-r--r--   0        0        0     4125 2023-06-24 20:29:37.266883 spacetraders-0.7.0/spacetraders/api/agents/get_my_agent.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:29:33.000673 spacetraders-0.7.0/spacetraders/api/contracts/__init__.py
+-rw-r--r--   0        0        0     4693 2023-06-24 20:29:37.260816 spacetraders-0.7.0/spacetraders/api/contracts/accept_contract.py
+-rw-r--r--   0        0        0     5626 2023-06-24 20:29:37.256620 spacetraders-0.7.0/spacetraders/api/contracts/deliver_contract.py
+-rw-r--r--   0        0        0     4597 2023-06-24 20:29:37.258777 spacetraders-0.7.0/spacetraders/api/contracts/fulfill_contract.py
+-rw-r--r--   0        0        0     4420 2023-06-24 20:29:37.264954 spacetraders-0.7.0/spacetraders/api/contracts/get_contract.py
+-rw-r--r--   0        0        0     4971 2023-06-24 20:29:37.262957 spacetraders-0.7.0/spacetraders/api/contracts/get_contracts.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:29:32.933836 spacetraders-0.7.0/spacetraders/api/default/__init__.py
+-rw-r--r--   0        0        0     4349 2023-06-24 20:29:37.254483 spacetraders-0.7.0/spacetraders/api/default/get_status.py
+-rw-r--r--   0        0        0     7032 2023-06-24 20:29:37.252421 spacetraders-0.7.0/spacetraders/api/default/register.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:29:32.997177 spacetraders-0.7.0/spacetraders/api/factions/__init__.py
+-rw-r--r--   0        0        0     4405 2023-06-24 20:29:37.260808 spacetraders-0.7.0/spacetraders/api/factions/get_faction.py
+-rw-r--r--   0        0        0     4976 2023-06-24 20:29:37.258693 spacetraders-0.7.0/spacetraders/api/factions/get_factions.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:29:33.006677 spacetraders-0.7.0/spacetraders/api/fleet/__init__.py
+-rw-r--r--   0        0        0     5084 2023-06-24 20:29:37.252290 spacetraders-0.7.0/spacetraders/api/fleet/create_chart.py
+-rw-r--r--   0        0        0     4934 2023-06-24 20:29:37.269622 spacetraders-0.7.0/spacetraders/api/fleet/create_ship_ship_scan.py
+-rw-r--r--   0        0        0     5041 2023-06-24 20:29:37.274022 spacetraders-0.7.0/spacetraders/api/fleet/create_ship_system_scan.py
+-rw-r--r--   0        0        0     5265 2023-06-24 20:29:37.252336 spacetraders-0.7.0/spacetraders/api/fleet/create_ship_waypoint_scan.py
+-rw-r--r--   0        0        0     6196 2023-06-24 20:29:37.274124 spacetraders-0.7.0/spacetraders/api/fleet/create_survey.py
+-rw-r--r--   0        0        0     5279 2023-06-24 20:29:37.275010 spacetraders-0.7.0/spacetraders/api/fleet/dock_ship.py
+-rw-r--r--   0        0        0     5757 2023-06-24 20:29:37.258716 spacetraders-0.7.0/spacetraders/api/fleet/extract_resources.py
+-rw-r--r--   0        0        0     4482 2023-06-24 20:29:37.273105 spacetraders-0.7.0/spacetraders/api/fleet/get_mounts.py
+-rw-r--r--   0        0        0     4425 2023-06-24 20:29:37.263003 spacetraders-0.7.0/spacetraders/api/fleet/get_my_ship.py
+-rw-r--r--   0        0        0     4499 2023-06-24 20:29:37.267434 spacetraders-0.7.0/spacetraders/api/fleet/get_my_ship_cargo.py
+-rw-r--r--   0        0        0     4988 2023-06-24 20:29:37.269241 spacetraders-0.7.0/spacetraders/api/fleet/get_my_ships.py
+-rw-r--r--   0        0        0     5562 2023-06-24 20:29:37.270076 spacetraders-0.7.0/spacetraders/api/fleet/get_ship_cooldown.py
+-rw-r--r--   0        0        0     4414 2023-06-24 20:29:37.271452 spacetraders-0.7.0/spacetraders/api/fleet/get_ship_nav.py
+-rw-r--r--   0        0        0     5734 2023-06-24 20:29:37.266779 spacetraders-0.7.0/spacetraders/api/fleet/install_mount.py
+-rw-r--r--   0        0        0     4905 2023-06-24 20:29:37.271231 spacetraders-0.7.0/spacetraders/api/fleet/jettison.py
+-rw-r--r--   0        0        0     5999 2023-06-24 20:29:37.267846 spacetraders-0.7.0/spacetraders/api/fleet/jump_ship.py
+-rw-r--r--   0        0        0     5985 2023-06-24 20:29:37.256613 spacetraders-0.7.0/spacetraders/api/fleet/navigate_ship.py
+-rw-r--r--   0        0        0     5533 2023-06-24 20:29:37.269555 spacetraders-0.7.0/spacetraders/api/fleet/negotiate_contract.py
+-rw-r--r--   0        0        0     5382 2023-06-24 20:29:37.254358 spacetraders-0.7.0/spacetraders/api/fleet/orbit_ship.py
+-rw-r--r--   0        0        0     5209 2023-06-24 20:29:37.272140 spacetraders-0.7.0/spacetraders/api/fleet/patch_ship_nav.py
+-rw-r--r--   0        0        0     6004 2023-06-24 20:29:37.273035 spacetraders-0.7.0/spacetraders/api/fleet/purchase_cargo.py
+-rw-r--r--   0        0        0     5550 2023-06-24 20:29:37.271640 spacetraders-0.7.0/spacetraders/api/fleet/purchase_ship.py
+-rw-r--r--   0        0        0     5599 2023-06-24 20:29:37.272066 spacetraders-0.7.0/spacetraders/api/fleet/refuel_ship.py
+-rw-r--r--   0        0        0     5558 2023-06-24 20:29:37.265577 spacetraders-0.7.0/spacetraders/api/fleet/remove_mount.py
+-rw-r--r--   0        0        0     5318 2023-06-24 20:29:37.256437 spacetraders-0.7.0/spacetraders/api/fleet/sell_cargo.py
+-rw-r--r--   0        0        0     5679 2023-06-24 20:29:37.261097 spacetraders-0.7.0/spacetraders/api/fleet/ship_refine.py
+-rw-r--r--   0        0        0     5929 2023-06-24 20:29:37.268935 spacetraders-0.7.0/spacetraders/api/fleet/transfer_cargo.py
+-rw-r--r--   0        0        0     5633 2023-06-24 20:29:37.254472 spacetraders-0.7.0/spacetraders/api/fleet/warp_ship.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:29:32.986313 spacetraders-0.7.0/spacetraders/api/systems/__init__.py
+-rw-r--r--   0        0        0     5135 2023-06-24 20:29:37.260834 spacetraders-0.7.0/spacetraders/api/systems/get_jump_gate.py
+-rw-r--r--   0        0        0     5369 2023-06-24 20:29:37.254413 spacetraders-0.7.0/spacetraders/api/systems/get_market.py
+-rw-r--r--   0        0        0     5091 2023-06-24 20:29:37.265086 spacetraders-0.7.0/spacetraders/api/systems/get_shipyard.py
+-rw-r--r--   0        0        0     4469 2023-06-24 20:29:37.252252 spacetraders-0.7.0/spacetraders/api/systems/get_system.py
+-rw-r--r--   0        0        0     5554 2023-06-24 20:29:37.263180 spacetraders-0.7.0/spacetraders/api/systems/get_system_waypoints.py
+-rw-r--r--   0        0        0     4930 2023-06-24 20:29:37.258779 spacetraders-0.7.0/spacetraders/api/systems/get_systems.py
+-rw-r--r--   0        0        0     4914 2023-06-24 20:29:37.256673 spacetraders-0.7.0/spacetraders/api/systems/get_waypoint.py
+-rw-r--r--   0        0        0     4384 2023-06-24 20:29:36.106117 spacetraders-0.7.0/spacetraders/client.py
+-rw-r--r--   0        0        0      470 2023-06-24 20:29:36.024133 spacetraders-0.7.0/spacetraders/errors.py
+-rw-r--r--   0        0        0    15600 2023-06-24 20:29:36.227660 spacetraders-0.7.0/spacetraders/models/__init__.py
+-rw-r--r--   0        0        0     1269 2023-06-24 20:29:37.273588 spacetraders-0.7.0/spacetraders/models/accept_contract_response_200.py
+-rw-r--r--   0        0        0     1332 2023-06-24 20:29:37.275575 spacetraders-0.7.0/spacetraders/models/accept_contract_response_200_data.py
+-rw-r--r--   0        0        0     1662 2023-06-24 20:29:37.267518 spacetraders-0.7.0/spacetraders/models/agent.py
+-rw-r--r--   0        0        0     1666 2023-06-24 20:29:37.271683 spacetraders-0.7.0/spacetraders/models/chart.py
+-rw-r--r--   0        0        0     1898 2023-06-24 20:29:37.274449 spacetraders-0.7.0/spacetraders/models/connected_system.py
+-rw-r--r--   0        0        0     2260 2023-06-24 20:29:37.269929 spacetraders-0.7.0/spacetraders/models/contract.py
+-rw-r--r--   0        0        0     1712 2023-06-24 20:29:37.274921 spacetraders-0.7.0/spacetraders/models/contract_deliver_good.py
+-rw-r--r--   0        0        0     1340 2023-06-24 20:29:37.274496 spacetraders-0.7.0/spacetraders/models/contract_payment.py
+-rw-r--r--   0        0        0     1685 2023-06-24 20:29:37.273114 spacetraders-0.7.0/spacetraders/models/contract_terms.py
+-rw-r--r--   0        0        0      201 2023-06-24 20:29:33.411910 spacetraders-0.7.0/spacetraders/models/contract_type.py
+-rw-r--r--   0        0        0     1744 2023-06-24 20:29:37.273296 spacetraders-0.7.0/spacetraders/models/cooldown.py
+-rw-r--r--   0        0        0     1251 2023-06-24 20:29:37.274448 spacetraders-0.7.0/spacetraders/models/create_chart_response_201.py
+-rw-r--r--   0        0        0     1469 2023-06-24 20:29:37.257059 spacetraders-0.7.0/spacetraders/models/create_chart_response_201_data.py
+-rw-r--r--   0        0        0     1304 2023-06-24 20:29:37.251912 spacetraders-0.7.0/spacetraders/models/create_ship_ship_scan_response_201.py
+-rw-r--r--   0        0        0     1448 2023-06-24 20:29:37.253238 spacetraders-0.7.0/spacetraders/models/create_ship_ship_scan_response_201_data.py
+-rw-r--r--   0        0        0     1316 2023-06-24 20:29:37.259029 spacetraders-0.7.0/spacetraders/models/create_ship_system_scan_response_201.py
+-rw-r--r--   0        0        0     1468 2023-06-24 20:29:37.260487 spacetraders-0.7.0/spacetraders/models/create_ship_system_scan_response_201_data.py
+-rw-r--r--   0        0        0     1328 2023-06-24 20:29:37.269579 spacetraders-0.7.0/spacetraders/models/create_ship_waypoint_scan_response_201.py
+-rw-r--r--   0        0        0     1488 2023-06-24 20:29:37.268046 spacetraders-0.7.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
+-rw-r--r--   0        0        0     1257 2023-06-24 20:29:37.275222 spacetraders-0.7.0/spacetraders/models/create_survey_response_201.py
+-rw-r--r--   0        0        0     1430 2023-06-24 20:29:37.259354 spacetraders-0.7.0/spacetraders/models/create_survey_response_201_data.py
+-rw-r--r--   0        0        0     1470 2023-06-24 20:29:37.260394 spacetraders-0.7.0/spacetraders/models/deliver_contract_json_body.py
+-rw-r--r--   0        0        0     1275 2023-06-24 20:29:37.257743 spacetraders-0.7.0/spacetraders/models/deliver_contract_response_200.py
+-rw-r--r--   0        0        0     1356 2023-06-24 20:29:37.255066 spacetraders-0.7.0/spacetraders/models/deliver_contract_response_200_data.py
+-rw-r--r--   0        0        0     1292 2023-06-24 20:29:37.251913 spacetraders-0.7.0/spacetraders/models/dock_ship_dock_ship_200_response.py
+-rw-r--r--   0        0        0     1227 2023-06-24 20:29:37.257677 spacetraders-0.7.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py
+-rw-r--r--   0        0        0     1368 2023-06-24 20:29:37.255383 spacetraders-0.7.0/spacetraders/models/extract_resources_json_body.py
+-rw-r--r--   0        0        0     1281 2023-06-24 20:29:37.270863 spacetraders-0.7.0/spacetraders/models/extract_resources_response_201.py
+-rw-r--r--   0        0        0     1572 2023-06-24 20:29:37.267932 spacetraders-0.7.0/spacetraders/models/extract_resources_response_201_data.py
+-rw-r--r--   0        0        0     1369 2023-06-24 20:29:37.259979 spacetraders-0.7.0/spacetraders/models/extraction.py
+-rw-r--r--   0        0        0     1370 2023-06-24 20:29:37.263352 spacetraders-0.7.0/spacetraders/models/extraction_yield.py
+-rw-r--r--   0        0        0     1866 2023-06-24 20:29:37.270834 spacetraders-0.7.0/spacetraders/models/faction.py
+-rw-r--r--   0        0        0      547 2023-06-24 20:29:33.363711 spacetraders-0.7.0/spacetraders/models/faction_symbols.py
+-rw-r--r--   0        0        0     1421 2023-06-24 20:29:37.260205 spacetraders-0.7.0/spacetraders/models/faction_trait.py
+-rw-r--r--   0        0        0     1869 2023-06-24 20:29:33.464077 spacetraders-0.7.0/spacetraders/models/faction_trait_symbol.py
+-rw-r--r--   0        0        0     1275 2023-06-24 20:29:37.259694 spacetraders-0.7.0/spacetraders/models/fulfill_contract_response_200.py
+-rw-r--r--   0        0        0     1334 2023-06-24 20:29:37.255161 spacetraders-0.7.0/spacetraders/models/fulfill_contract_response_200_data.py
+-rw-r--r--   0        0        0     1193 2023-06-24 20:29:37.257297 spacetraders-0.7.0/spacetraders/models/get_contract_response_200.py
+-rw-r--r--   0        0        0     1311 2023-06-24 20:29:37.261772 spacetraders-0.7.0/spacetraders/models/get_contracts_response_200.py
+-rw-r--r--   0        0        0     1186 2023-06-24 20:29:37.251912 spacetraders-0.7.0/spacetraders/models/get_faction_response_200.py
+-rw-r--r--   0        0        0     1305 2023-06-24 20:29:37.270313 spacetraders-0.7.0/spacetraders/models/get_factions_response_200.py
+-rw-r--r--   0        0        0     1176 2023-06-24 20:29:37.262583 spacetraders-0.7.0/spacetraders/models/get_jump_gate_response_200.py
+-rw-r--r--   0        0        0     1163 2023-06-24 20:29:37.262053 spacetraders-0.7.0/spacetraders/models/get_market_response_200.py
+-rw-r--r--   0        0        0     1208 2023-06-24 20:29:37.263245 spacetraders-0.7.0/spacetraders/models/get_mounts_get_mounts_200_response.py
+-rw-r--r--   0        0        0     1176 2023-06-24 20:29:37.256954 spacetraders-0.7.0/spacetraders/models/get_my_agent_response_200.py
+-rw-r--r--   0        0        0     1206 2023-06-24 20:29:37.270565 spacetraders-0.7.0/spacetraders/models/get_my_ship_cargo_response_200.py
+-rw-r--r--   0        0        0     1169 2023-06-24 20:29:37.262033 spacetraders-0.7.0/spacetraders/models/get_my_ship_response_200.py
+-rw-r--r--   0        0        0     1291 2023-06-24 20:29:37.256300 spacetraders-0.7.0/spacetraders/models/get_my_ships_response_200.py
+-rw-r--r--   0        0        0     1262 2023-06-24 20:29:37.260599 spacetraders-0.7.0/spacetraders/models/get_ship_cooldown_response_200.py
+-rw-r--r--   0        0        0     1210 2023-06-24 20:29:37.269398 spacetraders-0.7.0/spacetraders/models/get_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1175 2023-06-24 20:29:37.254866 spacetraders-0.7.0/spacetraders/models/get_shipyard_response_200.py
+-rw-r--r--   0        0        0     2628 2023-06-24 20:29:37.271035 spacetraders-0.7.0/spacetraders/models/get_status_response_200.py
+-rw-r--r--   0        0        0     1213 2023-06-24 20:29:37.260541 spacetraders-0.7.0/spacetraders/models/get_status_response_200_announcements_item.py
+-rw-r--r--   0        0        0     1897 2023-06-24 20:29:37.253760 spacetraders-0.7.0/spacetraders/models/get_status_response_200_leaderboards.py
+-rw-r--r--   0        0        0     1304 2023-06-24 20:29:37.272512 spacetraders-0.7.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py
+-rw-r--r--   0        0        0     1346 2023-06-24 20:29:37.255422 spacetraders-0.7.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py
+-rw-r--r--   0        0        0     1191 2023-06-24 20:29:37.261039 spacetraders-0.7.0/spacetraders/models/get_status_response_200_links_item.py
+-rw-r--r--   0        0        0     1314 2023-06-24 20:29:37.256461 spacetraders-0.7.0/spacetraders/models/get_status_response_200_server_resets.py
+-rw-r--r--   0        0        0     1483 2023-06-24 20:29:37.268384 spacetraders-0.7.0/spacetraders/models/get_status_response_200_stats.py
+-rw-r--r--   0        0        0     1163 2023-06-24 20:29:37.255075 spacetraders-0.7.0/spacetraders/models/get_system_response_200.py
+-rw-r--r--   0        0        0     1323 2023-06-24 20:29:37.275267 spacetraders-0.7.0/spacetraders/models/get_system_waypoints_response_200.py
+-rw-r--r--   0        0        0     1299 2023-06-24 20:29:37.273759 spacetraders-0.7.0/spacetraders/models/get_systems_response_200.py
+-rw-r--r--   0        0        0     1266 2023-06-24 20:29:37.262895 spacetraders-0.7.0/spacetraders/models/get_waypoint_response_200.py
+-rw-r--r--   0        0        0     1340 2023-06-24 20:29:37.259253 spacetraders-0.7.0/spacetraders/models/install_mount_install_mount_201_response.py
+-rw-r--r--   0        0        0     1855 2023-06-24 20:29:37.253675 spacetraders-0.7.0/spacetraders/models/install_mount_install_mount_201_response_data.py
+-rw-r--r--   0        0        0     1148 2023-06-24 20:29:37.264648 spacetraders-0.7.0/spacetraders/models/install_mount_install_mount_request.py
+-rw-r--r--   0        0        0     1300 2023-06-24 20:29:37.262150 spacetraders-0.7.0/spacetraders/models/jettison_json_body.py
+-rw-r--r--   0        0        0     1232 2023-06-24 20:29:37.273013 spacetraders-0.7.0/spacetraders/models/jettison_response_200.py
+-rw-r--r--   0        0        0     1205 2023-06-24 20:29:37.266835 spacetraders-0.7.0/spacetraders/models/jettison_response_200_data.py
+-rw-r--r--   0        0        0     1606 2023-06-24 20:29:37.273250 spacetraders-0.7.0/spacetraders/models/jump_gate.py
+-rw-r--r--   0        0        0     1168 2023-06-24 20:29:37.259392 spacetraders-0.7.0/spacetraders/models/jump_ship_json_body.py
+-rw-r--r--   0        0        0     1233 2023-06-24 20:29:37.271942 spacetraders-0.7.0/spacetraders/models/jump_ship_response_200.py
+-rw-r--r--   0        0        0     1409 2023-06-24 20:29:37.265907 spacetraders-0.7.0/spacetraders/models/jump_ship_response_200_data.py
+-rw-r--r--   0        0        0     2398 2023-06-24 20:29:37.263607 spacetraders-0.7.0/spacetraders/models/market.py
+-rw-r--r--   0        0        0     1880 2023-06-24 20:29:37.274291 spacetraders-0.7.0/spacetraders/models/market_trade_good.py
+-rw-r--r--   0        0        0      224 2023-06-24 20:29:33.570681 spacetraders-0.7.0/spacetraders/models/market_trade_good_supply.py
+-rw-r--r--   0        0        0     2148 2023-06-24 20:29:37.276130 spacetraders-0.7.0/spacetraders/models/market_transaction.py
+-rw-r--r--   0        0        0      170 2023-06-24 20:29:33.538978 spacetraders-0.7.0/spacetraders/models/market_transaction_type.py
+-rw-r--r--   0        0        0     1536 2023-06-24 20:29:37.251920 spacetraders-0.7.0/spacetraders/models/meta.py
+-rw-r--r--   0        0        0     1176 2023-06-24 20:29:37.256356 spacetraders-0.7.0/spacetraders/models/navigate_ship_json_body.py
+-rw-r--r--   0        0        0     1257 2023-06-24 20:29:37.267932 spacetraders-0.7.0/spacetraders/models/navigate_ship_response_200.py
+-rw-r--r--   0        0        0     1444 2023-06-24 20:29:37.264238 spacetraders-0.7.0/spacetraders/models/navigate_ship_response_200_data.py
+-rw-r--r--   0        0        0     1400 2023-06-24 20:29:37.252033 spacetraders-0.7.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py
+-rw-r--r--   0        0        0     1259 2023-06-24 20:29:37.261520 spacetraders-0.7.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py
+-rw-r--r--   0        0        0     1304 2023-06-24 20:29:37.264151 spacetraders-0.7.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py
+-rw-r--r--   0        0        0     1231 2023-06-24 20:29:37.267085 spacetraders-0.7.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
+-rw-r--r--   0        0        0     1420 2023-06-24 20:29:37.271428 spacetraders-0.7.0/spacetraders/models/patch_ship_nav_json_body.py
+-rw-r--r--   0        0        0     1214 2023-06-24 20:29:37.261379 spacetraders-0.7.0/spacetraders/models/patch_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1352 2023-06-24 20:29:37.254578 spacetraders-0.7.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
+-rw-r--r--   0        0        0     1558 2023-06-24 20:29:37.262169 spacetraders-0.7.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1322 2023-06-24 20:29:37.268620 spacetraders-0.7.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py
+-rw-r--r--   0        0        0     1346 2023-06-24 20:29:37.263538 spacetraders-0.7.0/spacetraders/models/purchase_ship_json_body.py
+-rw-r--r--   0        0        0     1257 2023-06-24 20:29:37.265131 spacetraders-0.7.0/spacetraders/models/purchase_ship_response_201.py
+-rw-r--r--   0        0        0     1511 2023-06-24 20:29:37.265279 spacetraders-0.7.0/spacetraders/models/purchase_ship_response_201_data.py
+-rw-r--r--   0        0        0     1546 2023-06-24 20:29:37.263768 spacetraders-0.7.0/spacetraders/models/refuel_ship_json_body.py
+-rw-r--r--   0        0        0     1245 2023-06-24 20:29:37.252030 spacetraders-0.7.0/spacetraders/models/refuel_ship_response_200.py
+-rw-r--r--   0        0        0     1616 2023-06-24 20:29:37.258230 spacetraders-0.7.0/spacetraders/models/refuel_ship_response_200_data.py
+-rw-r--r--   0        0        0     1628 2023-06-24 20:29:37.260857 spacetraders-0.7.0/spacetraders/models/register_json_body.py
+-rw-r--r--   0        0        0     1232 2023-06-24 20:29:37.269174 spacetraders-0.7.0/spacetraders/models/register_response_201.py
+-rw-r--r--   0        0        0     1665 2023-06-24 20:29:37.272872 spacetraders-0.7.0/spacetraders/models/register_response_201_data.py
+-rw-r--r--   0        0        0     1328 2023-06-24 20:29:37.274184 spacetraders-0.7.0/spacetraders/models/remove_mount_remove_mount_201_response.py
+-rw-r--r--   0        0        0     1851 2023-06-24 20:29:37.264571 spacetraders-0.7.0/spacetraders/models/remove_mount_remove_mount_201_response_data.py
+-rw-r--r--   0        0        0     1179 2023-06-24 20:29:37.263145 spacetraders-0.7.0/spacetraders/models/remove_mount_remove_mount_request.py
+-rw-r--r--   0        0        0     2482 2023-06-24 20:29:37.258559 spacetraders-0.7.0/spacetraders/models/scanned_ship.py
+-rw-r--r--   0        0        0     1170 2023-06-24 20:29:37.264382 spacetraders-0.7.0/spacetraders/models/scanned_ship_engine.py
+-rw-r--r--   0        0        0     1166 2023-06-24 20:29:37.267376 spacetraders-0.7.0/spacetraders/models/scanned_ship_frame.py
+-rw-r--r--   0        0        0     1174 2023-06-24 20:29:37.258826 spacetraders-0.7.0/spacetraders/models/scanned_ship_mounts_item.py
+-rw-r--r--   0        0        0     1174 2023-06-24 20:29:37.254277 spacetraders-0.7.0/spacetraders/models/scanned_ship_reactor.py
+-rw-r--r--   0        0        0     1709 2023-06-24 20:29:37.253710 spacetraders-0.7.0/spacetraders/models/scanned_system.py
+-rw-r--r--   0        0        0     2451 2023-06-24 20:29:37.260669 spacetraders-0.7.0/spacetraders/models/scanned_waypoint.py
+-rw-r--r--   0        0        0     1304 2023-06-24 20:29:37.255599 spacetraders-0.7.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py
+-rw-r--r--   0        0        0     1542 2023-06-24 20:29:37.266731 spacetraders-0.7.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1323 2023-06-24 20:29:37.259214 spacetraders-0.7.0/spacetraders/models/sell_cargo_sell_cargo_request.py
+-rw-r--r--   0        0        0     3230 2023-06-24 20:29:37.254032 spacetraders-0.7.0/spacetraders/models/ship.py
+-rw-r--r--   0        0        0     1504 2023-06-24 20:29:37.266323 spacetraders-0.7.0/spacetraders/models/ship_cargo.py
+-rw-r--r--   0        0        0     1510 2023-06-24 20:29:37.258883 spacetraders-0.7.0/spacetraders/models/ship_cargo_item.py
+-rw-r--r--   0        0        0     2248 2023-06-24 20:29:37.269821 spacetraders-0.7.0/spacetraders/models/ship_crew.py
+-rw-r--r--   0        0        0      167 2023-06-24 20:29:33.313610 spacetraders-0.7.0/spacetraders/models/ship_crew_rotation.py
+-rw-r--r--   0        0        0     2135 2023-06-24 20:29:37.263267 spacetraders-0.7.0/spacetraders/models/ship_engine.py
+-rw-r--r--   0        0        0      319 2023-06-24 20:29:33.254096 spacetraders-0.7.0/spacetraders/models/ship_engine_symbol.py
+-rw-r--r--   0        0        0     2904 2023-06-24 20:29:37.274828 spacetraders-0.7.0/spacetraders/models/ship_frame.py
+-rw-r--r--   0        0        0      694 2023-06-24 20:29:33.478392 spacetraders-0.7.0/spacetraders/models/ship_frame_symbol.py
+-rw-r--r--   0        0        0     1709 2023-06-24 20:29:37.264749 spacetraders-0.7.0/spacetraders/models/ship_fuel.py
+-rw-r--r--   0        0        0     1451 2023-06-24 20:29:37.258181 spacetraders-0.7.0/spacetraders/models/ship_fuel_consumed.py
+-rw-r--r--   0        0        0     1812 2023-06-24 20:29:37.258141 spacetraders-0.7.0/spacetraders/models/ship_modification_transaction.py
+-rw-r--r--   0        0        0     2306 2023-06-24 20:29:37.268133 spacetraders-0.7.0/spacetraders/models/ship_module.py
+-rw-r--r--   0        0        0     1033 2023-06-24 20:29:33.277679 spacetraders-0.7.0/spacetraders/models/ship_module_symbol.py
+-rw-r--r--   0        0        0     2226 2023-06-24 20:29:37.264182 spacetraders-0.7.0/spacetraders/models/ship_mount.py
+-rw-r--r--   0        0        0      572 2023-06-24 20:29:33.515951 spacetraders-0.7.0/spacetraders/models/ship_mount_deposits_item.py
+-rw-r--r--   0        0        0      854 2023-06-24 20:29:33.333297 spacetraders-0.7.0/spacetraders/models/ship_mount_symbol.py
+-rw-r--r--   0        0        0     2114 2023-06-24 20:29:37.256214 spacetraders-0.7.0/spacetraders/models/ship_nav.py
+-rw-r--r--   0        0        0      206 2023-06-24 20:29:33.336106 spacetraders-0.7.0/spacetraders/models/ship_nav_flight_mode.py
+-rw-r--r--   0        0        0     1891 2023-06-24 20:29:37.262313 spacetraders-0.7.0/spacetraders/models/ship_nav_route.py
+-rw-r--r--   0        0        0     1650 2023-06-24 20:29:37.274434 spacetraders-0.7.0/spacetraders/models/ship_nav_route_waypoint.py
+-rw-r--r--   0        0        0      196 2023-06-24 20:29:33.330456 spacetraders-0.7.0/spacetraders/models/ship_nav_status.py
+-rw-r--r--   0        0        0     2200 2023-06-24 20:29:37.266800 spacetraders-0.7.0/spacetraders/models/ship_reactor.py
+-rw-r--r--   0        0        0      344 2023-06-24 20:29:33.525865 spacetraders-0.7.0/spacetraders/models/ship_reactor_symbol.py
+-rw-r--r--   0        0        0     1303 2023-06-24 20:29:37.271757 spacetraders-0.7.0/spacetraders/models/ship_refine_json_body.py
+-rw-r--r--   0        0        0      330 2023-06-24 20:29:33.497285 spacetraders-0.7.0/spacetraders/models/ship_refine_json_body_produce.py
+-rw-r--r--   0        0        0     1316 2023-06-24 20:29:37.272261 spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response.py
+-rw-r--r--   0        0        0     2197 2023-06-24 20:29:37.265176 spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response_data.py
+-rw-r--r--   0        0        0     1305 2023-06-24 20:29:37.252074 spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response_data_consumed_item.py
+-rw-r--r--   0        0        0     1305 2023-06-24 20:29:37.258347 spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response_data_produced_item.py
+-rw-r--r--   0        0        0     1477 2023-06-24 20:29:37.270018 spacetraders-0.7.0/spacetraders/models/ship_registration.py
+-rw-r--r--   0        0        0     1541 2023-06-24 20:29:37.252123 spacetraders-0.7.0/spacetraders/models/ship_requirements.py
+-rw-r--r--   0        0        0      479 2023-06-24 20:29:33.265907 spacetraders-0.7.0/spacetraders/models/ship_role.py
+-rw-r--r--   0        0        0      549 2023-06-24 20:29:33.259345 spacetraders-0.7.0/spacetraders/models/ship_type.py
+-rw-r--r--   0        0        0     2009 2023-06-24 20:29:37.266832 spacetraders-0.7.0/spacetraders/models/shipyard.py
+-rw-r--r--   0        0        0     2511 2023-06-24 20:29:37.266673 spacetraders-0.7.0/spacetraders/models/shipyard_ship.py
+-rw-r--r--   0        0        0     1238 2023-06-24 20:29:37.270611 spacetraders-0.7.0/spacetraders/models/shipyard_ship_types_item.py
+-rw-r--r--   0        0        0     1761 2023-06-24 20:29:37.255242 spacetraders-0.7.0/spacetraders/models/shipyard_transaction.py
+-rw-r--r--   0        0        0     2228 2023-06-24 20:29:37.253937 spacetraders-0.7.0/spacetraders/models/survey.py
+-rw-r--r--   0        0        0     1209 2023-06-24 20:29:37.253331 spacetraders-0.7.0/spacetraders/models/survey_deposit.py
+-rw-r--r--   0        0        0      181 2023-06-24 20:29:33.611132 spacetraders-0.7.0/spacetraders/models/survey_size.py
+-rw-r--r--   0        0        0     1918 2023-06-24 20:29:37.265530 spacetraders-0.7.0/spacetraders/models/system.py
+-rw-r--r--   0        0        0     1213 2023-06-24 20:29:37.266034 spacetraders-0.7.0/spacetraders/models/system_faction.py
+-rw-r--r--   0        0        0      405 2023-06-24 20:29:33.506563 spacetraders-0.7.0/spacetraders/models/system_type.py
+-rw-r--r--   0        0        0     1460 2023-06-24 20:29:37.268481 spacetraders-0.7.0/spacetraders/models/system_waypoint.py
+-rw-r--r--   0        0        0     1424 2023-06-24 20:29:37.272042 spacetraders-0.7.0/spacetraders/models/trade_good.py
+-rw-r--r--   0        0        0     4422 2023-06-24 20:29:33.280231 spacetraders-0.7.0/spacetraders/models/trade_symbol.py
+-rw-r--r--   0        0        0     1352 2023-06-24 20:29:37.269510 spacetraders-0.7.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
+-rw-r--r--   0        0        0     1241 2023-06-24 20:29:37.274468 spacetraders-0.7.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
+-rw-r--r--   0        0        0     1453 2023-06-24 20:29:37.269452 spacetraders-0.7.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py
+-rw-r--r--   0        0        0     1168 2023-06-24 20:29:37.265632 spacetraders-0.7.0/spacetraders/models/warp_ship_json_body.py
+-rw-r--r--   0        0        0     1233 2023-06-24 20:29:37.265279 spacetraders-0.7.0/spacetraders/models/warp_ship_response_200.py
+-rw-r--r--   0        0        0     1436 2023-06-24 20:29:37.261914 spacetraders-0.7.0/spacetraders/models/warp_ship_response_200_data.py
+-rw-r--r--   0        0        0     2510 2023-06-24 20:29:37.257639 spacetraders-0.7.0/spacetraders/models/waypoint.py
+-rw-r--r--   0        0        0     1257 2023-06-24 20:29:37.253158 spacetraders-0.7.0/spacetraders/models/waypoint_faction.py
+-rw-r--r--   0        0        0     1215 2023-06-24 20:29:37.256725 spacetraders-0.7.0/spacetraders/models/waypoint_orbital.py
+-rw-r--r--   0        0        0     1427 2023-06-24 20:29:37.275639 spacetraders-0.7.0/spacetraders/models/waypoint_trait.py
+-rw-r--r--   0        0        0     2200 2023-06-24 20:29:33.305812 spacetraders-0.7.0/spacetraders/models/waypoint_trait_symbol.py
+-rw-r--r--   0        0        0      381 2023-06-24 20:29:33.378026 spacetraders-0.7.0/spacetraders/models/waypoint_type.py
+-rw-r--r--   0        0        0     1341 2023-06-24 20:29:37.262762 spacetraders-0.7.0/spacetraders/types.py
+-rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 spacetraders-0.7.0/PKG-INFO
```

### Comparing `spacetraders-0.6.0/README.md` & `spacetraders-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/pyproject.toml` & `spacetraders-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacetraders"
-version = "0.6.0"
+version = "0.7.0"
 description = "Python API for Space Traders"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "spacetraders"}]
 
 [tool.poetry.dependencies]
```

### Comparing `spacetraders-0.6.0/spacetraders/api/agents/get_my_agent.py` & `spacetraders-0.7.0/spacetraders/api/agents/get_my_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 
 def sync_detailed(
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetMyAgentResponse200]:
-    """My Agent Details
+    """Get Agent
 
      Fetch your agent's details.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -107,15 +107,15 @@
 
 
 async def asyncio_detailed(
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetMyAgentResponse200]:
-    """My Agent Details
+    """Get Agent
 
      Fetch your agent's details.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/contracts/accept_contract.py` & `spacetraders-0.7.0/spacetraders/api/contracts/fulfill_contract.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.accept_contract_response_200 import AcceptContractResponse200
+from ...models.fulfill_contract_response_200 import FulfillContractResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     contract_id: str,
     *,
     _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/contracts/{contractId}/accept".format(
+    url = "{}/my/contracts/{contractId}/fulfill".format(
         _client.base_url, contractId=contract_id
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
@@ -30,55 +30,55 @@
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[AcceptContractResponse200]:
+) -> Optional[FulfillContractResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = AcceptContractResponse200(**response.json())
+        response_200 = FulfillContractResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[AcceptContractResponse200]:
+) -> Response[FulfillContractResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     contract_id: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[AcceptContractResponse200]:
-    """Accept Contract
+) -> Response[FulfillContractResponse200]:
+    """Fulfill Contract
 
-     Accept a contract.
+     Fulfill a contract. Can only be used on contracts that have all of their delivery terms fulfilled.
 
     Args:
         contract_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[AcceptContractResponse200]
+        Response[FulfillContractResponse200]
     """
 
     kwargs = _get_kwargs(
         contract_id=contract_id,
         _client=_client,
     )
 
@@ -115,28 +115,28 @@
 
 
 async def asyncio_detailed(
     contract_id: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[AcceptContractResponse200]:
-    """Accept Contract
+) -> Response[FulfillContractResponse200]:
+    """Fulfill Contract
 
-     Accept a contract.
+     Fulfill a contract. Can only be used on contracts that have all of their delivery terms fulfilled.
 
     Args:
         contract_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[AcceptContractResponse200]
+        Response[FulfillContractResponse200]
     """
 
     kwargs = _get_kwargs(
         contract_id=contract_id,
         _client=_client,
     )
```

### Comparing `spacetraders-0.6.0/spacetraders/api/contracts/deliver_contract.py` & `spacetraders-0.7.0/spacetraders/api/contracts/deliver_contract.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,17 +64,23 @@
 def sync_detailed(
     contract_id: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: DeliverContractJsonBody,
 ) -> Response[DeliverContractResponse200]:
-    """Deliver Contract
+    """Deliver Cargo to Contract
 
-     Deliver cargo on a given contract.
+     Deliver cargo to a contract.
+
+    In order to use this API, a ship must be at the delivery location (denoted in the delivery terms as
+    `destinationSymbol` of a contract) and must have a number of units of a good required by this
+    contract in its cargo.
+
+    Cargo that was delivered will be removed from the ship's cargo.
 
     Args:
         contract_id (str):
         json_body (DeliverContractJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -127,17 +133,23 @@
 async def asyncio_detailed(
     contract_id: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: DeliverContractJsonBody,
 ) -> Response[DeliverContractResponse200]:
-    """Deliver Contract
+    """Deliver Cargo to Contract
+
+     Deliver cargo to a contract.
+
+    In order to use this API, a ship must be at the delivery location (denoted in the delivery terms as
+    `destinationSymbol` of a contract) and must have a number of units of a good required by this
+    contract in its cargo.
 
-     Deliver cargo on a given contract.
+    Cargo that was delivered will be removed from the ship's cargo.
 
     Args:
         contract_id (str):
         json_body (DeliverContractJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/contracts/fulfill_contract.py` & `spacetraders-0.7.0/spacetraders/api/contracts/get_contract.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,83 +2,83 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.fulfill_contract_response_200 import FulfillContractResponse200
+from ...models.get_contract_response_200 import GetContractResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     contract_id: str,
     *,
     _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/contracts/{contractId}/fulfill".format(
+    url = "{}/my/contracts/{contractId}".format(
         _client.base_url, contractId=contract_id
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[FulfillContractResponse200]:
+) -> Optional[GetContractResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = FulfillContractResponse200(**response.json())
+        response_200 = GetContractResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[FulfillContractResponse200]:
+) -> Response[GetContractResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     contract_id: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[FulfillContractResponse200]:
-    """Fulfill Contract
+) -> Response[GetContractResponse200]:
+    """Get Contract
 
-     Fulfill a contract
+     Get the details of a contract by ID.
 
     Args:
         contract_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[FulfillContractResponse200]
+        Response[GetContractResponse200]
     """
 
     kwargs = _get_kwargs(
         contract_id=contract_id,
         _client=_client,
     )
 
@@ -115,28 +115,28 @@
 
 
 async def asyncio_detailed(
     contract_id: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[FulfillContractResponse200]:
-    """Fulfill Contract
+) -> Response[GetContractResponse200]:
+    """Get Contract
 
-     Fulfill a contract
+     Get the details of a contract by ID.
 
     Args:
         contract_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[FulfillContractResponse200]
+        Response[GetContractResponse200]
     """
 
     kwargs = _get_kwargs(
         contract_id=contract_id,
         _client=_client,
     )
```

### Comparing `spacetraders-0.6.0/spacetraders/api/contracts/get_contract.py` & `spacetraders-0.7.0/spacetraders/api/factions/get_faction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.get_contract_response_200 import GetContractResponse200
+from ...client import Client
+from ...models.get_faction_response_200 import GetFactionResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
-    contract_id: str,
+    faction_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/my/contracts/{contractId}".format(
-        _client.base_url, contractId=contract_id
+    url = "{}/factions/{factionSymbol}".format(
+        _client.base_url, factionSymbol=faction_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
@@ -30,59 +30,59 @@
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[GetContractResponse200]:
+) -> Optional[GetFactionResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetContractResponse200(**response.json())
+        response_200 = GetFactionResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[GetContractResponse200]:
+) -> Response[GetFactionResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    contract_id: str,
+    faction_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetContractResponse200]:
-    """Get Contract
+) -> Response[GetFactionResponse200]:
+    """Get Faction
 
-     Get the details of a contract by ID.
+     View the details of a faction.
 
     Args:
-        contract_id (str):
+        faction_symbol (str):  Example: COSMIC.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetContractResponse200]
+        Response[GetFactionResponse200]
     """
 
     kwargs = _get_kwargs(
-        contract_id=contract_id,
+        faction_symbol=faction_symbol,
         _client=_client,
     )
 
     response = httpx.request(
         verify=_client.verify_ssl,
         **kwargs,
     )
@@ -111,36 +111,36 @@
             data=details.get("data"),
             headers=resp.headers,
         )
     )
 
 
 async def asyncio_detailed(
-    contract_id: str,
+    faction_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetContractResponse200]:
-    """Get Contract
+) -> Response[GetFactionResponse200]:
+    """Get Faction
 
-     Get the details of a contract by ID.
+     View the details of a faction.
 
     Args:
-        contract_id (str):
+        faction_symbol (str):  Example: COSMIC.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetContractResponse200]
+        Response[GetFactionResponse200]
     """
 
     kwargs = _get_kwargs(
-        contract_id=contract_id,
+        faction_symbol=faction_symbol,
         _client=_client,
     )
 
     async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
         response = await c.request(**kwargs)
 
     resp = _build_response(client=_client, response=response)
```

### Comparing `spacetraders-0.6.0/spacetraders/api/contracts/get_contracts.py` & `spacetraders-0.7.0/spacetraders/api/contracts/get_contracts.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from ...models.get_contracts_response_200 import GetContractsResponse200
 from ...types import UNSET, ApiError, Error, Response, Unset
 
 
 def _get_kwargs(
     *,
     _client: AuthenticatedClient,
-    page: Union[Unset, None, int] = UNSET,
-    limit: Union[Unset, None, int] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
 ) -> Dict[str, Any]:
     url = "{}/my/contracts".format(_client.base_url)
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -63,24 +63,24 @@
     )
 
 
 def sync_detailed(
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    page: Union[Unset, None, int] = UNSET,
-    limit: Union[Unset, None, int] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
 ) -> Response[GetContractsResponse200]:
     """List Contracts
 
-     List all of your contracts.
+     Return a paginated list of all your contracts.
 
     Args:
-        page (Union[Unset, None, int]):
-        limit (Union[Unset, None, int]):
+        page (Union[Unset, None, int]):  Default: 1.
+        limit (Union[Unset, None, int]):  Default: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetContractsResponse200]
@@ -124,24 +124,24 @@
     )
 
 
 async def asyncio_detailed(
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    page: Union[Unset, None, int] = UNSET,
-    limit: Union[Unset, None, int] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
 ) -> Response[GetContractsResponse200]:
     """List Contracts
 
-     List all of your contracts.
+     Return a paginated list of all your contracts.
 
     Args:
-        page (Union[Unset, None, int]):
-        limit (Union[Unset, None, int]):
+        page (Union[Unset, None, int]):  Default: 1.
+        limit (Union[Unset, None, int]):  Default: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetContractsResponse200]
```

### Comparing `spacetraders-0.6.0/spacetraders/api/default/get_status.py` & `spacetraders-0.7.0/spacetraders/api/default/get_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import Client
+from ...client import AuthenticatedClient, Client
 from ...models.get_status_response_200 import GetStatusResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/".format(_client.base_url)
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
@@ -51,20 +51,22 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetStatusResponse200]:
     """Get Status
 
      Return the status of the game server.
+    This also includes a few global elements, such as announcements, server reset dates and
+    leaderboards.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetStatusResponse200]
@@ -104,20 +106,22 @@
             headers=resp.headers,
         )
     )
 
 
 async def asyncio_detailed(
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetStatusResponse200]:
     """Get Status
 
      Return the status of the game server.
+    This also includes a few global elements, such as announcements, server reset dates and
+    leaderboards.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetStatusResponse200]
```

### Comparing `spacetraders-0.6.0/spacetraders/api/default/register.py` & `spacetraders-0.7.0/spacetraders/api/default/register.py`

 * *Files 16% similar despite different names*

```diff
@@ -62,37 +62,34 @@
     *,
     _client: Client,
     raise_on_error: Optional[bool] = None,
     **json_body: RegisterJsonBody,
 ) -> Response[RegisterResponse201]:
     """Register New Agent
 
-     Creates a new agent and ties it to a temporary Account.
-
-    The agent symbol is a 3-14 character string that will represent your agent. This symbol will prefix
-    the symbol of every ship you own. Agent symbols will be cast to all uppercase characters.
-
-    A new agent will be granted an authorization token, a contract with their starting faction, a
-    command ship with a jump drive, and one hundred thousand credits.
+     Creates a new agent and ties it to an account.
+    The agent symbol must consist of a 3-14 character string, and will be used to represent your agent.
+    This symbol will prefix the symbol of every ship you own. Agent symbols will be cast to all
+    uppercase characters.
+
+    This new agent will be tied to a starting faction of your choice, which determines your starting
+    location, and will be granted an authorization token, a contract with their starting faction, a
+    command ship that can fly across space with advanced capabilities, a small probe ship that can be
+    used for reconnaissance, and 150,000 credits.
 
     > #### Keep your token safe and secure
     >
     > Save your token during the alpha phase. There is no way to regenerate this token without starting
     a new agent. In the future you will be able to generate and manage your tokens from the SpaceTraders
     website.
 
-    You can accept your contract using the `/my/contracts/{contractId}/accept` endpoint. You will want
-    to navigate your command ship to a nearby asteroid field and execute the
-    `/my/ships/{shipSymbol}/extract` endpoint to mine various types of ores and minerals.
-
-    Return to the contract destination and execute the `/my/ships/{shipSymbol}/deliver` endpoint to
-    deposit goods into the contract.
-
-    When your contract is fulfilled, you can call `/my/contracts/{contractId}/fulfill` to retrieve
-    payment.
+    If you are new to SpaceTraders, It is recommended to register with the COSMIC faction, a faction
+    that is well connected to the rest of the universe. After registering, you should try our
+    interactive [quickstart guide](https://docs.spacetraders.io/quickstart/new-game) which will walk you
+    through basic API requests in just a few minutes.
 
     Args:
         json_body (RegisterJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -144,37 +141,34 @@
     *,
     _client: Client,
     raise_on_error: Optional[bool] = None,
     **json_body: RegisterJsonBody,
 ) -> Response[RegisterResponse201]:
     """Register New Agent
 
-     Creates a new agent and ties it to a temporary Account.
-
-    The agent symbol is a 3-14 character string that will represent your agent. This symbol will prefix
-    the symbol of every ship you own. Agent symbols will be cast to all uppercase characters.
-
-    A new agent will be granted an authorization token, a contract with their starting faction, a
-    command ship with a jump drive, and one hundred thousand credits.
+     Creates a new agent and ties it to an account.
+    The agent symbol must consist of a 3-14 character string, and will be used to represent your agent.
+    This symbol will prefix the symbol of every ship you own. Agent symbols will be cast to all
+    uppercase characters.
+
+    This new agent will be tied to a starting faction of your choice, which determines your starting
+    location, and will be granted an authorization token, a contract with their starting faction, a
+    command ship that can fly across space with advanced capabilities, a small probe ship that can be
+    used for reconnaissance, and 150,000 credits.
 
     > #### Keep your token safe and secure
     >
     > Save your token during the alpha phase. There is no way to regenerate this token without starting
     a new agent. In the future you will be able to generate and manage your tokens from the SpaceTraders
     website.
 
-    You can accept your contract using the `/my/contracts/{contractId}/accept` endpoint. You will want
-    to navigate your command ship to a nearby asteroid field and execute the
-    `/my/ships/{shipSymbol}/extract` endpoint to mine various types of ores and minerals.
-
-    Return to the contract destination and execute the `/my/ships/{shipSymbol}/deliver` endpoint to
-    deposit goods into the contract.
-
-    When your contract is fulfilled, you can call `/my/contracts/{contractId}/fulfill` to retrieve
-    payment.
+    If you are new to SpaceTraders, It is recommended to register with the COSMIC faction, a faction
+    that is well connected to the rest of the universe. After registering, you should try our
+    interactive [quickstart guide](https://docs.spacetraders.io/quickstart/new-game) which will walk you
+    through basic API requests in just a few minutes.
 
     Args:
         json_body (RegisterJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/factions/get_faction.py` & `spacetraders-0.7.0/spacetraders/api/fleet/create_ship_ship_scan.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,93 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import Client
-from ...models.get_faction_response_200 import GetFactionResponse200
+from ...client import AuthenticatedClient, Client
+from ...models.create_ship_ship_scan_response_201 import CreateShipShipScanResponse201
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
-    faction_symbol: str = "CGR",
+    ship_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/factions/{factionSymbol}".format(
-        _client.base_url, factionSymbol=faction_symbol
+    url = "{}/my/ships/{shipSymbol}/scan/ships".format(
+        _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
-        "method": "get",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[GetFactionResponse200]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = GetFactionResponse200(**response.json())
+) -> Optional[CreateShipShipScanResponse201]:
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = CreateShipShipScanResponse201(**response.json())
 
-        return response_200
+        return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[GetFactionResponse200]:
+) -> Response[CreateShipShipScanResponse201]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    faction_symbol: str = "CGR",
+    ship_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetFactionResponse200]:
-    """Get Faction
+) -> Response[CreateShipShipScanResponse201]:
+    """Scan Ships
 
-     View the details of a faction.
+     Scan for nearby ships, retrieving information for all ships in range.
+
+    Requires a ship to have the `Sensor Array` mount installed to use.
+
+    The ship will enter a cooldown after using this function, during which it cannot execute certain
+    actions.
 
     Args:
-        faction_symbol (str):  Default: 'CGR'.
+        ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetFactionResponse200]
+        Response[CreateShipShipScanResponse201]
     """
 
     kwargs = _get_kwargs(
-        faction_symbol=faction_symbol,
+        ship_symbol=ship_symbol,
         _client=_client,
     )
 
     response = httpx.request(
         verify=_client.verify_ssl,
         **kwargs,
     )
@@ -111,36 +116,41 @@
             data=details.get("data"),
             headers=resp.headers,
         )
     )
 
 
 async def asyncio_detailed(
-    faction_symbol: str = "CGR",
+    ship_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetFactionResponse200]:
-    """Get Faction
+) -> Response[CreateShipShipScanResponse201]:
+    """Scan Ships
+
+     Scan for nearby ships, retrieving information for all ships in range.
+
+    Requires a ship to have the `Sensor Array` mount installed to use.
 
-     View the details of a faction.
+    The ship will enter a cooldown after using this function, during which it cannot execute certain
+    actions.
 
     Args:
-        faction_symbol (str):  Default: 'CGR'.
+        ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetFactionResponse200]
+        Response[CreateShipShipScanResponse201]
     """
 
     kwargs = _get_kwargs(
-        faction_symbol=faction_symbol,
+        ship_symbol=ship_symbol,
         _client=_client,
     )
 
     async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
         response = await c.request(**kwargs)
 
     resp = _build_response(client=_client, response=response)
```

### Comparing `spacetraders-0.6.0/spacetraders/api/factions/get_factions.py` & `spacetraders-0.7.0/spacetraders/api/factions/get_factions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import Client
+from ...client import AuthenticatedClient, Client
 from ...models.get_factions_response_200 import GetFactionsResponse200
 from ...types import UNSET, ApiError, Error, Response, Unset
 
 
 def _get_kwargs(
     *,
-    _client: Client,
-    page: Union[Unset, None, int] = UNSET,
-    limit: Union[Unset, None, int] = UNSET,
+    _client: AuthenticatedClient,
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
 ) -> Dict[str, Any]:
     url = "{}/factions".format(_client.base_url)
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -61,26 +61,26 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    page: Union[Unset, None, int] = UNSET,
-    limit: Union[Unset, None, int] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
 ) -> Response[GetFactionsResponse200]:
     """List Factions
 
-     List all discovered factions in the game.
+     Return a paginated list of all the factions in the game.
 
     Args:
-        page (Union[Unset, None, int]):
-        limit (Union[Unset, None, int]):
+        page (Union[Unset, None, int]):  Default: 1.
+        limit (Union[Unset, None, int]):  Default: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetFactionsResponse200]
@@ -122,26 +122,26 @@
             headers=resp.headers,
         )
     )
 
 
 async def asyncio_detailed(
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    page: Union[Unset, None, int] = UNSET,
-    limit: Union[Unset, None, int] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
 ) -> Response[GetFactionsResponse200]:
     """List Factions
 
-     List all discovered factions in the game.
+     Return a paginated list of all the factions in the game.
 
     Args:
-        page (Union[Unset, None, int]):
-        limit (Union[Unset, None, int]):
+        page (Union[Unset, None, int]):  Default: 1.
+        limit (Union[Unset, None, int]):  Default: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetFactionsResponse200]
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/create_chart.py` & `spacetraders-0.7.0/spacetraders/api/fleet/get_mounts.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,88 +2,83 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.create_chart_response_201 import CreateChartResponse201
+from ...models.get_mounts_get_mounts_200_response import GetMountsGetMounts200Response
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}/chart".format(
+    url = "{}/my/ships/{shipSymbol}/mounts".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[CreateChartResponse201]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateChartResponse201(**response.json())
+) -> Optional[GetMountsGetMounts200Response]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = GetMountsGetMounts200Response(**response.json())
 
-        return response_201
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[CreateChartResponse201]:
+) -> Response[GetMountsGetMounts200Response]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[CreateChartResponse201]:
-    """Create Chart
+) -> Response[GetMountsGetMounts200Response]:
+    """Get Mounts
 
-     Command a ship to chart the current waypoint.
-
-    Waypoints in the universe are uncharted by default. These locations will not show up in the API
-    until they have been charted by a ship.
-
-    Charting a location will record your agent as the one who created the chart.
+     Get the mounts installed on a ship.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateChartResponse201]
+        Response[GetMountsGetMounts200Response]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
     )
 
@@ -120,33 +115,28 @@
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[CreateChartResponse201]:
-    """Create Chart
-
-     Command a ship to chart the current waypoint.
-
-    Waypoints in the universe are uncharted by default. These locations will not show up in the API
-    until they have been charted by a ship.
+) -> Response[GetMountsGetMounts200Response]:
+    """Get Mounts
 
-    Charting a location will record your agent as the one who created the chart.
+     Get the mounts installed on a ship.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateChartResponse201]
+        Response[GetMountsGetMounts200Response]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
     )
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/create_ship_ship_scan.py` & `spacetraders-0.7.0/spacetraders/api/fleet/create_ship_system_scan.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.create_ship_ship_scan_response_201 import CreateShipShipScanResponse201
+from ...models.create_ship_system_scan_response_201 import (
+    CreateShipSystemScanResponse201,
+)
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}/scan/ships".format(
+    url = "{}/my/ships/{shipSymbol}/scan/systems".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
@@ -30,55 +32,59 @@
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[CreateShipShipScanResponse201]:
+) -> Optional[CreateShipSystemScanResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateShipShipScanResponse201(**response.json())
+        response_201 = CreateShipSystemScanResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[CreateShipShipScanResponse201]:
+) -> Response[CreateShipSystemScanResponse201]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[CreateShipShipScanResponse201]:
-    """Scan Ships
+) -> Response[CreateShipSystemScanResponse201]:
+    """Scan Systems
 
-     Activate your ship's sensor arrays to scan for ship information.
+     Scan for nearby systems, retrieving information on the systems' distance from the ship and their
+    waypoints. Requires a ship to have the `Sensor Array` mount installed to use.
+
+    The ship will enter a cooldown after using this function, during which it cannot execute certain
+    actions.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateShipShipScanResponse201]
+        Response[CreateShipSystemScanResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
     )
 
@@ -115,28 +121,32 @@
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[CreateShipShipScanResponse201]:
-    """Scan Ships
+) -> Response[CreateShipSystemScanResponse201]:
+    """Scan Systems
+
+     Scan for nearby systems, retrieving information on the systems' distance from the ship and their
+    waypoints. Requires a ship to have the `Sensor Array` mount installed to use.
 
-     Activate your ship's sensor arrays to scan for ship information.
+    The ship will enter a cooldown after using this function, during which it cannot execute certain
+    actions.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateShipShipScanResponse201]
+        Response[CreateShipSystemScanResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
     )
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/create_ship_system_scan.py` & `spacetraders-0.7.0/spacetraders/api/fleet/create_ship_waypoint_scan.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.create_ship_system_scan_response_201 import (
-    CreateShipSystemScanResponse201,
+from ...models.create_ship_waypoint_scan_response_201 import (
+    CreateShipWaypointScanResponse201,
 )
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}/scan/systems".format(
+    url = "{}/my/ships/{shipSymbol}/scan/waypoints".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
@@ -32,55 +32,62 @@
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[CreateShipSystemScanResponse201]:
+) -> Optional[CreateShipWaypointScanResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateShipSystemScanResponse201(**response.json())
+        response_201 = CreateShipWaypointScanResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[CreateShipSystemScanResponse201]:
+) -> Response[CreateShipWaypointScanResponse201]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[CreateShipSystemScanResponse201]:
-    """Scan Systems
+) -> Response[CreateShipWaypointScanResponse201]:
+    """Scan Waypoints
 
-     Activate your ship's sensor arrays to scan for system information.
+     Scan for nearby waypoints, retrieving detailed information on each waypoint in range. Scanning
+    uncharted waypoints will allow you to ignore their uncharted state and will list the waypoints'
+    traits.
+
+    Requires a ship to have the `Sensor Array` mount installed to use.
+
+    The ship will enter a cooldown after using this function, during which it cannot execute certain
+    actions.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateShipSystemScanResponse201]
+        Response[CreateShipWaypointScanResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
     )
 
@@ -117,28 +124,35 @@
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[CreateShipSystemScanResponse201]:
-    """Scan Systems
+) -> Response[CreateShipWaypointScanResponse201]:
+    """Scan Waypoints
+
+     Scan for nearby waypoints, retrieving detailed information on each waypoint in range. Scanning
+    uncharted waypoints will allow you to ignore their uncharted state and will list the waypoints'
+    traits.
+
+    Requires a ship to have the `Sensor Array` mount installed to use.
 
-     Activate your ship's sensor arrays to scan for system information.
+    The ship will enter a cooldown after using this function, during which it cannot execute certain
+    actions.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateShipSystemScanResponse201]
+        Response[CreateShipWaypointScanResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
     )
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/create_ship_waypoint_scan.py` & `spacetraders-0.7.0/spacetraders/api/fleet/get_my_ship.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,85 +2,81 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.create_ship_waypoint_scan_response_201 import (
-    CreateShipWaypointScanResponse201,
-)
+from ...models.get_my_ship_response_200 import GetMyShipResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}/scan/waypoints".format(
-        _client.base_url, shipSymbol=ship_symbol
-    )
+    url = "{}/my/ships/{shipSymbol}".format(_client.base_url, shipSymbol=ship_symbol)
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[CreateShipWaypointScanResponse201]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateShipWaypointScanResponse201(**response.json())
+) -> Optional[GetMyShipResponse200]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = GetMyShipResponse200(**response.json())
 
-        return response_201
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[CreateShipWaypointScanResponse201]:
+) -> Response[GetMyShipResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[CreateShipWaypointScanResponse201]:
-    """Scan Waypoints
+) -> Response[GetMyShipResponse200]:
+    """Get Ship
 
-     Activate your ship's sensor arrays to scan for waypoint information.
+     Retrieve the details of a ship under your agent's ownership.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateShipWaypointScanResponse201]
+        Response[GetMyShipResponse200]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
     )
 
@@ -117,28 +113,28 @@
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[CreateShipWaypointScanResponse201]:
-    """Scan Waypoints
+) -> Response[GetMyShipResponse200]:
+    """Get Ship
 
-     Activate your ship's sensor arrays to scan for waypoint information.
+     Retrieve the details of a ship under your agent's ownership.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateShipWaypointScanResponse201]
+        Response[GetMyShipResponse200]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
     )
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/create_survey.py` & `spacetraders-0.7.0/spacetraders/api/fleet/create_survey.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,21 +60,28 @@
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[CreateSurveyResponse201]:
     """Create Survey
 
-     If you want to target specific yields for an extraction, you can survey a waypoint, such as an
-    asteroid field, and send the survey in the body of the extract request. Each survey may have
-    multiple deposits, and if a symbol shows up more than once, that indicates a higher chance of
-    extracting that resource.
+     Create surveys on a waypoint that can be extracted such as asteroid fields. A survey focuses on
+    specific types of deposits from the extracted location. When ships extract using this survey, they
+    are guaranteed to procure a high amount of one of the goods in the survey.
 
-    Your ship will enter a cooldown between consecutive survey requests. Surveys will eventually expire
-    after a period of time. Multiple ships can use the same survey for extraction.
+    In order to use a survey, send the entire survey details in the body of the extract request.
+
+    Each survey may have multiple deposits, and if a symbol shows up more than once, that indicates a
+    higher chance of extracting that resource.
+
+    Your ship will enter a cooldown after surveying in which it is unable to perform certain actions.
+    Surveys will eventually expire after a period of time or will be exhausted after being extracted
+    several times based on the survey's size. Multiple ships can use the same survey for extraction.
+
+    A ship must have the `Surveyor` mount installed in order to use this function.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -124,21 +131,28 @@
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[CreateSurveyResponse201]:
     """Create Survey
 
-     If you want to target specific yields for an extraction, you can survey a waypoint, such as an
-    asteroid field, and send the survey in the body of the extract request. Each survey may have
-    multiple deposits, and if a symbol shows up more than once, that indicates a higher chance of
-    extracting that resource.
+     Create surveys on a waypoint that can be extracted such as asteroid fields. A survey focuses on
+    specific types of deposits from the extracted location. When ships extract using this survey, they
+    are guaranteed to procure a high amount of one of the goods in the survey.
+
+    In order to use a survey, send the entire survey details in the body of the extract request.
+
+    Each survey may have multiple deposits, and if a symbol shows up more than once, that indicates a
+    higher chance of extracting that resource.
+
+    Your ship will enter a cooldown after surveying in which it is unable to perform certain actions.
+    Surveys will eventually expire after a period of time or will be exhausted after being extracted
+    several times based on the survey's size. Multiple ships can use the same survey for extraction.
 
-    Your ship will enter a cooldown between consecutive survey requests. Surveys will eventually expire
-    after a period of time. Multiple ships can use the same survey for extraction.
+    A ship must have the `Surveyor` mount installed in order to use this function.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/dock_ship.py` & `spacetraders-0.7.0/spacetraders/api/fleet/dock_ship.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,16 +60,19 @@
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[DockShipDockShip200Response]:
     """Dock Ship
 
-     Attempt to dock your ship at it's current location. Docking will only succeed if the waypoint is a
-    dockable location, and your ship is capable of docking at the time of the request.
+     Attempt to dock your ship at its current location. Docking will only succeed if your ship is capable
+    of docking at the time of the request.
+
+    Docked ships can access elements in their current location, such as the market or a shipyard, but
+    cannot do actions that require the ship to be above surface such as navigating or extracting.
 
     The endpoint is idempotent - successive calls will succeed even if the ship is already docked.
 
     Args:
         ship_symbol (str):
 
     Raises:
@@ -121,16 +124,19 @@
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[DockShipDockShip200Response]:
     """Dock Ship
 
-     Attempt to dock your ship at it's current location. Docking will only succeed if the waypoint is a
-    dockable location, and your ship is capable of docking at the time of the request.
+     Attempt to dock your ship at its current location. Docking will only succeed if your ship is capable
+    of docking at the time of the request.
+
+    Docked ships can access elements in their current location, such as the market or a shipyard, but
+    cannot do actions that require the ship to be above surface such as navigating or extracting.
 
     The endpoint is idempotent - successive calls will succeed even if the ship is already docked.
 
     Args:
         ship_symbol (str):
 
     Raises:
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/extract_resources.py` & `spacetraders-0.7.0/spacetraders/api/fleet/extract_resources.py`

 * *Files 15% similar despite different names*

```diff
@@ -66,16 +66,20 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: ExtractResourcesJsonBody,
 ) -> Response[ExtractResourcesResponse201]:
     """Extract Resources
 
-     Extract resources from the waypoint into your ship. Send an optional survey as the payload to target
-    specific yields.
+     Extract resources from a waypoint that can be extracted, such as asteroid fields, into your ship.
+    Send an optional survey as the payload to target specific yields.
+
+    The ship must be in orbit to be able to extract and must have mining equipments installed that can
+    extract goods, such as the `Gas Siphon` mount for gas-based goods or `Mining Laser` mount for ore-
+    based goods.
 
     Args:
         ship_symbol (str):
         json_body (ExtractResourcesJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -130,16 +134,20 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: ExtractResourcesJsonBody,
 ) -> Response[ExtractResourcesResponse201]:
     """Extract Resources
 
-     Extract resources from the waypoint into your ship. Send an optional survey as the payload to target
-    specific yields.
+     Extract resources from a waypoint that can be extracted, such as asteroid fields, into your ship.
+    Send an optional survey as the payload to target specific yields.
+
+    The ship must be in orbit to be able to extract and must have mining equipments installed that can
+    extract goods, such as the `Gas Siphon` mount for gas-based goods or `Mining Laser` mount for ore-
+    based goods.
 
     Args:
         ship_symbol (str):
         json_body (ExtractResourcesJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/get_mounts.py` & `spacetraders-0.7.0/spacetraders/api/fleet/get_my_ship_cargo.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.get_mounts_get_mounts_200_response import GetMountsGetMounts200Response
+from ...models.get_my_ship_cargo_response_200 import GetMyShipCargoResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}/mounts".format(
+    url = "{}/my/ships/{shipSymbol}/cargo".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
@@ -30,55 +30,55 @@
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[GetMountsGetMounts200Response]:
+) -> Optional[GetMyShipCargoResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMountsGetMounts200Response(**response.json())
+        response_200 = GetMyShipCargoResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[GetMountsGetMounts200Response]:
+) -> Response[GetMyShipCargoResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetMountsGetMounts200Response]:
-    """Get Mounts
+) -> Response[GetMyShipCargoResponse200]:
+    """Get Ship Cargo
 
-     Get the mounts on a ship.
+     Retrieve the cargo of a ship under your agent's ownership.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetMountsGetMounts200Response]
+        Response[GetMyShipCargoResponse200]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
     )
 
@@ -115,28 +115,28 @@
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetMountsGetMounts200Response]:
-    """Get Mounts
+) -> Response[GetMyShipCargoResponse200]:
+    """Get Ship Cargo
 
-     Get the mounts on a ship.
+     Retrieve the cargo of a ship under your agent's ownership.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetMountsGetMounts200Response]
+        Response[GetMyShipCargoResponse200]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
     )
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/get_my_ship.py` & `spacetraders-0.7.0/spacetraders/api/systems/get_system.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.get_my_ship_response_200 import GetMyShipResponse200
+from ...models.get_system_response_200 import GetSystemResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
-    ship_symbol: str,
+    system_symbol: str = "X1-OE",
     *,
     _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}".format(_client.base_url, shipSymbol=ship_symbol)
+    url = "{}/systems/{systemSymbol}".format(
+        _client.base_url, systemSymbol=system_symbol
+    )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
@@ -28,59 +30,59 @@
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[GetMyShipResponse200]:
+) -> Optional[GetSystemResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMyShipResponse200(**response.json())
+        response_200 = GetSystemResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[GetMyShipResponse200]:
+) -> Response[GetSystemResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    ship_symbol: str,
+    system_symbol: str = "X1-OE",
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetMyShipResponse200]:
-    """Get Ship
+) -> Response[GetSystemResponse200]:
+    """Get System
 
-     Retrieve the details of your ship.
+     Get the details of a system.
 
     Args:
-        ship_symbol (str):
+        system_symbol (str):  Default: 'X1-OE'.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetMyShipResponse200]
+        Response[GetSystemResponse200]
     """
 
     kwargs = _get_kwargs(
-        ship_symbol=ship_symbol,
+        system_symbol=system_symbol,
         _client=_client,
     )
 
     response = httpx.request(
         verify=_client.verify_ssl,
         **kwargs,
     )
@@ -109,36 +111,36 @@
             data=details.get("data"),
             headers=resp.headers,
         )
     )
 
 
 async def asyncio_detailed(
-    ship_symbol: str,
+    system_symbol: str = "X1-OE",
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetMyShipResponse200]:
-    """Get Ship
+) -> Response[GetSystemResponse200]:
+    """Get System
 
-     Retrieve the details of your ship.
+     Get the details of a system.
 
     Args:
-        ship_symbol (str):
+        system_symbol (str):  Default: 'X1-OE'.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetMyShipResponse200]
+        Response[GetSystemResponse200]
     """
 
     kwargs = _get_kwargs(
-        ship_symbol=ship_symbol,
+        system_symbol=system_symbol,
         _client=_client,
     )
 
     async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
         response = await c.request(**kwargs)
 
     resp = _build_response(client=_client, response=response)
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/get_my_ship_cargo.py` & `spacetraders-0.7.0/spacetraders/api/systems/get_systems.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,99 @@
 import json
 from http import HTTPStatus
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.get_my_ship_cargo_response_200 import GetMyShipCargoResponse200
-from ...types import ApiError, Error, Response
+from ...models.get_systems_response_200 import GetSystemsResponse200
+from ...types import UNSET, ApiError, Error, Response, Unset
 
 
 def _get_kwargs(
-    ship_symbol: str,
     *,
     _client: AuthenticatedClient,
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}/cargo".format(
-        _client.base_url, shipSymbol=ship_symbol
-    )
+    url = "{}/systems".format(_client.base_url)
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
+    params: Dict[str, Any] = {}
+    params["page"] = page
+
+    params["limit"] = limit
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
+        "params": params,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[GetMyShipCargoResponse200]:
+) -> Optional[GetSystemsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMyShipCargoResponse200(**response.json())
+        response_200 = GetSystemsResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[GetMyShipCargoResponse200]:
+) -> Response[GetSystemsResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetMyShipCargoResponse200]:
-    """Get Ship Cargo
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
+) -> Response[GetSystemsResponse200]:
+    """List Systems
 
-     Retrieve the cargo of your ship.
+     Return a paginated list of all systems.
 
     Args:
-        ship_symbol (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        limit (Union[Unset, None, int]):  Default: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetMyShipCargoResponse200]
+        Response[GetSystemsResponse200]
     """
 
     kwargs = _get_kwargs(
-        ship_symbol=ship_symbol,
         _client=_client,
+        page=page,
+        limit=limit,
     )
 
     response = httpx.request(
         verify=_client.verify_ssl,
         **kwargs,
     )
 
@@ -111,37 +121,40 @@
             data=details.get("data"),
             headers=resp.headers,
         )
     )
 
 
 async def asyncio_detailed(
-    ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetMyShipCargoResponse200]:
-    """Get Ship Cargo
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
+) -> Response[GetSystemsResponse200]:
+    """List Systems
 
-     Retrieve the cargo of your ship.
+     Return a paginated list of all systems.
 
     Args:
-        ship_symbol (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        limit (Union[Unset, None, int]):  Default: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetMyShipCargoResponse200]
+        Response[GetSystemsResponse200]
     """
 
     kwargs = _get_kwargs(
-        ship_symbol=ship_symbol,
         _client=_client,
+        page=page,
+        limit=limit,
     )
 
     async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
         response = await c.request(**kwargs)
 
     resp = _build_response(client=_client, response=response)
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/get_my_ships.py` & `spacetraders-0.7.0/spacetraders/api/fleet/get_my_ships.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from ...models.get_my_ships_response_200 import GetMyShipsResponse200
 from ...types import UNSET, ApiError, Error, Response, Unset
 
 
 def _get_kwargs(
     *,
     _client: AuthenticatedClient,
-    page: Union[Unset, None, int] = UNSET,
-    limit: Union[Unset, None, int] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
 ) -> Dict[str, Any]:
     url = "{}/my/ships".format(_client.base_url)
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -63,24 +63,24 @@
     )
 
 
 def sync_detailed(
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    page: Union[Unset, None, int] = UNSET,
-    limit: Union[Unset, None, int] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
 ) -> Response[GetMyShipsResponse200]:
     """List Ships
 
-     Retrieve all of your ships.
+     Return a paginated list of all of ships under your agent's ownership.
 
     Args:
-        page (Union[Unset, None, int]):
-        limit (Union[Unset, None, int]):
+        page (Union[Unset, None, int]):  Default: 1.
+        limit (Union[Unset, None, int]):  Default: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetMyShipsResponse200]
@@ -124,24 +124,24 @@
     )
 
 
 async def asyncio_detailed(
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    page: Union[Unset, None, int] = UNSET,
-    limit: Union[Unset, None, int] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
 ) -> Response[GetMyShipsResponse200]:
     """List Ships
 
-     Retrieve all of your ships.
+     Return a paginated list of all of ships under your agent's ownership.
 
     Args:
-        page (Union[Unset, None, int]):
-        limit (Union[Unset, None, int]):
+        page (Union[Unset, None, int]):  Default: 1.
+        limit (Union[Unset, None, int]):  Default: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetMyShipsResponse200]
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/get_ship_cooldown.py` & `spacetraders-0.7.0/spacetraders/api/fleet/get_ship_cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/get_ship_nav.py` & `spacetraders-0.7.0/spacetraders/api/fleet/get_ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/install_mount.py` & `spacetraders-0.7.0/spacetraders/api/fleet/install_mount.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,19 @@
     raise_on_error: Optional[bool] = None,
     **json_body: InstallMountInstallMountRequest,
 ) -> Response[InstallMountInstallMount201Response]:
     """Install Mount
 
      Install a mount on a ship.
 
+    In order to install a mount, the ship must be docked and located in a waypoint that has a `Shipyard`
+    trait. The ship also must have the mount to install in its cargo hold.
+
+    An installation fee will be deduced by the Shipyard for installing the mount on the ship.
+
     Args:
         ship_symbol (str):
         json_body (InstallMountInstallMountRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -135,14 +140,19 @@
     raise_on_error: Optional[bool] = None,
     **json_body: InstallMountInstallMountRequest,
 ) -> Response[InstallMountInstallMount201Response]:
     """Install Mount
 
      Install a mount on a ship.
 
+    In order to install a mount, the ship must be docked and located in a waypoint that has a `Shipyard`
+    trait. The ship also must have the mount to install in its cargo hold.
+
+    An installation fee will be deduced by the Shipyard for installing the mount on the ship.
+
     Args:
         ship_symbol (str):
         json_body (InstallMountInstallMountRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/jettison.py` & `spacetraders-0.7.0/spacetraders/api/fleet/jettison.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/jump_ship.py` & `spacetraders-0.7.0/spacetraders/api/fleet/jump_ship.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,17 +66,22 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: JumpShipJsonBody,
 ) -> Response[JumpShipResponse200]:
     """Jump Ship
 
-     Jump your ship instantly to a target system. When used while in orbit or docked to a jump gate
-    waypoint, any ship can use this command. When used elsewhere, jumping requires a jump drive unit and
-    consumes a unit of antimatter (which needs to be in your cargo).
+     Jump your ship instantly to a target system. The ship must be in orbit to use this function. When
+    used while in orbit of a Jump Gate waypoint, any ship can use this command, jumping to the target
+    system's Jump Gate waypoint.
+
+    When used elsewhere, jumping requires the ship to have a `Jump Drive` module installed and consumes
+    a unit of antimatter from the ship's cargo. The command will fail if there is no antimatter to
+    consume. When jumping via the `Jump Drive` module, the ship ends up at its largest source of energy
+    in the system, such as a gas planet or a jump gate.
 
     Args:
         ship_symbol (str):
         json_body (JumpShipJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -131,17 +136,22 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: JumpShipJsonBody,
 ) -> Response[JumpShipResponse200]:
     """Jump Ship
 
-     Jump your ship instantly to a target system. When used while in orbit or docked to a jump gate
-    waypoint, any ship can use this command. When used elsewhere, jumping requires a jump drive unit and
-    consumes a unit of antimatter (which needs to be in your cargo).
+     Jump your ship instantly to a target system. The ship must be in orbit to use this function. When
+    used while in orbit of a Jump Gate waypoint, any ship can use this command, jumping to the target
+    system's Jump Gate waypoint.
+
+    When used elsewhere, jumping requires the ship to have a `Jump Drive` module installed and consumes
+    a unit of antimatter from the ship's cargo. The command will fail if there is no antimatter to
+    consume. When jumping via the `Jump Drive` module, the ship ends up at its largest source of energy
+    in the system, such as a gas planet or a jump gate.
 
     Args:
         ship_symbol (str):
         json_body (JumpShipJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/navigate_ship.py` & `spacetraders-0.7.0/spacetraders/api/fleet/navigate_ship.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,22 +66,22 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: NavigateShipJsonBody,
 ) -> Response[NavigateShipResponse200]:
     """Navigate Ship
 
-     Navigate to a target destination. The destination must be located within the same system as the
-    ship. Navigating will consume the necessary fuel and supplies from the ship's manifest, and will pay
-    out crew wages from the agent's account.
+     Navigate to a target destination. The ship must be in orbit to use this function. The destination
+    waypoint must be within the same system as the ship's current location. Navigating will consume the
+    necessary fuel from the ship's manifest based on the distance to the target waypoint.
 
     The returned response will detail the route information including the expected time of arrival. Most
     ship actions are unavailable until the ship has arrived at it's destination.
 
-    To travel between systems, see the ship's warp or jump actions.
+    To travel between systems, see the ship's Warp or Jump actions.
 
     Args:
         ship_symbol (str):
         json_body (NavigateShipJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -136,22 +136,22 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: NavigateShipJsonBody,
 ) -> Response[NavigateShipResponse200]:
     """Navigate Ship
 
-     Navigate to a target destination. The destination must be located within the same system as the
-    ship. Navigating will consume the necessary fuel and supplies from the ship's manifest, and will pay
-    out crew wages from the agent's account.
+     Navigate to a target destination. The ship must be in orbit to use this function. The destination
+    waypoint must be within the same system as the ship's current location. Navigating will consume the
+    necessary fuel from the ship's manifest based on the distance to the target waypoint.
 
     The returned response will detail the route information including the expected time of arrival. Most
     ship actions are unavailable until the ship has arrived at it's destination.
 
-    To travel between systems, see the ship's warp or jump actions.
+    To travel between systems, see the ship's Warp or Jump actions.
 
     Args:
         ship_symbol (str):
         json_body (NavigateShipJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/negotiate_contract.py` & `spacetraders-0.7.0/spacetraders/api/fleet/negotiate_contract.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,33 +12,29 @@
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
-    json_body: Any,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/negotiate/contract".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body
-
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
-        "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[NegotiateContractNegotiateContract200Response]:
     if response.status_code == HTTPStatus.CREATED:
@@ -63,36 +59,41 @@
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    **json_body: Any,
 ) -> Response[NegotiateContractNegotiateContract200Response]:
     """Negotiate Contract
 
+     Negotiate a new contract with the HQ.
+
+    In order to negotiate a new contract, an agent must not have ongoing or offered contracts over the
+    allowed maximum amount. Currently the maximum contracts an agent can have at a time is 1.
+
+    Once a contract is negotiated, it is added to the list of contracts offered to the agent, which the
+    agent can then accept.
+
+    The ship must be present at a faction's HQ waypoint to negotiate a contract with that faction.
+
     Args:
         ship_symbol (str):
-        json_body (Any):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[NegotiateContractNegotiateContract200Response]
     """
 
-    json_body = Any.parse_obj(json_body)
-
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=_client.verify_ssl,
         **kwargs,
     )
 
@@ -124,36 +125,41 @@
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    **json_body: Any,
 ) -> Response[NegotiateContractNegotiateContract200Response]:
     """Negotiate Contract
 
+     Negotiate a new contract with the HQ.
+
+    In order to negotiate a new contract, an agent must not have ongoing or offered contracts over the
+    allowed maximum amount. Currently the maximum contracts an agent can have at a time is 1.
+
+    Once a contract is negotiated, it is added to the list of contracts offered to the agent, which the
+    agent can then accept.
+
+    The ship must be present at a faction's HQ waypoint to negotiate a contract with that faction.
+
     Args:
         ship_symbol (str):
-        json_body (Any):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[NegotiateContractNegotiateContract200Response]
     """
 
-    json_body = Any.parse_obj(json_body)
-
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
         response = await c.request(**kwargs)
 
     resp = _build_response(client=_client, response=response)
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/orbit_ship.py` & `spacetraders-0.7.0/spacetraders/api/fleet/orbit_ship.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,17 +60,21 @@
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[OrbitShipOrbitShip200Response]:
     """Orbit Ship
 
-     Attempt to move your ship into orbit at it's current location. The request will only succeed if your
+     Attempt to move your ship into orbit at its current location. The request will only succeed if your
     ship is capable of moving into orbit at the time of the request.
 
+    Orbiting ships are able to do actions that require the ship to be above surface such as navigating
+    or extracting, but cannot access elements in their current waypoint, such as the market or a
+    shipyard.
+
     The endpoint is idempotent - successive calls will succeed even if the ship is already in orbit.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -121,17 +125,21 @@
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[OrbitShipOrbitShip200Response]:
     """Orbit Ship
 
-     Attempt to move your ship into orbit at it's current location. The request will only succeed if your
+     Attempt to move your ship into orbit at its current location. The request will only succeed if your
     ship is capable of moving into orbit at the time of the request.
 
+    Orbiting ships are able to do actions that require the ship to be above surface such as navigating
+    or extracting, but cannot access elements in their current waypoint, such as the market or a
+    shipyard.
+
     The endpoint is idempotent - successive calls will succeed even if the ship is already in orbit.
 
     Args:
         ship_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/patch_ship_nav.py` & `spacetraders-0.7.0/spacetraders/api/fleet/patch_ship_nav.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,18 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: PatchShipNavJsonBody,
 ) -> Response[PatchShipNavResponse200]:
     """Patch Ship Nav
 
-     Update the nav data of a ship, such as the flight mode.
+     Update the nav configuration of a ship.
+
+    Currently only supports configuring the Flight Mode of the ship, which affects its speed and fuel
+    consumption.
 
     Args:
         ship_symbol (str):
         json_body (PatchShipNavJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -129,15 +132,18 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: PatchShipNavJsonBody,
 ) -> Response[PatchShipNavResponse200]:
     """Patch Ship Nav
 
-     Update the nav data of a ship, such as the flight mode.
+     Update the nav configuration of a ship.
+
+    Currently only supports configuring the Flight Mode of the ship, which affects its speed and fuel
+    consumption.
 
     Args:
         ship_symbol (str):
         json_body (PatchShipNavJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/purchase_cargo.py` & `spacetraders-0.7.0/spacetraders/api/fleet/purchase_cargo.py`

 * *Files 18% similar despite different names*

```diff
@@ -70,15 +70,23 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: PurchaseCargoPurchaseCargoRequest,
 ) -> Response[PurchaseCargoPurchaseCargo201Response]:
     """Purchase Cargo
 
-     Purchase cargo.
+     Purchase cargo from a market.
+
+    The ship must be docked in a waypoint that has `Marketplace` trait, and the market must be selling a
+    good to be able to purchase it.
+
+    The maximum amount of units of a good that can be purchased in each transaction are denoted by the
+    `tradeVolume` value of the good, which can be viewed by using the Get Market action.
+
+    Purchased goods are added to the ship's cargo hold.
 
     Args:
         ship_symbol (str):
         json_body (PurchaseCargoPurchaseCargoRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -133,15 +141,23 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: PurchaseCargoPurchaseCargoRequest,
 ) -> Response[PurchaseCargoPurchaseCargo201Response]:
     """Purchase Cargo
 
-     Purchase cargo.
+     Purchase cargo from a market.
+
+    The ship must be docked in a waypoint that has `Marketplace` trait, and the market must be selling a
+    good to be able to purchase it.
+
+    The maximum amount of units of a good that can be purchased in each transaction are denoted by the
+    `tradeVolume` value of the good, which can be viewed by using the Get Market action.
+
+    Purchased goods are added to the ship's cargo hold.
 
     Args:
         ship_symbol (str):
         json_body (PurchaseCargoPurchaseCargoRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/purchase_ship.py` & `spacetraders-0.7.0/spacetraders/api/systems/get_jump_gate.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,92 +2,95 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.purchase_ship_json_body import PurchaseShipJsonBody
-from ...models.purchase_ship_response_201 import PurchaseShipResponse201
+from ...models.get_jump_gate_response_200 import GetJumpGateResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
+    system_symbol: str,
+    waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
-    json_body: PurchaseShipJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships".format(_client.base_url)
+    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/jump-gate".format(
+        _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
+    )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict(by_alias=True)
-
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
-        "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[PurchaseShipResponse201]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = PurchaseShipResponse201(**response.json())
+) -> Optional[GetJumpGateResponse200]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = GetJumpGateResponse200(**response.json())
 
-        return response_201
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[PurchaseShipResponse201]:
+) -> Response[GetJumpGateResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    system_symbol: str,
+    waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    **json_body: PurchaseShipJsonBody,
-) -> Response[PurchaseShipResponse201]:
-    """Purchase Ship
+) -> Response[GetJumpGateResponse200]:
+    """Get Jump Gate
+
+     Get jump gate details for a waypoint. Requires a waypoint of type `JUMP_GATE` to use.
 
-     Purchase a ship
+    The response will return all systems that are have a Jump Gate in range of this Jump Gate. Those
+    systems can be jumped to from this Jump Gate.
 
     Args:
-        json_body (PurchaseShipJsonBody):
+        system_symbol (str):
+        waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PurchaseShipResponse201]
+        Response[GetJumpGateResponse200]
     """
 
-    json_body = PurchaseShipJsonBody.parse_obj(json_body)
-
     kwargs = _get_kwargs(
+        system_symbol=system_symbol,
+        waypoint_symbol=waypoint_symbol,
         _client=_client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=_client.verify_ssl,
         **kwargs,
     )
 
@@ -115,39 +118,43 @@
             data=details.get("data"),
             headers=resp.headers,
         )
     )
 
 
 async def asyncio_detailed(
+    system_symbol: str,
+    waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    **json_body: PurchaseShipJsonBody,
-) -> Response[PurchaseShipResponse201]:
-    """Purchase Ship
+) -> Response[GetJumpGateResponse200]:
+    """Get Jump Gate
+
+     Get jump gate details for a waypoint. Requires a waypoint of type `JUMP_GATE` to use.
 
-     Purchase a ship
+    The response will return all systems that are have a Jump Gate in range of this Jump Gate. Those
+    systems can be jumped to from this Jump Gate.
 
     Args:
-        json_body (PurchaseShipJsonBody):
+        system_symbol (str):
+        waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PurchaseShipResponse201]
+        Response[GetJumpGateResponse200]
     """
 
-    json_body = PurchaseShipJsonBody.parse_obj(json_body)
-
     kwargs = _get_kwargs(
+        system_symbol=system_symbol,
+        waypoint_symbol=waypoint_symbol,
         _client=_client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
         response = await c.request(**kwargs)
 
     resp = _build_response(client=_client, response=response)
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/refuel_ship.py` & `spacetraders-0.7.0/spacetraders/api/systems/get_waypoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,87 +2,93 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.refuel_ship_response_200 import RefuelShipResponse200
+from ...models.get_waypoint_response_200 import GetWaypointResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
-    ship_symbol: str,
+    system_symbol: str,
+    waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}/refuel".format(
-        _client.base_url, shipSymbol=ship_symbol
+    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}".format(
+        _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[RefuelShipResponse200]:
+) -> Optional[GetWaypointResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = RefuelShipResponse200(**response.json())
+        response_200 = GetWaypointResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[RefuelShipResponse200]:
+) -> Response[GetWaypointResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    ship_symbol: str,
+    system_symbol: str,
+    waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[RefuelShipResponse200]:
-    """Refuel Ship
+) -> Response[GetWaypointResponse200]:
+    """Get Waypoint
 
-     Refuel your ship from the local market.
+     View the details of a waypoint.
+
+    If the waypoint is uncharted, it will return the 'Uncharted' trait instead of its actual traits.
 
     Args:
-        ship_symbol (str):
+        system_symbol (str):
+        waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[RefuelShipResponse200]
+        Response[GetWaypointResponse200]
     """
 
     kwargs = _get_kwargs(
-        ship_symbol=ship_symbol,
+        system_symbol=system_symbol,
+        waypoint_symbol=waypoint_symbol,
         _client=_client,
     )
 
     response = httpx.request(
         verify=_client.verify_ssl,
         **kwargs,
     )
@@ -111,36 +117,41 @@
             data=details.get("data"),
             headers=resp.headers,
         )
     )
 
 
 async def asyncio_detailed(
-    ship_symbol: str,
+    system_symbol: str,
+    waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[RefuelShipResponse200]:
-    """Refuel Ship
+) -> Response[GetWaypointResponse200]:
+    """Get Waypoint
+
+     View the details of a waypoint.
 
-     Refuel your ship from the local market.
+    If the waypoint is uncharted, it will return the 'Uncharted' trait instead of its actual traits.
 
     Args:
-        ship_symbol (str):
+        system_symbol (str):
+        waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[RefuelShipResponse200]
+        Response[GetWaypointResponse200]
     """
 
     kwargs = _get_kwargs(
-        ship_symbol=ship_symbol,
+        system_symbol=system_symbol,
+        waypoint_symbol=waypoint_symbol,
         _client=_client,
     )
 
     async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
         response = await c.request(**kwargs)
 
     resp = _build_response(client=_client, response=response)
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/remove_mount.py` & `spacetraders-0.7.0/spacetraders/api/fleet/remove_mount.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,14 +70,19 @@
     raise_on_error: Optional[bool] = None,
     **json_body: RemoveMountRemoveMountRequest,
 ) -> Response[RemoveMountRemoveMount201Response]:
     """Remove Mount
 
      Remove a mount from a ship.
 
+    The ship must be docked in a waypoint that has the `Shipyard` trait, and must have the desired mount
+    that it wish to remove installed.
+
+    A removal fee will be deduced from the agent by the Shipyard.
+
     Args:
         ship_symbol (str):
         json_body (RemoveMountRemoveMountRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -133,14 +138,19 @@
     raise_on_error: Optional[bool] = None,
     **json_body: RemoveMountRemoveMountRequest,
 ) -> Response[RemoveMountRemoveMount201Response]:
     """Remove Mount
 
      Remove a mount from a ship.
 
+    The ship must be docked in a waypoint that has the `Shipyard` trait, and must have the desired mount
+    that it wish to remove installed.
+
+    A removal fee will be deduced from the agent by the Shipyard.
+
     Args:
         ship_symbol (str):
         json_body (RemoveMountRemoveMountRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/sell_cargo.py` & `spacetraders-0.7.0/spacetraders/api/fleet/sell_cargo.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,16 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: SellCargoSellCargoRequest,
 ) -> Response[SellCargoSellCargo201Response]:
     """Sell Cargo
 
-     Sell cargo.
+     Sell cargo in your ship to a market that trades this cargo. The ship must be docked in a waypoint
+    that has the `Marketplace` trait in order to use this function.
 
     Args:
         ship_symbol (str):
         json_body (SellCargoSellCargoRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -129,15 +130,16 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: SellCargoSellCargoRequest,
 ) -> Response[SellCargoSellCargo201Response]:
     """Sell Cargo
 
-     Sell cargo.
+     Sell cargo in your ship to a market that trades this cargo. The ship must be docked in a waypoint
+    that has the `Marketplace` trait in order to use this function.
 
     Args:
         ship_symbol (str):
         json_body (SellCargoSellCargoRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/ship_refine.py` & `spacetraders-0.7.0/spacetraders/api/fleet/warp_ship.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,28 +2,26 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.ship_refine_json_body import ShipRefineJsonBody
-from ...models.ship_refine_ship_refine_200_response import (
-    ShipRefineShipRefine200Response,
-)
+from ...models.warp_ship_json_body import WarpShipJsonBody
+from ...models.warp_ship_response_200 import WarpShipResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
-    json_body: ShipRefineJsonBody,
+    json_body: WarpShipJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}/refine".format(
+    url = "{}/my/ships/{shipSymbol}/warp".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     json_json_body = json_body.dict(by_alias=True)
@@ -37,61 +35,65 @@
         "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[ShipRefineShipRefine200Response]:
+) -> Optional[WarpShipResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ShipRefineShipRefine200Response(**response.json())
+        response_200 = WarpShipResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[ShipRefineShipRefine200Response]:
+) -> Response[WarpShipResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    **json_body: ShipRefineJsonBody,
-) -> Response[ShipRefineShipRefine200Response]:
-    """Ship Refine
+    **json_body: WarpShipJsonBody,
+) -> Response[WarpShipResponse200]:
+    """Warp Ship
+
+     Warp your ship to a target destination in another system. The ship must be in orbit to use this
+    function and must have the `Warp Drive` module installed. Warping will consume the necessary fuel
+    from the ship's manifest.
 
-     Attempt to refine the raw materials on your ship. The request will only succeed if your ship is
-    capable of refining at the time of the request.
+    The returned response will detail the route information including the expected time of arrival. Most
+    ship actions are unavailable until the ship has arrived at its destination.
 
     Args:
         ship_symbol (str):
-        json_body (ShipRefineJsonBody):
+        json_body (WarpShipJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ShipRefineShipRefine200Response]
+        Response[WarpShipResponse200]
     """
 
-    json_body = ShipRefineJsonBody.parse_obj(json_body)
+    json_body = WarpShipJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
 
@@ -128,34 +130,38 @@
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    **json_body: ShipRefineJsonBody,
-) -> Response[ShipRefineShipRefine200Response]:
-    """Ship Refine
+    **json_body: WarpShipJsonBody,
+) -> Response[WarpShipResponse200]:
+    """Warp Ship
+
+     Warp your ship to a target destination in another system. The ship must be in orbit to use this
+    function and must have the `Warp Drive` module installed. Warping will consume the necessary fuel
+    from the ship's manifest.
 
-     Attempt to refine the raw materials on your ship. The request will only succeed if your ship is
-    capable of refining at the time of the request.
+    The returned response will detail the route information including the expected time of arrival. Most
+    ship actions are unavailable until the ship has arrived at its destination.
 
     Args:
         ship_symbol (str):
-        json_body (ShipRefineJsonBody):
+        json_body (WarpShipJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ShipRefineShipRefine200Response]
+        Response[WarpShipResponse200]
     """
 
-    json_body = ShipRefineJsonBody.parse_obj(json_body)
+    json_body = WarpShipJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/transfer_cargo.py` & `spacetraders-0.7.0/spacetraders/api/fleet/transfer_cargo.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,20 @@
     raise_on_error: Optional[bool] = None,
     **json_body: TransferCargoTransferCargoRequest,
 ) -> Response[TransferCargoTransferCargo200Response]:
     """Transfer Cargo
 
      Transfer cargo between ships.
 
+    The receiving ship must be in the same waypoint as the transferring ship, and it must able to hold
+    the additional cargo after the transfer is complete. Both ships also must be in the same state,
+    either both are docked or both are orbiting.
+
+    The response body's cargo shows the cargo of the transferring ship after the transfer is complete.
+
     Args:
         ship_symbol (str):
         json_body (TransferCargoTransferCargoRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -135,14 +141,20 @@
     raise_on_error: Optional[bool] = None,
     **json_body: TransferCargoTransferCargoRequest,
 ) -> Response[TransferCargoTransferCargo200Response]:
     """Transfer Cargo
 
      Transfer cargo between ships.
 
+    The receiving ship must be in the same waypoint as the transferring ship, and it must able to hold
+    the additional cargo after the transfer is complete. Both ships also must be in the same state,
+    either both are docked or both are orbiting.
+
+    The response body's cargo shows the cargo of the transferring ship after the transfer is complete.
+
     Args:
         ship_symbol (str):
         json_body (TransferCargoTransferCargoRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/fleet/warp_ship.py` & `spacetraders-0.7.0/spacetraders/api/fleet/refuel_ship.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.warp_ship_json_body import WarpShipJsonBody
-from ...models.warp_ship_response_200 import WarpShipResponse200
+from ...models.refuel_ship_json_body import RefuelShipJsonBody
+from ...models.refuel_ship_response_200 import RefuelShipResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
-    json_body: WarpShipJsonBody,
+    json_body: RefuelShipJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}/warp".format(
+    url = "{}/my/ships/{shipSymbol}/refuel".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     json_json_body = json_body.dict(by_alias=True)
@@ -35,64 +35,67 @@
         "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[WarpShipResponse200]:
+) -> Optional[RefuelShipResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = WarpShipResponse200(**response.json())
+        response_200 = RefuelShipResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[WarpShipResponse200]:
+) -> Response[RefuelShipResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    **json_body: WarpShipJsonBody,
-) -> Response[WarpShipResponse200]:
-    """Warp Ship
+    **json_body: RefuelShipJsonBody,
+) -> Response[RefuelShipResponse200]:
+    """Refuel Ship
 
-     Warp your ship to a target destination in another system. Warping will consume the necessary fuel
-    and supplies from the ship's manifest, and will pay out crew wages from the agent's account.
+     Refuel your ship by buying fuel from the local market.
 
-    The returned response will detail the route information including the expected time of arrival. Most
-    ship actions are unavailable until the ship has arrived at it's destination.
+    Requires the ship to be docked in a waypoint that has the `Marketplace` trait, and the market must
+    be selling fuel in order to refuel.
+
+    Each fuel bought from the market replenishes 100 units in your ship's fuel.
+
+    Ships will always be refuel to their frame's maximum fuel capacity when using this action.
 
     Args:
         ship_symbol (str):
-        json_body (WarpShipJsonBody):
+        json_body (RefuelShipJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[WarpShipResponse200]
+        Response[RefuelShipResponse200]
     """
 
-    json_body = WarpShipJsonBody.parse_obj(json_body)
+    json_body = RefuelShipJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
 
@@ -129,37 +132,40 @@
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-    **json_body: WarpShipJsonBody,
-) -> Response[WarpShipResponse200]:
-    """Warp Ship
+    **json_body: RefuelShipJsonBody,
+) -> Response[RefuelShipResponse200]:
+    """Refuel Ship
+
+     Refuel your ship by buying fuel from the local market.
+
+    Requires the ship to be docked in a waypoint that has the `Marketplace` trait, and the market must
+    be selling fuel in order to refuel.
 
-     Warp your ship to a target destination in another system. Warping will consume the necessary fuel
-    and supplies from the ship's manifest, and will pay out crew wages from the agent's account.
+    Each fuel bought from the market replenishes 100 units in your ship's fuel.
 
-    The returned response will detail the route information including the expected time of arrival. Most
-    ship actions are unavailable until the ship has arrived at it's destination.
+    Ships will always be refuel to their frame's maximum fuel capacity when using this action.
 
     Args:
         ship_symbol (str):
-        json_body (WarpShipJsonBody):
+        json_body (RefuelShipJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[WarpShipResponse200]
+        Response[RefuelShipResponse200]
     """
 
-    json_body = WarpShipJsonBody.parse_obj(json_body)
+    json_body = RefuelShipJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.6.0/spacetraders/api/systems/get_jump_gate.py` & `spacetraders-0.7.0/spacetraders/api/systems/get_shipyard.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.get_jump_gate_response_200 import GetJumpGateResponse200
+from ...models.get_shipyard_response_200 import GetShipyardResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/jump-gate".format(
+    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/shipyard".format(
         _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
@@ -31,57 +31,59 @@
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[GetJumpGateResponse200]:
+) -> Optional[GetShipyardResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetJumpGateResponse200(**response.json())
+        response_200 = GetShipyardResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[GetJumpGateResponse200]:
+) -> Response[GetShipyardResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetJumpGateResponse200]:
-    """Get Jump Gate
+) -> Response[GetShipyardResponse200]:
+    """Get Shipyard
 
-     Get jump gate details for a waypoint.
+     Get the shipyard for a waypoint. Requires a waypoint that has the `Shipyard` trait to use. Send a
+    ship to the waypoint to access data on ships that are currently available for purchase and recent
+    transactions.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetJumpGateResponse200]
+        Response[GetShipyardResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
         _client=_client,
     )
@@ -120,29 +122,31 @@
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetJumpGateResponse200]:
-    """Get Jump Gate
+) -> Response[GetShipyardResponse200]:
+    """Get Shipyard
 
-     Get jump gate details for a waypoint.
+     Get the shipyard for a waypoint. Requires a waypoint that has the `Shipyard` trait to use. Send a
+    ship to the waypoint to access data on ships that are currently available for purchase and recent
+    transactions.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetJumpGateResponse200]
+        Response[GetShipyardResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
         _client=_client,
     )
```

### Comparing `spacetraders-0.6.0/spacetraders/api/systems/get_market.py` & `spacetraders-0.7.0/spacetraders/api/systems/get_market.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,17 +62,20 @@
     waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetMarketResponse200]:
     """Get Market
 
-     Retrieve imports, exports and exchange data from a marketplace. Imports can be sold, exports can be
-    purchased, and exchange goods can be purchased or sold. Send a ship to the waypoint to access trade
-    good prices and recent transactions.
+     Retrieve imports, exports and exchange data from a marketplace. Requires a waypoint that has the
+    `Marketplace` trait to use.
+
+    Send a ship to the waypoint to access trade good prices and recent transactions. Refer to the
+    [Market Overview page](https://docs.spacetraders.io/game-concepts/markets) to gain better a
+    understanding of the market in the game.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -125,17 +128,20 @@
     waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetMarketResponse200]:
     """Get Market
 
-     Retrieve imports, exports and exchange data from a marketplace. Imports can be sold, exports can be
-    purchased, and exchange goods can be purchased or sold. Send a ship to the waypoint to access trade
-    good prices and recent transactions.
+     Retrieve imports, exports and exchange data from a marketplace. Requires a waypoint that has the
+    `Marketplace` trait to use.
+
+    Send a ship to the waypoint to access trade good prices and recent transactions. Refer to the
+    [Market Overview page](https://docs.spacetraders.io/game-concepts/markets) to gain better a
+    understanding of the market in the game.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `spacetraders-0.6.0/spacetraders/api/systems/get_shipyard.py` & `spacetraders-0.7.0/spacetraders/api/systems/get_system_waypoints.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,107 @@
 import json
 from http import HTTPStatus
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.get_shipyard_response_200 import GetShipyardResponse200
-from ...types import ApiError, Error, Response
+from ...models.get_system_waypoints_response_200 import GetSystemWaypointsResponse200
+from ...types import UNSET, ApiError, Error, Response, Unset
 
 
 def _get_kwargs(
     system_symbol: str,
-    waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
 ) -> Dict[str, Any]:
-    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/shipyard".format(
-        _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
+    url = "{}/systems/{systemSymbol}/waypoints".format(
+        _client.base_url, systemSymbol=system_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
+    params: Dict[str, Any] = {}
+    params["page"] = page
+
+    params["limit"] = limit
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
+        "params": params,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[GetShipyardResponse200]:
+) -> Optional[GetSystemWaypointsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetShipyardResponse200(**response.json())
+        response_200 = GetSystemWaypointsResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[GetShipyardResponse200]:
+) -> Response[GetSystemWaypointsResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     system_symbol: str,
-    waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetShipyardResponse200]:
-    """Get Shipyard
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
+) -> Response[GetSystemWaypointsResponse200]:
+    """List Waypoints in System
 
-     Get the shipyard for a waypoint. Send a ship to the waypoint to access ships that are currently
-    available for purchase and recent transactions.
+     Return a paginated list of all of the waypoints for a given system.
+
+    If a waypoint is uncharted, it will return the `Uncharted` trait instead of its actual traits.
 
     Args:
         system_symbol (str):
-        waypoint_symbol (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        limit (Union[Unset, None, int]):  Default: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetShipyardResponse200]
+        Response[GetSystemWaypointsResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
-        waypoint_symbol=waypoint_symbol,
         _client=_client,
+        page=page,
+        limit=limit,
     )
 
     response = httpx.request(
         verify=_client.verify_ssl,
         **kwargs,
     )
 
@@ -117,40 +130,44 @@
             headers=resp.headers,
         )
     )
 
 
 async def asyncio_detailed(
     system_symbol: str,
-    waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetShipyardResponse200]:
-    """Get Shipyard
+    page: Union[Unset, None, int] = 1,
+    limit: Union[Unset, None, int] = 10,
+) -> Response[GetSystemWaypointsResponse200]:
+    """List Waypoints in System
+
+     Return a paginated list of all of the waypoints for a given system.
 
-     Get the shipyard for a waypoint. Send a ship to the waypoint to access ships that are currently
-    available for purchase and recent transactions.
+    If a waypoint is uncharted, it will return the `Uncharted` trait instead of its actual traits.
 
     Args:
         system_symbol (str):
-        waypoint_symbol (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        limit (Union[Unset, None, int]):  Default: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetShipyardResponse200]
+        Response[GetSystemWaypointsResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
-        waypoint_symbol=waypoint_symbol,
         _client=_client,
+        page=page,
+        limit=limit,
     )
 
     async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
         response = await c.request(**kwargs)
 
     resp = _build_response(client=_client, response=response)
```

### Comparing `spacetraders-0.6.0/spacetraders/client.py` & `spacetraders-0.7.0/spacetraders/client.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/__init__.py` & `spacetraders-0.7.0/spacetraders/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from .dock_ship_dock_ship_200_response_data import DockShipDockShip200ResponseData
 from .extract_resources_json_body import ExtractResourcesJsonBody
 from .extract_resources_response_201 import ExtractResourcesResponse201
 from .extract_resources_response_201_data import ExtractResourcesResponse201Data
 from .extraction import Extraction
 from .extraction_yield import ExtractionYield
 from .faction import Faction
+from .faction_symbols import FactionSymbols
 from .faction_trait import FactionTrait
 from .faction_trait_symbol import FactionTraitSymbol
 from .fulfill_contract_response_200 import FulfillContractResponse200
 from .fulfill_contract_response_200_data import FulfillContractResponse200Data
 from .get_contract_response_200 import GetContractResponse200
 from .get_contracts_response_200 import GetContractsResponse200
 from .get_faction_response_200 import GetFactionResponse200
@@ -74,17 +75,14 @@
 from .get_waypoint_response_200 import GetWaypointResponse200
 from .install_mount_install_mount_201_response import (
     InstallMountInstallMount201Response,
 )
 from .install_mount_install_mount_201_response_data import (
     InstallMountInstallMount201ResponseData,
 )
-from .install_mount_install_mount_201_response_data_transaction import (
-    InstallMountInstallMount201ResponseDataTransaction,
-)
 from .install_mount_install_mount_request import InstallMountInstallMountRequest
 from .jettison_json_body import JettisonJsonBody
 from .jettison_response_200 import JettisonResponse200
 from .jettison_response_200_data import JettisonResponse200Data
 from .jump_gate import JumpGate
 from .jump_ship_json_body import JumpShipJsonBody
 from .jump_ship_response_200 import JumpShipResponse200
@@ -114,26 +112,24 @@
 from .purchase_cargo_purchase_cargo_201_response_data import (
     PurchaseCargoPurchaseCargo201ResponseData,
 )
 from .purchase_cargo_purchase_cargo_request import PurchaseCargoPurchaseCargoRequest
 from .purchase_ship_json_body import PurchaseShipJsonBody
 from .purchase_ship_response_201 import PurchaseShipResponse201
 from .purchase_ship_response_201_data import PurchaseShipResponse201Data
+from .refuel_ship_json_body import RefuelShipJsonBody
 from .refuel_ship_response_200 import RefuelShipResponse200
 from .refuel_ship_response_200_data import RefuelShipResponse200Data
 from .register_json_body import RegisterJsonBody
 from .register_response_201 import RegisterResponse201
 from .register_response_201_data import RegisterResponse201Data
 from .remove_mount_remove_mount_201_response import RemoveMountRemoveMount201Response
 from .remove_mount_remove_mount_201_response_data import (
     RemoveMountRemoveMount201ResponseData,
 )
-from .remove_mount_remove_mount_201_response_data_transaction import (
-    RemoveMountRemoveMount201ResponseDataTransaction,
-)
 from .remove_mount_remove_mount_request import RemoveMountRemoveMountRequest
 from .scanned_ship import ScannedShip
 from .scanned_ship_engine import ScannedShipEngine
 from .scanned_ship_frame import ScannedShipFrame
 from .scanned_ship_mounts_item import ScannedShipMountsItem
 from .scanned_ship_reactor import ScannedShipReactor
 from .scanned_system import ScannedSystem
@@ -148,37 +144,38 @@
 from .ship_crew_rotation import ShipCrewRotation
 from .ship_engine import ShipEngine
 from .ship_engine_symbol import ShipEngineSymbol
 from .ship_frame import ShipFrame
 from .ship_frame_symbol import ShipFrameSymbol
 from .ship_fuel import ShipFuel
 from .ship_fuel_consumed import ShipFuelConsumed
+from .ship_modification_transaction import ShipModificationTransaction
 from .ship_module import ShipModule
 from .ship_module_symbol import ShipModuleSymbol
 from .ship_mount import ShipMount
 from .ship_mount_deposits_item import ShipMountDepositsItem
 from .ship_mount_symbol import ShipMountSymbol
 from .ship_nav import ShipNav
 from .ship_nav_flight_mode import ShipNavFlightMode
 from .ship_nav_route import ShipNavRoute
 from .ship_nav_route_waypoint import ShipNavRouteWaypoint
 from .ship_nav_status import ShipNavStatus
 from .ship_reactor import ShipReactor
 from .ship_reactor_symbol import ShipReactorSymbol
 from .ship_refine_json_body import ShipRefineJsonBody
 from .ship_refine_json_body_produce import ShipRefineJsonBodyProduce
-from .ship_refine_ship_refine_200_response import ShipRefineShipRefine200Response
-from .ship_refine_ship_refine_200_response_data import (
-    ShipRefineShipRefine200ResponseData,
+from .ship_refine_ship_refine_201_response import ShipRefineShipRefine201Response
+from .ship_refine_ship_refine_201_response_data import (
+    ShipRefineShipRefine201ResponseData,
 )
-from .ship_refine_ship_refine_200_response_data_consumed_item import (
-    ShipRefineShipRefine200ResponseDataConsumedItem,
+from .ship_refine_ship_refine_201_response_data_consumed_item import (
+    ShipRefineShipRefine201ResponseDataConsumedItem,
 )
-from .ship_refine_ship_refine_200_response_data_produced_item import (
-    ShipRefineShipRefine200ResponseDataProducedItem,
+from .ship_refine_ship_refine_201_response_data_produced_item import (
+    ShipRefineShipRefine201ResponseDataProducedItem,
 )
 from .ship_registration import ShipRegistration
 from .ship_requirements import ShipRequirements
 from .ship_role import ShipRole
 from .ship_type import ShipType
 from .shipyard import Shipyard
 from .shipyard_ship import ShipyardShip
@@ -239,14 +236,15 @@
     "DockShipDockShip200ResponseData",
     "Extraction",
     "ExtractionYield",
     "ExtractResourcesJsonBody",
     "ExtractResourcesResponse201",
     "ExtractResourcesResponse201Data",
     "Faction",
+    "FactionSymbols",
     "FactionTrait",
     "FactionTraitSymbol",
     "FulfillContractResponse200",
     "FulfillContractResponse200Data",
     "GetContractResponse200",
     "GetContractsResponse200",
     "GetFactionResponse200",
@@ -271,15 +269,14 @@
     "GetStatusResponse200Stats",
     "GetSystemResponse200",
     "GetSystemsResponse200",
     "GetSystemWaypointsResponse200",
     "GetWaypointResponse200",
     "InstallMountInstallMount201Response",
     "InstallMountInstallMount201ResponseData",
-    "InstallMountInstallMount201ResponseDataTransaction",
     "InstallMountInstallMountRequest",
     "JettisonJsonBody",
     "JettisonResponse200",
     "JettisonResponse200Data",
     "JumpGate",
     "JumpShipJsonBody",
     "JumpShipResponse200",
@@ -301,22 +298,22 @@
     "PatchShipNavResponse200",
     "PurchaseCargoPurchaseCargo201Response",
     "PurchaseCargoPurchaseCargo201ResponseData",
     "PurchaseCargoPurchaseCargoRequest",
     "PurchaseShipJsonBody",
     "PurchaseShipResponse201",
     "PurchaseShipResponse201Data",
+    "RefuelShipJsonBody",
     "RefuelShipResponse200",
     "RefuelShipResponse200Data",
     "RegisterJsonBody",
     "RegisterResponse201",
     "RegisterResponse201Data",
     "RemoveMountRemoveMount201Response",
     "RemoveMountRemoveMount201ResponseData",
-    "RemoveMountRemoveMount201ResponseDataTransaction",
     "RemoveMountRemoveMountRequest",
     "ScannedShip",
     "ScannedShipEngine",
     "ScannedShipFrame",
     "ScannedShipMountsItem",
     "ScannedShipReactor",
     "ScannedSystem",
@@ -331,32 +328,33 @@
     "ShipCrewRotation",
     "ShipEngine",
     "ShipEngineSymbol",
     "ShipFrame",
     "ShipFrameSymbol",
     "ShipFuel",
     "ShipFuelConsumed",
+    "ShipModificationTransaction",
     "ShipModule",
     "ShipModuleSymbol",
     "ShipMount",
     "ShipMountDepositsItem",
     "ShipMountSymbol",
     "ShipNav",
     "ShipNavFlightMode",
     "ShipNavRoute",
     "ShipNavRouteWaypoint",
     "ShipNavStatus",
     "ShipReactor",
     "ShipReactorSymbol",
     "ShipRefineJsonBody",
     "ShipRefineJsonBodyProduce",
-    "ShipRefineShipRefine200Response",
-    "ShipRefineShipRefine200ResponseData",
-    "ShipRefineShipRefine200ResponseDataConsumedItem",
-    "ShipRefineShipRefine200ResponseDataProducedItem",
+    "ShipRefineShipRefine201Response",
+    "ShipRefineShipRefine201ResponseData",
+    "ShipRefineShipRefine201ResponseDataConsumedItem",
+    "ShipRefineShipRefine201ResponseDataProducedItem",
     "ShipRegistration",
     "ShipRequirements",
     "ShipRole",
     "ShipType",
     "Shipyard",
     "ShipyardShip",
     "ShipyardShipTypesItem",
```

### Comparing `spacetraders-0.6.0/spacetraders/models/accept_contract_response_200.py` & `spacetraders-0.7.0/spacetraders/models/accept_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/accept_contract_response_200_data.py` & `spacetraders-0.7.0/spacetraders/models/accept_contract_response_200_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 T = TypeVar("T", bound="AcceptContractResponse200Data")
 
 
 class AcceptContractResponse200Data(BaseModel):
     """
     Attributes:
-        agent (Agent):
-        contract (Contract):
+        agent (Agent): Agent details.
+        contract (Contract): Contract details.
     """
 
     agent: "Agent" = Field(alias="agent")
     contract: "Contract" = Field(alias="contract")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
```

### Comparing `spacetraders-0.6.0/spacetraders/models/agent.py` & `spacetraders-0.7.0/spacetraders/models/agent.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 
 from ..types import Unset
 
 T = TypeVar("T", bound="Agent")
 
 
 class Agent(BaseModel):
-    """
+    """Agent details.
+
     Attributes:
-        account_id (str):
-        symbol (str):
+        account_id (str): Account ID that is tied to this agent.
+        symbol (str): Symbol of the agent.
         headquarters (str): The headquarters of the agent.
         credits_ (int): The number of credits the agent has available. Credits can be negative if funds have been
             overdrawn.
         starting_faction (str): The faction the agent started with.
     """
 
     account_id: str = Field(alias="accountId")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/chart.py` & `spacetraders-0.7.0/spacetraders/models/chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 T = TypeVar("T", bound="Chart")
 
 
 class Chart(BaseModel):
     """The chart of a system or waypoint, which makes the location visible to other agents.
 
     Attributes:
-        waypoint_symbol (Union[Unset, str]):
-        submitted_by (Union[Unset, str]):
-        submitted_on (Union[Unset, datetime.datetime]):
+        waypoint_symbol (Union[Unset, str]): The symbol of the waypoint.
+        submitted_by (Union[Unset, str]): The agent that submitted the chart for this waypoint.
+        submitted_on (Union[Unset, datetime.datetime]): The time the chart for this waypoint was submitted.
     """
 
     waypoint_symbol: Union[Unset, str] = Field(UNSET, alias="waypointSymbol")
     submitted_by: Union[Unset, str] = Field(UNSET, alias="submittedBy")
     submitted_on: Union[Unset, datetime.datetime] = Field(UNSET, alias="submittedOn")
     additional_properties: Dict[str, Any] = {}
```

### Comparing `spacetraders-0.6.0/spacetraders/models/connected_system.py` & `spacetraders-0.7.0/spacetraders/models/connected_system.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 T = TypeVar("T", bound="ConnectedSystem")
 
 
 class ConnectedSystem(BaseModel):
     """
     Attributes:
-        symbol (str):
-        sector_symbol (str):
+        symbol (str): The symbol of the system.
+        sector_symbol (str): The sector of this system.
         type (SystemType): The type of waypoint.
-        x (int):
-        y (int):
-        distance (int):
+        x (int): Position in the universe in the x axis.
+        y (int): Position in the universe in the y axis.
+        distance (int): The distance of this system to the connected Jump Gate.
         faction_symbol (Union[Unset, str]): The symbol of the faction that owns the connected jump gate in the system.
     """
 
     symbol: str = Field(alias="symbol")
     sector_symbol: str = Field(alias="sectorSymbol")
     type: SystemType = Field(alias="type")
     x: int = Field(alias="x")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/contract.py` & `spacetraders-0.7.0/spacetraders/models/contract.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 from ..models.contract_type import ContractType
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="Contract")
 
 
 class Contract(BaseModel):
-    """
+    """Contract details.
+
     Attributes:
-        id (str):
+        id (str): ID of the contract.
         faction_symbol (str): The symbol of the faction that this contract is for.
-        type (ContractType):
-        terms (ContractTerms):
+        type (ContractType): Type of contract.
+        terms (ContractTerms): Terms of the contract needed to fulfill it.
         accepted (bool): Whether the contract has been accepted by the agent
         fulfilled (bool): Whether the contract has been fulfilled
         expiration (datetime.datetime): Deprecated in favor of deadlineToAccept
         deadline_to_accept (Union[Unset, datetime.datetime]): The time at which the contract is no longer available to
             be accepted
     """
```

### Comparing `spacetraders-0.6.0/spacetraders/models/contract_deliver_good.py` & `spacetraders-0.7.0/spacetraders/models/contract_deliver_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/contract_payment.py` & `spacetraders-0.7.0/spacetraders/models/contract_payment.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/contract_terms.py` & `spacetraders-0.7.0/spacetraders/models/contract_terms.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 from ..models.contract_payment import ContractPayment
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="ContractTerms")
 
 
 class ContractTerms(BaseModel):
-    """
+    """Terms of the contract needed to fulfill it.
+
     Attributes:
         deadline (datetime.datetime): The deadline for the contract.
         payment (ContractPayment):
-        deliver (Union[Unset, List['ContractDeliverGood']]):
+        deliver (Union[Unset, List['ContractDeliverGood']]): The cargo that needs to be delivered to fulfill the
+            contract.
     """
 
     deadline: datetime.datetime = Field(alias="deadline")
     payment: "ContractPayment" = Field(alias="payment")
     deliver: Union[Unset, List["ContractDeliverGood"]] = Field(UNSET, alias="deliver")
     additional_properties: Dict[str, Any] = {}
```

### Comparing `spacetraders-0.6.0/spacetraders/models/cooldown.py` & `spacetraders-0.7.0/spacetraders/models/cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/create_chart_response_201.py` & `spacetraders-0.7.0/spacetraders/models/create_chart_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/create_chart_response_201_data.py` & `spacetraders-0.7.0/spacetraders/models/create_chart_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/create_ship_ship_scan_response_201.py` & `spacetraders-0.7.0/spacetraders/models/create_ship_ship_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/create_ship_ship_scan_response_201_data.py` & `spacetraders-0.7.0/spacetraders/models/create_ship_ship_scan_response_201_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 T = TypeVar("T", bound="CreateShipShipScanResponse201Data")
 
 
 class CreateShipShipScanResponse201Data(BaseModel):
     """
     Attributes:
         cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
-        ships (List['ScannedShip']):
+        ships (List['ScannedShip']): List of scanned ships.
     """
 
     cooldown: "Cooldown" = Field(alias="cooldown")
     ships: List["ScannedShip"] = Field(alias="ships")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
```

### Comparing `spacetraders-0.6.0/spacetraders/models/create_ship_system_scan_response_201.py` & `spacetraders-0.7.0/spacetraders/models/create_ship_system_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/create_ship_system_scan_response_201_data.py` & `spacetraders-0.7.0/spacetraders/models/create_ship_system_scan_response_201_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 T = TypeVar("T", bound="CreateShipSystemScanResponse201Data")
 
 
 class CreateShipSystemScanResponse201Data(BaseModel):
     """
     Attributes:
         cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
-        systems (List['ScannedSystem']):
+        systems (List['ScannedSystem']): List of scanned systems.
     """
 
     cooldown: "Cooldown" = Field(alias="cooldown")
     systems: List["ScannedSystem"] = Field(alias="systems")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
```

### Comparing `spacetraders-0.6.0/spacetraders/models/create_ship_waypoint_scan_response_201.py` & `spacetraders-0.7.0/spacetraders/models/create_ship_waypoint_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py` & `spacetraders-0.7.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 T = TypeVar("T", bound="CreateShipWaypointScanResponse201Data")
 
 
 class CreateShipWaypointScanResponse201Data(BaseModel):
     """
     Attributes:
         cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
-        waypoints (List['ScannedWaypoint']):
+        waypoints (List['ScannedWaypoint']): List of scanned waypoints.
     """
 
     cooldown: "Cooldown" = Field(alias="cooldown")
     waypoints: List["ScannedWaypoint"] = Field(alias="waypoints")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
```

### Comparing `spacetraders-0.6.0/spacetraders/models/create_survey_response_201.py` & `spacetraders-0.7.0/spacetraders/models/create_survey_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/create_survey_response_201_data.py` & `spacetraders-0.7.0/spacetraders/models/create_survey_response_201_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 T = TypeVar("T", bound="CreateSurveyResponse201Data")
 
 
 class CreateSurveyResponse201Data(BaseModel):
     """
     Attributes:
         cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
-        surveys (List['Survey']):
+        surveys (List['Survey']): Surveys created by this action.
     """
 
     cooldown: "Cooldown" = Field(alias="cooldown")
     surveys: List["Survey"] = Field(alias="surveys")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
```

### Comparing `spacetraders-0.6.0/spacetraders/models/deliver_contract_json_body.py` & `spacetraders-0.7.0/spacetraders/models/jettison_json_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,28 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.trade_symbol import TradeSymbol
 from ..types import Unset
 
-T = TypeVar("T", bound="DeliverContractJsonBody")
+T = TypeVar("T", bound="JettisonJsonBody")
 
 
-class DeliverContractJsonBody(BaseModel):
+class JettisonJsonBody(BaseModel):
     """
     Attributes:
-        ship_symbol (str):
-        trade_symbol (str):
-        units (int):
+        symbol (TradeSymbol): The good's symbol.
+        units (int): Amount of units to jettison of this good.
     """
 
-    ship_symbol: str = Field(alias="shipSymbol")
-    trade_symbol: str = Field(alias="tradeSymbol")
+    symbol: TradeSymbol = Field(alias="symbol")
     units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/deliver_contract_response_200.py` & `spacetraders-0.7.0/spacetraders/models/deliver_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/deliver_contract_response_200_data.py` & `spacetraders-0.7.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,29 +4,26 @@
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..models.contract import Contract
-from ..models.ship_cargo import ShipCargo
 from ..types import Unset
 
-T = TypeVar("T", bound="DeliverContractResponse200Data")
+T = TypeVar("T", bound="NegotiateContractNegotiateContract200ResponseData")
 
 
-class DeliverContractResponse200Data(BaseModel):
+class NegotiateContractNegotiateContract200ResponseData(BaseModel):
     """
     Attributes:
-        contract (Contract):
-        cargo (ShipCargo):
+        contract (Contract): Contract details.
     """
 
     contract: "Contract" = Field(alias="contract")
-    cargo: "ShipCargo" = Field(alias="cargo")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/dock_ship_dock_ship_200_response.py` & `spacetraders-0.7.0/spacetraders/models/dock_ship_dock_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py` & `spacetraders-0.7.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/extract_resources_json_body.py` & `spacetraders-0.7.0/spacetraders/models/extract_resources_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/extract_resources_response_201.py` & `spacetraders-0.7.0/spacetraders/models/extract_resources_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/extract_resources_response_201_data.py` & `spacetraders-0.7.0/spacetraders/models/extract_resources_response_201_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 T = TypeVar("T", bound="ExtractResourcesResponse201Data")
 
 
 class ExtractResourcesResponse201Data(BaseModel):
     """
     Attributes:
         cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
-        extraction (Extraction):
-        cargo (ShipCargo):
+        extraction (Extraction): Extraction details.
+        cargo (ShipCargo): Ship cargo details.
     """
 
     cooldown: "Cooldown" = Field(alias="cooldown")
     extraction: "Extraction" = Field(alias="extraction")
     cargo: "ShipCargo" = Field(alias="cargo")
     additional_properties: Dict[str, Any] = {}
```

### Comparing `spacetraders-0.6.0/spacetraders/models/extraction.py` & `spacetraders-0.7.0/spacetraders/models/system_faction.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,29 +3,27 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.extraction_yield import ExtractionYield
+from ..models.faction_symbols import FactionSymbols
 from ..types import Unset
 
-T = TypeVar("T", bound="Extraction")
+T = TypeVar("T", bound="SystemFaction")
 
 
-class Extraction(BaseModel):
+class SystemFaction(BaseModel):
     """
     Attributes:
-        ship_symbol (str):
-        yield_ (ExtractionYield):
+        symbol (FactionSymbols): The symbol of the faction.
     """
 
-    ship_symbol: str = Field(alias="shipSymbol")
-    yield_: "ExtractionYield" = Field(alias="yield")
+    symbol: FactionSymbols = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/extraction_yield.py` & `spacetraders-0.7.0/spacetraders/models/extraction_yield.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,29 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.trade_symbol import TradeSymbol
 from ..types import Unset
 
 T = TypeVar("T", bound="ExtractionYield")
 
 
 class ExtractionYield(BaseModel):
-    """
+    """A yield from the extraction operation.
+
     Attributes:
-        symbol (str):
+        symbol (TradeSymbol): The good's symbol.
         units (int): The number of units extracted that were placed into the ship's cargo hold.
     """
 
-    symbol: str = Field(alias="symbol")
+    symbol: TradeSymbol = Field(alias="symbol")
     units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/faction.py` & `spacetraders-0.7.0/spacetraders/models/warp_ship_json_body.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,37 +3,26 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.faction_trait import FactionTrait
 from ..types import Unset
 
-T = TypeVar("T", bound="Faction")
+T = TypeVar("T", bound="WarpShipJsonBody")
 
 
-class Faction(BaseModel):
+class WarpShipJsonBody(BaseModel):
     """
     Attributes:
-        symbol (str):
-        name (str):
-        description (str):
-        headquarters (str):
-        traits (List['FactionTrait']):
-        is_recruiting (bool): Whether or not the faction is currently recruiting new agents.
+        waypoint_symbol (str): The target destination.
     """
 
-    symbol: str = Field(alias="symbol")
-    name: str = Field(alias="name")
-    description: str = Field(alias="description")
-    headquarters: str = Field(alias="headquarters")
-    traits: List["FactionTrait"] = Field(alias="traits")
-    is_recruiting: bool = Field(alias="isRecruiting")
+    waypoint_symbol: str = Field(alias="waypointSymbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/faction_trait.py` & `spacetraders-0.7.0/spacetraders/models/faction_trait.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/faction_trait_symbol.py` & `spacetraders-0.7.0/spacetraders/models/faction_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/fulfill_contract_response_200.py` & `spacetraders-0.7.0/spacetraders/models/fulfill_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/fulfill_contract_response_200_data.py` & `spacetraders-0.7.0/spacetraders/models/get_contracts_response_200.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,30 +3,30 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.agent import Agent
 from ..models.contract import Contract
+from ..models.meta import Meta
 from ..types import Unset
 
-T = TypeVar("T", bound="FulfillContractResponse200Data")
+T = TypeVar("T", bound="GetContractsResponse200")
 
 
-class FulfillContractResponse200Data(BaseModel):
+class GetContractsResponse200(BaseModel):
     """
     Attributes:
-        agent (Agent):
-        contract (Contract):
+        data (List['Contract']):
+        meta (Meta): Meta details for pagination.
     """
 
-    agent: "Agent" = Field(alias="agent")
-    contract: "Contract" = Field(alias="contract")
+    data: List["Contract"] = Field(alias="data")
+    meta: "Meta" = Field(alias="meta")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_contract_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_contract_response_200.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 T = TypeVar("T", bound="GetContractResponse200")
 
 
 class GetContractResponse200(BaseModel):
     """
     Attributes:
-        data (Contract):
+        data (Contract): Contract details.
     """
 
     data: "Contract" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_contracts_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_my_ships_response_200.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,29 +3,29 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.contract import Contract
 from ..models.meta import Meta
+from ..models.ship import Ship
 from ..types import Unset
 
-T = TypeVar("T", bound="GetContractsResponse200")
+T = TypeVar("T", bound="GetMyShipsResponse200")
 
 
-class GetContractsResponse200(BaseModel):
+class GetMyShipsResponse200(BaseModel):
     """
     Attributes:
-        data (List['Contract']):
-        meta (Meta):
+        data (List['Ship']):
+        meta (Meta): Meta details for pagination.
     """
 
-    data: List["Contract"] = Field(alias="data")
+    data: List["Ship"] = Field(alias="data")
     meta: "Meta" = Field(alias="meta")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_faction_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_factions_response_200.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,29 @@
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..models.faction import Faction
+from ..models.meta import Meta
 from ..types import Unset
 
-T = TypeVar("T", bound="GetFactionResponse200")
+T = TypeVar("T", bound="GetFactionsResponse200")
 
 
-class GetFactionResponse200(BaseModel):
+class GetFactionsResponse200(BaseModel):
     """
     Attributes:
-        data (Faction):
+        data (List['Faction']):
+        meta (Meta): Meta details for pagination.
     """
 
-    data: "Faction" = Field(alias="data")
+    data: List["Faction"] = Field(alias="data")
+    meta: "Meta" = Field(alias="meta")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_factions_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_systems_response_200.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,29 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.faction import Faction
 from ..models.meta import Meta
+from ..models.system import System
 from ..types import Unset
 
-T = TypeVar("T", bound="GetFactionsResponse200")
+T = TypeVar("T", bound="GetSystemsResponse200")
 
 
-class GetFactionsResponse200(BaseModel):
+class GetSystemsResponse200(BaseModel):
     """
     Attributes:
-        data (List['Faction']):
-        meta (Meta):
+        data (List['System']):
+        meta (Meta): Meta details for pagination.
     """
 
-    data: List["Faction"] = Field(alias="data")
+    data: List["System"] = Field(alias="data")
     meta: "Meta" = Field(alias="meta")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_jump_gate_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_jump_gate_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/get_market_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_market_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/get_mounts_get_mounts_200_response.py` & `spacetraders-0.7.0/spacetraders/models/get_mounts_get_mounts_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/get_my_agent_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_my_agent_response_200.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 T = TypeVar("T", bound="GetMyAgentResponse200")
 
 
 class GetMyAgentResponse200(BaseModel):
     """
     Attributes:
-        data (Agent):
+        data (Agent): Agent details.
     """
 
     data: "Agent" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_my_ship_cargo_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_my_ship_cargo_response_200.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 T = TypeVar("T", bound="GetMyShipCargoResponse200")
 
 
 class GetMyShipCargoResponse200(BaseModel):
     """
     Attributes:
-        data (ShipCargo):
+        data (ShipCargo): Ship cargo details.
     """
 
     data: "ShipCargo" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_my_ship_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_my_ship_response_200.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 T = TypeVar("T", bound="GetMyShipResponse200")
 
 
 class GetMyShipResponse200(BaseModel):
     """
     Attributes:
-        data (Ship): A ship
+        data (Ship): Ship details.
     """
 
     data: "Ship" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_my_ships_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_ship_nav_response_200.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,30 +3,27 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.meta import Meta
-from ..models.ship import Ship
+from ..models.ship_nav import ShipNav
 from ..types import Unset
 
-T = TypeVar("T", bound="GetMyShipsResponse200")
+T = TypeVar("T", bound="GetShipNavResponse200")
 
 
-class GetMyShipsResponse200(BaseModel):
+class GetShipNavResponse200(BaseModel):
     """
     Attributes:
-        data (List['Ship']):
-        meta (Meta):
+        data (ShipNav): The navigation information of the ship.
     """
 
-    data: List["Ship"] = Field(alias="data")
-    meta: "Meta" = Field(alias="meta")
+    data: "ShipNav" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_ship_cooldown_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_ship_cooldown_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/get_ship_nav_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_shipyard_response_200.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,27 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.ship_nav import ShipNav
+from ..models.shipyard import Shipyard
 from ..types import Unset
 
-T = TypeVar("T", bound="GetShipNavResponse200")
+T = TypeVar("T", bound="GetShipyardResponse200")
 
 
-class GetShipNavResponse200(BaseModel):
+class GetShipyardResponse200(BaseModel):
     """
     Attributes:
-        data (ShipNav): The navigation information of the ship.
+        data (Shipyard):
     """
 
-    data: "ShipNav" = Field(alias="data")
+    data: "Shipyard" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_shipyard_response_200.py` & `spacetraders-0.7.0/spacetraders/models/remove_mount_remove_mount_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,27 +3,26 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.shipyard import Shipyard
 from ..types import Unset
 
-T = TypeVar("T", bound="GetShipyardResponse200")
+T = TypeVar("T", bound="RemoveMountRemoveMountRequest")
 
 
-class GetShipyardResponse200(BaseModel):
+class RemoveMountRemoveMountRequest(BaseModel):
     """
     Attributes:
-        data (Shipyard):
+        symbol (str): The symbol of the mount to remove.
     """
 
-    data: "Shipyard" = Field(alias="data")
+    symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_status_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_status_response_200.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,19 @@
 from ..models.get_status_response_200_stats import GetStatusResponse200Stats
 from ..types import Unset
 
 T = TypeVar("T", bound="GetStatusResponse200")
 
 
 class GetStatusResponse200(BaseModel):
-    """OK
-
+    """
     Attributes:
         status (str): The current status of the game server.
         version (str): The current version of the API.
-        reset_date (str): The date and time when the game server was last reset.
+        reset_date (str): The date when the game server was last reset.
         description (str):
         stats (GetStatusResponse200Stats):
         leaderboards (GetStatusResponse200Leaderboards):
         server_resets (GetStatusResponse200ServerResets):
         announcements (List['GetStatusResponse200AnnouncementsItem']):
         links (List['GetStatusResponse200LinksItem']):
     """
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_status_response_200_announcements_item.py` & `spacetraders-0.7.0/spacetraders/models/get_status_response_200_announcements_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/get_status_response_200_leaderboards.py` & `spacetraders-0.7.0/spacetraders/models/get_status_response_200_leaderboards.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 
 T = TypeVar("T", bound="GetStatusResponse200Leaderboards")
 
 
 class GetStatusResponse200Leaderboards(BaseModel):
     """
     Attributes:
-        most_credits (List['GetStatusResponse200LeaderboardsMostCreditsItem']):
-        most_submitted_charts (List['GetStatusResponse200LeaderboardsMostSubmittedChartsItem']):
+        most_credits (List['GetStatusResponse200LeaderboardsMostCreditsItem']): Top agents with the most credits.
+        most_submitted_charts (List['GetStatusResponse200LeaderboardsMostSubmittedChartsItem']): Top agents with the
+            most charted submitted.
     """
 
     most_credits: List["GetStatusResponse200LeaderboardsMostCreditsItem"] = Field(
         alias="mostCredits"
     )
     most_submitted_charts: List[
         "GetStatusResponse200LeaderboardsMostSubmittedChartsItem"
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py` & `spacetraders-0.7.0/spacetraders/models/get_status_response_200_links_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,26 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="GetStatusResponse200LeaderboardsMostCreditsItem")
+T = TypeVar("T", bound="GetStatusResponse200LinksItem")
 
 
-class GetStatusResponse200LeaderboardsMostCreditsItem(BaseModel):
+class GetStatusResponse200LinksItem(BaseModel):
     """
     Attributes:
-        agent_symbol (str):
-        credits_ (int):
+        name (str):
+        url (str):
     """
 
-    agent_symbol: str = Field(alias="agentSymbol")
-    credits_: int = Field(alias="credits")
+    name: str = Field(alias="name")
+    url: str = Field(alias="url")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py` & `spacetraders-0.7.0/spacetraders/models/navigate_ship_json_body.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,26 +5,24 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="GetStatusResponse200LeaderboardsMostSubmittedChartsItem")
+T = TypeVar("T", bound="NavigateShipJsonBody")
 
 
-class GetStatusResponse200LeaderboardsMostSubmittedChartsItem(BaseModel):
+class NavigateShipJsonBody(BaseModel):
     """
     Attributes:
-        agent_symbol (str):
-        chart_count (int):
+        waypoint_symbol (str): The target destination.
     """
 
-    agent_symbol: str = Field(alias="agentSymbol")
-    chart_count: int = Field(alias="chartCount")
+    waypoint_symbol: str = Field(alias="waypointSymbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_status_response_200_links_item.py` & `spacetraders-0.7.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,26 +5,26 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="GetStatusResponse200LinksItem")
+T = TypeVar("T", bound="GetStatusResponse200LeaderboardsMostSubmittedChartsItem")
 
 
-class GetStatusResponse200LinksItem(BaseModel):
+class GetStatusResponse200LeaderboardsMostSubmittedChartsItem(BaseModel):
     """
     Attributes:
-        name (str):
-        url (str):
+        agent_symbol (str): Symbol of the agent.
+        chart_count (int): Amount of charts done by the agent.
     """
 
-    name: str = Field(alias="name")
-    url: str = Field(alias="url")
+    agent_symbol: str = Field(alias="agentSymbol")
+    chart_count: int = Field(alias="chartCount")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_status_response_200_server_resets.py` & `spacetraders-0.7.0/spacetraders/models/get_status_response_200_server_resets.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/get_status_response_200_stats.py` & `spacetraders-0.7.0/spacetraders/models/jump_ship_json_body.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,30 +5,24 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="GetStatusResponse200Stats")
+T = TypeVar("T", bound="JumpShipJsonBody")
 
 
-class GetStatusResponse200Stats(BaseModel):
+class JumpShipJsonBody(BaseModel):
     """
     Attributes:
-        agents (int):
-        ships (int):
-        systems (int):
-        waypoints (int):
+        system_symbol (str): The system symbol to jump to.
     """
 
-    agents: int = Field(alias="agents")
-    ships: int = Field(alias="ships")
-    systems: int = Field(alias="systems")
-    waypoints: int = Field(alias="waypoints")
+    system_symbol: str = Field(alias="systemSymbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_system_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_system_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/get_system_waypoints_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_system_waypoints_response_200.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 T = TypeVar("T", bound="GetSystemWaypointsResponse200")
 
 
 class GetSystemWaypointsResponse200(BaseModel):
     """
     Attributes:
         data (List['Waypoint']):
-        meta (Meta):
+        meta (Meta): Meta details for pagination.
     """
 
     data: List["Waypoint"] = Field(alias="data")
     meta: "Meta" = Field(alias="meta")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_systems_response_200.py` & `spacetraders-0.7.0/spacetraders/models/scanned_ship_engine.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,30 +3,27 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.meta import Meta
-from ..models.system import System
 from ..types import Unset
 
-T = TypeVar("T", bound="GetSystemsResponse200")
+T = TypeVar("T", bound="ScannedShipEngine")
 
 
-class GetSystemsResponse200(BaseModel):
-    """
+class ScannedShipEngine(BaseModel):
+    """The engine of the ship.
+
     Attributes:
-        data (List['System']):
-        meta (Meta):
+        symbol (str): The symbol of the engine.
     """
 
-    data: List["System"] = Field(alias="data")
-    meta: "Meta" = Field(alias="meta")
+    symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/get_waypoint_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_waypoint_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/install_mount_install_mount_201_response.py` & `spacetraders-0.7.0/spacetraders/models/install_mount_install_mount_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/install_mount_install_mount_201_response_data.py` & `spacetraders-0.7.0/spacetraders/models/install_mount_install_mount_201_response_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,39 +4,36 @@
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..models.agent import Agent
-from ..models.install_mount_install_mount_201_response_data_transaction import (
-    InstallMountInstallMount201ResponseDataTransaction,
-)
 from ..models.ship_cargo import ShipCargo
+from ..models.ship_modification_transaction import ShipModificationTransaction
 from ..models.ship_mount import ShipMount
 from ..types import Unset
 
 T = TypeVar("T", bound="InstallMountInstallMount201ResponseData")
 
 
 class InstallMountInstallMount201ResponseData(BaseModel):
     """
     Attributes:
-        agent (Agent):
-        mounts (List['ShipMount']):
-        cargo (ShipCargo):
-        transaction (InstallMountInstallMount201ResponseDataTransaction):
+        agent (Agent): Agent details.
+        mounts (List['ShipMount']): List of installed mounts after the installation of the new mount.
+        cargo (ShipCargo): Ship cargo details.
+        transaction (ShipModificationTransaction): Result of a transaction for a ship modification, such as installing a
+            mount or a module.
     """
 
     agent: "Agent" = Field(alias="agent")
     mounts: List["ShipMount"] = Field(alias="mounts")
     cargo: "ShipCargo" = Field(alias="cargo")
-    transaction: "InstallMountInstallMount201ResponseDataTransaction" = Field(
-        alias="transaction"
-    )
+    transaction: "ShipModificationTransaction" = Field(alias="transaction")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/install_mount_install_mount_201_response_data_transaction.py` & `spacetraders-0.7.0/spacetraders/models/system_waypoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-import datetime
 from typing import (
     Any,
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.waypoint_type import WaypointType
 from ..types import Unset
 
-T = TypeVar("T", bound="InstallMountInstallMount201ResponseDataTransaction")
+T = TypeVar("T", bound="SystemWaypoint")
 
 
-class InstallMountInstallMount201ResponseDataTransaction(BaseModel):
+class SystemWaypoint(BaseModel):
     """
     Attributes:
-        total_price (int): The total price of the transaction.
-        timestamp (datetime.datetime): The timestamp of the transaction.
+        symbol (str): The symbol of the waypoint.
+        type (WaypointType): The type of waypoint.
+        x (int): Position in the universe in the x axis.
+        y (int): Position in the universe in the y axis.
     """
 
-    total_price: int = Field(alias="totalPrice")
-    timestamp: datetime.datetime = Field(alias="timestamp")
+    symbol: str = Field(alias="symbol")
+    type: WaypointType = Field(alias="type")
+    x: int = Field(alias="x")
+    y: int = Field(alias="y")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/install_mount_install_mount_request.py` & `spacetraders-0.7.0/spacetraders/models/install_mount_install_mount_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/jettison_json_body.py` & `spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response_data_consumed_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,25 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="JettisonJsonBody")
+T = TypeVar("T", bound="ShipRefineShipRefine201ResponseDataConsumedItem")
 
 
-class JettisonJsonBody(BaseModel):
+class ShipRefineShipRefine201ResponseDataConsumedItem(BaseModel):
     """
     Attributes:
-        symbol (str):
-        units (int):
+        trade_symbol (str): Symbol of the good.
+        units (int): Amount of units of the good.
     """
 
-    symbol: str = Field(alias="symbol")
+    trade_symbol: str = Field(alias="tradeSymbol")
     units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/jettison_response_200.py` & `spacetraders-0.7.0/spacetraders/models/jettison_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/jettison_response_200_data.py` & `spacetraders-0.7.0/spacetraders/models/jettison_response_200_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 T = TypeVar("T", bound="JettisonResponse200Data")
 
 
 class JettisonResponse200Data(BaseModel):
     """
     Attributes:
-        cargo (ShipCargo):
+        cargo (ShipCargo): Ship cargo details.
     """
 
     cargo: "ShipCargo" = Field(alias="cargo")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/jump_gate.py` & `spacetraders-0.7.0/spacetraders/models/jump_gate.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/jump_ship_json_body.py` & `spacetraders-0.7.0/spacetraders/models/scanned_ship_reactor.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,24 +5,25 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="JumpShipJsonBody")
+T = TypeVar("T", bound="ScannedShipReactor")
 
 
-class JumpShipJsonBody(BaseModel):
-    """
+class ScannedShipReactor(BaseModel):
+    """The reactor of the ship.
+
     Attributes:
-        system_symbol (str): The system symbol to jump to.
+        symbol (str): The symbol of the reactor.
     """
 
-    system_symbol: str = Field(alias="systemSymbol")
+    symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/jump_ship_response_200.py` & `spacetraders-0.7.0/spacetraders/models/jump_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/jump_ship_response_200_data.py` & `spacetraders-0.7.0/spacetraders/models/jump_ship_response_200_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from typing import (
     Any,
     Dict,
     List,
     TypeVar,
-    Union,
 )
 
 from pydantic import BaseModel, Field
 
 from ..models.cooldown import Cooldown
 from ..models.ship_nav import ShipNav
-from ..types import UNSET, Unset
+from ..types import Unset
 
 T = TypeVar("T", bound="JumpShipResponse200Data")
 
 
 class JumpShipResponse200Data(BaseModel):
     """
     Attributes:
         cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
-        nav (Union[Unset, ShipNav]): The navigation information of the ship.
+        nav (ShipNav): The navigation information of the ship.
     """
 
     cooldown: "Cooldown" = Field(alias="cooldown")
-    nav: Union[Unset, "ShipNav"] = Field(UNSET, alias="nav")
+    nav: "ShipNav" = Field(alias="nav")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/market.py` & `spacetraders-0.7.0/spacetraders/models/market.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/market_trade_good.py` & `spacetraders-0.7.0/spacetraders/models/market_trade_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/market_transaction.py` & `spacetraders-0.7.0/spacetraders/models/market_transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from ..models.market_transaction_type import MarketTransactionType
 from ..types import Unset
 
 T = TypeVar("T", bound="MarketTransaction")
 
 
 class MarketTransaction(BaseModel):
-    """
+    """Result of a transaction with a market.
+
     Attributes:
         waypoint_symbol (str): The symbol of the waypoint where the transaction took place.
         ship_symbol (str): The symbol of the ship that made the transaction.
         trade_symbol (str): The symbol of the trade good.
         type (MarketTransactionType): The type of transaction.
         units (int): The number of units of the transaction.
         price_per_unit (int): The price per unit of the transaction.
```

### Comparing `spacetraders-0.6.0/spacetraders/models/meta.py` & `spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response_data_produced_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,26 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="Meta")
+T = TypeVar("T", bound="ShipRefineShipRefine201ResponseDataProducedItem")
 
 
-class Meta(BaseModel):
+class ShipRefineShipRefine201ResponseDataProducedItem(BaseModel):
     """
     Attributes:
-        total (int):
-        page (int):
-        limit (int):
+        trade_symbol (str): Symbol of the good.
+        units (int): Amount of units of the good.
     """
 
-    total: int = Field(alias="total")
-    page: int = Field(alias="page")
-    limit: int = Field(alias="limit")
+    trade_symbol: str = Field(alias="tradeSymbol")
+    units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/navigate_ship_json_body.py` & `spacetraders-0.7.0/spacetraders/models/scanned_ship_mounts_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,24 +5,25 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="NavigateShipJsonBody")
+T = TypeVar("T", bound="ScannedShipMountsItem")
 
 
-class NavigateShipJsonBody(BaseModel):
-    """
+class ScannedShipMountsItem(BaseModel):
+    """A mount on the ship.
+
     Attributes:
-        waypoint_symbol (str): The target destination.
+        symbol (str): The symbol of the mount.
     """
 
-    waypoint_symbol: str = Field(alias="waypointSymbol")
+    symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/navigate_ship_response_200.py` & `spacetraders-0.7.0/spacetraders/models/navigate_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/navigate_ship_response_200_data.py` & `spacetraders-0.7.0/spacetraders/models/navigate_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py` & `spacetraders-0.7.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py` & `spacetraders-0.7.0/spacetraders/models/register_response_201_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,27 +3,38 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.agent import Agent
 from ..models.contract import Contract
+from ..models.faction import Faction
+from ..models.ship import Ship
 from ..types import Unset
 
-T = TypeVar("T", bound="NegotiateContractNegotiateContract200ResponseData")
+T = TypeVar("T", bound="RegisterResponse201Data")
 
 
-class NegotiateContractNegotiateContract200ResponseData(BaseModel):
+class RegisterResponse201Data(BaseModel):
     """
     Attributes:
-        contract (Contract):
+        agent (Agent): Agent details.
+        contract (Contract): Contract details.
+        faction (Faction): Faction details.
+        ship (Ship): Ship details.
+        token (str): A Bearer token for accessing secured API endpoints.
     """
 
+    agent: "Agent" = Field(alias="agent")
     contract: "Contract" = Field(alias="contract")
+    faction: "Faction" = Field(alias="faction")
+    ship: "Ship" = Field(alias="ship")
+    token: str = Field(alias="token")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py` & `spacetraders-0.7.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py` & `spacetraders-0.7.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/patch_ship_nav_json_body.py` & `spacetraders-0.7.0/spacetraders/models/patch_ship_nav_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/patch_ship_nav_response_200.py` & `spacetraders-0.7.0/spacetraders/models/patch_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py` & `spacetraders-0.7.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py` & `spacetraders-0.7.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 T = TypeVar("T", bound="PurchaseCargoPurchaseCargo201ResponseData")
 
 
 class PurchaseCargoPurchaseCargo201ResponseData(BaseModel):
     """
     Attributes:
-        agent (Agent):
-        cargo (ShipCargo):
-        transaction (MarketTransaction):
+        agent (Agent): Agent details.
+        cargo (ShipCargo): Ship cargo details.
+        transaction (MarketTransaction): Result of a transaction with a market.
     """
 
     agent: "Agent" = Field(alias="agent")
     cargo: "ShipCargo" = Field(alias="cargo")
     transaction: "MarketTransaction" = Field(alias="transaction")
     additional_properties: Dict[str, Any] = {}
```

### Comparing `spacetraders-0.6.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py` & `spacetraders-0.7.0/spacetraders/models/deliver_contract_json_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,28 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="PurchaseCargoPurchaseCargoRequest")
+T = TypeVar("T", bound="DeliverContractJsonBody")
 
 
-class PurchaseCargoPurchaseCargoRequest(BaseModel):
+class DeliverContractJsonBody(BaseModel):
     """
     Attributes:
-        symbol (str):
-        units (int):
+        ship_symbol (str): Symbol of a ship located in the destination to deliver a contract and that has a good to
+            deliver in its cargo.
+        trade_symbol (str): The symbol of the good to deliver.
+        units (int): Amount of units to deliver.
     """
 
-    symbol: str = Field(alias="symbol")
+    ship_symbol: str = Field(alias="shipSymbol")
+    trade_symbol: str = Field(alias="tradeSymbol")
     units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/purchase_ship_json_body.py` & `spacetraders-0.7.0/spacetraders/models/purchase_ship_json_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 T = TypeVar("T", bound="PurchaseShipJsonBody")
 
 
 class PurchaseShipJsonBody(BaseModel):
     """
     Attributes:
-        ship_type (ShipType):
+        ship_type (ShipType): Type of ship
         waypoint_symbol (str): The symbol of the waypoint you want to purchase the ship at.
     """
 
     ship_type: ShipType = Field(alias="shipType")
     waypoint_symbol: str = Field(alias="waypointSymbol")
     additional_properties: Dict[str, Any] = {}
```

### Comparing `spacetraders-0.6.0/spacetraders/models/purchase_ship_response_201.py` & `spacetraders-0.7.0/spacetraders/models/purchase_ship_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/purchase_ship_response_201_data.py` & `spacetraders-0.7.0/spacetraders/models/purchase_ship_response_201_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 T = TypeVar("T", bound="PurchaseShipResponse201Data")
 
 
 class PurchaseShipResponse201Data(BaseModel):
     """
     Attributes:
-        agent (Agent):
-        ship (Ship): A ship
-        transaction (ShipyardTransaction):
+        agent (Agent): Agent details.
+        ship (Ship): Ship details.
+        transaction (ShipyardTransaction): Results of a transaction with a shipyard.
     """
 
     agent: "Agent" = Field(alias="agent")
     ship: "Ship" = Field(alias="ship")
     transaction: "ShipyardTransaction" = Field(alias="transaction")
     additional_properties: Dict[str, Any] = {}
```

### Comparing `spacetraders-0.6.0/spacetraders/models/refuel_ship_response_200.py` & `spacetraders-0.7.0/spacetraders/models/refuel_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/refuel_ship_response_200_data.py` & `spacetraders-0.7.0/spacetraders/models/refuel_ship_response_200_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 T = TypeVar("T", bound="RefuelShipResponse200Data")
 
 
 class RefuelShipResponse200Data(BaseModel):
     """
     Attributes:
-        agent (Agent):
+        agent (Agent): Agent details.
         fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
             or action.
-        transaction (MarketTransaction):
+        transaction (MarketTransaction): Result of a transaction with a market.
     """
 
     agent: "Agent" = Field(alias="agent")
     fuel: "ShipFuel" = Field(alias="fuel")
     transaction: "MarketTransaction" = Field(alias="transaction")
     additional_properties: Dict[str, Any] = {}
```

### Comparing `spacetraders-0.6.0/spacetraders/models/register_json_body.py` & `spacetraders-0.7.0/spacetraders/models/refuel_ship_json_body.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,28 +6,27 @@
     Union,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RegisterJsonBody")
+T = TypeVar("T", bound="RefuelShipJsonBody")
 
 
-class RegisterJsonBody(BaseModel):
+class RefuelShipJsonBody(BaseModel):
     """
     Attributes:
-        faction (Any): The faction you choose determines your headquarters. Example: COSMIC.
-        symbol (str): How other agents will see your ships and information. Example: BADGER.
-        email (Union[Unset, str]): Your email address. This is used if you reserved your call sign between resets.
+        units (Union[Unset, int]): The amount of fuel to fill in the ship's tanks. When not specified, the ship will be
+            refueled to its maximum fuel capacity. If the amount specified is greater than the ship's remaining capacity,
+            the ship will only be refueled to its maximum fuel capacity. The amount specified is not in market units but in
+            ship fuel units. Example: 100.
     """
 
-    faction: Any = Field(alias="faction")
-    symbol: str = Field(alias="symbol")
-    email: Union[Unset, str] = Field(UNSET, alias="email")
+    units: Union[Unset, int] = Field(UNSET, alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/register_response_201.py` & `spacetraders-0.7.0/spacetraders/models/register_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/register_response_201_data.py` & `spacetraders-0.7.0/spacetraders/models/fulfill_contract_response_200_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,36 +5,28 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..models.agent import Agent
 from ..models.contract import Contract
-from ..models.faction import Faction
-from ..models.ship import Ship
 from ..types import Unset
 
-T = TypeVar("T", bound="RegisterResponse201Data")
+T = TypeVar("T", bound="FulfillContractResponse200Data")
 
 
-class RegisterResponse201Data(BaseModel):
+class FulfillContractResponse200Data(BaseModel):
     """
     Attributes:
-        agent (Agent):
-        contract (Contract):
-        faction (Faction):
-        ship (Ship): A ship
-        token (str): A Bearer token for accessing secured API endpoints.
+        agent (Agent): Agent details.
+        contract (Contract): Contract details.
     """
 
     agent: "Agent" = Field(alias="agent")
     contract: "Contract" = Field(alias="contract")
-    faction: "Faction" = Field(alias="faction")
-    ship: "Ship" = Field(alias="ship")
-    token: str = Field(alias="token")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/remove_mount_remove_mount_201_response.py` & `spacetraders-0.7.0/spacetraders/models/remove_mount_remove_mount_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/remove_mount_remove_mount_201_response_data.py` & `spacetraders-0.7.0/spacetraders/models/remove_mount_remove_mount_201_response_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,39 +4,36 @@
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..models.agent import Agent
-from ..models.remove_mount_remove_mount_201_response_data_transaction import (
-    RemoveMountRemoveMount201ResponseDataTransaction,
-)
 from ..models.ship_cargo import ShipCargo
+from ..models.ship_modification_transaction import ShipModificationTransaction
 from ..models.ship_mount import ShipMount
 from ..types import Unset
 
 T = TypeVar("T", bound="RemoveMountRemoveMount201ResponseData")
 
 
 class RemoveMountRemoveMount201ResponseData(BaseModel):
     """
     Attributes:
-        agent (Agent):
-        mounts (List['ShipMount']):
-        cargo (ShipCargo):
-        transaction (RemoveMountRemoveMount201ResponseDataTransaction):
+        agent (Agent): Agent details.
+        mounts (List['ShipMount']): List of installed mounts after the removal of the selected mount.
+        cargo (ShipCargo): Ship cargo details.
+        transaction (ShipModificationTransaction): Result of a transaction for a ship modification, such as installing a
+            mount or a module.
     """
 
     agent: "Agent" = Field(alias="agent")
     mounts: List["ShipMount"] = Field(alias="mounts")
     cargo: "ShipCargo" = Field(alias="cargo")
-    transaction: "RemoveMountRemoveMount201ResponseDataTransaction" = Field(
-        alias="transaction"
-    )
+    transaction: "ShipModificationTransaction" = Field(alias="transaction")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/remove_mount_remove_mount_201_response_data_transaction.py` & `spacetraders-0.7.0/spacetraders/models/shipyard_transaction.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,25 +6,32 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="RemoveMountRemoveMount201ResponseDataTransaction")
+T = TypeVar("T", bound="ShipyardTransaction")
 
 
-class RemoveMountRemoveMount201ResponseDataTransaction(BaseModel):
-    """
+class ShipyardTransaction(BaseModel):
+    """Results of a transaction with a shipyard.
+
     Attributes:
-        total_price (int): The total price of the transaction.
+        waypoint_symbol (str): The symbol of the waypoint where the transaction took place.
+        ship_symbol (str): The symbol of the ship that was the subject of the transaction.
+        price (int): The price of the transaction.
+        agent_symbol (str): The symbol of the agent that made the transaction.
         timestamp (datetime.datetime): The timestamp of the transaction.
     """
 
-    total_price: int = Field(alias="totalPrice")
+    waypoint_symbol: str = Field(alias="waypointSymbol")
+    ship_symbol: str = Field(alias="shipSymbol")
+    price: int = Field(alias="price")
+    agent_symbol: str = Field(alias="agentSymbol")
     timestamp: datetime.datetime = Field(alias="timestamp")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/remove_mount_remove_mount_request.py` & `spacetraders-0.7.0/spacetraders/models/scanned_ship_frame.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,22 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="RemoveMountRemoveMountRequest")
+T = TypeVar("T", bound="ScannedShipFrame")
 
 
-class RemoveMountRemoveMountRequest(BaseModel):
-    """
+class ScannedShipFrame(BaseModel):
+    """The frame of the ship.
+
     Attributes:
-        symbol (str):
+        symbol (str): The symbol of the frame.
     """
 
     symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/scanned_ship.py` & `spacetraders-0.7.0/spacetraders/models/scanned_ship.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Attributes:
         symbol (str): The globally unique identifier of the ship.
         registration (ShipRegistration): The public registration information of the ship
         nav (ShipNav): The navigation information of the ship.
         engine (ScannedShipEngine): The engine of the ship.
         frame (Union[Unset, ScannedShipFrame]): The frame of the ship.
         reactor (Union[Unset, ScannedShipReactor]): The reactor of the ship.
-        mounts (Union[Unset, List['ScannedShipMountsItem']]):
+        mounts (Union[Unset, List['ScannedShipMountsItem']]): List of mounts installed in the ship.
     """
 
     symbol: str = Field(alias="symbol")
     registration: "ShipRegistration" = Field(alias="registration")
     nav: "ShipNav" = Field(alias="nav")
     engine: "ScannedShipEngine" = Field(alias="engine")
     frame: Union[Unset, "ScannedShipFrame"] = Field(UNSET, alias="frame")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/scanned_ship_engine.py` & `spacetraders-0.7.0/spacetraders/models/waypoint_faction.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,28 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.faction_symbols import FactionSymbols
 from ..types import Unset
 
-T = TypeVar("T", bound="ScannedShipEngine")
+T = TypeVar("T", bound="WaypointFaction")
 
 
-class ScannedShipEngine(BaseModel):
-    """The engine of the ship.
+class WaypointFaction(BaseModel):
+    """The faction that controls the waypoint.
 
     Attributes:
-        symbol (str):
+        symbol (FactionSymbols): The symbol of the faction.
     """
 
-    symbol: str = Field(alias="symbol")
+    symbol: FactionSymbols = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/scanned_ship_frame.py` & `spacetraders-0.7.0/spacetraders/models/get_faction_response_200.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,27 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.faction import Faction
 from ..types import Unset
 
-T = TypeVar("T", bound="ScannedShipFrame")
+T = TypeVar("T", bound="GetFactionResponse200")
 
 
-class ScannedShipFrame(BaseModel):
-    """The frame of the ship.
-
+class GetFactionResponse200(BaseModel):
+    """
     Attributes:
-        symbol (str):
+        data (Faction): Faction details.
     """
 
-    symbol: str = Field(alias="symbol")
+    data: "Faction" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/scanned_ship_mounts_item.py` & `spacetraders-0.7.0/spacetraders/models/ship_refine_json_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,27 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.ship_refine_json_body_produce import ShipRefineJsonBodyProduce
 from ..types import Unset
 
-T = TypeVar("T", bound="ScannedShipMountsItem")
+T = TypeVar("T", bound="ShipRefineJsonBody")
 
 
-class ScannedShipMountsItem(BaseModel):
-    """A mount on the ship.
-
+class ShipRefineJsonBody(BaseModel):
+    """
     Attributes:
-        symbol (str):
+        produce (ShipRefineJsonBodyProduce): The type of good to produce out of the refining process.
     """
 
-    symbol: str = Field(alias="symbol")
+    produce: ShipRefineJsonBodyProduce = Field(alias="produce")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/scanned_ship_reactor.py` & `spacetraders-0.7.0/spacetraders/models/survey_deposit.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,22 +5,22 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="ScannedShipReactor")
+T = TypeVar("T", bound="SurveyDeposit")
 
 
-class ScannedShipReactor(BaseModel):
-    """The reactor of the ship.
+class SurveyDeposit(BaseModel):
+    """A surveyed deposit of a mineral or resource available for extraction.
 
     Attributes:
-        symbol (str):
+        symbol (str): The symbol of the deposit.
     """
 
     symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/scanned_system.py` & `spacetraders-0.7.0/spacetraders/models/scanned_system.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 from ..models.system_type import SystemType
 from ..types import Unset
 
 T = TypeVar("T", bound="ScannedSystem")
 
 
 class ScannedSystem(BaseModel):
-    """
+    """Details of a system was that scanned.
+
     Attributes:
-        symbol (str):
-        sector_symbol (str):
+        symbol (str): Symbol of the system.
+        sector_symbol (str): Symbol of the system's sector.
         type (SystemType): The type of waypoint.
-        x (int):
-        y (int):
-        distance (int):
+        x (int): Position in the universe in the x axis.
+        y (int): Position in the universe in the y axis.
+        distance (int): The system's distance from the scanning ship.
     """
 
     symbol: str = Field(alias="symbol")
     sector_symbol: str = Field(alias="sectorSymbol")
     type: SystemType = Field(alias="type")
     x: int = Field(alias="x")
     y: int = Field(alias="y")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/scanned_waypoint.py` & `spacetraders-0.7.0/spacetraders/models/waypoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 from ..models.chart import Chart
 from ..models.waypoint_faction import WaypointFaction
 from ..models.waypoint_orbital import WaypointOrbital
 from ..models.waypoint_trait import WaypointTrait
 from ..models.waypoint_type import WaypointType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ScannedWaypoint")
+T = TypeVar("T", bound="Waypoint")
 
 
-class ScannedWaypoint(BaseModel):
+class Waypoint(BaseModel):
     """A waypoint is a location that ships can travel to such as a Planet, Moon or Space Station.
 
     Attributes:
-        symbol (str):
+        symbol (str): Symbol fo the waypoint.
         type (WaypointType): The type of waypoint.
-        system_symbol (str):
-        x (int):
-        y (int):
-        orbitals (List['WaypointOrbital']):
+        system_symbol (str): The symbol of the system this waypoint belongs to.
+        x (int): Position in the universe in the x axis.
+        y (int): Position in the universe in the Y axis.
+        orbitals (List['WaypointOrbital']): Waypoints that orbit this waypoint.
         traits (List['WaypointTrait']): The traits of the waypoint.
-        faction (Union[Unset, WaypointFaction]):
+        faction (Union[Unset, WaypointFaction]): The faction that controls the waypoint.
         chart (Union[Unset, Chart]): The chart of a system or waypoint, which makes the location visible to other
             agents.
     """
 
     symbol: str = Field(alias="symbol")
     type: WaypointType = Field(alias="type")
     system_symbol: str = Field(alias="systemSymbol")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py` & `spacetraders-0.7.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py` & `spacetraders-0.7.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 T = TypeVar("T", bound="SellCargoSellCargo201ResponseData")
 
 
 class SellCargoSellCargo201ResponseData(BaseModel):
     """
     Attributes:
-        agent (Agent):
-        cargo (ShipCargo):
-        transaction (MarketTransaction):
+        agent (Agent): Agent details.
+        cargo (ShipCargo): Ship cargo details.
+        transaction (MarketTransaction): Result of a transaction with a market.
     """
 
     agent: "Agent" = Field(alias="agent")
     cargo: "ShipCargo" = Field(alias="cargo")
     transaction: "MarketTransaction" = Field(alias="transaction")
     additional_properties: Dict[str, Any] = {}
```

### Comparing `spacetraders-0.6.0/spacetraders/models/sell_cargo_sell_cargo_request.py` & `spacetraders-0.7.0/spacetraders/models/deliver_contract_response_200_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,28 +3,30 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.contract import Contract
+from ..models.ship_cargo import ShipCargo
 from ..types import Unset
 
-T = TypeVar("T", bound="SellCargoSellCargoRequest")
+T = TypeVar("T", bound="DeliverContractResponse200Data")
 
 
-class SellCargoSellCargoRequest(BaseModel):
+class DeliverContractResponse200Data(BaseModel):
     """
     Attributes:
-        symbol (str):
-        units (int):
+        contract (Contract): Contract details.
+        cargo (ShipCargo): Ship cargo details.
     """
 
-    symbol: str = Field(alias="symbol")
-    units: int = Field(alias="units")
+    contract: "Contract" = Field(alias="contract")
+    cargo: "ShipCargo" = Field(alias="cargo")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship.py` & `spacetraders-0.7.0/spacetraders/models/ship.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 from ..models.ship_registration import ShipRegistration
 from ..types import Unset
 
 T = TypeVar("T", bound="Ship")
 
 
 class Ship(BaseModel):
-    """A ship
+    """Ship details.
 
     Attributes:
-        symbol (str): The globally unique identifier of the ship in the following format: `[AGENT_SYMBOL]_[HEX_ID]`
+        symbol (str): The globally unique identifier of the ship in the following format: `[AGENT_SYMBOL]-[HEX_ID]`
         registration (ShipRegistration): The public registration information of the ship
         nav (ShipNav): The navigation information of the ship.
         crew (ShipCrew): The ship's crew service and maintain the ship's systems and equipment.
         frame (ShipFrame): The frame of the ship. The frame determines the number of modules and mounting points of the
             ship, as well as base fuel capacity. As the condition of the frame takes more wear, the ship will become more
             sluggish and less maneuverable.
         reactor (ShipReactor): The reactor of the ship. The reactor is responsible for powering the ship's systems and
             weapons.
         engine (ShipEngine): The engine determines how quickly a ship travels between waypoints.
-        modules (List['ShipModule']):
-        mounts (List['ShipMount']):
-        cargo (ShipCargo):
+        modules (List['ShipModule']): Modules installed in this ship.
+        mounts (List['ShipMount']): Mounts installed in this ship.
+        cargo (ShipCargo): Ship cargo details.
         fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
             or action.
     """
 
     symbol: str = Field(alias="symbol")
     registration: "ShipRegistration" = Field(alias="registration")
     nav: "ShipNav" = Field(alias="nav")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_cargo.py` & `spacetraders-0.7.0/spacetraders/models/ship_cargo.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from ..models.ship_cargo_item import ShipCargoItem
 from ..types import Unset
 
 T = TypeVar("T", bound="ShipCargo")
 
 
 class ShipCargo(BaseModel):
-    """
+    """Ship cargo details.
+
     Attributes:
         capacity (int): The max number of items that can be stored in the cargo hold.
         units (int): The number of items currently stored in the cargo hold.
         inventory (List['ShipCargoItem']): The items currently in the cargo hold.
     """
 
     capacity: int = Field(alias="capacity")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_cargo_item.py` & `spacetraders-0.7.0/spacetraders/models/ship_cargo_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_crew.py` & `spacetraders-0.7.0/spacetraders/models/ship_crew.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_engine.py` & `spacetraders-0.7.0/spacetraders/models/ship_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 T = TypeVar("T", bound="ShipEngine")
 
 
 class ShipEngine(BaseModel):
     """The engine determines how quickly a ship travels between waypoints.
 
     Attributes:
-        symbol (ShipEngineSymbol):
-        name (str):
-        description (str):
-        speed (int):
+        symbol (ShipEngineSymbol): The symbol of the engine.
+        name (str): The name of the engine.
+        description (str): The description of the engine.
+        speed (int): The speed stat of this engine. The higher the speed, the faster a ship can travel from one point to
+            another. Reduces the time of arrival when navigating the ship.
         requirements (ShipRequirements): The requirements for installation on a ship
         condition (Union[Unset, int]): Condition is a range of 0 to 100 where 0 is completely worn out and 100 is brand
             new.
     """
 
     symbol: ShipEngineSymbol = Field(alias="symbol")
     name: str = Field(alias="name")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_frame.py` & `spacetraders-0.7.0/spacetraders/models/ship_frame.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,23 @@
 
 class ShipFrame(BaseModel):
     """The frame of the ship. The frame determines the number of modules and mounting points of the ship, as well as base
     fuel capacity. As the condition of the frame takes more wear, the ship will become more sluggish and less
     maneuverable.
 
         Attributes:
-            symbol (ShipFrameSymbol):
-            name (str):
-            description (str):
-            module_slots (int):
-            mounting_points (int):
-            fuel_capacity (int):
+            symbol (ShipFrameSymbol): Symbol of the frame.
+            name (str): Name of the frame.
+            description (str): Description of the frame.
+            module_slots (int): The amount of slots that can be dedicated to modules installed in the ship. Each installed
+                module take up a number of slots, and once there are no more slots, no new modules can be installed.
+            mounting_points (int): The amount of slots that can be dedicated to mounts installed in the ship. Each installed
+                mount takes up a number of points, and once there are no more points remaining, no new mounts can be installed.
+            fuel_capacity (int): The maximum amount of fuel that can be stored in this ship. When refueling, the ship will
+                be refueled to this amount.
             requirements (ShipRequirements): The requirements for installation on a ship
             condition (Union[Unset, int]): Condition is a range of 0 to 100 where 0 is completely worn out and 100 is brand
                 new.
     """
 
     symbol: ShipFrameSymbol = Field(alias="symbol")
     name: str = Field(alias="name")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_frame_symbol.py` & `spacetraders-0.7.0/spacetraders/models/ship_frame_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_fuel.py` & `spacetraders-0.7.0/spacetraders/models/ship_fuel.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 class ShipFuel(BaseModel):
     """Details of the ship's fuel tanks including how much fuel was consumed during the last transit or action.
 
     Attributes:
         current (int): The current amount of fuel in the ship's tanks.
         capacity (int): The maximum amount of fuel the ship's tanks can hold.
-        consumed (Union[Unset, ShipFuelConsumed]):
+        consumed (Union[Unset, ShipFuelConsumed]): An object that only shows up when an action has consumed fuel in the
+            process. Shows the fuel consumption data.
     """
 
     current: int = Field(alias="current")
     capacity: int = Field(alias="capacity")
     consumed: Union[Unset, "ShipFuelConsumed"] = Field(UNSET, alias="consumed")
     additional_properties: Dict[str, Any] = {}
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_fuel_consumed.py` & `spacetraders-0.7.0/spacetraders/models/ship_fuel_consumed.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 from ..types import Unset
 
 T = TypeVar("T", bound="ShipFuelConsumed")
 
 
 class ShipFuelConsumed(BaseModel):
-    """
+    """An object that only shows up when an action has consumed fuel in the process. Shows the fuel consumption data.
+
     Attributes:
         amount (int): The amount of fuel consumed by the most recent transit or action.
         timestamp (datetime.datetime): The time at which the fuel was consumed.
     """
 
     amount: int = Field(alias="amount")
     timestamp: datetime.datetime = Field(alias="timestamp")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_module.py` & `spacetraders-0.7.0/spacetraders/models/ship_module.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 
 
 class ShipModule(BaseModel):
     """A module can be installed in a ship and provides a set of capabilities such as storage space or quarters for crew.
     Module installations are permanent.
 
         Attributes:
-            symbol (ShipModuleSymbol):
-            name (str):
+            symbol (ShipModuleSymbol): The symbol of the module.
+            name (str): Name of this module.
+            description (str): Description of this module.
             requirements (ShipRequirements): The requirements for installation on a ship
-            capacity (Union[Unset, int]):
-            range_ (Union[Unset, int]):
-            description (Union[Unset, str]):
+            capacity (Union[Unset, int]): Modules that provide capacity, such as cargo hold or crew quarters will show this
+                value to denote how much of a bonus the module grants.
+            range_ (Union[Unset, int]): Modules that have a range will such as a sensor array show this value to denote how
+                far can the module reach with its capabilities.
     """
 
     symbol: ShipModuleSymbol = Field(alias="symbol")
     name: str = Field(alias="name")
+    description: str = Field(alias="description")
     requirements: "ShipRequirements" = Field(alias="requirements")
     capacity: Union[Unset, int] = Field(UNSET, alias="capacity")
     range_: Union[Unset, int] = Field(UNSET, alias="range")
-    description: Union[Unset, str] = Field(UNSET, alias="description")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_module_symbol.py` & `spacetraders-0.7.0/spacetraders/models/ship_module_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_mount.py` & `spacetraders-0.7.0/spacetraders/models/ship_mount.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 T = TypeVar("T", bound="ShipMount")
 
 
 class ShipMount(BaseModel):
     """A mount is installed on the exterier of a ship.
 
     Attributes:
-        symbol (ShipMountSymbol):
-        name (str):
+        symbol (ShipMountSymbol): Symbo of this mount.
+        name (str): Name of this mount.
         requirements (ShipRequirements): The requirements for installation on a ship
-        description (Union[Unset, str]):
-        strength (Union[Unset, int]):
-        deposits (Union[Unset, List[ShipMountDepositsItem]]):
+        description (Union[Unset, str]): Description of this mount.
+        strength (Union[Unset, int]): Mounts that have this value, such as mining lasers, denote how powerful this
+            mount's capabilities are.
+        deposits (Union[Unset, List[ShipMountDepositsItem]]): Mounts that have this value denote what goods can be
+            produced from using the mount.
     """
 
     symbol: ShipMountSymbol = Field(alias="symbol")
     name: str = Field(alias="name")
     requirements: "ShipRequirements" = Field(alias="requirements")
     description: Union[Unset, str] = Field(UNSET, alias="description")
     strength: Union[Unset, int] = Field(UNSET, alias="strength")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_mount_deposits_item.py` & `spacetraders-0.7.0/spacetraders/models/ship_mount_deposits_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_mount_symbol.py` & `spacetraders-0.7.0/spacetraders/models/ship_mount_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_nav.py` & `spacetraders-0.7.0/spacetraders/models/ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_nav_route.py` & `spacetraders-0.7.0/spacetraders/models/ship_nav_route.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_nav_route_waypoint.py` & `spacetraders-0.7.0/spacetraders/models/ship_modification_transaction.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
+import datetime
 from typing import (
     Any,
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.waypoint_type import WaypointType
 from ..types import Unset
 
-T = TypeVar("T", bound="ShipNavRouteWaypoint")
+T = TypeVar("T", bound="ShipModificationTransaction")
 
 
-class ShipNavRouteWaypoint(BaseModel):
-    """The destination or departure of a ships nav route.
+class ShipModificationTransaction(BaseModel):
+    """Result of a transaction for a ship modification, such as installing a mount or a module.
 
     Attributes:
-        symbol (str):
-        type (WaypointType): The type of waypoint.
-        system_symbol (str):
-        x (int):
-        y (int):
+        waypoint_symbol (str): The symbol of the waypoint where the transaction took place.
+        ship_symbol (str): The symbol of the ship that made the transaction.
+        trade_symbol (str): The symbol of the trade good.
+        total_price (int): The total price of the transaction.
+        timestamp (datetime.datetime): The timestamp of the transaction.
     """
 
-    symbol: str = Field(alias="symbol")
-    type: WaypointType = Field(alias="type")
-    system_symbol: str = Field(alias="systemSymbol")
-    x: int = Field(alias="x")
-    y: int = Field(alias="y")
+    waypoint_symbol: str = Field(alias="waypointSymbol")
+    ship_symbol: str = Field(alias="shipSymbol")
+    trade_symbol: str = Field(alias="tradeSymbol")
+    total_price: int = Field(alias="totalPrice")
+    timestamp: datetime.datetime = Field(alias="timestamp")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_reactor.py` & `spacetraders-0.7.0/spacetraders/models/shipyard_ship.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,40 +4,51 @@
     List,
     TypeVar,
     Union,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.ship_reactor_symbol import ShipReactorSymbol
-from ..models.ship_requirements import ShipRequirements
+from ..models.ship_engine import ShipEngine
+from ..models.ship_frame import ShipFrame
+from ..models.ship_module import ShipModule
+from ..models.ship_mount import ShipMount
+from ..models.ship_reactor import ShipReactor
+from ..models.ship_type import ShipType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipReactor")
+T = TypeVar("T", bound="ShipyardShip")
 
 
-class ShipReactor(BaseModel):
-    """The reactor of the ship. The reactor is responsible for powering the ship's systems and weapons.
-
+class ShipyardShip(BaseModel):
+    """
     Attributes:
-        symbol (ShipReactorSymbol):
         name (str):
         description (str):
-        power_output (int):
-        requirements (ShipRequirements): The requirements for installation on a ship
-        condition (Union[Unset, int]): Condition is a range of 0 to 100 where 0 is completely worn out and 100 is brand
-            new.
+        purchase_price (int):
+        frame (ShipFrame): The frame of the ship. The frame determines the number of modules and mounting points of the
+            ship, as well as base fuel capacity. As the condition of the frame takes more wear, the ship will become more
+            sluggish and less maneuverable.
+        reactor (ShipReactor): The reactor of the ship. The reactor is responsible for powering the ship's systems and
+            weapons.
+        engine (ShipEngine): The engine determines how quickly a ship travels between waypoints.
+        modules (List['ShipModule']):
+        mounts (List['ShipMount']):
+        type (Union[Unset, ShipType]): Type of ship
     """
 
-    symbol: ShipReactorSymbol = Field(alias="symbol")
     name: str = Field(alias="name")
     description: str = Field(alias="description")
-    power_output: int = Field(alias="powerOutput")
-    requirements: "ShipRequirements" = Field(alias="requirements")
-    condition: Union[Unset, int] = Field(UNSET, alias="condition")
+    purchase_price: int = Field(alias="purchasePrice")
+    frame: "ShipFrame" = Field(alias="frame")
+    reactor: "ShipReactor" = Field(alias="reactor")
+    engine: "ShipEngine" = Field(alias="engine")
+    modules: List["ShipModule"] = Field(alias="modules")
+    mounts: List["ShipMount"] = Field(alias="mounts")
+    type: Union[Unset, ShipType] = Field(UNSET, alias="type")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_refine_json_body.py` & `spacetraders-0.7.0/spacetraders/models/extraction.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,27 +3,30 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.ship_refine_json_body_produce import ShipRefineJsonBodyProduce
+from ..models.extraction_yield import ExtractionYield
 from ..types import Unset
 
-T = TypeVar("T", bound="ShipRefineJsonBody")
+T = TypeVar("T", bound="Extraction")
 
 
-class ShipRefineJsonBody(BaseModel):
-    """
+class Extraction(BaseModel):
+    """Extraction details.
+
     Attributes:
-        produce (ShipRefineJsonBodyProduce):
+        ship_symbol (str): Symbol of the ship that executed the extraction.
+        yield_ (ExtractionYield): A yield from the extraction operation.
     """
 
-    produce: ShipRefineJsonBodyProduce = Field(alias="produce")
+    ship_symbol: str = Field(alias="shipSymbol")
+    yield_: "ExtractionYield" = Field(alias="yield")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response.py` & `spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,29 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.ship_refine_ship_refine_200_response_data import (
-    ShipRefineShipRefine200ResponseData,
+from ..models.ship_refine_ship_refine_201_response_data import (
+    ShipRefineShipRefine201ResponseData,
 )
 from ..types import Unset
 
-T = TypeVar("T", bound="ShipRefineShipRefine200Response")
+T = TypeVar("T", bound="ShipRefineShipRefine201Response")
 
 
-class ShipRefineShipRefine200Response(BaseModel):
+class ShipRefineShipRefine201Response(BaseModel):
     """
     Attributes:
-        data (ShipRefineShipRefine200ResponseData):
+        data (ShipRefineShipRefine201ResponseData):
     """
 
-    data: "ShipRefineShipRefine200ResponseData" = Field(alias="data")
+    data: "ShipRefineShipRefine201ResponseData" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py` & `spacetraders-0.7.0/spacetraders/models/ship_refine_ship_refine_201_response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,40 +5,42 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..models.cooldown import Cooldown
 from ..models.ship_cargo import ShipCargo
-from ..models.ship_refine_ship_refine_200_response_data_consumed_item import (
-    ShipRefineShipRefine200ResponseDataConsumedItem,
+from ..models.ship_refine_ship_refine_201_response_data_consumed_item import (
+    ShipRefineShipRefine201ResponseDataConsumedItem,
 )
-from ..models.ship_refine_ship_refine_200_response_data_produced_item import (
-    ShipRefineShipRefine200ResponseDataProducedItem,
+from ..models.ship_refine_ship_refine_201_response_data_produced_item import (
+    ShipRefineShipRefine201ResponseDataProducedItem,
 )
 from ..types import Unset
 
-T = TypeVar("T", bound="ShipRefineShipRefine200ResponseData")
+T = TypeVar("T", bound="ShipRefineShipRefine201ResponseData")
 
 
-class ShipRefineShipRefine200ResponseData(BaseModel):
+class ShipRefineShipRefine201ResponseData(BaseModel):
     """
     Attributes:
-        cargo (ShipCargo):
+        cargo (ShipCargo): Ship cargo details.
         cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
-        produced (List['ShipRefineShipRefine200ResponseDataProducedItem']):
-        consumed (List['ShipRefineShipRefine200ResponseDataConsumedItem']):
+        produced (List['ShipRefineShipRefine201ResponseDataProducedItem']): Goods that were produced by this refining
+            process.
+        consumed (List['ShipRefineShipRefine201ResponseDataConsumedItem']): Goods that were consumed during this
+            refining process.
     """
 
     cargo: "ShipCargo" = Field(alias="cargo")
     cooldown: "Cooldown" = Field(alias="cooldown")
-    produced: List["ShipRefineShipRefine200ResponseDataProducedItem"] = Field(
+    produced: List["ShipRefineShipRefine201ResponseDataProducedItem"] = Field(
         alias="produced"
     )
-    consumed: List["ShipRefineShipRefine200ResponseDataConsumedItem"] = Field(
+    consumed: List["ShipRefineShipRefine201ResponseDataConsumedItem"] = Field(
         alias="consumed"
     )
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py` & `spacetraders-0.7.0/spacetraders/models/waypoint_orbital.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from typing import (
     Any,
     Dict,
     List,
     TypeVar,
-    Union,
 )
 
 from pydantic import BaseModel, Field
 
-from ..types import UNSET, Unset
+from ..types import Unset
 
-T = TypeVar("T", bound="ShipRefineShipRefine200ResponseDataConsumedItem")
+T = TypeVar("T", bound="WaypointOrbital")
 
 
-class ShipRefineShipRefine200ResponseDataConsumedItem(BaseModel):
-    """
+class WaypointOrbital(BaseModel):
+    """An orbital is another waypoint that orbits a parent waypoint.
+
     Attributes:
-        trade_symbol (Union[Unset, str]):
-        units (Union[Unset, int]):
+        symbol (str): The symbol of the orbiting waypoint.
     """
 
-    trade_symbol: Union[Unset, str] = Field(UNSET, alias="tradeSymbol")
-    units: Union[Unset, int] = Field(UNSET, alias="units")
+    symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py` & `spacetraders-0.7.0/spacetraders/models/get_status_response_200_stats.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from typing import (
     Any,
     Dict,
     List,
     TypeVar,
-    Union,
 )
 
 from pydantic import BaseModel, Field
 
-from ..types import UNSET, Unset
+from ..types import Unset
 
-T = TypeVar("T", bound="ShipRefineShipRefine200ResponseDataProducedItem")
+T = TypeVar("T", bound="GetStatusResponse200Stats")
 
 
-class ShipRefineShipRefine200ResponseDataProducedItem(BaseModel):
+class GetStatusResponse200Stats(BaseModel):
     """
     Attributes:
-        trade_symbol (Union[Unset, str]):
-        units (Union[Unset, int]):
+        agents (int): Number of registered agents in the game.
+        ships (int): Total number of ships in the game.
+        systems (int): Total number of systems in the game.
+        waypoints (int): Total number of waypoints in the game.
     """
 
-    trade_symbol: Union[Unset, str] = Field(UNSET, alias="tradeSymbol")
-    units: Union[Unset, int] = Field(UNSET, alias="units")
+    agents: int = Field(alias="agents")
+    ships: int = Field(alias="ships")
+    systems: int = Field(alias="systems")
+    waypoints: int = Field(alias="waypoints")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_registration.py` & `spacetraders-0.7.0/spacetraders/models/ship_registration.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_requirements.py` & `spacetraders-0.7.0/spacetraders/models/ship_requirements.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/ship_type.py` & `spacetraders-0.7.0/spacetraders/models/ship_type.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/shipyard.py` & `spacetraders-0.7.0/spacetraders/models/shipyard.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/shipyard_ship_types_item.py` & `spacetraders-0.7.0/spacetraders/models/shipyard_ship_types_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 T = TypeVar("T", bound="ShipyardShipTypesItem")
 
 
 class ShipyardShipTypesItem(BaseModel):
     """
     Attributes:
-        type (Union[Unset, ShipType]):
+        type (Union[Unset, ShipType]): Type of ship
     """
 
     type: Union[Unset, ShipType] = Field(UNSET, alias="type")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/shipyard_transaction.py` & `spacetraders-0.7.0/spacetraders/models/faction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-import datetime
 from typing import (
     Any,
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.faction_symbols import FactionSymbols
+from ..models.faction_trait import FactionTrait
 from ..types import Unset
 
-T = TypeVar("T", bound="ShipyardTransaction")
+T = TypeVar("T", bound="Faction")
 
 
-class ShipyardTransaction(BaseModel):
-    """
+class Faction(BaseModel):
+    """Faction details.
+
     Attributes:
-        waypoint_symbol (str): The symbol of the waypoint where the transaction took place.
-        ship_symbol (str): The symbol of the ship that was purchased.
-        price (int): The price of the transaction.
-        agent_symbol (str): The symbol of the agent that made the transaction.
-        timestamp (datetime.datetime): The timestamp of the transaction.
+        symbol (FactionSymbols): The symbol of the faction.
+        name (str): Name of the faction.
+        description (str): Description of the faction.
+        headquarters (str): The waypoint in which the faction's HQ is located in.
+        traits (List['FactionTrait']): List of traits that define this faction.
+        is_recruiting (bool): Whether or not the faction is currently recruiting new agents.
     """
 
-    waypoint_symbol: str = Field(alias="waypointSymbol")
-    ship_symbol: str = Field(alias="shipSymbol")
-    price: int = Field(alias="price")
-    agent_symbol: str = Field(alias="agentSymbol")
-    timestamp: datetime.datetime = Field(alias="timestamp")
+    symbol: FactionSymbols = Field(alias="symbol")
+    name: str = Field(alias="name")
+    description: str = Field(alias="description")
+    headquarters: str = Field(alias="headquarters")
+    traits: List["FactionTrait"] = Field(alias="traits")
+    is_recruiting: bool = Field(alias="isRecruiting")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/survey.py` & `spacetraders-0.7.0/spacetraders/models/survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/survey_deposit.py` & `spacetraders-0.7.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,27 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.ship_cargo import ShipCargo
 from ..types import Unset
 
-T = TypeVar("T", bound="SurveyDeposit")
+T = TypeVar("T", bound="TransferCargoTransferCargo200ResponseData")
 
 
-class SurveyDeposit(BaseModel):
-    """A surveyed deposit of a mineral or resource available for extraction.
-
+class TransferCargoTransferCargo200ResponseData(BaseModel):
+    """
     Attributes:
-        symbol (str): The symbol of the deposit.
+        cargo (ShipCargo): Ship cargo details.
     """
 
-    symbol: str = Field(alias="symbol")
+    cargo: "ShipCargo" = Field(alias="cargo")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/system.py` & `spacetraders-0.7.0/spacetraders/models/system.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 T = TypeVar("T", bound="System")
 
 
 class System(BaseModel):
     """
     Attributes:
-        symbol (str):
-        sector_symbol (str):
+        symbol (str): The symbol of the system.
+        sector_symbol (str): The symbol of the sector.
         type (SystemType): The type of waypoint.
-        x (int):
-        y (int):
-        waypoints (List['SystemWaypoint']):
-        factions (List['SystemFaction']):
+        x (int): Position in the universe in the x axis.
+        y (int): Position in the universe in the y axis.
+        waypoints (List['SystemWaypoint']): Waypoints in this system.
+        factions (List['SystemFaction']): Factions that control this system.
     """
 
     symbol: str = Field(alias="symbol")
     sector_symbol: str = Field(alias="sectorSymbol")
     type: SystemType = Field(alias="type")
     x: int = Field(alias="x")
     y: int = Field(alias="y")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/system_faction.py` & `spacetraders-0.7.0/spacetraders/models/trade_good.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,32 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.trade_symbol import TradeSymbol
 from ..types import Unset
 
-T = TypeVar("T", bound="SystemFaction")
+T = TypeVar("T", bound="TradeGood")
 
 
-class SystemFaction(BaseModel):
-    """
+class TradeGood(BaseModel):
+    """A good that can be traded for other goods or currency.
+
     Attributes:
-        symbol (str):
+        symbol (TradeSymbol): The good's symbol.
+        name (str): The name of the good.
+        description (str): The description of the good.
     """
 
-    symbol: str = Field(alias="symbol")
+    symbol: TradeSymbol = Field(alias="symbol")
+    name: str = Field(alias="name")
+    description: str = Field(alias="description")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/system_waypoint.py` & `spacetraders-0.7.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,33 +3,31 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.waypoint_type import WaypointType
+from ..models.trade_symbol import TradeSymbol
 from ..types import Unset
 
-T = TypeVar("T", bound="SystemWaypoint")
+T = TypeVar("T", bound="TransferCargoTransferCargoRequest")
 
 
-class SystemWaypoint(BaseModel):
+class TransferCargoTransferCargoRequest(BaseModel):
     """
     Attributes:
-        symbol (str):
-        type (WaypointType): The type of waypoint.
-        x (int):
-        y (int):
+        trade_symbol (TradeSymbol): The good's symbol.
+        units (int): Amount of units to transfer.
+        ship_symbol (str): The symbol of the ship to transfer to.
     """
 
-    symbol: str = Field(alias="symbol")
-    type: WaypointType = Field(alias="type")
-    x: int = Field(alias="x")
-    y: int = Field(alias="y")
+    trade_symbol: TradeSymbol = Field(alias="tradeSymbol")
+    units: int = Field(alias="units")
+    ship_symbol: str = Field(alias="shipSymbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/trade_good.py` & `spacetraders-0.7.0/spacetraders/models/waypoint_trait.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,29 +3,29 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.trade_symbol import TradeSymbol
+from ..models.waypoint_trait_symbol import WaypointTraitSymbol
 from ..types import Unset
 
-T = TypeVar("T", bound="TradeGood")
+T = TypeVar("T", bound="WaypointTrait")
 
 
-class TradeGood(BaseModel):
+class WaypointTrait(BaseModel):
     """
     Attributes:
-        symbol (TradeSymbol):
-        name (str):
-        description (str):
+        symbol (WaypointTraitSymbol): The unique identifier of the trait.
+        name (str): The name of the trait.
+        description (str): A description of the trait.
     """
 
-    symbol: TradeSymbol = Field(alias="symbol")
+    symbol: WaypointTraitSymbol = Field(alias="symbol")
     name: str = Field(alias="name")
     description: str = Field(alias="description")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.6.0/spacetraders/models/trade_symbol.py` & `spacetraders-0.7.0/spacetraders/models/trade_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py` & `spacetraders-0.7.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py` & `spacetraders-0.7.0/spacetraders/models/warp_ship_response_200_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,31 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.ship_cargo import ShipCargo
+from ..models.ship_fuel import ShipFuel
+from ..models.ship_nav import ShipNav
 from ..types import Unset
 
-T = TypeVar("T", bound="TransferCargoTransferCargo200ResponseData")
+T = TypeVar("T", bound="WarpShipResponse200Data")
 
 
-class TransferCargoTransferCargo200ResponseData(BaseModel):
+class WarpShipResponse200Data(BaseModel):
     """
     Attributes:
-        cargo (ShipCargo):
+        fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
+            or action.
+        nav (ShipNav): The navigation information of the ship.
     """
 
-    cargo: "ShipCargo" = Field(alias="cargo")
+    fuel: "ShipFuel" = Field(alias="fuel")
+    nav: "ShipNav" = Field(alias="nav")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py` & `spacetraders-0.7.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,30 +3,29 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.trade_symbol import TradeSymbol
 from ..types import Unset
 
-T = TypeVar("T", bound="TransferCargoTransferCargoRequest")
+T = TypeVar("T", bound="PurchaseCargoPurchaseCargoRequest")
 
 
-class TransferCargoTransferCargoRequest(BaseModel):
+class PurchaseCargoPurchaseCargoRequest(BaseModel):
     """
     Attributes:
-        trade_symbol (str):
-        units (int):
-        ship_symbol (str):
+        symbol (TradeSymbol): The good's symbol.
+        units (int): Amounts of units to purchase.
     """
 
-    trade_symbol: str = Field(alias="tradeSymbol")
+    symbol: TradeSymbol = Field(alias="symbol")
     units: int = Field(alias="units")
-    ship_symbol: str = Field(alias="shipSymbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/warp_ship_json_body.py` & `spacetraders-0.7.0/spacetraders/models/warp_ship_response_200.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,27 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.warp_ship_response_200_data import WarpShipResponse200Data
 from ..types import Unset
 
-T = TypeVar("T", bound="WarpShipJsonBody")
+T = TypeVar("T", bound="WarpShipResponse200")
 
 
-class WarpShipJsonBody(BaseModel):
+class WarpShipResponse200(BaseModel):
     """
     Attributes:
-        waypoint_symbol (str): The target destination.
+        data (WarpShipResponse200Data):
     """
 
-    waypoint_symbol: str = Field(alias="waypointSymbol")
+    data: "WarpShipResponse200Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/warp_ship_response_200.py` & `spacetraders-0.7.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,28 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.warp_ship_response_200_data import WarpShipResponse200Data
 from ..types import Unset
 
-T = TypeVar("T", bound="WarpShipResponse200")
+T = TypeVar("T", bound="GetStatusResponse200LeaderboardsMostCreditsItem")
 
 
-class WarpShipResponse200(BaseModel):
+class GetStatusResponse200LeaderboardsMostCreditsItem(BaseModel):
     """
     Attributes:
-        data (WarpShipResponse200Data):
+        agent_symbol (str): Symbol of the agent.
+        credits_ (int): Amount of credits.
     """
 
-    data: "WarpShipResponse200Data" = Field(alias="data")
+    agent_symbol: str = Field(alias="agentSymbol")
+    credits_: int = Field(alias="credits")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/warp_ship_response_200_data.py` & `spacetraders-0.7.0/spacetraders/models/sell_cargo_sell_cargo_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,31 +3,29 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.ship_fuel import ShipFuel
-from ..models.ship_nav import ShipNav
+from ..models.trade_symbol import TradeSymbol
 from ..types import Unset
 
-T = TypeVar("T", bound="WarpShipResponse200Data")
+T = TypeVar("T", bound="SellCargoSellCargoRequest")
 
 
-class WarpShipResponse200Data(BaseModel):
+class SellCargoSellCargoRequest(BaseModel):
     """
     Attributes:
-        fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
-            or action.
-        nav (ShipNav): The navigation information of the ship.
+        symbol (TradeSymbol): The good's symbol.
+        units (int): Amounts of units to sell of the selected good.
     """
 
-    fuel: "ShipFuel" = Field(alias="fuel")
-    nav: "ShipNav" = Field(alias="nav")
+    symbol: TradeSymbol = Field(alias="symbol")
+    units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/waypoint.py` & `spacetraders-0.7.0/spacetraders/models/scanned_waypoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 from ..models.chart import Chart
 from ..models.waypoint_faction import WaypointFaction
 from ..models.waypoint_orbital import WaypointOrbital
 from ..models.waypoint_trait import WaypointTrait
 from ..models.waypoint_type import WaypointType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Waypoint")
+T = TypeVar("T", bound="ScannedWaypoint")
 
 
-class Waypoint(BaseModel):
-    """A waypoint is a location that ships can travel to such as a Planet, Moon or Space Station.
+class ScannedWaypoint(BaseModel):
+    """A waypoint that was scanned by a ship.
 
     Attributes:
-        symbol (str):
+        symbol (str): Symbol of the waypoint.
         type (WaypointType): The type of waypoint.
-        system_symbol (str):
-        x (int):
-        y (int):
-        orbitals (List['WaypointOrbital']):
+        system_symbol (str): Symbol of the system.
+        x (int): Position in the universe in the x axis.
+        y (int): Position in the universe in the y axis.
+        orbitals (List['WaypointOrbital']): List of waypoints that orbit this waypoint.
         traits (List['WaypointTrait']): The traits of the waypoint.
-        faction (Union[Unset, WaypointFaction]):
+        faction (Union[Unset, WaypointFaction]): The faction that controls the waypoint.
         chart (Union[Unset, Chart]): The chart of a system or waypoint, which makes the location visible to other
             agents.
     """
 
     symbol: str = Field(alias="symbol")
     type: WaypointType = Field(alias="type")
     system_symbol: str = Field(alias="systemSymbol")
```

### Comparing `spacetraders-0.6.0/spacetraders/models/waypoint_faction.py` & `spacetraders-0.7.0/spacetraders/models/meta.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,24 +5,30 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="WaypointFaction")
+T = TypeVar("T", bound="Meta")
 
 
-class WaypointFaction(BaseModel):
-    """
+class Meta(BaseModel):
+    """Meta details for pagination.
+
     Attributes:
-        symbol (str):
+        total (int): Shows the total amount of items of this kind that exist.
+        page (int): A page denotes an amount of items, offset from the first item. Each page holds an amount of items
+            equal to the `limit`. Default: 1.
+        limit (int): The amount of items in each page. Limits how many items can be fetched at once. Default: 10.
     """
 
-    symbol: str = Field(alias="symbol")
+    total: int = Field(alias="total")
+    page: int = Field(1, alias="page")
+    limit: int = Field(10, alias="limit")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/waypoint_trait.py` & `spacetraders-0.7.0/spacetraders/models/register_json_body.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from typing import (
     Any,
     Dict,
     List,
     TypeVar,
+    Union,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.waypoint_trait_symbol import WaypointTraitSymbol
-from ..types import Unset
+from ..models.faction_symbols import FactionSymbols
+from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="WaypointTrait")
+T = TypeVar("T", bound="RegisterJsonBody")
 
 
-class WaypointTrait(BaseModel):
+class RegisterJsonBody(BaseModel):
     """
     Attributes:
-        symbol (WaypointTraitSymbol): The unique identifier of the trait.
-        name (str): The name of the trait.
-        description (str): A description of the trait.
+        faction (FactionSymbols): The symbol of the faction.
+        symbol (str): Your desired agent symbol. This will be a unique name used to represent your agent, and will be
+            the prefix for your ships. Example: BADGER.
+        email (Union[Unset, str]): Your email address. This is used if you reserved your call sign between resets.
     """
 
-    symbol: WaypointTraitSymbol = Field(alias="symbol")
-    name: str = Field(alias="name")
-    description: str = Field(alias="description")
+    faction: FactionSymbols = Field(alias="faction")
+    symbol: str = Field(alias="symbol")
+    email: Union[Unset, str] = Field(UNSET, alias="email")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.6.0/spacetraders/models/waypoint_trait_symbol.py` & `spacetraders-0.7.0/spacetraders/models/waypoint_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/spacetraders/types.py` & `spacetraders-0.7.0/spacetraders/types.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.6.0/PKG-INFO` & `spacetraders-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetraders
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python API for Space Traders
 License: Apache-2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

