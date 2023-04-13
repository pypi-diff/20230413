# Comparing `tmp/netdoc-0.9.54.tar.gz` & `tmp/netdoc-0.9.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netdoc-0.9.54.tar", last modified: Mon Apr 10 14:52:53 2023, max compression
+gzip compressed data, was "netdoc-0.9.55.tar", last modified: Thu Apr 13 18:43:38 2023, max compression
```

## Comparing `netdoc-0.9.54.tar` & `netdoc-0.9.55.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.793375 netdoc-0.9.54/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.54/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      241 2023-04-05 08:40:22.000000 netdoc-0.9.54/MANIFEST.in
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-10 14:52:53.793375 netdoc-0.9.54/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     9691 2023-04-09 16:39:50.000000 netdoc-0.9.54/README.md
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.433368 netdoc-0.9.54/netdoc/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2147 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.457368 netdoc-0.9.54/netdoc/api/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/api/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2812 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/api/serializers.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      597 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/api/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1207 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/api/views.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.461368 netdoc-0.9.54/netdoc/discoverers/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/discoverers/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6978 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/discoverers/netmiko_cisco_ios.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5160 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/discoverers/netmiko_cisco_nxos.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6514 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/discoverers/netmiko_cisco_xr.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6406 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/discoverers/netmiko_hp_comware.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4511 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/discoverers/netmiko_linux.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3613 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/filtersets.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6587 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/forms.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.529370 netdoc-0.9.54/netdoc/ingestors/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1205 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3682 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2014 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2457 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1705 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      822 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1544 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1951 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2602 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3930 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1660 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      886 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1010 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1238 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3649 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2349 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      824 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2000 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2668 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3907 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1509 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2020 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      888 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      909 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1204 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1529 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3645 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2347 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1802 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2892 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2709 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_route.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      980 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1562 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      894 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2980 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1385 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2626 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1038 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1687 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2035 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2933 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3935 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1514 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      895 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      899 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1202 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_linux_arp__an.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1008 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_linux_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1412 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_linux_ip_address_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1933 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_linux_ip_link_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2450 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_linux_ip_route_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      711 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/ingestors/netmiko_linux_ip_vrf_show.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.541370 netdoc-0.9.54/netdoc/migrations/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13632 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/migrations/0001_initial.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1800 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3399 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3022 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      577 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      453 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/migrations/0006_alter_routetableentry_metric.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      419 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/migrations/0007_discoverylog_supported.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/migrations/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15079 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/models.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2436 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/navigation.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2988 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/nornir_inventory.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.541370 netdoc-0.9.54/netdoc/reports/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5880 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/reports/NetDoc.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.585371 netdoc-0.9.54/netdoc/schemas/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1937 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/arptableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4319 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/cable.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/credential.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4216 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/device.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1508 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/devicerole.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1714 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/devicetype.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3905 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/discoverable.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3176 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/discoverylog.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8799 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1362 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/ipaddress.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1978 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/macaddresstableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1453 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/manufacturer.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/prefix.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2904 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/routetableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      884 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/site.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1623 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2476 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/schemas/vrf.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.585371 netdoc-0.9.54/netdoc/scripts/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13085 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/scripts/NetDoc.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.421368 netdoc-0.9.54/netdoc/static/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.421368 netdoc-0.9.54/netdoc/static/netdoc/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.589371 netdoc-0.9.54/netdoc/static/netdoc/css/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/css/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/css/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)   220164 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/css/vis-network.min.css
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.749374 netdoc-0.9.54/netdoc/static/netdoc/img/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      305 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/access-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/backup.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    28633 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/circuit.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8387 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/core-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     9522 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/distribution-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15596 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/firewall.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1614 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/internal-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5537 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/isp-cpe-material.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5079 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/non-racked-devices.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15857 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/power-feed.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18685 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/power-panel.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4710 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/power-units.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    34335 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/provider-networks.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13504 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/router.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4484 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/server.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/storage.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8308 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/unknown.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/wan-network.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6975 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/img/wireless-ap.png
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.761374 netdoc-0.9.54/netdoc/static/netdoc/js/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/js/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/js/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4198 2023-04-05 14:32:29.000000 netdoc-0.9.54/netdoc/static/netdoc/js/diagram.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/js/netdoc.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)   702066 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/js/vis-network.min.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)  1930592 2023-04-05 08:40:22.000000 netdoc-0.9.54/netdoc/static/netdoc/js/vis-network.min.js.map
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8198 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/tables.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3912 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/tasks.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.421368 netdoc-0.9.54/netdoc/templates/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.781374 netdoc-0.9.54/netdoc/templates/netdoc/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3038 2023-04-05 14:48:16.000000 netdoc-0.9.54/netdoc/templates/netdoc/arptableentry.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.781374 netdoc-0.9.54/netdoc/templates/netdoc/buttons/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      451 2023-04-05 14:48:17.000000 netdoc-0.9.54/netdoc/templates/netdoc/buttons/discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      337 2023-04-05 14:48:17.000000 netdoc-0.9.54/netdoc/templates/netdoc/buttons/export.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1669 2023-04-05 14:48:16.000000 netdoc-0.9.54/netdoc/templates/netdoc/credential.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1371 2023-04-05 14:48:16.000000 netdoc-0.9.54/netdoc/templates/netdoc/diagram.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2639 2023-04-05 14:48:17.000000 netdoc-0.9.54/netdoc/templates/netdoc/discoverable.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1211 2023-04-05 14:48:16.000000 netdoc-0.9.54/netdoc/templates/netdoc/discoverable_bulk_discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      617 2023-04-05 14:48:16.000000 netdoc-0.9.54/netdoc/templates/netdoc/discoverable_discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      993 2023-04-05 14:48:16.000000 netdoc-0.9.54/netdoc/templates/netdoc/discoverable_list.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5108 2023-04-05 14:48:16.000000 netdoc-0.9.54/netdoc/templates/netdoc/discoverylog.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.781374 netdoc-0.9.54/netdoc/templates/netdoc/htmx/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1005 2023-04-05 14:48:17.000000 netdoc-0.9.54/netdoc/templates/netdoc/htmx/discover_form.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1025 2023-04-05 14:48:17.000000 netdoc-0.9.54/netdoc/templates/netdoc/htmx/logexport_form.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3046 2023-04-05 14:48:16.000000 netdoc-0.9.54/netdoc/templates/netdoc/macaddresstableentry.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.781374 netdoc-0.9.54/netdoc/templatetags/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/templatetags/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.793375 netdoc-0.9.54/netdoc/templatetags/__pycache__/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      148 2023-04-05 14:49:51.000000 netdoc-0.9.54/netdoc/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-04-05 14:49:51.000000 netdoc-0.9.54/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      890 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/templatetags/netdoc_buttons.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.793375 netdoc-0.9.54/netdoc/tests/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/tests/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15086 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/tests/test.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    11155 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/topologies.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5128 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    27050 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/utils.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18389 2023-04-10 14:52:50.000000 netdoc-0.9.54/netdoc/views.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-10 14:52:53.457368 netdoc-0.9.54/netdoc.egg-info/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-10 14:52:52.000000 netdoc-0.9.54/netdoc.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6905 2023-04-10 14:52:52.000000 netdoc-0.9.54/netdoc.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-10 14:52:52.000000 netdoc-0.9.54/netdoc.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-05 14:49:45.000000 netdoc-0.9.54/netdoc.egg-info/not-zip-safe
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      132 2023-04-10 14:52:52.000000 netdoc-0.9.54/netdoc.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        7 2023-04-10 14:52:52.000000 netdoc-0.9.54/netdoc.egg-info/top_level.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-04-10 14:52:53.793375 netdoc-0.9.54/setup.cfg
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1272 2023-04-10 14:52:50.000000 netdoc-0.9.54/setup.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.55/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      241 2023-04-05 08:40:22.000000 netdoc-0.9.55/MANIFEST.in
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-13 18:43:38.029746 netdoc-0.9.55/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     9911 2023-04-10 16:30:59.000000 netdoc-0.9.55/README.md
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.881743 netdoc-0.9.55/netdoc/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2147 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.897744 netdoc-0.9.55/netdoc/api/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/api/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2812 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/api/serializers.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      597 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/api/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1207 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/api/views.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.901744 netdoc-0.9.55/netdoc/discoverers/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/discoverers/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6978 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/discoverers/netmiko_cisco_ios.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5160 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/discoverers/netmiko_cisco_nxos.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6514 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/discoverers/netmiko_cisco_xr.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6406 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/discoverers/netmiko_hp_comware.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4511 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/discoverers/netmiko_linux.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3613 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/filtersets.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6587 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/forms.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.917744 netdoc-0.9.55/netdoc/ingestors/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1205 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3682 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2014 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2457 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1705 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      822 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1544 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1951 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2602 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3930 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1660 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      886 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1010 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1238 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3649 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2349 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      824 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2000 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2668 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3907 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1509 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2020 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      888 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      909 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1204 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1529 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3645 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2347 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1802 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2892 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2709 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_route.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      980 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1562 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      894 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2980 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1385 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2626 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1038 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1687 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2035 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2933 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3935 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1514 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      895 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      899 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1202 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_linux_arp__an.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1008 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_linux_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1412 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_address_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1933 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_link_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2450 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_route_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      711 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_vrf_show.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.917744 netdoc-0.9.55/netdoc/migrations/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13632 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/migrations/0001_initial.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1800 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3399 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3022 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      577 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      453 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/migrations/0006_alter_routetableentry_metric.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      419 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/migrations/0007_discoverylog_supported.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/migrations/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15079 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/models.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2436 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/navigation.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2988 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/nornir_inventory.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.921744 netdoc-0.9.55/netdoc/reports/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5880 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/reports/NetDoc.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.921744 netdoc-0.9.55/netdoc/schemas/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1937 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/arptableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4319 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/cable.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/credential.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4216 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/device.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1508 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/devicerole.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1714 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/devicetype.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3905 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/discoverable.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3176 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/discoverylog.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8799 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1362 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/ipaddress.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1978 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/macaddresstableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1453 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/manufacturer.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/prefix.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2904 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/routetableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      884 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/site.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1623 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2476 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/vrf.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.921744 netdoc-0.9.55/netdoc/scripts/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13085 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/scripts/NetDoc.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.873743 netdoc-0.9.55/netdoc/static/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.877743 netdoc-0.9.55/netdoc/static/netdoc/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.925744 netdoc-0.9.55/netdoc/static/netdoc/css/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/css/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/css/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)   220164 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/css/vis-network.min.css
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.017746 netdoc-0.9.55/netdoc/static/netdoc/img/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      305 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/access-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/backup.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    28633 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/circuit.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8387 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/core-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     9522 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/distribution-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15596 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/firewall.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1614 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/internal-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5537 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/isp-cpe-material.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5079 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/non-racked-devices.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15857 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/power-feed.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18685 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/power-panel.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4710 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/power-units.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    34335 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/provider-networks.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13504 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/router.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4484 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/server.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/storage.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8308 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/unknown.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/wan-network.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6975 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/wireless-ap.png
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.021746 netdoc-0.9.55/netdoc/static/netdoc/js/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/js/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/js/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4198 2023-04-05 14:32:29.000000 netdoc-0.9.55/netdoc/static/netdoc/js/diagram.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/js/netdoc.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)   702066 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/js/vis-network.min.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)  1930592 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/js/vis-network.min.js.map
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8198 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/tables.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3912 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/tasks.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.877743 netdoc-0.9.55/netdoc/templates/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/netdoc/templates/netdoc/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3038 2023-04-10 16:21:20.000000 netdoc-0.9.55/netdoc/templates/netdoc/arptableentry.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/netdoc/templates/netdoc/buttons/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      451 2023-04-10 16:17:25.000000 netdoc-0.9.55/netdoc/templates/netdoc/buttons/discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      337 2023-04-10 16:17:25.000000 netdoc-0.9.55/netdoc/templates/netdoc/buttons/export.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1669 2023-04-10 16:21:17.000000 netdoc-0.9.55/netdoc/templates/netdoc/credential.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1439 2023-04-10 16:29:06.000000 netdoc-0.9.55/netdoc/templates/netdoc/diagram.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2654 2023-04-10 16:23:32.000000 netdoc-0.9.55/netdoc/templates/netdoc/discoverable.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1217 2023-04-10 16:26:08.000000 netdoc-0.9.55/netdoc/templates/netdoc/discoverable_bulk_discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      638 2023-04-10 16:26:30.000000 netdoc-0.9.55/netdoc/templates/netdoc/discoverable_discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-04-10 16:23:40.000000 netdoc-0.9.55/netdoc/templates/netdoc/discoverable_list.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5123 2023-04-10 16:23:17.000000 netdoc-0.9.55/netdoc/templates/netdoc/discoverylog.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/netdoc/templates/netdoc/htmx/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1005 2023-04-10 16:17:25.000000 netdoc-0.9.55/netdoc/templates/netdoc/htmx/discover_form.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1025 2023-04-10 16:17:25.000000 netdoc-0.9.55/netdoc/templates/netdoc/htmx/logexport_form.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3046 2023-04-10 16:20:47.000000 netdoc-0.9.55/netdoc/templates/netdoc/macaddresstableentry.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/netdoc/templatetags/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/templatetags/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/netdoc/templatetags/__pycache__/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      148 2023-04-10 14:52:59.000000 netdoc-0.9.55/netdoc/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-04-10 14:52:59.000000 netdoc-0.9.55/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      890 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/templatetags/netdoc_buttons.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/netdoc/tests/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/tests/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15086 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/tests/test.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    11155 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/topologies.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5128 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    27100 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/utils.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18389 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/views.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.897744 netdoc-0.9.55/netdoc.egg-info/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-13 18:43:37.000000 netdoc-0.9.55/netdoc.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6905 2023-04-13 18:43:37.000000 netdoc-0.9.55/netdoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-13 18:43:37.000000 netdoc-0.9.55/netdoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-05 14:49:45.000000 netdoc-0.9.55/netdoc.egg-info/not-zip-safe
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      132 2023-04-13 18:43:37.000000 netdoc-0.9.55/netdoc.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        7 2023-04-13 18:43:37.000000 netdoc-0.9.55/netdoc.egg-info/top_level.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-04-13 18:43:38.029746 netdoc-0.9.55/setup.cfg
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1272 2023-04-13 18:43:34.000000 netdoc-0.9.55/setup.py
```

### Comparing `netdoc-0.9.54/LICENSE` & `netdoc-0.9.55/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/README.md` & `netdoc-0.9.55/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -161,14 +161,34 @@
 ~~~
 cd ~/src/netdoc
 /opt/netbox/venv/bin/python3 setup.py develop
 /opt/netbox/venv/bin/python3 manage.py runserver 0.0.0.0:8000 --insecure
 /opt/netbox/venv/bin/python3 manage.py rqworker high default low
 ~~~
 
+### Testing
+
+Install pre-commit:
+
+~~~
+pip install pre-commit
+~~~
+
+Test:
+
+~~~
+pre-commit run --all-files
+~~~
+
+Test Django scenario:
+
+~~~
+/opt/netbox/venv/bin/python3 /opt/netbox/netbox/manage.py test netdoc --keepdb
+~~~
+
 ## Debugging
 
 Discover script:
 
 ~~~
 from netdoc import tasks
```

### Comparing `netdoc-0.9.54/netdoc/__init__.py` & `netdoc-0.9.55/netdoc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Main class."""
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.9.54"
+__version__ = "0.9.55"
 
 import os
 import pkgutil
 import shutil
 
 from django.conf import settings
```

### Comparing `netdoc-0.9.54/netdoc/api/serializers.py` & `netdoc-0.9.55/netdoc/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/api/urls.py` & `netdoc-0.9.55/netdoc/api/urls.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/api/views.py` & `netdoc-0.9.55/netdoc/api/views.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/discoverers/netmiko_cisco_ios.py` & `netdoc-0.9.55/netdoc/discoverers/netmiko_cisco_ios.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/discoverers/netmiko_cisco_nxos.py` & `netdoc-0.9.55/netdoc/discoverers/netmiko_cisco_nxos.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/discoverers/netmiko_cisco_xr.py` & `netdoc-0.9.55/netdoc/discoverers/netmiko_cisco_xr.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/discoverers/netmiko_hp_comware.py` & `netdoc-0.9.55/netdoc/discoverers/netmiko_hp_comware.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/discoverers/netmiko_linux.py` & `netdoc-0.9.55/netdoc/discoverers/netmiko_linux.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/filtersets.py` & `netdoc-0.9.55/netdoc/filtersets.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/forms.py` & `netdoc-0.9.55/netdoc/forms.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_hostname.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_hostname.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_hostname.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_arp.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_route.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_route.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_arp.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_interface.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_hp_comware_hostname.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_linux_arp__an.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_linux_arp__an.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_linux_hostname.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_linux_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_linux_ip_address_show.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_address_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_linux_ip_link_show.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_link_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_linux_ip_route_show.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_route_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/ingestors/netmiko_linux_ip_vrf_show.py` & `netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_vrf_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/migrations/0001_initial.py` & `netdoc-0.9.55/netdoc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py` & `netdoc-0.9.55/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py` & `netdoc-0.9.55/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py` & `netdoc-0.9.55/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py` & `netdoc-0.9.55/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/models.py` & `netdoc-0.9.55/netdoc/models.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/navigation.py` & `netdoc-0.9.55/netdoc/navigation.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/nornir_inventory.py` & `netdoc-0.9.55/netdoc/nornir_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/reports/NetDoc.py` & `netdoc-0.9.55/netdoc/reports/NetDoc.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/arptableentry.py` & `netdoc-0.9.55/netdoc/schemas/arptableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/cable.py` & `netdoc-0.9.55/netdoc/schemas/cable.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/credential.py` & `netdoc-0.9.55/netdoc/schemas/credential.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/device.py` & `netdoc-0.9.55/netdoc/schemas/device.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/devicerole.py` & `netdoc-0.9.55/netdoc/schemas/devicerole.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/devicetype.py` & `netdoc-0.9.55/netdoc/schemas/devicetype.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/discoverable.py` & `netdoc-0.9.55/netdoc/schemas/discoverable.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/discoverylog.py` & `netdoc-0.9.55/netdoc/schemas/discoverylog.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/interface.py` & `netdoc-0.9.55/netdoc/schemas/interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/ipaddress.py` & `netdoc-0.9.55/netdoc/schemas/ipaddress.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/macaddresstableentry.py` & `netdoc-0.9.55/netdoc/schemas/macaddresstableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/manufacturer.py` & `netdoc-0.9.55/netdoc/schemas/manufacturer.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/prefix.py` & `netdoc-0.9.55/netdoc/schemas/prefix.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/routetableentry.py` & `netdoc-0.9.55/netdoc/schemas/routetableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/site.py` & `netdoc-0.9.55/netdoc/schemas/site.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/vlan.py` & `netdoc-0.9.55/netdoc/schemas/vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/schemas/vrf.py` & `netdoc-0.9.55/netdoc/schemas/vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/scripts/NetDoc.py` & `netdoc-0.9.55/netdoc/scripts/NetDoc.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/css/LICENSE` & `netdoc-0.9.55/netdoc/static/netdoc/css/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/css/vis-network.min.css` & `netdoc-0.9.55/netdoc/static/netdoc/css/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/LICENSE` & `netdoc-0.9.55/netdoc/static/netdoc/img/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/access-switch.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/access-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/backup.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/backup.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/circuit.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/circuit.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/core-switch.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/core-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/distribution-switch.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/distribution-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/firewall.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/firewall.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/internal-switch.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/internal-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/isp-cpe-material.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/isp-cpe-material.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/non-racked-devices.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/non-racked-devices.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/power-feed.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/power-feed.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/power-panel.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/power-panel.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/power-units.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/power-units.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/provider-networks.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/provider-networks.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/router.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/router.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/server.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/server.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/storage.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/storage.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/unknown.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/unknown.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/wan-network.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/wan-network.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/img/wireless-ap.png` & `netdoc-0.9.55/netdoc/static/netdoc/img/wireless-ap.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/js/LICENSE` & `netdoc-0.9.55/netdoc/static/netdoc/js/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/js/diagram.js` & `netdoc-0.9.55/netdoc/static/netdoc/js/diagram.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/js/netdoc.js` & `netdoc-0.9.55/netdoc/static/netdoc/js/netdoc.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/js/vis-network.min.js` & `netdoc-0.9.55/netdoc/static/netdoc/js/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/static/netdoc/js/vis-network.min.js.map` & `netdoc-0.9.55/netdoc/static/netdoc/js/vis-network.min.js.map`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/tables.py` & `netdoc-0.9.55/netdoc/tables.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/tasks.py` & `netdoc-0.9.55/netdoc/tasks.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/templates/netdoc/arptableentry.html` & `netdoc-0.9.55/netdoc/templates/netdoc/arptableentry.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'generic/object.html' %}
+{% extends "generic/object.html" %}
 {% load render_table from django_tables2 %}
 {% comment %}
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 {% endcomment %}
@@ -16,27 +16,27 @@
             <div class="card">
                 <h5 class="card-header">ARP table entry</h5>
                 <div class="card-body">
                     <table class="table table-hover attr-table">
                         <tr>
                             <th scope="row">Device</th>
                             <td>
-                                <a href="{% url 'dcim:device' object.interface.device.pk %}">{{ object.interface.device.name }}</a>
+                                <a href="{% url "dcim:device" object.interface.device.pk %}">{{ object.interface.device.name }}</a>
                             </td>
                         </tr>
                         <tr>
                             <th scope="row">Device role</th>
                             <td>
-                                <a href="{% url 'dcim:devicerole' object.interface.device.device_role.pk %}">{{ object.interface.device.device_role.name }}</a>
+                                <a href="{% url "dcim:devicerole" object.interface.device.device_role.pk %}">{{ object.interface.device.device_role.name }}</a>
                             </td>
                         </tr>
                         <tr>
                             <th scope="row">Interface</th>
                             <td>
-                                <a href="{% url 'dcim:interface' object.interface.pk %}">{{ object.interface.name }}</a>
+                                <a href="{% url "dcim:interface" object.interface.pk %}">{{ object.interface.name }}</a>
                             </td>
                         </tr>
                         <tr>
                             <th scope="row">IP Address</th>
                             <td>{{ object.ip_address }}</td>
                         </tr>
                         <tr>
@@ -45,19 +45,19 @@
                                 {{ object.mac_address }}
                                 {% if object.vendor %}({{ object.vendor }}){% endif %}
                             </td>
                         </tr>
                     </table>
                 </div>
             </div>
-            {% include 'inc/panels/custom_fields.html' %}
+            {% include "inc/panels/custom_fields.html" %}
         </div>
         <div class="col col-md-6">
-            {% include 'inc/panels/tags.html' %}
-            {% include 'inc/panels/comments.html' %}
+            {% include "inc/panels/tags.html" %}
+            {% include "inc/panels/comments.html" %}
         </div>
     </div>
     <div class="row mb-3">
         <div class="col col-md-12">
             <div class="card">
                 <h5 class="card-header">Relevant ARP address table entries</h5>
                 <div class="card-body table-responsive">{% render_table arp_table %}</div>
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-{% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
+{% extends "generic/object.html" %} {% load render_table from django_tables2 %}
 {% comment %} __author__ = "Andrea Dainese" __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese" __license__ = "GPLv3" {%
 endcomment %} {% block controls %} {% endblock controls %} {% block tabs %} {%
 endblock tabs %} {% block content %}
 ** ARP table entry **
-Device      {{_object.interface.device.name_}}
-Device role {{_object.interface.device.device_role.name_}}
-Interface   {{_object.interface.name_}}
+Device       object.interface.device.pk %}">{{ object.interface.device.name }}
+Device role  object.interface.device.device_role.pk %}">{
+            { object.interface.device.device_role.name }}
+Interface    object.interface.pk %}">{{ object.interface.name }}
 IP Address  {{ object.ip_address }}
 MAC Address {{ object.mac_address }} {% if object.vendor %}({{ object.vendor
             }}){% endif %}
-{% include 'inc/panels/custom_fields.html' %}
-{% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
+{% include "inc/panels/custom_fields.html" %}
+{% include "inc/panels/tags.html" %} {% include "inc/panels/comments.html" %}
 ** Relevant ARP address table entries **
 {% render_table arp_table %}
 ** Relevant MAC address table entries **
 {% render_table macaddress_table %}
 {% endblock content %}
```

### Comparing `netdoc-0.9.54/netdoc/templates/netdoc/credential.html` & `netdoc-0.9.55/netdoc/templates/netdoc/credential.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'generic/object.html' %}
+{% extends "generic/object.html" %}
 {% load render_table from django_tables2 %}
 {% comment %}
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 {% endcomment %}
@@ -24,19 +24,19 @@
                         <tr>
                             <th scope="row">Devices</th>
                             <td>{{ object.discoverables.count }}</td>
                         </tr>
                     </table>
                 </div>
             </div>
-            {% include 'inc/panels/custom_fields.html' %}
+            {% include "inc/panels/custom_fields.html" %}
         </div>
         <div class="col col-md-6">
-            {% include 'inc/panels/tags.html' %}
-            {% include 'inc/panels/comments.html' %}
+            {% include "inc/panels/tags.html" %}
+            {% include "inc/panels/comments.html" %}
         </div>
     </div>
     <div class="row">
         <div class="col col-md-12">
             <div class="card">
                 <h5 class="card-header">Devices</h5>
                 <div class="card-body table-responsive">{% render_table discoverables_table %}</div>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-{% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
+{% extends "generic/object.html" %} {% load render_table from django_tables2 %}
 {% comment %} __author__ = "Andrea Dainese" __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese" __license__ = "GPLv3" {%
 endcomment %} {% block content %}
 ** Credential **
 Name     {{ object.name }}
 Username {{ object.username }}
 Devices  {{ object.discoverables.count }}
-{% include 'inc/panels/custom_fields.html' %}
-{% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
+{% include "inc/panels/custom_fields.html" %}
+{% include "inc/panels/tags.html" %} {% include "inc/panels/comments.html" %}
 ** Devices **
 {% render_table discoverables_table %}
 {% endblock content %}
```

### Comparing `netdoc-0.9.54/netdoc/templates/netdoc/diagram.html` & `netdoc-0.9.55/netdoc/templates/netdoc/diagram.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-{% extends 'generic/object.html' %}
+{% extends "generic/object.html" %}
 {% load static %}
 {% load netdoc_buttons %}
 {% comment %}
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 {% endcomment %}
 {% block head %}
-    <link rel="stylesheet" href="{% static 'netdoc/css/vis-network.min.css' %}">
-{% endblock %}
-{% block title %}Diagram {{ object.name }}{% endblock %}
+    <link rel="stylesheet" href="{% static "netdoc/css/vis-network.min.css" %}" />
+{% endblock head %}
+{% block title %}Diagram {{ object.name }}{% endblock title %}
 {% block extra_controls %}
     <a id="btnToggleDiagramMode" class="btn btn-sm btn-secondary" href="#"></a>
     <a id="btnSaveDiagram" class="btn btn-sm btn-primary" href="#">
         <i class="mdi mdi-upload"></i>
         Save
     </a>
     {% export_button object %}
 {% endblock extra_controls %}
 {% block tabs %}
 {% endblock tabs %}
 {% block content-wrapper %}
     <div class="content h-100 p-0">
+        <!-- djlint:off -->
         <div id="visgraph" class="" style="height: 70vh;"></div>
+        <!-- djlint:on -->
     </div>
 {% endblock content-wrapper %}
 {% block javascript %}
     {{ topology_details|json_script:"topology_details_json" }}
     {{ topology_data|json_script:"topology_data_json" }}
     <script type="text/javascript"
-            src="{% static 'netdoc/js/vis-network.min.js' %}"></script>
-    <script type="text/javascript" src="{% static 'netdoc/js/netdoc.js' %}"></script>
-    <script type="text/javascript" src="{% static 'netdoc/js/diagram.js' %}"></script>
+            src="{% static "netdoc/js/vis-network.min.js" %}"></script>
+    <script type="text/javascript" src="{% static "netdoc/js/netdoc.js" %}"></script>
+    <script type="text/javascript" src="{% static "netdoc/js/diagram.js" %}"></script>
 {% endblock javascript %}
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
-{% extends 'generic/object.html' %} {% load static %} {% load netdoc_buttons %}
+{% extends "generic/object.html" %} {% load static %} {% load netdoc_buttons %}
 {% comment %} __author__ = "Andrea Dainese" __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese" __license__ = "GPLv3" {%
 endcomment %} {% block head %}
- {% endblock %} {% block title %}Diagram {{ object.name }}{% endblock %} {%
-block extra_controls %}
+ss/vis-network.min.css" %}" /> {% endblock head %} {% block title %}Diagram {
+{ object.name }}{% endblock title %} {% block extra_controls %}
  Save
  {% export_button object %} {% endblock extra_controls %} {% block tabs %} {%
 endblock tabs %} {% block content-wrapper %}
 {% endblock content-wrapper %} {% block javascript %} {
 { topology_details|json_script:"topology_details_json" }} {
 { topology_data|json_script:"topology_data_json" }}
- {% endblock javascript %}
+s/vis-network.min.js" %}">
+s/netdoc.js" %}">
+s/diagram.js" %}">
+{% endblock javascript %}
```

### Comparing `netdoc-0.9.54/netdoc/templates/netdoc/discoverable.html` & `netdoc-0.9.55/netdoc/templates/netdoc/discoverable.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'generic/object.html' %}
+{% extends "generic/object.html" %}
 {% load render_table from django_tables2 %}
 {% load helpers %}
 {% load perms %}
 {% load plugins %}
 {% load netdoc_buttons %}
 {% comment %}
 __author__ = "Andrea Dainese"
@@ -10,15 +10,15 @@
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 {% endcomment %}
 {% block extra_controls %}
     {% if request.user|can_change:object %}
         {% discover_button object %}
     {% endif %}
-{% endblock %}
+{% endblock extra_controls %}
 {% block content %}
     <div class="row mb-3">
         <div class="col col-md-6">
             <div class="card">
                 <h5 class="card-header">Discoverable</h5>
                 <div class="card-body">
                     <table class="table table-hover attr-table">
@@ -30,15 +30,15 @@
                             <th scope="row">Mode</th>
                             <td>{{ object.mode }}</td>
                         </tr>
                         <tr>
                             <th scope="row">Device</th>
                             <td>
                                 {% if object.device %}
-                                    <a href="{% url 'dcim:device' object.device.pk %}">{{ object.device }}</a>
+                                    <a href="{% url "dcim:device" object.device.pk %}">{{ object.device }}</a>
                                 {% endif %}
                             </td>
                         </tr>
                         <tr>
                             <th scope="row">Site</th>
                             <td>{{ object.site }}</td>
                         </tr>
@@ -49,19 +49,19 @@
                         <tr>
                             <th scope="row">Total logs</th>
                             <td>{{ object.discoverylogs_count }}</td>
                         </tr>
                     </table>
                 </div>
             </div>
-            {% include 'inc/panels/custom_fields.html' %}
+            {% include "inc/panels/custom_fields.html" %}
         </div>
         <div class="col col-md-6">
-            {% include 'inc/panels/tags.html' %}
-            {% include 'inc/panels/comments.html' %}
+            {% include "inc/panels/tags.html" %}
+            {% include "inc/panels/comments.html" %}
         </div>
     </div>
     <div class="row">
         <div class="col col-md-12">
             <div class="card">
                 <h5 class="card-header">Discovery Logs</h5>
                 <div class="card-body table-responsive">{% render_table discoverylogs_table %}</div>
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
-{% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
+{% extends "generic/object.html" %} {% load render_table from django_tables2 %}
 {% load helpers %} {% load perms %} {% load plugins %} {% load netdoc_buttons
 %} {% comment %} __author__ = "Andrea Dainese" __contact__ =
 "andrea@adainese.it" __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3" {% endcomment %} {% block extra_controls %} {% if
 request.user|can_change:object %} {% discover_button object %} {% endif %} {%
-endblock %} {% block content %}
+endblock extra_controls %} {% block content %}
 ** Discoverable **
 Address    {{ object.address }}
 Mode       {{ object.mode }}
-Device     {% if object.device %} {{_object.device_}} {% endif %}
+           {% if object.device %}
+Device      object.device.pk %}">{{ object.device }}
+            {% endif %}
 Site       {{ object.site }}
 Credential {{ object.credential }}
 Total logs {{ object.discoverylogs_count }}
-{% include 'inc/panels/custom_fields.html' %}
-{% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
+{% include "inc/panels/custom_fields.html" %}
+{% include "inc/panels/tags.html" %} {% include "inc/panels/comments.html" %}
 ** Discovery Logs **
 {% render_table discoverylogs_table %}
 {% endblock content %}
```

### Comparing `netdoc-0.9.54/netdoc/templates/netdoc/discoverable_bulk_discover.html` & `netdoc-0.9.55/netdoc/templates/netdoc/discoverable_bulk_discover.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-{% extends 'base/layout.html' %}
+{% extends "base/layout.html" %}
 {% load helpers %}
 {% load render_table from django_tables2 %}
 {% comment %}
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 {% endcomment %}
 {% comment %}
 Replace "templates/generic/bulk_delete.html".
 {% endcomment %}
-{% block title %}Discover {{ table.rows|length }} {{ model|meta:"verbose_name_plural"|bettertitle }}?{% endblock %}
+{% block title %}Discover {{ table.rows|length }} {{ model|meta:"verbose_name_plural"|bettertitle }}?{% endblock title %}
 {% block content %}
     <div class="container-xl px-0">
-        <div class="table-responsive">{% render_table table 'inc/table.html' %}</div>
+        <div class="table-responsive">{% render_table table "inc/table.html" %}</div>
         <div class="row mt-3">
             <form action="" method="post">
                 {% csrf_token %}
                 {% for field in form.hidden_fields %}{{ field }}{% endfor %}
                 <div class="text-end">
                     <a href="{{ return_url }}" class="btn btn-outline-dark">Cancel</a>
                     <button type="submit" name="_confirm" class="btn btn-secondary">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-{% extends 'base/layout.html' %} {% load helpers %} {% load render_table from
+{% extends "base/layout.html" %} {% load helpers %} {% load render_table from
 django_tables2 %} {% comment %} __author__ = "Andrea Dainese" __contact__ =
 "andrea@adainese.it" __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3" {% endcomment %} {% comment %} Replace "templates/
 generic/bulk_delete.html". {% endcomment %} {% block title %}Discover {
 { table.rows|length }} {{ model|meta:"verbose_name_plural"|bettertitle }}?{%
-endblock %} {% block content %}
-{% render_table table 'inc/table.html' %}
+endblock title %} {% block content %}
+{% render_table table "inc/table.html" %}
 {% csrf_token %} {% for field in form.hidden_fields %}{{ field }}{% endfor %}
 Cancel  Discover {{ table.rows|length }} {{ model|meta:"verbose_name_plural" }}
 {% endblock content %}
```

### Comparing `netdoc-0.9.54/netdoc/templates/netdoc/discoverable_discover.html` & `netdoc-0.9.55/netdoc/templates/netdoc/discoverable_discover.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-{% extends 'base/layout.html' %}
+{% extends "base/layout.html" %}
 {% load helpers %}
 {% load form_helpers %}
 {% comment %}
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 {% endcomment %}
-{% block title %}Discover {{ object|meta:"verbose_name" }}?{% endblock %}
-{% block header %}{% endblock %}
+{% block title %}Discover {{ object|meta:"verbose_name" }}?{% endblock title %}
+{% block header %}{% endblock header %}
 {% block content %}
     <div class="modal" tabindex="-1" style="display: block; position: static">
         <div class="modal-dialog">
-            <div class="modal-content">{% include 'netdoc/htmx/discover_form.html' %}</div>
+            <div class="modal-content">{% include "netdoc/htmx/discover_form.html" %}</div>
         </div>
     </div>
-{% endblock %}
+{% endblock content %}
```

### Comparing `netdoc-0.9.54/netdoc/templates/netdoc/discoverable_list.html` & `netdoc-0.9.55/netdoc/templates/netdoc/discoverable_list.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-{% extends 'generic/object_list.html' %}
+{% extends "generic/object_list.html" %}
 {% load buttons %}
 {% comment %}
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 {% endcomment %}
 {% comment %}
 Add "Discover Selected" button to the generic template.
 {% endcomment %}
 {% block bulk_buttons %}
-    {% if 'bulk_discover' in actions %}
+    {% if "bulk_discover" in actions %}
         <button type="submit"
                 name="_discover"
-                formaction="{% url 'plugins:netdoc:discoverable_bulk_discover' %}?return_url={% url 'plugins:netdoc:discoverable_list' %}"
+                formaction="{% url "plugins:netdoc:discoverable_bulk_discover" %}?return_url={% url "plugins:netdoc:discoverable_list" %}"
                 class="btn btn-secondary btn-sm">
             <i class="mdi mdi-refresh" aria-hidden="true"></i> Discover Selected
         </button>
     {% endif %}
-    {% if 'bulk_edit' in actions %}
+    {% if "bulk_edit" in actions %}
         {% bulk_edit_button model query_params=request.GET %}
     {% endif %}
-    {% if 'bulk_delete' in actions %}
+    {% if "bulk_delete" in actions %}
         {% bulk_delete_button model query_params=request.GET %}
     {% endif %}
-{% endblock %}
+{% endblock bulk_buttons %}
```

### Comparing `netdoc-0.9.54/netdoc/templates/netdoc/discoverylog.html` & `netdoc-0.9.55/netdoc/templates/netdoc/discoverylog.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'generic/object.html' %}
+{% extends "generic/object.html" %}
 {% load render_table from django_tables2 %}
 {% load buttons %}
 {% load custom_links %}
 {% load helpers %}
 {% load perms %}
 {% load plugins %}
 {% load netdoc_buttons %}
@@ -18,15 +18,15 @@
         <div class="control-group">
             {% plugin_buttons object %}
             {# Extra buttons #}
             {% block extra_controls %}
                 {% if request.user|can_change:object %}
                     {% export_button object %}
                 {% endif %}
-            {% endblock %}
+            {% endblock extra_controls %}
             {% if request.user|can_delete:object %}
                 {% delete_button object %}
             {% endif %}
         </div>
         <div class="control-group">{% custom_links object %}</div>
     </div>
 {% endblock controls %}
@@ -40,22 +40,22 @@
                         <tr>
                             <th scope="row">Created at</th>
                             <td>{{ object.created }}</td>
                         </tr>
                         <tr>
                             <th scope="row">Discoverable</th>
                             <td>
-                                <a href="{% url 'plugins:netdoc:discoverable' object.discoverable.pk %}">{{ object.discoverable }}</a>
+                                <a href="{% url "plugins:netdoc:discoverable" object.discoverable.pk %}">{{ object.discoverable }}</a>
                             </td>
                         </tr>
                         <tr>
                             <th scope="row">Device</th>
                             <td>
                                 {% if object.discoverable.device %}
-                                    <a href="{% url 'dcim:device' object.discoverable.device.pk %}">{{ object.discoverable.device }}</a>
+                                    <a href="{% url "dcim:device" object.discoverable.device.pk %}">{{ object.discoverable.device }}</a>
                                 {% else %}
                                     {{ object.ip_address }}
                                 {% endif %}
                             </td>
                         </tr>
                         <tr>
                             <th scope="row">Template (to parse raw output)</th>
@@ -80,19 +80,19 @@
                         <tr>
                             <th scope="row">Parsed output ingested successfully?</th>
                             <td>{{ object.ingested }}</td>
                         </tr>
                     </table>
                 </div>
             </div>
-            {% include 'inc/panels/custom_fields.html' %}
+            {% include "inc/panels/custom_fields.html" %}
         </div>
         <div class="col col-md-6">
-            {% include 'inc/panels/tags.html' %}
-            {% include 'inc/panels/comments.html' %}
+            {% include "inc/panels/tags.html" %}
+            {% include "inc/panels/comments.html" %}
         </div>
     </div>
     <div class="row">
         <div class="col col-md-12">
             <div class="card">
                 <h5 class="card-header">Task parameters</h5>
                 <div class="card-body table-responsive">
```

#### html2text {}

```diff
@@ -1,33 +1,36 @@
-{% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
+{% extends "generic/object.html" %} {% load render_table from django_tables2 %}
 {% load buttons %} {% load custom_links %} {% load helpers %} {% load perms %}
 {% load plugins %} {% load netdoc_buttons %} {% comment %} __author__ = "Andrea
 Dainese" __contact__ = "andrea@adainese.it" __copyright__ = "Copyright 2022,
 Andrea Dainese" __license__ = "GPLv3" {% endcomment %} {% block controls %} {#
 Clone/Edit/Delete Buttons #}
 {% plugin_buttons object %} {# Extra buttons #} {% block extra_controls %} {%
 if request.user|can_change:object %} {% export_button object %} {% endif %} {%
-endblock %} {% if request.user|can_delete:object %} {% delete_button object %}
-{% endif %}
+endblock extra_controls %} {% if request.user|can_delete:object %} {%
+delete_button object %} {% endif %}
 {% custom_links object %}
 {% endblock controls %} {% block content %}
 ** Discovery log **
 Created at                           {{ object.created }}
-Discoverable                         {{_object.discoverable_}}
-                                     {% if object.discoverable.device %} {
-Device                               {_object.discoverable.device_}} {% else %}
-                                     {{ object.ip_address }} {% endif %}
+Discoverable                          object.discoverable.pk %}">{
+                                     { object.discoverable }}
+                                     {% if object.discoverable.device %}
+                                      object.discoverable.device.pk %}">{
+Device                               { object.discoverable.device }}
+                                      {% else %} {{ object.ip_address }} {%
+                                     endif %}
 Template (to parse raw output)       {{ object.template }}
 Command                              {{ object.command }}
 Contains configuration?              {{ object.configuration }}
 Command executed successfully?       {{ object.success }}
 Command output parsed successfully?  {{ object.parsed }}
 Parsed output ingested successfully? {{ object.ingested }}
-{% include 'inc/panels/custom_fields.html' %}
-{% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
+{% include "inc/panels/custom_fields.html" %}
+{% include "inc/panels/tags.html" %} {% include "inc/panels/comments.html" %}
 ** Task parameters **
 {{ object.details }}
 ** Raw output **
 {{ object.raw_output }}
 {% if object.parsed_output %}
 ** {% if object.parsed %} Parsed output {% else %} Parsing errors {% endif %}
 **
```

### Comparing `netdoc-0.9.54/netdoc/templates/netdoc/htmx/discover_form.html` & `netdoc-0.9.55/netdoc/templates/netdoc/htmx/discover_form.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/templates/netdoc/htmx/logexport_form.html` & `netdoc-0.9.55/netdoc/templates/netdoc/htmx/logexport_form.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/templates/netdoc/macaddresstableentry.html` & `netdoc-0.9.55/netdoc/templates/netdoc/macaddresstableentry.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'generic/object.html' %}
+{% extends "generic/object.html" %}
 {% load render_table from django_tables2 %}
 {% comment %}
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 {% endcomment %}
@@ -16,27 +16,27 @@
             <div class="card">
                 <h5 class="card-header">MAC address table entry</h5>
                 <div class="card-body">
                     <table class="table table-hover attr-table">
                         <tr>
                             <th scope="row">Device</th>
                             <td>
-                                <a href="{% url 'dcim:device' object.interface.device.pk %}">{{ object.interface.device.name }}</a>
+                                <a href="{% url "dcim:device" object.interface.device.pk %}">{{ object.interface.device.name }}</a>
                             </td>
                         </tr>
                         <tr>
                             <th scope="row">Device role</th>
                             <td>
-                                <a href="{% url 'dcim:devicerole' object.interface.device.device_role.pk %}">{{ object.interface.device.device_role.name }}</a>
+                                <a href="{% url "dcim:devicerole" object.interface.device.device_role.pk %}">{{ object.interface.device.device_role.name }}</a>
                             </td>
                         </tr>
                         <tr>
                             <th scope="row">Interface</th>
                             <td>
-                                <a href="{% url 'dcim:interface' object.interface.pk %}">{{ object.interface.name }}</a>
+                                <a href="{% url "dcim:interface" object.interface.pk %}">{{ object.interface.name }}</a>
                             </td>
                         </tr>
                         <tr>
                             <th scope="row">IP Address</th>
                             <td>{{ object.ip_address }}</td>
                         </tr>
                         <tr>
@@ -45,19 +45,19 @@
                                 {{ object.mac_address }}
                                 {% if object.vendor %}({{ object.vendor }}){% endif %}
                             </td>
                         </tr>
                     </table>
                 </div>
             </div>
-            {% include 'inc/panels/custom_fields.html' %}
+            {% include "inc/panels/custom_fields.html" %}
         </div>
         <div class="col col-md-6">
-            {% include 'inc/panels/tags.html' %}
-            {% include 'inc/panels/comments.html' %}
+            {% include "inc/panels/tags.html" %}
+            {% include "inc/panels/comments.html" %}
         </div>
     </div>
     <div class="row mb-3">
         <div class="col col-md-12">
             <div class="card">
                 <h5 class="card-header">Relevant ARP address table entries</h5>
                 <div class="card-body table-responsive">{% render_table arp_table %}</div>
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-{% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
+{% extends "generic/object.html" %} {% load render_table from django_tables2 %}
 {% comment %} __author__ = "Andrea Dainese" __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese" __license__ = "GPLv3" {%
 endcomment %} {% block controls %} {% endblock controls %} {% block tabs %} {%
 endblock tabs %} {% block content %}
 ** MAC address table entry **
-Device      {{_object.interface.device.name_}}
-Device role {{_object.interface.device.device_role.name_}}
-Interface   {{_object.interface.name_}}
+Device       object.interface.device.pk %}">{{ object.interface.device.name }}
+Device role  object.interface.device.device_role.pk %}">{
+            { object.interface.device.device_role.name }}
+Interface    object.interface.pk %}">{{ object.interface.name }}
 IP Address  {{ object.ip_address }}
 MAC Address {{ object.mac_address }} {% if object.vendor %}({{ object.vendor
             }}){% endif %}
-{% include 'inc/panels/custom_fields.html' %}
-{% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
+{% include "inc/panels/custom_fields.html" %}
+{% include "inc/panels/tags.html" %} {% include "inc/panels/comments.html" %}
 ** Relevant ARP address table entries **
 {% render_table arp_table %}
 ** Relevant MAC address table entries **
 {% render_table macaddress_table %}
 {% endblock content %}
```

### Comparing `netdoc-0.9.54/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc` & `netdoc-0.9.55/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr  5 14:49:42 2023 UTC, .py size: 890 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 868a 2d64 7a03 0000  o.........-dz...
+00000000: 6f0d 0d0a 0000 0000 c222 3464 7a03 0000  o........"4dz...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 6406 6c05 6d06 5a06 0100 6405  Z.d.d.l.m.Z...d.
 00000050: 6407 6c07 6d08 5a08 0100 6405 6408 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6506 a00b a100 5a0c 650c  m.Z...e.....Z.e.
 00000070: a00d 6409 a101 640a 640b 8400 8301 5a0e  ..d...d.d.....Z.
```

### Comparing `netdoc-0.9.54/netdoc/templatetags/netdoc_buttons.py` & `netdoc-0.9.55/netdoc/templatetags/netdoc_buttons.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/tests/test.py` & `netdoc-0.9.55/netdoc/tests/test.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/topologies.py` & `netdoc-0.9.55/netdoc/topologies.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/urls.py` & `netdoc-0.9.55/netdoc/urls.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc/utils.py` & `netdoc-0.9.55/netdoc/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,14 +506,16 @@
     Return True if the link is up, False elsewhere.
     """
     status = status.lower()
     if "up" in status:
         return True
     if "down" in status:
         return False
+    if "disabled" in status:
+        return False
     raise ValueError(f"Invalid interface status {status}")
 
 
 def normalize_interface_type(name="", encapsulation=""):
     """Return interface type from name/encapsulation."""
     label = normalize_interface_label(name)
     encapsulation = encapsulation.lower()
```

### Comparing `netdoc-0.9.54/netdoc/views.py` & `netdoc-0.9.55/netdoc/views.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/netdoc.egg-info/SOURCES.txt` & `netdoc-0.9.55/netdoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.54/setup.py` & `netdoc-0.9.55/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     twine upload dist/*
 """
 
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.9.54"
+__version__ = "0.9.55"
 
 from setuptools import find_packages, setup
 
 setup(
     name="netdoc",
     version=__version__,
     description="Network Documentation plugin for NetBox",
```

