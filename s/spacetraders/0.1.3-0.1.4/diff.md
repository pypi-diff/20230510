# Comparing `tmp/spacetraders-0.1.3.tar.gz` & `tmp/spacetraders-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetraders-0.1.3.tar", max compression
+gzip compressed data, was "spacetraders-0.1.4.tar", max compression
```

## Comparing `spacetraders-0.1.3.tar` & `spacetraders-0.1.4.tar`

### file list

```diff
@@ -1,208 +1,208 @@
--rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.1.3/README.md
--rw-r--r--   0        0        0      501 2023-05-10 04:38:42.349681 spacetraders-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      160 2023-05-10 04:04:46.359674 spacetraders-0.1.3/spacetraders/__init__.py
--rw-r--r--   0        0        0       47 2023-05-10 04:04:45.839674 spacetraders-0.1.3/spacetraders/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 04:04:45.879674 spacetraders-0.1.3/spacetraders/api/agents/__init__.py
--rw-r--r--   0        0        0     3816 2023-05-10 04:04:46.449674 spacetraders-0.1.3/spacetraders/api/agents/get_my_agent.py
--rw-r--r--   0        0        0        0 2023-05-10 04:04:45.879674 spacetraders-0.1.3/spacetraders/api/contracts/__init__.py
--rw-r--r--   0        0        0     4288 2023-05-10 04:04:46.459674 spacetraders-0.1.3/spacetraders/api/contracts/accept_contract.py
--rw-r--r--   0        0        0     5017 2023-05-10 04:04:46.479674 spacetraders-0.1.3/spacetraders/api/contracts/deliver_contract.py
--rw-r--r--   0        0        0     4306 2023-05-10 04:04:46.449674 spacetraders-0.1.3/spacetraders/api/contracts/fulfill_contract.py
--rw-r--r--   0        0        0     4287 2023-05-10 04:04:46.479674 spacetraders-0.1.3/spacetraders/api/contracts/get_contract.py
--rw-r--r--   0        0        0     5013 2023-05-10 04:04:46.499674 spacetraders-0.1.3/spacetraders/api/contracts/get_contracts.py
--rw-r--r--   0        0        0        0 2023-05-10 04:04:45.849674 spacetraders-0.1.3/spacetraders/api/default/__init__.py
--rw-r--r--   0        0        0     9110 2023-05-10 04:04:46.509674 spacetraders-0.1.3/spacetraders/api/default/register.py
--rw-r--r--   0        0        0        0 2023-05-10 04:04:45.879674 spacetraders-0.1.3/spacetraders/api/factions/__init__.py
--rw-r--r--   0        0        0     4359 2023-05-10 04:04:46.449674 spacetraders-0.1.3/spacetraders/api/factions/get_faction.py
--rw-r--r--   0        0        0     4983 2023-05-10 04:04:46.489674 spacetraders-0.1.3/spacetraders/api/factions/get_factions.py
--rw-r--r--   0        0        0        0 2023-05-10 04:04:45.879674 spacetraders-0.1.3/spacetraders/api/fleet/__init__.py
--rw-r--r--   0        0        0     5253 2023-05-10 04:04:46.479674 spacetraders-0.1.3/spacetraders/api/fleet/create_chart.py
--rw-r--r--   0        0        0     4511 2023-05-10 04:04:46.439674 spacetraders-0.1.3/spacetraders/api/fleet/create_ship_ship_scan.py
--rw-r--r--   0        0        0     4564 2023-05-10 04:04:46.469674 spacetraders-0.1.3/spacetraders/api/fleet/create_ship_system_scan.py
--rw-r--r--   0        0        0     4608 2023-05-10 04:04:46.519674 spacetraders-0.1.3/spacetraders/api/fleet/create_ship_waypoint_scan.py
--rw-r--r--   0        0        0     6211 2023-05-10 04:04:46.449674 spacetraders-0.1.3/spacetraders/api/fleet/create_survey.py
--rw-r--r--   0        0        0     5354 2023-05-10 04:04:46.509674 spacetraders-0.1.3/spacetraders/api/fleet/dock_ship.py
--rw-r--r--   0        0        0     5394 2023-05-10 04:04:46.499674 spacetraders-0.1.3/spacetraders/api/fleet/extract_resources.py
--rw-r--r--   0        0        0     4234 2023-05-10 04:04:46.509674 spacetraders-0.1.3/spacetraders/api/fleet/get_my_ship.py
--rw-r--r--   0        0        0     4336 2023-05-10 04:04:46.549674 spacetraders-0.1.3/spacetraders/api/fleet/get_my_ship_cargo.py
--rw-r--r--   0        0        0     4968 2023-05-10 04:04:46.589674 spacetraders-0.1.3/spacetraders/api/fleet/get_my_ships.py
--rw-r--r--   0        0        0     6388 2023-05-10 04:04:46.589674 spacetraders-0.1.3/spacetraders/api/fleet/get_ship_cooldown.py
--rw-r--r--   0        0        0     4279 2023-05-10 04:04:46.539674 spacetraders-0.1.3/spacetraders/api/fleet/get_ship_nav.py
--rw-r--r--   0        0        0     4872 2023-05-10 04:04:46.599674 spacetraders-0.1.3/spacetraders/api/fleet/jettison.py
--rw-r--r--   0        0        0     5162 2023-05-10 04:04:46.609674 spacetraders-0.1.3/spacetraders/api/fleet/jump_ship.py
--rw-r--r--   0        0        0     6798 2023-05-10 04:04:46.609674 spacetraders-0.1.3/spacetraders/api/fleet/navigate_ship.py
--rw-r--r--   0        0        0     5329 2023-05-10 04:04:46.569674 spacetraders-0.1.3/spacetraders/api/fleet/orbit_ship.py
--rw-r--r--   0        0        0     5002 2023-05-10 04:04:46.619674 spacetraders-0.1.3/spacetraders/api/fleet/patch_ship_nav.py
--rw-r--r--   0        0        0     5209 2023-05-10 04:04:46.609674 spacetraders-0.1.3/spacetraders/api/fleet/purchase_cargo.py
--rw-r--r--   0        0        0     4445 2023-05-10 04:04:46.639674 spacetraders-0.1.3/spacetraders/api/fleet/purchase_ship.py
--rw-r--r--   0        0        0     4300 2023-05-10 04:04:46.619674 spacetraders-0.1.3/spacetraders/api/fleet/refuel_ship.py
--rw-r--r--   0        0        0     4963 2023-05-10 04:04:46.699674 spacetraders-0.1.3/spacetraders/api/fleet/sell_cargo.py
--rw-r--r--   0        0        0     5465 2023-05-10 04:04:46.609674 spacetraders-0.1.3/spacetraders/api/fleet/ship_refine.py
--rw-r--r--   0        0        0     5260 2023-05-10 04:04:46.599674 spacetraders-0.1.3/spacetraders/api/fleet/transfer_cargo.py
--rw-r--r--   0        0        0     6202 2023-05-10 04:04:46.629674 spacetraders-0.1.3/spacetraders/api/fleet/warp_ship.py
--rw-r--r--   0        0        0        0 2023-05-10 04:04:45.869674 spacetraders-0.1.3/spacetraders/api/systems/__init__.py
--rw-r--r--   0        0        0     4836 2023-05-10 04:04:46.729674 spacetraders-0.1.3/spacetraders/api/systems/get_jump_gate.py
--rw-r--r--   0        0        0     5622 2023-05-10 04:04:46.719674 spacetraders-0.1.3/spacetraders/api/systems/get_market.py
--rw-r--r--   0        0        0     4810 2023-05-10 04:04:46.649674 spacetraders-0.1.3/spacetraders/api/systems/get_shipyard.py
--rw-r--r--   0        0        0     4396 2023-05-10 04:04:46.689674 spacetraders-0.1.3/spacetraders/api/systems/get_system.py
--rw-r--r--   0        0        0     5942 2023-05-10 04:04:46.819674 spacetraders-0.1.3/spacetraders/api/systems/get_system_waypoints.py
--rw-r--r--   0        0        0     4982 2023-05-10 04:04:46.719674 spacetraders-0.1.3/spacetraders/api/systems/get_systems.py
--rw-r--r--   0        0        0     4797 2023-05-10 04:04:46.709674 spacetraders-0.1.3/spacetraders/api/systems/get_waypoint.py
--rw-r--r--   0        0        0     4202 2023-05-10 04:04:46.689674 spacetraders-0.1.3/spacetraders/client.py
--rw-r--r--   0        0        0      470 2023-05-10 04:04:46.609674 spacetraders-0.1.3/spacetraders/errors.py
--rw-r--r--   0        0        0    13081 2023-05-10 04:04:46.789674 spacetraders-0.1.3/spacetraders/models/__init__.py
--rw-r--r--   0        0        0     2021 2023-05-10 04:04:46.659674 spacetraders-0.1.3/spacetraders/models/accept_contract_response_200.py
--rw-r--r--   0        0        0     2138 2023-05-10 04:04:46.669674 spacetraders-0.1.3/spacetraders/models/accept_contract_response_200_data.py
--rw-r--r--   0        0        0     2216 2023-05-10 04:04:46.709674 spacetraders-0.1.3/spacetraders/models/agent.py
--rw-r--r--   0        0        0     2735 2023-05-10 04:04:46.699674 spacetraders-0.1.3/spacetraders/models/chart.py
--rw-r--r--   0        0        0     2817 2023-05-10 04:04:46.709674 spacetraders-0.1.3/spacetraders/models/connected_system.py
--rw-r--r--   0        0        0     3209 2023-05-10 04:04:46.749674 spacetraders-0.1.3/spacetraders/models/contract.py
--rw-r--r--   0        0        0     2675 2023-05-10 04:04:46.729674 spacetraders-0.1.3/spacetraders/models/contract_deliver_good.py
--rw-r--r--   0        0        0     1922 2023-05-10 04:04:46.719674 spacetraders-0.1.3/spacetraders/models/contract_payment.py
--rw-r--r--   0        0        0     3089 2023-05-10 04:04:46.759674 spacetraders-0.1.3/spacetraders/models/contract_terms.py
--rw-r--r--   0        0        0      201 2023-05-10 04:04:46.009674 spacetraders-0.1.3/spacetraders/models/contract_type.py
--rw-r--r--   0        0        0     2629 2023-05-10 04:04:46.799674 spacetraders-0.1.3/spacetraders/models/cooldown.py
--rw-r--r--   0        0        0     1929 2023-05-10 04:04:46.759674 spacetraders-0.1.3/spacetraders/models/create_chart_response_201.py
--rw-r--r--   0        0        0     2299 2023-05-10 04:04:46.779674 spacetraders-0.1.3/spacetraders/models/create_chart_response_201_data.py
--rw-r--r--   0        0        0     2106 2023-05-10 04:04:46.799674 spacetraders-0.1.3/spacetraders/models/create_ship_ship_scan_response_201.py
--rw-r--r--   0        0        0     2566 2023-05-10 04:04:46.799674 spacetraders-0.1.3/spacetraders/models/create_ship_ship_scan_response_201_data.py
--rw-r--r--   0        0        0     2134 2023-05-10 04:04:46.789674 spacetraders-0.1.3/spacetraders/models/create_ship_system_scan_response_201.py
--rw-r--r--   0        0        0     2638 2023-05-10 04:04:46.819674 spacetraders-0.1.3/spacetraders/models/create_ship_system_scan_response_201_data.py
--rw-r--r--   0        0        0     2162 2023-05-10 04:04:46.809674 spacetraders-0.1.3/spacetraders/models/create_ship_waypoint_scan_response_201.py
--rw-r--r--   0        0        0     2710 2023-05-10 04:04:46.779674 spacetraders-0.1.3/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
--rw-r--r--   0        0        0     1943 2023-05-10 04:04:46.799674 spacetraders-0.1.3/spacetraders/models/create_survey_response_201.py
--rw-r--r--   0        0        0     2526 2023-05-10 04:04:46.939674 spacetraders-0.1.3/spacetraders/models/create_survey_response_201_data.py
--rw-r--r--   0        0        0     1989 2023-05-10 04:04:46.779674 spacetraders-0.1.3/spacetraders/models/deliver_contract_json_body.py
--rw-r--r--   0        0        0     2052 2023-05-10 04:04:46.849674 spacetraders-0.1.3/spacetraders/models/deliver_contract_response_200.py
--rw-r--r--   0        0        0     2182 2023-05-10 04:04:46.819674 spacetraders-0.1.3/spacetraders/models/deliver_contract_response_200_data.py
--rw-r--r--   0        0        0     2078 2023-05-10 04:04:46.799674 spacetraders-0.1.3/spacetraders/models/dock_ship_dock_ship_200_response.py
--rw-r--r--   0        0        0     1833 2023-05-10 04:04:46.819674 spacetraders-0.1.3/spacetraders/models/dock_ship_dock_ship_200_response_data.py
--rw-r--r--   0        0        0     2215 2023-05-10 04:04:46.839674 spacetraders-0.1.3/spacetraders/models/extract_resources_json_body.py
--rw-r--r--   0        0        0     2066 2023-05-10 04:04:46.839674 spacetraders-0.1.3/spacetraders/models/extract_resources_response_201.py
--rw-r--r--   0        0        0     2666 2023-05-10 04:04:46.859674 spacetraders-0.1.3/spacetraders/models/extract_resources_response_201_data.py
--rw-r--r--   0        0        0     1980 2023-05-10 04:04:46.839674 spacetraders-0.1.3/spacetraders/models/extraction.py
--rw-r--r--   0        0        0     1750 2023-05-10 04:04:46.839674 spacetraders-0.1.3/spacetraders/models/extraction_yield.py
--rw-r--r--   0        0        0     2746 2023-05-10 04:04:46.939674 spacetraders-0.1.3/spacetraders/models/faction.py
--rw-r--r--   0        0        0     2067 2023-05-10 04:04:46.879674 spacetraders-0.1.3/spacetraders/models/faction_trait.py
--rw-r--r--   0        0        0     2091 2023-05-10 04:04:46.129674 spacetraders-0.1.3/spacetraders/models/faction_trait_symbol.py
--rw-r--r--   0        0        0     2052 2023-05-10 04:04:46.849674 spacetraders-0.1.3/spacetraders/models/fulfill_contract_response_200.py
--rw-r--r--   0        0        0     2143 2023-05-10 04:04:46.869674 spacetraders-0.1.3/spacetraders/models/fulfill_contract_response_200_data.py
--rw-r--r--   0        0        0     1755 2023-05-10 04:04:46.889674 spacetraders-0.1.3/spacetraders/models/get_contract_response_200.py
--rw-r--r--   0        0        0     2300 2023-05-10 04:04:46.879674 spacetraders-0.1.3/spacetraders/models/get_contracts_response_200.py
--rw-r--r--   0        0        0     1741 2023-05-10 04:04:46.869674 spacetraders-0.1.3/spacetraders/models/get_faction_response_200.py
--rw-r--r--   0        0        0     2286 2023-05-10 04:04:46.959674 spacetraders-0.1.3/spacetraders/models/get_factions_response_200.py
--rw-r--r--   0        0        0     1761 2023-05-10 04:04:46.909674 spacetraders-0.1.3/spacetraders/models/get_jump_gate_response_200.py
--rw-r--r--   0        0        0     1727 2023-05-10 04:04:46.879674 spacetraders-0.1.3/spacetraders/models/get_market_response_200.py
--rw-r--r--   0        0        0     1726 2023-05-10 04:04:46.889674 spacetraders-0.1.3/spacetraders/models/get_my_agent_response_200.py
--rw-r--r--   0        0        0     1788 2023-05-10 04:04:46.879674 spacetraders-0.1.3/spacetraders/models/get_my_ship_cargo_response_200.py
--rw-r--r--   0        0        0     1719 2023-05-10 04:04:46.889674 spacetraders-0.1.3/spacetraders/models/get_my_ship_response_200.py
--rw-r--r--   0        0        0     2257 2023-05-10 04:04:46.939674 spacetraders-0.1.3/spacetraders/models/get_my_ships_response_200.py
--rw-r--r--   0        0        0     1857 2023-05-10 04:04:46.909674 spacetraders-0.1.3/spacetraders/models/get_ship_cooldown_response_200.py
--rw-r--r--   0        0        0     1787 2023-05-10 04:04:46.919674 spacetraders-0.1.3/spacetraders/models/get_ship_nav_response_200.py
--rw-r--r--   0        0        0     1755 2023-05-10 04:04:46.979674 spacetraders-0.1.3/spacetraders/models/get_shipyard_response_200.py
--rw-r--r--   0        0        0     1727 2023-05-10 04:04:46.919674 spacetraders-0.1.3/spacetraders/models/get_system_response_200.py
--rw-r--r--   0        0        0     2333 2023-05-10 04:04:46.949674 spacetraders-0.1.3/spacetraders/models/get_system_waypoints_response_200.py
--rw-r--r--   0        0        0     2272 2023-05-10 04:04:46.969674 spacetraders-0.1.3/spacetraders/models/get_systems_response_200.py
--rw-r--r--   0        0        0     1846 2023-05-10 04:04:46.929674 spacetraders-0.1.3/spacetraders/models/get_waypoint_response_200.py
--rw-r--r--   0        0        0     1683 2023-05-10 04:04:46.929674 spacetraders-0.1.3/spacetraders/models/jettison_json_body.py
--rw-r--r--   0        0        0     1881 2023-05-10 04:04:46.939674 spacetraders-0.1.3/spacetraders/models/jettison_response_200.py
--rw-r--r--   0        0        0     1782 2023-05-10 04:04:46.939674 spacetraders-0.1.3/spacetraders/models/jettison_response_200_data.py
--rw-r--r--   0        0        0     3023 2023-05-10 04:04:46.989674 spacetraders-0.1.3/spacetraders/models/jump_gate.py
--rw-r--r--   0        0        0     1632 2023-05-10 04:04:46.949674 spacetraders-0.1.3/spacetraders/models/jump_ship_json_body.py
--rw-r--r--   0        0        0     1887 2023-05-10 04:04:46.969674 spacetraders-0.1.3/spacetraders/models/jump_ship_response_200.py
--rw-r--r--   0        0        0     2550 2023-05-10 04:04:46.999674 spacetraders-0.1.3/spacetraders/models/jump_ship_response_200_data.py
--rw-r--r--   0        0        0     5804 2023-05-10 04:04:47.109674 spacetraders-0.1.3/spacetraders/models/market.py
--rw-r--r--   0        0        0     2843 2023-05-10 04:04:46.989674 spacetraders-0.1.3/spacetraders/models/market_trade_good.py
--rw-r--r--   0        0        0      224 2023-05-10 04:04:46.019674 spacetraders-0.1.3/spacetraders/models/market_trade_good_supply.py
--rw-r--r--   0        0        0     3546 2023-05-10 04:04:47.019674 spacetraders-0.1.3/spacetraders/models/market_transaction.py
--rw-r--r--   0        0        0      170 2023-05-10 04:04:46.029674 spacetraders-0.1.3/spacetraders/models/market_transaction_type.py
--rw-r--r--   0        0        0     1749 2023-05-10 04:04:46.989674 spacetraders-0.1.3/spacetraders/models/meta.py
--rw-r--r--   0        0        0     1666 2023-05-10 04:04:46.969674 spacetraders-0.1.3/spacetraders/models/navigate_ship_json_body.py
--rw-r--r--   0        0        0     1943 2023-05-10 04:04:46.989674 spacetraders-0.1.3/spacetraders/models/navigate_ship_response_200.py
--rw-r--r--   0        0        0     2249 2023-05-10 04:04:47.039674 spacetraders-0.1.3/spacetraders/models/navigate_ship_response_200_data.py
--rw-r--r--   0        0        0     2106 2023-05-10 04:04:46.989674 spacetraders-0.1.3/spacetraders/models/orbit_ship_orbit_ship_200_response.py
--rw-r--r--   0        0        0     1843 2023-05-10 04:04:47.009674 spacetraders-0.1.3/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
--rw-r--r--   0        0        0     2200 2023-05-10 04:04:47.019674 spacetraders-0.1.3/spacetraders/models/patch_ship_nav_json_body.py
--rw-r--r--   0        0        0     1797 2023-05-10 04:04:47.029674 spacetraders-0.1.3/spacetraders/models/patch_ship_nav_response_200.py
--rw-r--r--   0        0        0     2218 2023-05-10 04:04:47.019674 spacetraders-0.1.3/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
--rw-r--r--   0        0        0     2662 2023-05-10 04:04:47.039674 spacetraders-0.1.3/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
--rw-r--r--   0        0        0     1774 2023-05-10 04:04:47.049674 spacetraders-0.1.3/spacetraders/models/purchase_cargo_purchase_cargo_request.py
--rw-r--r--   0        0        0     1960 2023-05-10 04:04:47.089674 spacetraders-0.1.3/spacetraders/models/purchase_ship_json_body.py
--rw-r--r--   0        0        0     1943 2023-05-10 04:04:47.039674 spacetraders-0.1.3/spacetraders/models/purchase_ship_response_201.py
--rw-r--r--   0        0        0     2553 2023-05-10 04:04:47.059674 spacetraders-0.1.3/spacetraders/models/purchase_ship_response_201_data.py
--rw-r--r--   0        0        0     1915 2023-05-10 04:04:47.049674 spacetraders-0.1.3/spacetraders/models/refuel_ship_response_200.py
--rw-r--r--   0        0        0     2198 2023-05-10 04:04:47.069674 spacetraders-0.1.3/spacetraders/models/refuel_ship_response_200_data.py
--rw-r--r--   0        0        0     1971 2023-05-10 04:04:47.049674 spacetraders-0.1.3/spacetraders/models/register_json_body.py
--rw-r--r--   0        0        0      244 2023-05-10 04:04:46.099674 spacetraders-0.1.3/spacetraders/models/register_json_body_faction.py
--rw-r--r--   0        0        0     1881 2023-05-10 04:04:47.079674 spacetraders-0.1.3/spacetraders/models/register_response_201.py
--rw-r--r--   0        0        0     2946 2023-05-10 04:04:47.099674 spacetraders-0.1.3/spacetraders/models/register_response_201_data.py
--rw-r--r--   0        0        0     5575 2023-05-10 04:04:47.149674 spacetraders-0.1.3/spacetraders/models/scanned_ship.py
--rw-r--r--   0        0        0     1560 2023-05-10 04:04:47.049674 spacetraders-0.1.3/spacetraders/models/scanned_ship_engine.py
--rw-r--r--   0        0        0     1554 2023-05-10 04:04:47.069674 spacetraders-0.1.3/spacetraders/models/scanned_ship_frame.py
--rw-r--r--   0        0        0     1580 2023-05-10 04:04:47.079674 spacetraders-0.1.3/spacetraders/models/scanned_ship_mounts_item.py
--rw-r--r--   0        0        0     1566 2023-05-10 04:04:47.079674 spacetraders-0.1.3/spacetraders/models/scanned_ship_reactor.py
--rw-r--r--   0        0        0     2390 2023-05-10 04:04:47.109674 spacetraders-0.1.3/spacetraders/models/scanned_system.py
--rw-r--r--   0        0        0     5283 2023-05-10 04:04:47.179674 spacetraders-0.1.3/spacetraders/models/scanned_waypoint.py
--rw-r--r--   0        0        0     2106 2023-05-10 04:04:47.099674 spacetraders-0.1.3/spacetraders/models/sell_cargo_sell_cargo_201_response.py
--rw-r--r--   0        0        0     2622 2023-05-10 04:04:47.129674 spacetraders-0.1.3/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
--rw-r--r--   0        0        0     1734 2023-05-10 04:04:47.099674 spacetraders-0.1.3/spacetraders/models/sell_cargo_sell_cargo_request.py
--rw-r--r--   0        0        0     6470 2023-05-10 04:04:47.199674 spacetraders-0.1.3/spacetraders/models/ship.py
--rw-r--r--   0        0        0     2590 2023-05-10 04:04:47.149674 spacetraders-0.1.3/spacetraders/models/ship_cargo.py
--rw-r--r--   0        0        0     2228 2023-05-10 04:04:47.129674 spacetraders-0.1.3/spacetraders/models/ship_cargo_item.py
--rw-r--r--   0        0        0     3202 2023-05-10 04:04:47.139674 spacetraders-0.1.3/spacetraders/models/ship_crew.py
--rw-r--r--   0        0        0      167 2023-05-10 04:04:45.979674 spacetraders-0.1.3/spacetraders/models/ship_crew_rotation.py
--rw-r--r--   0        0        0     3124 2023-05-10 04:04:47.149674 spacetraders-0.1.3/spacetraders/models/ship_engine.py
--rw-r--r--   0        0        0      319 2023-05-10 04:04:46.109674 spacetraders-0.1.3/spacetraders/models/ship_engine_symbol.py
--rw-r--r--   0        0        0     3873 2023-05-10 04:04:47.219674 spacetraders-0.1.3/spacetraders/models/ship_frame.py
--rw-r--r--   0        0        0      694 2023-05-10 04:04:45.989674 spacetraders-0.1.3/spacetraders/models/ship_frame_symbol.py
--rw-r--r--   0        0        0     2729 2023-05-10 04:04:47.169674 spacetraders-0.1.3/spacetraders/models/ship_fuel.py
--rw-r--r--   0        0        0     1943 2023-05-10 04:04:47.139674 spacetraders-0.1.3/spacetraders/models/ship_fuel_consumed.py
--rw-r--r--   0        0        0     3305 2023-05-10 04:04:47.189674 spacetraders-0.1.3/spacetraders/models/ship_module.py
--rw-r--r--   0        0        0     1033 2023-05-10 04:04:46.029674 spacetraders-0.1.3/spacetraders/models/ship_module_symbol.py
--rw-r--r--   0        0        0     3738 2023-05-10 04:04:47.199674 spacetraders-0.1.3/spacetraders/models/ship_mount.py
--rw-r--r--   0        0        0      572 2023-05-10 04:04:46.109674 spacetraders-0.1.3/spacetraders/models/ship_mount_deposits_item.py
--rw-r--r--   0        0        0      854 2023-05-10 04:04:46.109674 spacetraders-0.1.3/spacetraders/models/ship_mount_symbol.py
--rw-r--r--   0        0        0     3267 2023-05-10 04:04:47.189674 spacetraders-0.1.3/spacetraders/models/ship_nav.py
--rw-r--r--   0        0        0      206 2023-05-10 04:04:45.999674 spacetraders-0.1.3/spacetraders/models/ship_nav_flight_mode.py
--rw-r--r--   0        0        0     3062 2023-05-10 04:04:47.199674 spacetraders-0.1.3/spacetraders/models/ship_nav_route.py
--rw-r--r--   0        0        0     2310 2023-05-10 04:04:47.179674 spacetraders-0.1.3/spacetraders/models/ship_nav_route_waypoint.py
--rw-r--r--   0        0        0      196 2023-05-10 04:04:46.029674 spacetraders-0.1.3/spacetraders/models/ship_nav_status.py
--rw-r--r--   0        0        0     3227 2023-05-10 04:04:47.199674 spacetraders-0.1.3/spacetraders/models/ship_reactor.py
--rw-r--r--   0        0        0      344 2023-05-10 04:04:45.999674 spacetraders-0.1.3/spacetraders/models/ship_reactor_symbol.py
--rw-r--r--   0        0        0     1708 2023-05-10 04:04:47.179674 spacetraders-0.1.3/spacetraders/models/ship_refine_json_body.py
--rw-r--r--   0        0        0      330 2023-05-10 04:04:46.099674 spacetraders-0.1.3/spacetraders/models/ship_refine_json_body_produce.py
--rw-r--r--   0        0        0     2134 2023-05-10 04:04:47.199674 spacetraders-0.1.3/spacetraders/models/ship_refine_ship_refine_200_response.py
--rw-r--r--   0        0        0     4564 2023-05-10 04:04:47.239674 spacetraders-0.1.3/spacetraders/models/ship_refine_ship_refine_200_response_data.py
--rw-r--r--   0        0        0     2085 2023-05-10 04:04:47.209674 spacetraders-0.1.3/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
--rw-r--r--   0        0        0     2085 2023-05-10 04:04:47.209674 spacetraders-0.1.3/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
--rw-r--r--   0        0        0     2233 2023-05-10 04:04:47.209674 spacetraders-0.1.3/spacetraders/models/ship_registration.py
--rw-r--r--   0        0        0     2221 2023-05-10 04:04:47.219674 spacetraders-0.1.3/spacetraders/models/ship_requirements.py
--rw-r--r--   0        0        0      479 2023-05-10 04:04:46.089674 spacetraders-0.1.3/spacetraders/models/ship_role.py
--rw-r--r--   0        0        0      549 2023-05-10 04:04:45.989674 spacetraders-0.1.3/spacetraders/models/ship_type.py
--rw-r--r--   0        0        0     4568 2023-05-10 04:04:47.289674 spacetraders-0.1.3/spacetraders/models/shipyard.py
--rw-r--r--   0        0        0     5320 2023-05-10 04:04:47.299674 spacetraders-0.1.3/spacetraders/models/shipyard_ship.py
--rw-r--r--   0        0        0     1890 2023-05-10 04:04:47.279674 spacetraders-0.1.3/spacetraders/models/shipyard_ship_types_item.py
--rw-r--r--   0        0        0     2737 2023-05-10 04:04:47.259674 spacetraders-0.1.3/spacetraders/models/shipyard_transaction.py
--rw-r--r--   0        0        0     3608 2023-05-10 04:04:47.279674 spacetraders-0.1.3/spacetraders/models/survey.py
--rw-r--r--   0        0        0     1610 2023-05-10 04:04:47.249674 spacetraders-0.1.3/spacetraders/models/survey_deposit.py
--rw-r--r--   0        0        0      181 2023-05-10 04:04:46.009674 spacetraders-0.1.3/spacetraders/models/survey_size.py
--rw-r--r--   0        0        0     3656 2023-05-10 04:04:47.299674 spacetraders-0.1.3/spacetraders/models/system.py
--rw-r--r--   0        0        0     1513 2023-05-10 04:04:47.249674 spacetraders-0.1.3/spacetraders/models/system_faction.py
--rw-r--r--   0        0        0      405 2023-05-10 04:04:45.999674 spacetraders-0.1.3/spacetraders/models/system_type.py
--rw-r--r--   0        0        0     1993 2023-05-10 04:04:47.249674 spacetraders-0.1.3/spacetraders/models/system_waypoint.py
--rw-r--r--   0        0        0     1929 2023-05-10 04:04:47.249674 spacetraders-0.1.3/spacetraders/models/trade_good.py
--rw-r--r--   0        0        0     4422 2023-05-10 04:04:46.089674 spacetraders-0.1.3/spacetraders/models/trade_symbol.py
--rw-r--r--   0        0        0     2218 2023-05-10 04:04:47.269674 spacetraders-0.1.3/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
--rw-r--r--   0        0        0     1881 2023-05-10 04:04:47.269674 spacetraders-0.1.3/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
--rw-r--r--   0        0        0     2042 2023-05-10 04:04:47.259674 spacetraders-0.1.3/spacetraders/models/transfer_cargo_transfer_cargo_request.py
--rw-r--r--   0        0        0     1646 2023-05-10 04:04:47.269674 spacetraders-0.1.3/spacetraders/models/warp_ship_json_body.py
--rw-r--r--   0        0        0     1887 2023-05-10 04:04:47.279674 spacetraders-0.1.3/spacetraders/models/warp_ship_response_200.py
--rw-r--r--   0        0        0     2229 2023-05-10 04:04:47.289674 spacetraders-0.1.3/spacetraders/models/warp_ship_response_200_data.py
--rw-r--r--   0        0        0     5245 2023-05-10 04:04:47.329674 spacetraders-0.1.3/spacetraders/models/waypoint.py
--rw-r--r--   0        0        0     1523 2023-05-10 04:04:47.309674 spacetraders-0.1.3/spacetraders/models/waypoint_faction.py
--rw-r--r--   0        0        0     1585 2023-05-10 04:04:47.289674 spacetraders-0.1.3/spacetraders/models/waypoint_orbital.py
--rw-r--r--   0        0        0     2077 2023-05-10 04:04:47.299674 spacetraders-0.1.3/spacetraders/models/waypoint_trait.py
--rw-r--r--   0        0        0     2200 2023-05-10 04:04:46.129674 spacetraders-0.1.3/spacetraders/models/waypoint_trait_symbol.py
--rw-r--r--   0        0        0      381 2023-05-10 04:04:46.009674 spacetraders-0.1.3/spacetraders/models/waypoint_type.py
--rw-r--r--   0        0        0     1035 2023-05-10 04:04:47.289674 spacetraders-0.1.3/spacetraders/types.py
--rw-r--r--   0        0        0     3909 1970-01-01 00:00:00.000000 spacetraders-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.1.4/README.md
+-rw-r--r--   0        0        0      501 2023-05-10 04:44:30.269683 spacetraders-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      250 2023-05-10 04:44:08.369683 spacetraders-0.1.4/spacetraders/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-10 04:44:07.839682 spacetraders-0.1.4/spacetraders/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 04:44:07.879683 spacetraders-0.1.4/spacetraders/api/agents/__init__.py
+-rw-r--r--   0        0        0     3816 2023-05-10 04:44:08.429683 spacetraders-0.1.4/spacetraders/api/agents/get_my_agent.py
+-rw-r--r--   0        0        0        0 2023-05-10 04:44:07.879683 spacetraders-0.1.4/spacetraders/api/contracts/__init__.py
+-rw-r--r--   0        0        0     4288 2023-05-10 04:44:08.429683 spacetraders-0.1.4/spacetraders/api/contracts/accept_contract.py
+-rw-r--r--   0        0        0     5017 2023-05-10 04:44:08.449683 spacetraders-0.1.4/spacetraders/api/contracts/deliver_contract.py
+-rw-r--r--   0        0        0     4306 2023-05-10 04:44:08.439683 spacetraders-0.1.4/spacetraders/api/contracts/fulfill_contract.py
+-rw-r--r--   0        0        0     4287 2023-05-10 04:44:08.429683 spacetraders-0.1.4/spacetraders/api/contracts/get_contract.py
+-rw-r--r--   0        0        0     5013 2023-05-10 04:44:08.439683 spacetraders-0.1.4/spacetraders/api/contracts/get_contracts.py
+-rw-r--r--   0        0        0        0 2023-05-10 04:44:07.849683 spacetraders-0.1.4/spacetraders/api/default/__init__.py
+-rw-r--r--   0        0        0     9110 2023-05-10 04:44:08.439683 spacetraders-0.1.4/spacetraders/api/default/register.py
+-rw-r--r--   0        0        0        0 2023-05-10 04:44:07.879683 spacetraders-0.1.4/spacetraders/api/factions/__init__.py
+-rw-r--r--   0        0        0     4359 2023-05-10 04:44:08.429683 spacetraders-0.1.4/spacetraders/api/factions/get_faction.py
+-rw-r--r--   0        0        0     4983 2023-05-10 04:44:08.469683 spacetraders-0.1.4/spacetraders/api/factions/get_factions.py
+-rw-r--r--   0        0        0        0 2023-05-10 04:44:07.879683 spacetraders-0.1.4/spacetraders/api/fleet/__init__.py
+-rw-r--r--   0        0        0     5253 2023-05-10 04:44:08.449683 spacetraders-0.1.4/spacetraders/api/fleet/create_chart.py
+-rw-r--r--   0        0        0     4511 2023-05-10 04:44:08.549682 spacetraders-0.1.4/spacetraders/api/fleet/create_ship_ship_scan.py
+-rw-r--r--   0        0        0     4564 2023-05-10 04:44:08.469683 spacetraders-0.1.4/spacetraders/api/fleet/create_ship_system_scan.py
+-rw-r--r--   0        0        0     4608 2023-05-10 04:44:08.449683 spacetraders-0.1.4/spacetraders/api/fleet/create_ship_waypoint_scan.py
+-rw-r--r--   0        0        0     6211 2023-05-10 04:44:08.449683 spacetraders-0.1.4/spacetraders/api/fleet/create_survey.py
+-rw-r--r--   0        0        0     5354 2023-05-10 04:44:08.439683 spacetraders-0.1.4/spacetraders/api/fleet/dock_ship.py
+-rw-r--r--   0        0        0     5394 2023-05-10 04:44:08.459683 spacetraders-0.1.4/spacetraders/api/fleet/extract_resources.py
+-rw-r--r--   0        0        0     4234 2023-05-10 04:44:08.509683 spacetraders-0.1.4/spacetraders/api/fleet/get_my_ship.py
+-rw-r--r--   0        0        0     4336 2023-05-10 04:44:08.499683 spacetraders-0.1.4/spacetraders/api/fleet/get_my_ship_cargo.py
+-rw-r--r--   0        0        0     4968 2023-05-10 04:44:08.529682 spacetraders-0.1.4/spacetraders/api/fleet/get_my_ships.py
+-rw-r--r--   0        0        0     6388 2023-05-10 04:44:08.509683 spacetraders-0.1.4/spacetraders/api/fleet/get_ship_cooldown.py
+-rw-r--r--   0        0        0     4279 2023-05-10 04:44:08.509683 spacetraders-0.1.4/spacetraders/api/fleet/get_ship_nav.py
+-rw-r--r--   0        0        0     4872 2023-05-10 04:44:08.529682 spacetraders-0.1.4/spacetraders/api/fleet/jettison.py
+-rw-r--r--   0        0        0     5162 2023-05-10 04:44:08.509683 spacetraders-0.1.4/spacetraders/api/fleet/jump_ship.py
+-rw-r--r--   0        0        0     6798 2023-05-10 04:44:08.519683 spacetraders-0.1.4/spacetraders/api/fleet/navigate_ship.py
+-rw-r--r--   0        0        0     5329 2023-05-10 04:44:08.529682 spacetraders-0.1.4/spacetraders/api/fleet/orbit_ship.py
+-rw-r--r--   0        0        0     5002 2023-05-10 04:44:08.529682 spacetraders-0.1.4/spacetraders/api/fleet/patch_ship_nav.py
+-rw-r--r--   0        0        0     5209 2023-05-10 04:44:08.549682 spacetraders-0.1.4/spacetraders/api/fleet/purchase_cargo.py
+-rw-r--r--   0        0        0     4445 2023-05-10 04:44:08.539682 spacetraders-0.1.4/spacetraders/api/fleet/purchase_ship.py
+-rw-r--r--   0        0        0     4300 2023-05-10 04:44:08.539682 spacetraders-0.1.4/spacetraders/api/fleet/refuel_ship.py
+-rw-r--r--   0        0        0     4963 2023-05-10 04:44:08.569682 spacetraders-0.1.4/spacetraders/api/fleet/sell_cargo.py
+-rw-r--r--   0        0        0     5465 2023-05-10 04:44:08.569682 spacetraders-0.1.4/spacetraders/api/fleet/ship_refine.py
+-rw-r--r--   0        0        0     5260 2023-05-10 04:44:08.589682 spacetraders-0.1.4/spacetraders/api/fleet/transfer_cargo.py
+-rw-r--r--   0        0        0     6202 2023-05-10 04:44:08.599683 spacetraders-0.1.4/spacetraders/api/fleet/warp_ship.py
+-rw-r--r--   0        0        0        0 2023-05-10 04:44:07.869683 spacetraders-0.1.4/spacetraders/api/systems/__init__.py
+-rw-r--r--   0        0        0     4836 2023-05-10 04:44:08.589682 spacetraders-0.1.4/spacetraders/api/systems/get_jump_gate.py
+-rw-r--r--   0        0        0     5622 2023-05-10 04:44:08.579682 spacetraders-0.1.4/spacetraders/api/systems/get_market.py
+-rw-r--r--   0        0        0     4810 2023-05-10 04:44:08.589682 spacetraders-0.1.4/spacetraders/api/systems/get_shipyard.py
+-rw-r--r--   0        0        0     4396 2023-05-10 04:44:08.589682 spacetraders-0.1.4/spacetraders/api/systems/get_system.py
+-rw-r--r--   0        0        0     5942 2023-05-10 04:44:08.629683 spacetraders-0.1.4/spacetraders/api/systems/get_system_waypoints.py
+-rw-r--r--   0        0        0     4982 2023-05-10 04:44:08.629683 spacetraders-0.1.4/spacetraders/api/systems/get_systems.py
+-rw-r--r--   0        0        0     4797 2023-05-10 04:44:08.609683 spacetraders-0.1.4/spacetraders/api/systems/get_waypoint.py
+-rw-r--r--   0        0        0     4212 2023-05-10 04:44:08.629683 spacetraders-0.1.4/spacetraders/client.py
+-rw-r--r--   0        0        0      470 2023-05-10 04:44:08.549682 spacetraders-0.1.4/spacetraders/errors.py
+-rw-r--r--   0        0        0    13081 2023-05-10 04:44:08.739683 spacetraders-0.1.4/spacetraders/models/__init__.py
+-rw-r--r--   0        0        0     2021 2023-05-10 04:44:08.589682 spacetraders-0.1.4/spacetraders/models/accept_contract_response_200.py
+-rw-r--r--   0        0        0     2138 2023-05-10 04:44:08.629683 spacetraders-0.1.4/spacetraders/models/accept_contract_response_200_data.py
+-rw-r--r--   0        0        0     2216 2023-05-10 04:44:08.619683 spacetraders-0.1.4/spacetraders/models/agent.py
+-rw-r--r--   0        0        0     2735 2023-05-10 04:44:08.639683 spacetraders-0.1.4/spacetraders/models/chart.py
+-rw-r--r--   0        0        0     2817 2023-05-10 04:44:08.659683 spacetraders-0.1.4/spacetraders/models/connected_system.py
+-rw-r--r--   0        0        0     3209 2023-05-10 04:44:08.669683 spacetraders-0.1.4/spacetraders/models/contract.py
+-rw-r--r--   0        0        0     2675 2023-05-10 04:44:08.659683 spacetraders-0.1.4/spacetraders/models/contract_deliver_good.py
+-rw-r--r--   0        0        0     1922 2023-05-10 04:44:08.669683 spacetraders-0.1.4/spacetraders/models/contract_payment.py
+-rw-r--r--   0        0        0     3089 2023-05-10 04:44:08.679683 spacetraders-0.1.4/spacetraders/models/contract_terms.py
+-rw-r--r--   0        0        0      201 2023-05-10 04:44:08.009683 spacetraders-0.1.4/spacetraders/models/contract_type.py
+-rw-r--r--   0        0        0     2629 2023-05-10 04:44:08.679683 spacetraders-0.1.4/spacetraders/models/cooldown.py
+-rw-r--r--   0        0        0     1929 2023-05-10 04:44:08.709683 spacetraders-0.1.4/spacetraders/models/create_chart_response_201.py
+-rw-r--r--   0        0        0     2299 2023-05-10 04:44:08.719683 spacetraders-0.1.4/spacetraders/models/create_chart_response_201_data.py
+-rw-r--r--   0        0        0     2106 2023-05-10 04:44:08.719683 spacetraders-0.1.4/spacetraders/models/create_ship_ship_scan_response_201.py
+-rw-r--r--   0        0        0     2566 2023-05-10 04:44:08.699683 spacetraders-0.1.4/spacetraders/models/create_ship_ship_scan_response_201_data.py
+-rw-r--r--   0        0        0     2134 2023-05-10 04:44:08.689683 spacetraders-0.1.4/spacetraders/models/create_ship_system_scan_response_201.py
+-rw-r--r--   0        0        0     2638 2023-05-10 04:44:08.689683 spacetraders-0.1.4/spacetraders/models/create_ship_system_scan_response_201_data.py
+-rw-r--r--   0        0        0     2162 2023-05-10 04:44:08.699683 spacetraders-0.1.4/spacetraders/models/create_ship_waypoint_scan_response_201.py
+-rw-r--r--   0        0        0     2710 2023-05-10 04:44:08.719683 spacetraders-0.1.4/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
+-rw-r--r--   0        0        0     1943 2023-05-10 04:44:08.709683 spacetraders-0.1.4/spacetraders/models/create_survey_response_201.py
+-rw-r--r--   0        0        0     2526 2023-05-10 04:44:08.709683 spacetraders-0.1.4/spacetraders/models/create_survey_response_201_data.py
+-rw-r--r--   0        0        0     1989 2023-05-10 04:44:08.739683 spacetraders-0.1.4/spacetraders/models/deliver_contract_json_body.py
+-rw-r--r--   0        0        0     2052 2023-05-10 04:44:08.709683 spacetraders-0.1.4/spacetraders/models/deliver_contract_response_200.py
+-rw-r--r--   0        0        0     2182 2023-05-10 04:44:08.739683 spacetraders-0.1.4/spacetraders/models/deliver_contract_response_200_data.py
+-rw-r--r--   0        0        0     2078 2023-05-10 04:44:08.729683 spacetraders-0.1.4/spacetraders/models/dock_ship_dock_ship_200_response.py
+-rw-r--r--   0        0        0     1833 2023-05-10 04:44:08.719683 spacetraders-0.1.4/spacetraders/models/dock_ship_dock_ship_200_response_data.py
+-rw-r--r--   0        0        0     2215 2023-05-10 04:44:08.759683 spacetraders-0.1.4/spacetraders/models/extract_resources_json_body.py
+-rw-r--r--   0        0        0     2066 2023-05-10 04:44:08.739683 spacetraders-0.1.4/spacetraders/models/extract_resources_response_201.py
+-rw-r--r--   0        0        0     2666 2023-05-10 04:44:08.759683 spacetraders-0.1.4/spacetraders/models/extract_resources_response_201_data.py
+-rw-r--r--   0        0        0     1980 2023-05-10 04:44:08.749683 spacetraders-0.1.4/spacetraders/models/extraction.py
+-rw-r--r--   0        0        0     1750 2023-05-10 04:44:08.759683 spacetraders-0.1.4/spacetraders/models/extraction_yield.py
+-rw-r--r--   0        0        0     2746 2023-05-10 04:44:08.779682 spacetraders-0.1.4/spacetraders/models/faction.py
+-rw-r--r--   0        0        0     2067 2023-05-10 04:44:08.779682 spacetraders-0.1.4/spacetraders/models/faction_trait.py
+-rw-r--r--   0        0        0     2091 2023-05-10 04:44:08.119683 spacetraders-0.1.4/spacetraders/models/faction_trait_symbol.py
+-rw-r--r--   0        0        0     2052 2023-05-10 04:44:08.769683 spacetraders-0.1.4/spacetraders/models/fulfill_contract_response_200.py
+-rw-r--r--   0        0        0     2143 2023-05-10 04:44:08.769683 spacetraders-0.1.4/spacetraders/models/fulfill_contract_response_200_data.py
+-rw-r--r--   0        0        0     1755 2023-05-10 04:44:08.829682 spacetraders-0.1.4/spacetraders/models/get_contract_response_200.py
+-rw-r--r--   0        0        0     2300 2023-05-10 04:44:08.799682 spacetraders-0.1.4/spacetraders/models/get_contracts_response_200.py
+-rw-r--r--   0        0        0     1741 2023-05-10 04:44:08.769683 spacetraders-0.1.4/spacetraders/models/get_faction_response_200.py
+-rw-r--r--   0        0        0     2286 2023-05-10 04:44:08.809682 spacetraders-0.1.4/spacetraders/models/get_factions_response_200.py
+-rw-r--r--   0        0        0     1761 2023-05-10 04:44:08.789682 spacetraders-0.1.4/spacetraders/models/get_jump_gate_response_200.py
+-rw-r--r--   0        0        0     1727 2023-05-10 04:44:08.809682 spacetraders-0.1.4/spacetraders/models/get_market_response_200.py
+-rw-r--r--   0        0        0     1726 2023-05-10 04:44:08.789682 spacetraders-0.1.4/spacetraders/models/get_my_agent_response_200.py
+-rw-r--r--   0        0        0     1788 2023-05-10 04:44:08.839682 spacetraders-0.1.4/spacetraders/models/get_my_ship_cargo_response_200.py
+-rw-r--r--   0        0        0     1719 2023-05-10 04:44:08.789682 spacetraders-0.1.4/spacetraders/models/get_my_ship_response_200.py
+-rw-r--r--   0        0        0     2257 2023-05-10 04:44:08.839682 spacetraders-0.1.4/spacetraders/models/get_my_ships_response_200.py
+-rw-r--r--   0        0        0     1857 2023-05-10 04:44:08.809682 spacetraders-0.1.4/spacetraders/models/get_ship_cooldown_response_200.py
+-rw-r--r--   0        0        0     1787 2023-05-10 04:44:08.809682 spacetraders-0.1.4/spacetraders/models/get_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1755 2023-05-10 04:44:08.799682 spacetraders-0.1.4/spacetraders/models/get_shipyard_response_200.py
+-rw-r--r--   0        0        0     1727 2023-05-10 04:44:08.809682 spacetraders-0.1.4/spacetraders/models/get_system_response_200.py
+-rw-r--r--   0        0        0     2333 2023-05-10 04:44:08.839682 spacetraders-0.1.4/spacetraders/models/get_system_waypoints_response_200.py
+-rw-r--r--   0        0        0     2272 2023-05-10 04:44:08.839682 spacetraders-0.1.4/spacetraders/models/get_systems_response_200.py
+-rw-r--r--   0        0        0     1846 2023-05-10 04:44:08.819682 spacetraders-0.1.4/spacetraders/models/get_waypoint_response_200.py
+-rw-r--r--   0        0        0     1683 2023-05-10 04:44:08.859683 spacetraders-0.1.4/spacetraders/models/jettison_json_body.py
+-rw-r--r--   0        0        0     1881 2023-05-10 04:44:08.839682 spacetraders-0.1.4/spacetraders/models/jettison_response_200.py
+-rw-r--r--   0        0        0     1782 2023-05-10 04:44:08.859683 spacetraders-0.1.4/spacetraders/models/jettison_response_200_data.py
+-rw-r--r--   0        0        0     3023 2023-05-10 04:44:08.859683 spacetraders-0.1.4/spacetraders/models/jump_gate.py
+-rw-r--r--   0        0        0     1632 2023-05-10 04:44:08.839682 spacetraders-0.1.4/spacetraders/models/jump_ship_json_body.py
+-rw-r--r--   0        0        0     1887 2023-05-10 04:44:08.869683 spacetraders-0.1.4/spacetraders/models/jump_ship_response_200.py
+-rw-r--r--   0        0        0     2550 2023-05-10 04:44:08.869683 spacetraders-0.1.4/spacetraders/models/jump_ship_response_200_data.py
+-rw-r--r--   0        0        0     5804 2023-05-10 04:44:08.939683 spacetraders-0.1.4/spacetraders/models/market.py
+-rw-r--r--   0        0        0     2843 2023-05-10 04:44:08.919683 spacetraders-0.1.4/spacetraders/models/market_trade_good.py
+-rw-r--r--   0        0        0      224 2023-05-10 04:44:08.019683 spacetraders-0.1.4/spacetraders/models/market_trade_good_supply.py
+-rw-r--r--   0        0        0     3546 2023-05-10 04:44:08.879683 spacetraders-0.1.4/spacetraders/models/market_transaction.py
+-rw-r--r--   0        0        0      170 2023-05-10 04:44:08.019683 spacetraders-0.1.4/spacetraders/models/market_transaction_type.py
+-rw-r--r--   0        0        0     1749 2023-05-10 04:44:08.859683 spacetraders-0.1.4/spacetraders/models/meta.py
+-rw-r--r--   0        0        0     1666 2023-05-10 04:44:08.899683 spacetraders-0.1.4/spacetraders/models/navigate_ship_json_body.py
+-rw-r--r--   0        0        0     1943 2023-05-10 04:44:08.899683 spacetraders-0.1.4/spacetraders/models/navigate_ship_response_200.py
+-rw-r--r--   0        0        0     2249 2023-05-10 04:44:08.879683 spacetraders-0.1.4/spacetraders/models/navigate_ship_response_200_data.py
+-rw-r--r--   0        0        0     2106 2023-05-10 04:44:08.909683 spacetraders-0.1.4/spacetraders/models/orbit_ship_orbit_ship_200_response.py
+-rw-r--r--   0        0        0     1843 2023-05-10 04:44:08.889683 spacetraders-0.1.4/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
+-rw-r--r--   0        0        0     2200 2023-05-10 04:44:08.889683 spacetraders-0.1.4/spacetraders/models/patch_ship_nav_json_body.py
+-rw-r--r--   0        0        0     1797 2023-05-10 04:44:08.879683 spacetraders-0.1.4/spacetraders/models/patch_ship_nav_response_200.py
+-rw-r--r--   0        0        0     2218 2023-05-10 04:44:08.899683 spacetraders-0.1.4/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
+-rw-r--r--   0        0        0     2662 2023-05-10 04:44:08.939683 spacetraders-0.1.4/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1774 2023-05-10 04:44:08.909683 spacetraders-0.1.4/spacetraders/models/purchase_cargo_purchase_cargo_request.py
+-rw-r--r--   0        0        0     1960 2023-05-10 04:44:08.929683 spacetraders-0.1.4/spacetraders/models/purchase_ship_json_body.py
+-rw-r--r--   0        0        0     1943 2023-05-10 04:44:08.919683 spacetraders-0.1.4/spacetraders/models/purchase_ship_response_201.py
+-rw-r--r--   0        0        0     2553 2023-05-10 04:44:08.939683 spacetraders-0.1.4/spacetraders/models/purchase_ship_response_201_data.py
+-rw-r--r--   0        0        0     1915 2023-05-10 04:44:08.929683 spacetraders-0.1.4/spacetraders/models/refuel_ship_response_200.py
+-rw-r--r--   0        0        0     2198 2023-05-10 04:44:08.929683 spacetraders-0.1.4/spacetraders/models/refuel_ship_response_200_data.py
+-rw-r--r--   0        0        0     1971 2023-05-10 04:44:08.929683 spacetraders-0.1.4/spacetraders/models/register_json_body.py
+-rw-r--r--   0        0        0      244 2023-05-10 04:44:08.099683 spacetraders-0.1.4/spacetraders/models/register_json_body_faction.py
+-rw-r--r--   0        0        0     1881 2023-05-10 04:44:08.949683 spacetraders-0.1.4/spacetraders/models/register_response_201.py
+-rw-r--r--   0        0        0     2946 2023-05-10 04:44:08.959683 spacetraders-0.1.4/spacetraders/models/register_response_201_data.py
+-rw-r--r--   0        0        0     5575 2023-05-10 04:44:09.029682 spacetraders-0.1.4/spacetraders/models/scanned_ship.py
+-rw-r--r--   0        0        0     1560 2023-05-10 04:44:08.959683 spacetraders-0.1.4/spacetraders/models/scanned_ship_engine.py
+-rw-r--r--   0        0        0     1554 2023-05-10 04:44:08.979683 spacetraders-0.1.4/spacetraders/models/scanned_ship_frame.py
+-rw-r--r--   0        0        0     1580 2023-05-10 04:44:08.949683 spacetraders-0.1.4/spacetraders/models/scanned_ship_mounts_item.py
+-rw-r--r--   0        0        0     1566 2023-05-10 04:44:08.959683 spacetraders-0.1.4/spacetraders/models/scanned_ship_reactor.py
+-rw-r--r--   0        0        0     2390 2023-05-10 04:44:08.989683 spacetraders-0.1.4/spacetraders/models/scanned_system.py
+-rw-r--r--   0        0        0     5283 2023-05-10 04:44:09.089682 spacetraders-0.1.4/spacetraders/models/scanned_waypoint.py
+-rw-r--r--   0        0        0     2106 2023-05-10 04:44:08.979683 spacetraders-0.1.4/spacetraders/models/sell_cargo_sell_cargo_201_response.py
+-rw-r--r--   0        0        0     2622 2023-05-10 04:44:08.979683 spacetraders-0.1.4/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1734 2023-05-10 04:44:09.009683 spacetraders-0.1.4/spacetraders/models/sell_cargo_sell_cargo_request.py
+-rw-r--r--   0        0        0     6470 2023-05-10 04:44:09.049682 spacetraders-0.1.4/spacetraders/models/ship.py
+-rw-r--r--   0        0        0     2590 2023-05-10 04:44:08.999683 spacetraders-0.1.4/spacetraders/models/ship_cargo.py
+-rw-r--r--   0        0        0     2228 2023-05-10 04:44:08.999683 spacetraders-0.1.4/spacetraders/models/ship_cargo_item.py
+-rw-r--r--   0        0        0     3202 2023-05-10 04:44:09.019683 spacetraders-0.1.4/spacetraders/models/ship_crew.py
+-rw-r--r--   0        0        0      167 2023-05-10 04:44:07.969683 spacetraders-0.1.4/spacetraders/models/ship_crew_rotation.py
+-rw-r--r--   0        0        0     3124 2023-05-10 04:44:09.009683 spacetraders-0.1.4/spacetraders/models/ship_engine.py
+-rw-r--r--   0        0        0      319 2023-05-10 04:44:08.109683 spacetraders-0.1.4/spacetraders/models/ship_engine_symbol.py
+-rw-r--r--   0        0        0     3873 2023-05-10 04:44:09.049682 spacetraders-0.1.4/spacetraders/models/ship_frame.py
+-rw-r--r--   0        0        0      694 2023-05-10 04:44:07.989683 spacetraders-0.1.4/spacetraders/models/ship_frame_symbol.py
+-rw-r--r--   0        0        0     2729 2023-05-10 04:44:09.069682 spacetraders-0.1.4/spacetraders/models/ship_fuel.py
+-rw-r--r--   0        0        0     1943 2023-05-10 04:44:09.019683 spacetraders-0.1.4/spacetraders/models/ship_fuel_consumed.py
+-rw-r--r--   0        0        0     3305 2023-05-10 04:44:09.059682 spacetraders-0.1.4/spacetraders/models/ship_module.py
+-rw-r--r--   0        0        0     1033 2023-05-10 04:44:08.029682 spacetraders-0.1.4/spacetraders/models/ship_module_symbol.py
+-rw-r--r--   0        0        0     3738 2023-05-10 04:44:09.089682 spacetraders-0.1.4/spacetraders/models/ship_mount.py
+-rw-r--r--   0        0        0      572 2023-05-10 04:44:08.109683 spacetraders-0.1.4/spacetraders/models/ship_mount_deposits_item.py
+-rw-r--r--   0        0        0      854 2023-05-10 04:44:08.109683 spacetraders-0.1.4/spacetraders/models/ship_mount_symbol.py
+-rw-r--r--   0        0        0     3267 2023-05-10 04:44:09.039682 spacetraders-0.1.4/spacetraders/models/ship_nav.py
+-rw-r--r--   0        0        0      206 2023-05-10 04:44:07.999683 spacetraders-0.1.4/spacetraders/models/ship_nav_flight_mode.py
+-rw-r--r--   0        0        0     3062 2023-05-10 04:44:09.069682 spacetraders-0.1.4/spacetraders/models/ship_nav_route.py
+-rw-r--r--   0        0        0     2310 2023-05-10 04:44:09.059682 spacetraders-0.1.4/spacetraders/models/ship_nav_route_waypoint.py
+-rw-r--r--   0        0        0      196 2023-05-10 04:44:08.019683 spacetraders-0.1.4/spacetraders/models/ship_nav_status.py
+-rw-r--r--   0        0        0     3227 2023-05-10 04:44:09.059682 spacetraders-0.1.4/spacetraders/models/ship_reactor.py
+-rw-r--r--   0        0        0      344 2023-05-10 04:44:07.999683 spacetraders-0.1.4/spacetraders/models/ship_reactor_symbol.py
+-rw-r--r--   0        0        0     1708 2023-05-10 04:44:09.059682 spacetraders-0.1.4/spacetraders/models/ship_refine_json_body.py
+-rw-r--r--   0        0        0      330 2023-05-10 04:44:08.099683 spacetraders-0.1.4/spacetraders/models/ship_refine_json_body_produce.py
+-rw-r--r--   0        0        0     2134 2023-05-10 04:44:09.059682 spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response.py
+-rw-r--r--   0        0        0     4564 2023-05-10 04:44:09.149683 spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response_data.py
+-rw-r--r--   0        0        0     2085 2023-05-10 04:44:09.059682 spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
+-rw-r--r--   0        0        0     2085 2023-05-10 04:44:09.069682 spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
+-rw-r--r--   0        0        0     2233 2023-05-10 04:44:09.079682 spacetraders-0.1.4/spacetraders/models/ship_registration.py
+-rw-r--r--   0        0        0     2221 2023-05-10 04:44:09.089682 spacetraders-0.1.4/spacetraders/models/ship_requirements.py
+-rw-r--r--   0        0        0      479 2023-05-10 04:44:08.089682 spacetraders-0.1.4/spacetraders/models/ship_role.py
+-rw-r--r--   0        0        0      549 2023-05-10 04:44:07.989683 spacetraders-0.1.4/spacetraders/models/ship_type.py
+-rw-r--r--   0        0        0     4568 2023-05-10 04:44:09.139683 spacetraders-0.1.4/spacetraders/models/shipyard.py
+-rw-r--r--   0        0        0     5320 2023-05-10 04:44:09.169683 spacetraders-0.1.4/spacetraders/models/shipyard_ship.py
+-rw-r--r--   0        0        0     1890 2023-05-10 04:44:09.099683 spacetraders-0.1.4/spacetraders/models/shipyard_ship_types_item.py
+-rw-r--r--   0        0        0     2737 2023-05-10 04:44:09.119683 spacetraders-0.1.4/spacetraders/models/shipyard_transaction.py
+-rw-r--r--   0        0        0     3608 2023-05-10 04:44:09.139683 spacetraders-0.1.4/spacetraders/models/survey.py
+-rw-r--r--   0        0        0     1610 2023-05-10 04:44:09.119683 spacetraders-0.1.4/spacetraders/models/survey_deposit.py
+-rw-r--r--   0        0        0      181 2023-05-10 04:44:07.999683 spacetraders-0.1.4/spacetraders/models/survey_size.py
+-rw-r--r--   0        0        0     3656 2023-05-10 04:44:09.139683 spacetraders-0.1.4/spacetraders/models/system.py
+-rw-r--r--   0        0        0     1513 2023-05-10 04:44:09.109683 spacetraders-0.1.4/spacetraders/models/system_faction.py
+-rw-r--r--   0        0        0      405 2023-05-10 04:44:07.999683 spacetraders-0.1.4/spacetraders/models/system_type.py
+-rw-r--r--   0        0        0     1993 2023-05-10 04:44:09.149683 spacetraders-0.1.4/spacetraders/models/system_waypoint.py
+-rw-r--r--   0        0        0     1929 2023-05-10 04:44:09.129683 spacetraders-0.1.4/spacetraders/models/trade_good.py
+-rw-r--r--   0        0        0     4422 2023-05-10 04:44:08.089682 spacetraders-0.1.4/spacetraders/models/trade_symbol.py
+-rw-r--r--   0        0        0     2218 2023-05-10 04:44:09.119683 spacetraders-0.1.4/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
+-rw-r--r--   0        0        0     1881 2023-05-10 04:44:09.139683 spacetraders-0.1.4/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
+-rw-r--r--   0        0        0     2042 2023-05-10 04:44:09.159683 spacetraders-0.1.4/spacetraders/models/transfer_cargo_transfer_cargo_request.py
+-rw-r--r--   0        0        0     1646 2023-05-10 04:44:09.149683 spacetraders-0.1.4/spacetraders/models/warp_ship_json_body.py
+-rw-r--r--   0        0        0     1887 2023-05-10 04:44:09.149683 spacetraders-0.1.4/spacetraders/models/warp_ship_response_200.py
+-rw-r--r--   0        0        0     2229 2023-05-10 04:44:09.159683 spacetraders-0.1.4/spacetraders/models/warp_ship_response_200_data.py
+-rw-r--r--   0        0        0     5245 2023-05-10 04:44:09.199683 spacetraders-0.1.4/spacetraders/models/waypoint.py
+-rw-r--r--   0        0        0     1523 2023-05-10 04:44:09.159683 spacetraders-0.1.4/spacetraders/models/waypoint_faction.py
+-rw-r--r--   0        0        0     1585 2023-05-10 04:44:09.169683 spacetraders-0.1.4/spacetraders/models/waypoint_orbital.py
+-rw-r--r--   0        0        0     2077 2023-05-10 04:44:09.169683 spacetraders-0.1.4/spacetraders/models/waypoint_trait.py
+-rw-r--r--   0        0        0     2200 2023-05-10 04:44:08.119683 spacetraders-0.1.4/spacetraders/models/waypoint_trait_symbol.py
+-rw-r--r--   0        0        0      381 2023-05-10 04:44:07.999683 spacetraders-0.1.4/spacetraders/models/waypoint_type.py
+-rw-r--r--   0        0        0     1035 2023-05-10 04:44:09.159683 spacetraders-0.1.4/spacetraders/types.py
+-rw-r--r--   0        0        0     3909 1970-01-01 00:00:00.000000 spacetraders-0.1.4/PKG-INFO
```

### Comparing `spacetraders-0.1.3/README.md` & `spacetraders-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/agents/get_my_agent.py` & `spacetraders-0.1.4/spacetraders/api/agents/get_my_agent.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/contracts/accept_contract.py` & `spacetraders-0.1.4/spacetraders/api/contracts/accept_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/contracts/deliver_contract.py` & `spacetraders-0.1.4/spacetraders/api/contracts/deliver_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/contracts/fulfill_contract.py` & `spacetraders-0.1.4/spacetraders/api/contracts/fulfill_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/contracts/get_contract.py` & `spacetraders-0.1.4/spacetraders/api/contracts/get_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/contracts/get_contracts.py` & `spacetraders-0.1.4/spacetraders/api/contracts/get_contracts.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/default/register.py` & `spacetraders-0.1.4/spacetraders/api/default/register.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/factions/get_faction.py` & `spacetraders-0.1.4/spacetraders/api/factions/get_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/factions/get_factions.py` & `spacetraders-0.1.4/spacetraders/api/factions/get_factions.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/create_chart.py` & `spacetraders-0.1.4/spacetraders/api/fleet/create_chart.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/create_ship_ship_scan.py` & `spacetraders-0.1.4/spacetraders/api/fleet/create_ship_ship_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/create_ship_system_scan.py` & `spacetraders-0.1.4/spacetraders/api/fleet/create_ship_system_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/create_ship_waypoint_scan.py` & `spacetraders-0.1.4/spacetraders/api/fleet/create_ship_waypoint_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/create_survey.py` & `spacetraders-0.1.4/spacetraders/api/fleet/create_survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/dock_ship.py` & `spacetraders-0.1.4/spacetraders/api/fleet/dock_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/extract_resources.py` & `spacetraders-0.1.4/spacetraders/api/fleet/extract_resources.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/get_my_ship.py` & `spacetraders-0.1.4/spacetraders/api/fleet/get_my_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/get_my_ship_cargo.py` & `spacetraders-0.1.4/spacetraders/api/fleet/get_my_ship_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/get_my_ships.py` & `spacetraders-0.1.4/spacetraders/api/fleet/get_my_ships.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/get_ship_cooldown.py` & `spacetraders-0.1.4/spacetraders/api/fleet/get_ship_cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/get_ship_nav.py` & `spacetraders-0.1.4/spacetraders/api/fleet/get_ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/jettison.py` & `spacetraders-0.1.4/spacetraders/api/fleet/jettison.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/jump_ship.py` & `spacetraders-0.1.4/spacetraders/api/fleet/jump_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/navigate_ship.py` & `spacetraders-0.1.4/spacetraders/api/fleet/navigate_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/orbit_ship.py` & `spacetraders-0.1.4/spacetraders/api/fleet/orbit_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/patch_ship_nav.py` & `spacetraders-0.1.4/spacetraders/api/fleet/patch_ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/purchase_cargo.py` & `spacetraders-0.1.4/spacetraders/api/fleet/purchase_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/purchase_ship.py` & `spacetraders-0.1.4/spacetraders/api/fleet/purchase_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/refuel_ship.py` & `spacetraders-0.1.4/spacetraders/api/fleet/refuel_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/sell_cargo.py` & `spacetraders-0.1.4/spacetraders/api/fleet/sell_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/ship_refine.py` & `spacetraders-0.1.4/spacetraders/api/fleet/ship_refine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/transfer_cargo.py` & `spacetraders-0.1.4/spacetraders/api/fleet/transfer_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/fleet/warp_ship.py` & `spacetraders-0.1.4/spacetraders/api/fleet/warp_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/systems/get_jump_gate.py` & `spacetraders-0.1.4/spacetraders/api/systems/get_jump_gate.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/systems/get_market.py` & `spacetraders-0.1.4/spacetraders/api/systems/get_market.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/systems/get_shipyard.py` & `spacetraders-0.1.4/spacetraders/api/systems/get_shipyard.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/systems/get_system.py` & `spacetraders-0.1.4/spacetraders/api/systems/get_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/systems/get_system_waypoints.py` & `spacetraders-0.1.4/spacetraders/api/systems/get_system_waypoints.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/systems/get_systems.py` & `spacetraders-0.1.4/spacetraders/api/systems/get_systems.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/api/systems/get_waypoint.py` & `spacetraders-0.1.4/spacetraders/api/systems/get_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/client.py` & `spacetraders-0.1.4/spacetraders/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 import attr
 
 
 class APIStub:
     """A module importer that traverses the api directory based on getattr"""
 
-    def __init__(self, client, mod, exec):
+    def __init__(self, client, mod, exec_mode):
         self._module = mod
         self._client = client
-        self._exec_mode = exec
+        self._exec_mode = exec_mode
 
     def __getattr__(self, attr):
         if not hasattr(self._module, attr):
             imp = import_module(f".{attr}", self._module.__package__)
         else:
             imp = getattr(self._module, attr)
```

### Comparing `spacetraders-0.1.3/spacetraders/models/__init__.py` & `spacetraders-0.1.4/spacetraders/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/accept_contract_response_200.py` & `spacetraders-0.1.4/spacetraders/models/accept_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/accept_contract_response_200_data.py` & `spacetraders-0.1.4/spacetraders/models/accept_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/agent.py` & `spacetraders-0.1.4/spacetraders/models/agent.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/chart.py` & `spacetraders-0.1.4/spacetraders/models/chart.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/connected_system.py` & `spacetraders-0.1.4/spacetraders/models/connected_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/contract.py` & `spacetraders-0.1.4/spacetraders/models/contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/contract_deliver_good.py` & `spacetraders-0.1.4/spacetraders/models/contract_deliver_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/contract_payment.py` & `spacetraders-0.1.4/spacetraders/models/contract_payment.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/contract_terms.py` & `spacetraders-0.1.4/spacetraders/models/contract_terms.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/cooldown.py` & `spacetraders-0.1.4/spacetraders/models/cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/create_chart_response_201.py` & `spacetraders-0.1.4/spacetraders/models/create_chart_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/create_chart_response_201_data.py` & `spacetraders-0.1.4/spacetraders/models/create_chart_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/create_ship_ship_scan_response_201.py` & `spacetraders-0.1.4/spacetraders/models/create_ship_ship_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/create_ship_ship_scan_response_201_data.py` & `spacetraders-0.1.4/spacetraders/models/create_ship_ship_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/create_ship_system_scan_response_201.py` & `spacetraders-0.1.4/spacetraders/models/create_ship_system_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/create_ship_system_scan_response_201_data.py` & `spacetraders-0.1.4/spacetraders/models/create_ship_system_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/create_ship_waypoint_scan_response_201.py` & `spacetraders-0.1.4/spacetraders/models/create_ship_waypoint_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/create_ship_waypoint_scan_response_201_data.py` & `spacetraders-0.1.4/spacetraders/models/create_ship_waypoint_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/create_survey_response_201.py` & `spacetraders-0.1.4/spacetraders/models/create_survey_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/create_survey_response_201_data.py` & `spacetraders-0.1.4/spacetraders/models/create_survey_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/deliver_contract_json_body.py` & `spacetraders-0.1.4/spacetraders/models/deliver_contract_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/deliver_contract_response_200.py` & `spacetraders-0.1.4/spacetraders/models/deliver_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/deliver_contract_response_200_data.py` & `spacetraders-0.1.4/spacetraders/models/deliver_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/dock_ship_dock_ship_200_response.py` & `spacetraders-0.1.4/spacetraders/models/dock_ship_dock_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/dock_ship_dock_ship_200_response_data.py` & `spacetraders-0.1.4/spacetraders/models/dock_ship_dock_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/extract_resources_json_body.py` & `spacetraders-0.1.4/spacetraders/models/extract_resources_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/extract_resources_response_201.py` & `spacetraders-0.1.4/spacetraders/models/extract_resources_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/extract_resources_response_201_data.py` & `spacetraders-0.1.4/spacetraders/models/extract_resources_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/extraction.py` & `spacetraders-0.1.4/spacetraders/models/extraction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/extraction_yield.py` & `spacetraders-0.1.4/spacetraders/models/extraction_yield.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/faction.py` & `spacetraders-0.1.4/spacetraders/models/faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/faction_trait.py` & `spacetraders-0.1.4/spacetraders/models/faction_trait.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/faction_trait_symbol.py` & `spacetraders-0.1.4/spacetraders/models/faction_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/fulfill_contract_response_200.py` & `spacetraders-0.1.4/spacetraders/models/fulfill_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/fulfill_contract_response_200_data.py` & `spacetraders-0.1.4/spacetraders/models/fulfill_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_contract_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_contracts_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_contracts_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_faction_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_faction_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_factions_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_factions_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_jump_gate_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_jump_gate_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_market_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_market_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_my_agent_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_my_agent_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_my_ship_cargo_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_my_ship_cargo_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_my_ship_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_my_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_my_ships_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_my_ships_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_ship_cooldown_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_ship_cooldown_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_ship_nav_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_shipyard_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_shipyard_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_system_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_system_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_system_waypoints_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_system_waypoints_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_systems_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_systems_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/get_waypoint_response_200.py` & `spacetraders-0.1.4/spacetraders/models/get_waypoint_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/jettison_json_body.py` & `spacetraders-0.1.4/spacetraders/models/jettison_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/jettison_response_200.py` & `spacetraders-0.1.4/spacetraders/models/jettison_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/jettison_response_200_data.py` & `spacetraders-0.1.4/spacetraders/models/jettison_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/jump_gate.py` & `spacetraders-0.1.4/spacetraders/models/jump_gate.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/jump_ship_json_body.py` & `spacetraders-0.1.4/spacetraders/models/jump_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/jump_ship_response_200.py` & `spacetraders-0.1.4/spacetraders/models/jump_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/jump_ship_response_200_data.py` & `spacetraders-0.1.4/spacetraders/models/jump_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/market.py` & `spacetraders-0.1.4/spacetraders/models/market.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/market_trade_good.py` & `spacetraders-0.1.4/spacetraders/models/market_trade_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/market_transaction.py` & `spacetraders-0.1.4/spacetraders/models/market_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/meta.py` & `spacetraders-0.1.4/spacetraders/models/meta.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/navigate_ship_json_body.py` & `spacetraders-0.1.4/spacetraders/models/navigate_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/navigate_ship_response_200.py` & `spacetraders-0.1.4/spacetraders/models/navigate_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/navigate_ship_response_200_data.py` & `spacetraders-0.1.4/spacetraders/models/navigate_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/orbit_ship_orbit_ship_200_response.py` & `spacetraders-0.1.4/spacetraders/models/orbit_ship_orbit_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py` & `spacetraders-0.1.4/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/patch_ship_nav_json_body.py` & `spacetraders-0.1.4/spacetraders/models/patch_ship_nav_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/patch_ship_nav_response_200.py` & `spacetraders-0.1.4/spacetraders/models/patch_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py` & `spacetraders-0.1.4/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py` & `spacetraders-0.1.4/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/purchase_cargo_purchase_cargo_request.py` & `spacetraders-0.1.4/spacetraders/models/purchase_cargo_purchase_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/purchase_ship_json_body.py` & `spacetraders-0.1.4/spacetraders/models/purchase_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/purchase_ship_response_201.py` & `spacetraders-0.1.4/spacetraders/models/purchase_ship_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/purchase_ship_response_201_data.py` & `spacetraders-0.1.4/spacetraders/models/purchase_ship_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/refuel_ship_response_200.py` & `spacetraders-0.1.4/spacetraders/models/refuel_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/refuel_ship_response_200_data.py` & `spacetraders-0.1.4/spacetraders/models/refuel_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/register_json_body.py` & `spacetraders-0.1.4/spacetraders/models/register_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/register_response_201.py` & `spacetraders-0.1.4/spacetraders/models/register_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/register_response_201_data.py` & `spacetraders-0.1.4/spacetraders/models/register_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/scanned_ship.py` & `spacetraders-0.1.4/spacetraders/models/scanned_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/scanned_ship_engine.py` & `spacetraders-0.1.4/spacetraders/models/scanned_ship_engine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/scanned_ship_frame.py` & `spacetraders-0.1.4/spacetraders/models/scanned_ship_frame.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/scanned_ship_mounts_item.py` & `spacetraders-0.1.4/spacetraders/models/scanned_ship_mounts_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/scanned_ship_reactor.py` & `spacetraders-0.1.4/spacetraders/models/scanned_ship_reactor.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/scanned_system.py` & `spacetraders-0.1.4/spacetraders/models/scanned_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/scanned_waypoint.py` & `spacetraders-0.1.4/spacetraders/models/scanned_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/sell_cargo_sell_cargo_201_response.py` & `spacetraders-0.1.4/spacetraders/models/sell_cargo_sell_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py` & `spacetraders-0.1.4/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/sell_cargo_sell_cargo_request.py` & `spacetraders-0.1.4/spacetraders/models/sell_cargo_sell_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship.py` & `spacetraders-0.1.4/spacetraders/models/ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_cargo.py` & `spacetraders-0.1.4/spacetraders/models/ship_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_cargo_item.py` & `spacetraders-0.1.4/spacetraders/models/ship_cargo_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_crew.py` & `spacetraders-0.1.4/spacetraders/models/ship_crew.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_engine.py` & `spacetraders-0.1.4/spacetraders/models/ship_engine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_frame.py` & `spacetraders-0.1.4/spacetraders/models/ship_frame.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_frame_symbol.py` & `spacetraders-0.1.4/spacetraders/models/ship_frame_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_fuel.py` & `spacetraders-0.1.4/spacetraders/models/ship_fuel.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_fuel_consumed.py` & `spacetraders-0.1.4/spacetraders/models/ship_fuel_consumed.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_module.py` & `spacetraders-0.1.4/spacetraders/models/ship_module.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_module_symbol.py` & `spacetraders-0.1.4/spacetraders/models/ship_module_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_mount.py` & `spacetraders-0.1.4/spacetraders/models/ship_mount.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_mount_deposits_item.py` & `spacetraders-0.1.4/spacetraders/models/ship_mount_deposits_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_mount_symbol.py` & `spacetraders-0.1.4/spacetraders/models/ship_mount_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_nav.py` & `spacetraders-0.1.4/spacetraders/models/ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_nav_route.py` & `spacetraders-0.1.4/spacetraders/models/ship_nav_route.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_nav_route_waypoint.py` & `spacetraders-0.1.4/spacetraders/models/ship_nav_route_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_reactor.py` & `spacetraders-0.1.4/spacetraders/models/ship_reactor.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_refine_json_body.py` & `spacetraders-0.1.4/spacetraders/models/ship_refine_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_refine_ship_refine_200_response.py` & `spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_refine_ship_refine_200_response_data.py` & `spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py` & `spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py` & `spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_registration.py` & `spacetraders-0.1.4/spacetraders/models/ship_registration.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_requirements.py` & `spacetraders-0.1.4/spacetraders/models/ship_requirements.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/ship_type.py` & `spacetraders-0.1.4/spacetraders/models/ship_type.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/shipyard.py` & `spacetraders-0.1.4/spacetraders/models/shipyard.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/shipyard_ship.py` & `spacetraders-0.1.4/spacetraders/models/shipyard_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/shipyard_ship_types_item.py` & `spacetraders-0.1.4/spacetraders/models/shipyard_ship_types_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/shipyard_transaction.py` & `spacetraders-0.1.4/spacetraders/models/shipyard_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/survey.py` & `spacetraders-0.1.4/spacetraders/models/survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/survey_deposit.py` & `spacetraders-0.1.4/spacetraders/models/survey_deposit.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/system.py` & `spacetraders-0.1.4/spacetraders/models/system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/system_faction.py` & `spacetraders-0.1.4/spacetraders/models/system_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/system_waypoint.py` & `spacetraders-0.1.4/spacetraders/models/system_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/trade_good.py` & `spacetraders-0.1.4/spacetraders/models/trade_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/trade_symbol.py` & `spacetraders-0.1.4/spacetraders/models/trade_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py` & `spacetraders-0.1.4/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py` & `spacetraders-0.1.4/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/transfer_cargo_transfer_cargo_request.py` & `spacetraders-0.1.4/spacetraders/models/transfer_cargo_transfer_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/warp_ship_json_body.py` & `spacetraders-0.1.4/spacetraders/models/warp_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/warp_ship_response_200.py` & `spacetraders-0.1.4/spacetraders/models/warp_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/warp_ship_response_200_data.py` & `spacetraders-0.1.4/spacetraders/models/warp_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/waypoint.py` & `spacetraders-0.1.4/spacetraders/models/waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/waypoint_faction.py` & `spacetraders-0.1.4/spacetraders/models/waypoint_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/waypoint_orbital.py` & `spacetraders-0.1.4/spacetraders/models/waypoint_orbital.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/waypoint_trait.py` & `spacetraders-0.1.4/spacetraders/models/waypoint_trait.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/models/waypoint_trait_symbol.py` & `spacetraders-0.1.4/spacetraders/models/waypoint_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/spacetraders/types.py` & `spacetraders-0.1.4/spacetraders/types.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.3/PKG-INFO` & `spacetraders-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetraders
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python API for Space Traders
 License: Apache-2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

