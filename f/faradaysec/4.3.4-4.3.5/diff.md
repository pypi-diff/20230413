# Comparing `tmp/faradaysec-4.3.4.tar.gz` & `tmp/faradaysec-4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faradaysec-4.3.4.tar", last modified: Tue Apr 11 18:17:14 2023, max compression
+gzip compressed data, was "faradaysec-4.3.5.tar", last modified: Wed Apr 12 22:34:58 2023, max compression
```

## Comparing `faradaysec-4.3.4.tar` & `faradaysec-4.3.5.tar`

### file list

```diff
@@ -1,342 +1,342 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.467996 faradaysec-4.3.4/
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-04-11 18:16:50.000000 faradaysec-4.3.4/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    32681 2023-04-11 18:16:50.000000 faradaysec-4.3.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-04-11 18:16:50.000000 faradaysec-4.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7835 2023-04-11 18:17:14.467996 faradaysec-4.3.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6553 2023-04-11 18:16:50.000000 faradaysec-4.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.341983 faradaysec-4.3.4/faraday/
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/alembic.ini
--rwxrwxrwx   0 root         (0) root         (0)    11599 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.342984 faradaysec-4.3.4/faraday/migrations/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/README
--rw-rw-rw-   0 root         (0) root         (0)     2543 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/env.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.366986 faradaysec-4.3.4/faraday/migrations/versions/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      650 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/0409e696eeec_workspace_important_flag_and_risk_.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/06c48492f587_reformat_jira_issue_fields_value.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/077b7c925ded_add_last_run_to_executors.py
--rw-rw-rw-   0 root         (0) root         (0)     5283 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/085188e0a016_create_rules_tables.py
--rw-rw-rw-   0 root         (0) root         (0)      534 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/08d02214aedc_add_advanced_filter_to_executive_report_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1922 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/0d216660da28_add_notification_table.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/0ed0dab44def_add_tags_arguments_for_agent_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/1574fbcf72f5_disable_several_notifications_and_add_event_enabled_flag.py
--rw-rw-rw-   0 root         (0) root         (0)     3406 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/15d70093d262_severities_histogram_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2735 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/18891ca61db6_add_cascade_delete_from_workspace.py
--rw-rw-rw-   0 root         (0) root         (0)     2794 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/1b2533cc16fe_fix_custom_fields_display_name_was_used_.py
--rw-rw-rw-   0 root         (0) root         (0)     4346 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/1d328f7bf643_planner_model.py
--rw-rw-rw-   0 root         (0) root         (0)      838 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/1dbe9e8e4247_add_rule_execution_start_and_end_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1897 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/1e95dde5b9c8_cascade_on_kb.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/20f3d0c2f71f_alter_table_executive_report_add_.py
--rw-rw-rw-   0 root         (0) root         (0)     1553 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/247a90b029f2_fix_severities_ordering.py
--rw-rw-rw-   0 root         (0) root         (0)     2152 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/282ac9b6569f_add_agent_as_import_source_to_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/2a0de6132377_add_searchfilter_table.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/2ca03a8feef5_workspace_readonly.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/2db31733fb78_unique_field_name_in_customfield.py
--rw-rw-rw-   0 root         (0) root         (0)     1038 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/384784872dc1_add_weight_column_in_role.py
--rw-rw-rw-   0 root         (0) root         (0)     7804 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/38bb251889e6_bulks.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/3eb96406e88d_rename_important_with_importance_and_remove_check_constraint.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/3f771124f0a2_add_metadata_to_cf_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/47e53ddc0308_add_cwe.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/4bb882a7f9b5_enable_notifications_for_v3.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/4d7a8fdd94e4_rename_not_active_users.py
--rw-rw-rw-   0 root         (0) root         (0)     3746 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/526aa91cac98_vulnerability_merge_model.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/5272b3f5a820_add_markdown_column_to_exectuive_reports.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/5658775e113f_add_command_id_to_agent_execution.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/581121b181d8_add_owasp_model.py
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/59bed5515407_vuln_external_id.py
--rw-rw-rw-   0 root         (0) root         (0)     1910 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/5cf9660bba80_policyviolationvulnerabilityassociation_.py
--rw-rw-rw-   0 root         (0) root         (0)     1119 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/5d7a930c439e_cve_many_to_many.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/6471033046cb_added_delete_on_cascade_to_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/699402156cf4_update_risk_value.py
--rw-rw-rw-   0 root         (0) root         (0)     3030 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/7dea3a6caf51_cascade_in_vuls_relation.py
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/84f266a05be3_add_tool_column_to_vuln.py
--rw-rw-rw-   0 root         (0) root         (0)    13765 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/85aeb4185f98_refactor_cvss.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/877dd088c8cb_comment_ws_not_mandatory.py
--rw-rw-rw-   0 root         (0) root         (0)     4212 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/89115e133f0a_add_hosts_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/8a10ff3926a5_2fa_columns.py
--rw-rw-rw-   0 root         (0) root         (0)     3400 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/904a517a2f0c_create_executor_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1234 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/905261860ad0_user_types_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/97a9348d0406_add_fields_to_report.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/99a740945c44_add_index_into_vulnerability.py
--rw-rw-rw-   0 root         (0) root         (0)     2280 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/9c4091d1a09b_create_agent_table.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/9c678c44aa61_add_enabled_field_to_rule.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/a39a3a6e3f99_create_user_preferences_column.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/a4def820a5bb_alter_otp_secret_length_in_user.py
--rw-rw-rw-   0 root         (0) root         (0)    15209 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/a9fcf8444c79_add_notification_event_and_subscription_.py
--rw-rw-rw-   0 root         (0) root         (0)     3297 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/aa56852fa76d_update_rule_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     8670 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/abb7ed8c56b4_add_workflow_models.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/b1d15a55556d_remove_ticketing_tools_credentials.py
--rw-rw-rw-   0 root         (0) root         (0)     3532 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/b31fa447f00c_add_analytics_monthly_graphs_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/b49d8efbd0c2_add_configuration_table.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/b5065f401599_report_template_object_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1883 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/be1f942eba28_add_analytics_saved_graphics_model.py
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/be89aa03e35e_add_severities_column_to_executive_.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/cb25cf42bda7_remove_knowledge_base_aka_pasta_base.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/d3afdb4e0b11_add_enum_to_comment_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4134 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/d8f0b32a5c0e_cvss_model.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/e03a13c41a67_check_important_host.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/e61afb450465_add_custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     2585 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/ed403da439d4_agents_with_multiple_workspaces.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/f00247a92a14_add_agent_execution_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3494 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/f0439bf6688a_updating_to_a_role_model_to_use_faraday_.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/f0a507afabd4_adding_fs_uniquifier_to_user_model.py
--rw-rw-rw-   0 root         (0) root         (0)      746 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/f20aa8756612_change_executivereport_field_to_text.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/f28eae25416b_fix_constraint_in_cve_association.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/f6edb9a16479_add_type_to_reference_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2380 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/f82a9136c408_remove_ws_from_agents_and_make_schedule_.py
--rw-rw-rw-   0 root         (0) root         (0)     2198 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/f8a44acd0e41_add_new_user_role.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/migrations/versions/fa12b8322112_update_workflow_modules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.366986 faradaysec-4.3.4/faraday/openapi/
--rw-rw-rw-   0 root         (0) root         (0)   197333 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/openapi/faraday_swagger.json
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.370986 faradaysec-4.3.4/faraday/server/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.371986 faradaysec-4.3.4/faraday/server/api/
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    75862 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.380988 faradaysec-4.3.4/faraday/server/api/modules/
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4359 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/activity_feed.py
--rw-rw-rw-   0 root         (0) root         (0)    10163 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     1650 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/agent_auth_token.py
--rw-rw-rw-   0 root         (0) root         (0)    21460 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/bulk_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4899 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/commandsrun.py
--rw-rw-rw-   0 root         (0) root         (0)     3171 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/comments.py
--rw-rw-rw-   0 root         (0) root         (0)     5203 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/credentials.py
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     9914 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/export_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/get_exploits.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/global_commands.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/handlers.py
--rw-rw-rw-   0 root         (0) root         (0)    18611 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/hosts.py
--rw-rw-rw-   0 root         (0) root         (0)     1770 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/info.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/licenses.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/preferences.py
--rw-rw-rw-   0 root         (0) root         (0)     1114 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/search_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     6152 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/services.py
--rw-rw-rw-   0 root         (0) root         (0)     1174 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/session.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      728 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/settings_dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/settings_reports.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/swagger.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/token.py
--rw-rw-rw-   0 root         (0) root         (0)     5598 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/upload_reports.py
--rw-rw-rw-   0 root         (0) root         (0)    12827 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/vulnerability_template.py
--rw-rw-rw-   0 root         (0) root         (0)    54782 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/vulns.py
--rw-rw-rw-   0 root         (0) root         (0)     3337 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/websocket_auth.py
--rw-rw-rw-   0 root         (0) root         (0)    21793 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/api/modules/workspaces.py
--rw-rw-rw-   0 root         (0) root         (0)    23507 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.384988 faradaysec-4.3.4/faraday/server/commands/
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2981 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/commands/app_urls.py
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/commands/change_password.py
--rw-rw-rw-   0 root         (0) root         (0)     1134 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/commands/change_username.py
--rw-rw-rw-   0 root         (0) root         (0)     3513 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/commands/custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     2975 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/commands/faraday_schema_display.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/commands/import_vulnerability_template.py
--rw-rw-rw-   0 root         (0) root         (0)    20997 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/commands/initdb.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/commands/manage_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1588 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/commands/nginx_config.py
--rwxrwxrwx   0 root         (0) root         (0)     1235 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/commands/reset_db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.384988 faradaysec-4.3.4/faraday/server/commands/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1392 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/commands/templates/nginx_config.j2
--rw-rw-rw-   0 root         (0) root         (0)     4712 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/config.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/default.ini
--rw-rw-rw-   0 root         (0) root         (0)    15565 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/events.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/extensions.py
--rw-rw-rw-   0 root         (0) root         (0)     4615 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/fields.py
--rw-rw-rw-   0 root         (0) root         (0)   127381 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/models.py
--rw-rw-rw-   0 root         (0) root         (0)    12973 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.385988 faradaysec-4.3.4/faraday/server/threads/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/threads/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1388 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/threads/ping_home.py
--rw-rw-rw-   0 root         (0) root         (0)     6565 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/threads/reports_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.390988 faradaysec-4.3.4/faraday/server/utils/
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/agents.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/bulk_create.py
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/command.py
--rw-rw-rw-   0 root         (0) root         (0)     2505 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/cvss.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/cwe.py
--rw-rw-rw-   0 root         (0) root         (0)     8819 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/daemonize.py
--rw-rw-rw-   0 root         (0) root         (0)    12276 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/database.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     8469 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/export.py
--rw-rw-rw-   0 root         (0) root         (0)    12793 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/invalid_chars.py
--rw-rw-rw-   0 root         (0) root         (0)     2673 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      570 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/reference.py
--rw-rw-rw-   0 root         (0) root         (0)    30446 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/search.py
--rw-rw-rw-   0 root         (0) root         (0)     2645 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/utils/web.py
--rw-rw-rw-   0 root         (0) root         (0)     6871 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/web.py
--rw-rw-rw-   0 root         (0) root         (0)    11162 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/websocket_factories.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/server/websockets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.392989 faradaysec-4.3.4/faraday/server/www/
--rw-r--r--   0 root         (0) root         (0)    11309 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/asset-manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-03 14:26:20.000000 faradaysec-4.3.4/faraday/server/www/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     1918 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/index.html
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-04-03 14:26:20.000000 faradaysec-4.3.4/faraday/server/www/manifest.json
--rw-r--r--   0 root         (0) root         (0)    14688 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/precache-manifest.76e73c7b229a75e39d1b019b45394088.js
--rw-r--r--   0 root         (0) root         (0)     1181 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.336983 faradaysec-4.3.4/faraday/server/www/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.394989 faradaysec-4.3.4/faraday/server/www/static/css/
--rw-r--r--   0 root         (0) root         (0)   183537 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/css/2.b43efbd6.chunk.css
--rw-r--r--   0 root         (0) root         (0)   317573 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/css/2.b43efbd6.chunk.css.map
--rw-r--r--   0 root         (0) root         (0)   622929 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/css/main.bd546d28.chunk.css
--rw-r--r--   0 root         (0) root         (0)   507732 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/css/main.bd546d28.chunk.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.423992 faradaysec-4.3.4/faraday/server/www/static/js/
--rw-r--r--   0 root         (0) root         (0)  3063891 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/js/2.ebd7c667.chunk.js
--rw-r--r--   0 root         (0) root         (0)     5668 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/js/2.ebd7c667.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0) 17092240 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/js/2.ebd7c667.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)  1312116 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/js/main.8be13664.chunk.js
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/js/main.8be13664.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)  2617810 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/js/main.8be13664.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     1573 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/js/runtime-main.ea9693b3.js
--rw-r--r--   0 root         (0) root         (0)     8286 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/js/runtime-main.ea9693b3.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.462996 faradaysec-4.3.4/faraday/server/www/static/media/
--rw-r--r--   0 root         (0) root         (0)    79144 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/CentraNo2-Book.386f0594.otf
--rw-r--r--   0 root         (0) root         (0)    81720 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/CentraNo2-Medium.63911e85.otf
--rw-r--r--   0 root         (0) root         (0)     1117 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/Checkbox.b83098ac.svg
--rw-r--r--   0 root         (0) root         (0)      177 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/Checkbox_empty.195b4c92.svg
--rw-r--r--   0 root         (0) root         (0)     1263 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/Checkbox_ok.52c5a6cc.svg
--rw-r--r--   0 root         (0) root         (0)    76768 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/Sequel_Sans_Head_Bold.89985cf2.woff
--rw-r--r--   0 root         (0) root         (0)    82720 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/Sequel_Sans_Head_Book.b99ba59e.woff
--rw-r--r--   0 root         (0) root         (0)    78520 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/Sequel_Sans_Head_Medium.db87ffc9.woff
--rw-r--r--   0 root         (0) root         (0)    79728 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/Sequel_Sans_Head_Roman.db35328c.woff
--rw-r--r--   0 root         (0) root         (0)    77184 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/Sequel_Sans_Head_SemiBold.48873506.woff
--rw-r--r--   0 root         (0) root         (0)      713 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/activity-dashboard.b37176e7.svg
--rw-r--r--   0 root         (0) root         (0)     1569 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/agent_small.d1a2c9fe.svg
--rw-r--r--   0 root         (0) root         (0)      629 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/analytics.b5f3011a.svg
--rw-r--r--   0 root         (0) root         (0)     1313 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/api_link.dcbdf06d.svg
--rw-r--r--   0 root         (0) root         (0)      292 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/arrow-down.d8661d88.svg
--rw-r--r--   0 root         (0) root         (0)      294 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/arrow-right.ec48cf40.svg
--rw-r--r--   0 root         (0) root         (0)     1123 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/assets.581bf13b.svg
--rw-r--r--   0 root         (0) root         (0)     1555 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/automation.a512d67b.svg
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/clear.26371e5f.svg
--rw-r--r--   0 root         (0) root         (0)     1438 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/cog.6f2e860c.svg
--rw-r--r--   0 root         (0) root         (0)     3586 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/command.4ada7185.svg
--rw-r--r--   0 root         (0) root         (0)      387 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/copy.7e1b1006.svg
--rw-r--r--   0 root         (0) root         (0)      650 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/copy_link.852fb400.svg
--rw-r--r--   0 root         (0) root         (0)     2233 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/customAttributes.c7457305.svg
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/download-icon.eadbcf9c.svg
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/drag.b17c0ec9.svg
--rw-r--r--   0 root         (0) root         (0)    24438 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/empty-feed.3ebce7f3.png
--rw-r--r--   0 root         (0) root         (0)    18252 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/empty-vulns.1b2994f2.png
--rw-r--r--   0 root         (0) root         (0)      416 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/error-mark.364d0169.svg
--rw-r--r--   0 root         (0) root         (0)     1576 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/evidence-default.2dcc3b35.svg
--rw-r--r--   0 root         (0) root         (0)      215 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/exclamation_error.73360ffd.svg
--rw-r--r--   0 root         (0) root         (0)     1513 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/faraday-logo-nav.8385ead1.svg
--rw-r--r--   0 root         (0) root         (0)      241 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/faraday-logo.6f6c122b.svg
--rw-r--r--   0 root         (0) root         (0)    22547 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/faraday_loadingbar.13bdbd54.gif
--rw-r--r--   0 root         (0) root         (0)     5739 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/faraday_logo.3af44fcb.svg
--rw-r--r--   0 root         (0) root         (0)     4303 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/faraday_logo_product.57beba14.svg
--rw-r--r--   0 root         (0) root         (0)    29976 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ff_2fa.efd0850b.png
--rw-r--r--   0 root         (0) root         (0)    58320 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ff_analytics.b39bc4e5.png
--rw-r--r--   0 root         (0) root         (0)    80103 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ff_duplicates.46352b01.png
--rw-r--r--   0 root         (0) root         (0)    14262 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ff_ldap.e96f786d.png
--rw-r--r--   0 root         (0) root         (0)   137773 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ff_pipelines.165eec78.png
--rw-r--r--   0 root         (0) root         (0)    53910 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ff_planner.7afb07e6.png
--rw-r--r--   0 root         (0) root         (0)    87874 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ff_reporting.a9a7890d.png
--rw-r--r--   0 root         (0) root         (0)    67214 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ff_saml.119fe76f.png
--rw-r--r--   0 root         (0) root         (0)    63209 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ff_scheduler.b29ac5ec.png
--rw-r--r--   0 root         (0) root         (0)   171169 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ff_tags.ccc5427b.png
--rw-r--r--   0 root         (0) root         (0)   183858 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ff_users.ea35eac5.png
--rw-r--r--   0 root         (0) root         (0)     1454 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/generic_file.f9988671.svg
--rw-r--r--   0 root         (0) root         (0)      725 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/grid_view.580f3d12.svg
--rw-r--r--   0 root         (0) root         (0)      931 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/help-sysreq.5680b8ff.svg
--rw-r--r--   0 root         (0) root         (0)     1175 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/help.61ace590.svg
--rw-r--r--   0 root         (0) root         (0)     1027 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ico-web-shell.fc841a37.svg
--rw-r--r--   0 root         (0) root         (0)     1092 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-column.efe44a0e.svg
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-edit.a362c51d.svg
--rw-r--r--   0 root         (0) root         (0)      718 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-more.fd9db67e.svg
--rw-r--r--   0 root         (0) root         (0)      144 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-plus.8879f3f6.svg
--rw-r--r--   0 root         (0) root         (0)     1642 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-tags.c0f5d2b3.svg
--rw-r--r--   0 root         (0) root         (0)     1883 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-token.d7973c77.svg
--rw-r--r--   0 root         (0) root         (0)     1193 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-trash.b1589206.svg
--rw-r--r--   0 root         (0) root         (0)      922 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-trigger-disabled.af2d2680.svg
--rw-r--r--   0 root         (0) root         (0)      922 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-trigger.f9c88d81.svg
--rw-r--r--   0 root         (0) root         (0)      489 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-clipboard.c53f2936.svg
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-close-without-background.9b3b0c89.svg
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-close.9a5cad5c.svg
--rw-r--r--   0 root         (0) root         (0)      605 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-edit-enabled.a68d0409.svg
--rw-r--r--   0 root         (0) root         (0)      837 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-evidence.fdee90dd.svg
--rw-r--r--   0 root         (0) root         (0)      591 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-show-duplicates.79a1569d.svg
--rw-r--r--   0 root         (0) root         (0)      563 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-toolbar-confirmed-on.6c7a2996.svg
--rw-r--r--   0 root         (0) root         (0)     1037 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon-trash-red.1ebe0df4.svg
--rw-r--r--   0 root         (0) root         (0)      694 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon_clearsearch.e7b18936.svg
--rw-r--r--   0 root         (0) root         (0)      717 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon_close_error.459e6ef9.svg
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon_drag.d52758c1.svg
--rw-r--r--   0 root         (0) root         (0)      870 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon_edit.97c1ea04.svg
--rw-r--r--   0 root         (0) root         (0)      429 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon_filter_off.c7a0db30.svg
--rw-r--r--   0 root         (0) root         (0)      568 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon_filter_on.6de198fd.svg
--rw-r--r--   0 root         (0) root         (0)     1603 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon_help.1b34b217.svg
--rw-r--r--   0 root         (0) root         (0)     1074 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon_loupe.663ddfdd.svg
--rw-r--r--   0 root         (0) root         (0)      362 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon_modal_asset.f360b291.svg
--rw-r--r--   0 root         (0) root         (0)      822 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon_severity.b2244c26.svg
--rw-r--r--   0 root         (0) root         (0)      707 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon_upload.cd99484a.svg
--rw-r--r--   0 root         (0) root         (0)     1754 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/icon_users.0781ec97.svg
--rw-r--r--   0 root         (0) root         (0)      969 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/laptop_icon.21863406.svg
--rw-r--r--   0 root         (0) root         (0)      493 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/laquo.d5f6e3f8.svg
--rw-r--r--   0 root         (0) root         (0)     1455 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/list_view.cacc94c7.svg
--rw-r--r--   0 root         (0) root         (0)      649 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/mini-terminal.f5a8e1d0.svg
--rw-r--r--   0 root         (0) root         (0)     3222 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/new_vuln_modal_icon.033159cd.svg
--rw-r--r--   0 root         (0) root         (0)      393 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/next.0e62ddad.svg
--rw-r--r--   0 root         (0) root         (0)      283 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/next_arrow.407b029f.svg
--rw-r--r--   0 root         (0) root         (0)      837 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/noun-help.a93b0458.svg
--rw-r--r--   0 root         (0) root         (0)     1210 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/preferences_icons_Account.e0a4aa09.svg
--rw-r--r--   0 root         (0) root         (0)      757 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/preferences_icons_Authentication.1b59fc92.svg
--rw-r--r--   0 root         (0) root         (0)      390 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/prev.ecd34f23.svg
--rw-r--r--   0 root         (0) root         (0)      851 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/reload.0d7f0f5c.svg
--rw-r--r--   0 root         (0) root         (0)     1260 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/report_small.e8a3d444.svg
--rw-r--r--   0 root         (0) root         (0)     1195 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/reports.f38dca7f.svg
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/resize_bottom_right.eced93cf.svg
--rw-r--r--   0 root         (0) root         (0)     1483 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/save_template.d74f944a.svg
--rw-r--r--   0 root         (0) root         (0)     3621 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/services.0f83c980.svg
--rw-r--r--   0 root         (0) root         (0)      399 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/shape.9ea9d3d6.svg
--rw-r--r--   0 root         (0) root         (0)      482 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/sort.062a68ce.svg
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/star.8eb97b2c.svg
--rw-r--r--   0 root         (0) root         (0)      674 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/status.660ac4e6.svg
--rw-r--r--   0 root         (0) root         (0)     1126 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/tasks_icon.ba912fa5.svg
--rw-r--r--   0 root         (0) root         (0)      842 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/template.bc90870d.svg
--rw-r--r--   0 root         (0) root         (0)    16275 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_arachni.ac5b15cb.png
--rw-r--r--   0 root         (0) root         (0)    11697 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_nessus.8ed3098d.png
--rw-r--r--   0 root         (0) root         (0)    18860 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_nikto.9acc1459.png
--rw-r--r--   0 root         (0) root         (0)    21908 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_nmap.9a81da35.png
--rw-r--r--   0 root         (0) root         (0)    19674 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_openvas.88898507.png
--rw-r--r--   0 root         (0) root         (0)    19425 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_w3af.221ef0f2.png
--rw-r--r--   0 root         (0) root         (0)    14366 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_wpscan.92adc6c5.png
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/tool_trash.e6d04612.svg
--rw-r--r--   0 root         (0) root         (0)     2256 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/tool_wheel.1b4bc890.svg
--rw-r--r--   0 root         (0) root         (0)     1501 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/unknown_filetype.f6b0014d.svg
--rw-r--r--   0 root         (0) root         (0)     1670 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/vulnerabilities.bc957e73.svg
--rw-r--r--   0 root         (0) root         (0)     2873 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/warning-delete.33357364.svg
--rw-r--r--   0 root         (0) root         (0)      813 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/wf_arrow_collapsed.51829f9b.svg
--rw-r--r--   0 root         (0) root         (0)      905 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/wf_arrow_expand.06e6e9bd.svg
--rw-r--r--   0 root         (0) root         (0)     1261 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ws-lock.5d1e24be.svg
--rw-r--r--   0 root         (0) root         (0)     1233 2023-04-03 14:30:06.000000 faradaysec-4.3.4/faraday/server/www/static/media/ws-unlock.b7653513.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.464996 faradaysec-4.3.4/faraday/settings/
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3515 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/settings/base.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/settings/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/settings/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1284 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/settings/reports.py
--rw-rw-rw-   0 root         (0) root         (0)     1769 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/settings/smtp.py
--rw-rw-rw-   0 root         (0) root         (0)     6238 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/start_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.465996 faradaysec-4.3.4/faraday/utils/
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1205 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/utils/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5964 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/utils/faraday_openapi_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2023-04-11 18:16:50.000000 faradaysec-4.3.4/faraday/utils/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:17:14.467996 faradaysec-4.3.4/faradaysec.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7835 2023-04-11 18:17:14.000000 faradaysec-4.3.4/faradaysec.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16938 2023-04-11 18:17:14.000000 faradaysec-4.3.4/faradaysec.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 18:17:14.000000 faradaysec-4.3.4/faradaysec.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-04-11 18:17:14.000000 faradaysec-4.3.4/faradaysec.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1023 2023-04-11 18:17:14.000000 faradaysec-4.3.4/faradaysec.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 18:17:14.000000 faradaysec-4.3.4/faradaysec.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-04-11 18:16:50.000000 faradaysec-4.3.4/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-04-11 18:16:50.000000 faradaysec-4.3.4/requirements_dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-04-11 18:17:14.468996 faradaysec-4.3.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    10462 2023-04-11 18:16:50.000000 faradaysec-4.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.372980 faradaysec-4.3.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-04-12 22:34:29.000000 faradaysec-4.3.5/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    32681 2023-04-12 22:34:29.000000 faradaysec-4.3.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-04-12 22:34:29.000000 faradaysec-4.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7835 2023-04-12 22:34:58.372980 faradaysec-4.3.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6553 2023-04-12 22:34:29.000000 faradaysec-4.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.231971 faradaysec-4.3.5/faraday/
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      533 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/alembic.ini
+-rwxrwxrwx   0 root         (0) root         (0)    11599 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/manage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.232971 faradaysec-4.3.5/faraday/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/README
+-rw-rw-rw-   0 root         (0) root         (0)     2543 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/env.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.260973 faradaysec-4.3.5/faraday/migrations/versions/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      650 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/0409e696eeec_workspace_important_flag_and_risk_.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/06c48492f587_reformat_jira_issue_fields_value.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/077b7c925ded_add_last_run_to_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5283 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/085188e0a016_create_rules_tables.py
+-rw-rw-rw-   0 root         (0) root         (0)      534 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/08d02214aedc_add_advanced_filter_to_executive_report_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/0d216660da28_add_notification_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/0ed0dab44def_add_tags_arguments_for_agent_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/1574fbcf72f5_disable_several_notifications_and_add_event_enabled_flag.py
+-rw-rw-rw-   0 root         (0) root         (0)     3406 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/15d70093d262_severities_histogram_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2735 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/18891ca61db6_add_cascade_delete_from_workspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     2794 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/1b2533cc16fe_fix_custom_fields_display_name_was_used_.py
+-rw-rw-rw-   0 root         (0) root         (0)     4346 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/1d328f7bf643_planner_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      838 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/1dbe9e8e4247_add_rule_execution_start_and_end_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/1e95dde5b9c8_cascade_on_kb.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/20f3d0c2f71f_alter_table_executive_report_add_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1553 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/247a90b029f2_fix_severities_ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2152 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/282ac9b6569f_add_agent_as_import_source_to_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/2a0de6132377_add_searchfilter_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/2ca03a8feef5_workspace_readonly.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/2db31733fb78_unique_field_name_in_customfield.py
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/384784872dc1_add_weight_column_in_role.py
+-rw-rw-rw-   0 root         (0) root         (0)     7804 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/38bb251889e6_bulks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/3eb96406e88d_rename_important_with_importance_and_remove_check_constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/3f771124f0a2_add_metadata_to_cf_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/47e53ddc0308_add_cwe.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/4bb882a7f9b5_enable_notifications_for_v3.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/4d7a8fdd94e4_rename_not_active_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     3746 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/526aa91cac98_vulnerability_merge_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/5272b3f5a820_add_markdown_column_to_exectuive_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/5658775e113f_add_command_id_to_agent_execution.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/581121b181d8_add_owasp_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/59bed5515407_vuln_external_id.py
+-rw-rw-rw-   0 root         (0) root         (0)     1910 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/5cf9660bba80_policyviolationvulnerabilityassociation_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/5d7a930c439e_cve_many_to_many.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/6471033046cb_added_delete_on_cascade_to_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/699402156cf4_update_risk_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     3030 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/7dea3a6caf51_cascade_in_vuls_relation.py
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/84f266a05be3_add_tool_column_to_vuln.py
+-rw-rw-rw-   0 root         (0) root         (0)    13765 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/85aeb4185f98_refactor_cvss.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/877dd088c8cb_comment_ws_not_mandatory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4212 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/89115e133f0a_add_hosts_notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/8a10ff3926a5_2fa_columns.py
+-rw-rw-rw-   0 root         (0) root         (0)     3400 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/904a517a2f0c_create_executor_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/905261860ad0_user_types_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/97a9348d0406_add_fields_to_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/99a740945c44_add_index_into_vulnerability.py
+-rw-rw-rw-   0 root         (0) root         (0)     2280 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/9c4091d1a09b_create_agent_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/9c678c44aa61_add_enabled_field_to_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/a39a3a6e3f99_create_user_preferences_column.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/a4def820a5bb_alter_otp_secret_length_in_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    15209 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/a9fcf8444c79_add_notification_event_and_subscription_.py
+-rw-rw-rw-   0 root         (0) root         (0)     3297 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/aa56852fa76d_update_rule_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     8670 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/abb7ed8c56b4_add_workflow_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/b1d15a55556d_remove_ticketing_tools_credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)     3532 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/b31fa447f00c_add_analytics_monthly_graphs_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/b49d8efbd0c2_add_configuration_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/b5065f401599_report_template_object_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1883 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/be1f942eba28_add_analytics_saved_graphics_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/be89aa03e35e_add_severities_column_to_executive_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/cb25cf42bda7_remove_knowledge_base_aka_pasta_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/d3afdb4e0b11_add_enum_to_comment_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4134 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/d8f0b32a5c0e_cvss_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/e03a13c41a67_check_important_host.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/e61afb450465_add_custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2585 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/ed403da439d4_agents_with_multiple_workspaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/f00247a92a14_add_agent_execution_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3494 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/f0439bf6688a_updating_to_a_role_model_to_use_faraday_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/f0a507afabd4_adding_fs_uniquifier_to_user_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      746 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/f20aa8756612_change_executivereport_field_to_text.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/f28eae25416b_fix_constraint_in_cve_association.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/f6edb9a16479_add_type_to_reference_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2380 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/f82a9136c408_remove_ws_from_agents_and_make_schedule_.py
+-rw-rw-rw-   0 root         (0) root         (0)     2198 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/f8a44acd0e41_add_new_user_role.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/migrations/versions/fa12b8322112_update_workflow_modules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.260973 faradaysec-4.3.5/faraday/openapi/
+-rw-rw-rw-   0 root         (0) root         (0)   197333 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/openapi/faraday_swagger.json
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.265973 faradaysec-4.3.5/faraday/server/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.266973 faradaysec-4.3.5/faraday/server/api/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    75862 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.276974 faradaysec-4.3.5/faraday/server/api/modules/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4359 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/activity_feed.py
+-rw-rw-rw-   0 root         (0) root         (0)    10163 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/agent_auth_token.py
+-rw-rw-rw-   0 root         (0) root         (0)    21460 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/bulk_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4899 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/commandsrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     3171 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/comments.py
+-rw-rw-rw-   0 root         (0) root         (0)     5203 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     9914 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/export_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/get_exploits.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/global_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)    18611 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/hosts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/licenses.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/preferences.py
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/search_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6152 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      728 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/settings_dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/settings_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/swagger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/token.py
+-rw-rw-rw-   0 root         (0) root         (0)     5598 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/upload_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)    12827 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/vulnerability_template.py
+-rw-rw-rw-   0 root         (0) root         (0)    54782 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/vulns.py
+-rw-rw-rw-   0 root         (0) root         (0)     3337 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/websocket_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    21793 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/api/modules/workspaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    23507 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.280974 faradaysec-4.3.5/faraday/server/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2981 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/commands/app_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/commands/change_password.py
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/commands/change_username.py
+-rw-rw-rw-   0 root         (0) root         (0)     3513 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/commands/custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2975 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/commands/faraday_schema_display.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/commands/import_vulnerability_template.py
+-rw-rw-rw-   0 root         (0) root         (0)    20997 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/commands/initdb.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/commands/manage_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/commands/nginx_config.py
+-rwxrwxrwx   0 root         (0) root         (0)     1235 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/commands/reset_db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.280974 faradaysec-4.3.5/faraday/server/commands/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1392 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/commands/templates/nginx_config.j2
+-rw-rw-rw-   0 root         (0) root         (0)     4712 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/default.ini
+-rw-rw-rw-   0 root         (0) root         (0)    15565 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/events.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/extensions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4615 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)   127381 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    12973 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.281974 faradaysec-4.3.5/faraday/server/threads/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/threads/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/threads/ping_home.py
+-rw-rw-rw-   0 root         (0) root         (0)     6565 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/threads/reports_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.287975 faradaysec-4.3.5/faraday/server/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/agents.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/bulk_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/command.py
+-rw-rw-rw-   0 root         (0) root         (0)     2505 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/cvss.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/cwe.py
+-rw-rw-rw-   0 root         (0) root         (0)     8819 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/daemonize.py
+-rw-rw-rw-   0 root         (0) root         (0)    12276 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     8469 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/export.py
+-rw-rw-rw-   0 root         (0) root         (0)    12793 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/invalid_chars.py
+-rw-rw-rw-   0 root         (0) root         (0)     2673 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      570 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)    30446 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/utils/web.py
+-rw-rw-rw-   0 root         (0) root         (0)     6871 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    11162 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/websocket_factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/server/websockets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.289975 faradaysec-4.3.5/faraday/server/www/
+-rw-r--r--   0 root         (0) root         (0)    11309 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/asset-manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-03 14:26:20.000000 faradaysec-4.3.5/faraday/server/www/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/index.html
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-04-03 14:26:20.000000 faradaysec-4.3.5/faraday/server/www/manifest.json
+-rw-r--r--   0 root         (0) root         (0)    14688 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/precache-manifest.76e73c7b229a75e39d1b019b45394088.js
+-rw-r--r--   0 root         (0) root         (0)     1181 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.225971 faradaysec-4.3.5/faraday/server/www/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.292975 faradaysec-4.3.5/faraday/server/www/static/css/
+-rw-r--r--   0 root         (0) root         (0)   183537 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/css/2.b43efbd6.chunk.css
+-rw-r--r--   0 root         (0) root         (0)   317573 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/css/2.b43efbd6.chunk.css.map
+-rw-r--r--   0 root         (0) root         (0)   622929 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/css/main.bd546d28.chunk.css
+-rw-r--r--   0 root         (0) root         (0)   507732 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/css/main.bd546d28.chunk.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.322977 faradaysec-4.3.5/faraday/server/www/static/js/
+-rw-r--r--   0 root         (0) root         (0)  3063891 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/js/2.ebd7c667.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     5668 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/js/2.ebd7c667.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0) 17092240 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/js/2.ebd7c667.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)  1312116 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/js/main.8be13664.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/js/main.8be13664.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)  2617810 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/js/main.8be13664.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/js/runtime-main.ea9693b3.js
+-rw-r--r--   0 root         (0) root         (0)     8286 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/js/runtime-main.ea9693b3.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.367980 faradaysec-4.3.5/faraday/server/www/static/media/
+-rw-r--r--   0 root         (0) root         (0)    79144 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/CentraNo2-Book.386f0594.otf
+-rw-r--r--   0 root         (0) root         (0)    81720 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/CentraNo2-Medium.63911e85.otf
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/Checkbox.b83098ac.svg
+-rw-r--r--   0 root         (0) root         (0)      177 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/Checkbox_empty.195b4c92.svg
+-rw-r--r--   0 root         (0) root         (0)     1263 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/Checkbox_ok.52c5a6cc.svg
+-rw-r--r--   0 root         (0) root         (0)    76768 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/Sequel_Sans_Head_Bold.89985cf2.woff
+-rw-r--r--   0 root         (0) root         (0)    82720 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/Sequel_Sans_Head_Book.b99ba59e.woff
+-rw-r--r--   0 root         (0) root         (0)    78520 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/Sequel_Sans_Head_Medium.db87ffc9.woff
+-rw-r--r--   0 root         (0) root         (0)    79728 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/Sequel_Sans_Head_Roman.db35328c.woff
+-rw-r--r--   0 root         (0) root         (0)    77184 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/Sequel_Sans_Head_SemiBold.48873506.woff
+-rw-r--r--   0 root         (0) root         (0)      713 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/activity-dashboard.b37176e7.svg
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/agent_small.d1a2c9fe.svg
+-rw-r--r--   0 root         (0) root         (0)      629 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/analytics.b5f3011a.svg
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/api_link.dcbdf06d.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/arrow-down.d8661d88.svg
+-rw-r--r--   0 root         (0) root         (0)      294 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/arrow-right.ec48cf40.svg
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/assets.581bf13b.svg
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/automation.a512d67b.svg
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/clear.26371e5f.svg
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/cog.6f2e860c.svg
+-rw-r--r--   0 root         (0) root         (0)     3586 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/command.4ada7185.svg
+-rw-r--r--   0 root         (0) root         (0)      387 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/copy.7e1b1006.svg
+-rw-r--r--   0 root         (0) root         (0)      650 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/copy_link.852fb400.svg
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/customAttributes.c7457305.svg
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/download-icon.eadbcf9c.svg
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/drag.b17c0ec9.svg
+-rw-r--r--   0 root         (0) root         (0)    24438 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/empty-feed.3ebce7f3.png
+-rw-r--r--   0 root         (0) root         (0)    18252 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/empty-vulns.1b2994f2.png
+-rw-r--r--   0 root         (0) root         (0)      416 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/error-mark.364d0169.svg
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/evidence-default.2dcc3b35.svg
+-rw-r--r--   0 root         (0) root         (0)      215 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/exclamation_error.73360ffd.svg
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/faraday-logo-nav.8385ead1.svg
+-rw-r--r--   0 root         (0) root         (0)      241 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/faraday-logo.6f6c122b.svg
+-rw-r--r--   0 root         (0) root         (0)    22547 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/faraday_loadingbar.13bdbd54.gif
+-rw-r--r--   0 root         (0) root         (0)     5739 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/faraday_logo.3af44fcb.svg
+-rw-r--r--   0 root         (0) root         (0)     4303 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/faraday_logo_product.57beba14.svg
+-rw-r--r--   0 root         (0) root         (0)    29976 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ff_2fa.efd0850b.png
+-rw-r--r--   0 root         (0) root         (0)    58320 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ff_analytics.b39bc4e5.png
+-rw-r--r--   0 root         (0) root         (0)    80103 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ff_duplicates.46352b01.png
+-rw-r--r--   0 root         (0) root         (0)    14262 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ff_ldap.e96f786d.png
+-rw-r--r--   0 root         (0) root         (0)   137773 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ff_pipelines.165eec78.png
+-rw-r--r--   0 root         (0) root         (0)    53910 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ff_planner.7afb07e6.png
+-rw-r--r--   0 root         (0) root         (0)    87874 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ff_reporting.a9a7890d.png
+-rw-r--r--   0 root         (0) root         (0)    67214 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ff_saml.119fe76f.png
+-rw-r--r--   0 root         (0) root         (0)    63209 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ff_scheduler.b29ac5ec.png
+-rw-r--r--   0 root         (0) root         (0)   171169 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ff_tags.ccc5427b.png
+-rw-r--r--   0 root         (0) root         (0)   183858 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ff_users.ea35eac5.png
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/generic_file.f9988671.svg
+-rw-r--r--   0 root         (0) root         (0)      725 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/grid_view.580f3d12.svg
+-rw-r--r--   0 root         (0) root         (0)      931 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/help-sysreq.5680b8ff.svg
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/help.61ace590.svg
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ico-web-shell.fc841a37.svg
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-column.efe44a0e.svg
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-edit.a362c51d.svg
+-rw-r--r--   0 root         (0) root         (0)      718 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-more.fd9db67e.svg
+-rw-r--r--   0 root         (0) root         (0)      144 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-plus.8879f3f6.svg
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-tags.c0f5d2b3.svg
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-token.d7973c77.svg
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-trash.b1589206.svg
+-rw-r--r--   0 root         (0) root         (0)      922 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-trigger-disabled.af2d2680.svg
+-rw-r--r--   0 root         (0) root         (0)      922 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-trigger.f9c88d81.svg
+-rw-r--r--   0 root         (0) root         (0)      489 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-clipboard.c53f2936.svg
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-close-without-background.9b3b0c89.svg
+-rw-r--r--   0 root         (0) root         (0)      744 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-close.9a5cad5c.svg
+-rw-r--r--   0 root         (0) root         (0)      605 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-edit-enabled.a68d0409.svg
+-rw-r--r--   0 root         (0) root         (0)      837 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-evidence.fdee90dd.svg
+-rw-r--r--   0 root         (0) root         (0)      591 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-show-duplicates.79a1569d.svg
+-rw-r--r--   0 root         (0) root         (0)      563 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-toolbar-confirmed-on.6c7a2996.svg
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon-trash-red.1ebe0df4.svg
+-rw-r--r--   0 root         (0) root         (0)      694 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon_clearsearch.e7b18936.svg
+-rw-r--r--   0 root         (0) root         (0)      717 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon_close_error.459e6ef9.svg
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon_drag.d52758c1.svg
+-rw-r--r--   0 root         (0) root         (0)      870 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon_edit.97c1ea04.svg
+-rw-r--r--   0 root         (0) root         (0)      429 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon_filter_off.c7a0db30.svg
+-rw-r--r--   0 root         (0) root         (0)      568 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon_filter_on.6de198fd.svg
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon_help.1b34b217.svg
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon_loupe.663ddfdd.svg
+-rw-r--r--   0 root         (0) root         (0)      362 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon_modal_asset.f360b291.svg
+-rw-r--r--   0 root         (0) root         (0)      822 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon_severity.b2244c26.svg
+-rw-r--r--   0 root         (0) root         (0)      707 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon_upload.cd99484a.svg
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/icon_users.0781ec97.svg
+-rw-r--r--   0 root         (0) root         (0)      969 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/laptop_icon.21863406.svg
+-rw-r--r--   0 root         (0) root         (0)      493 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/laquo.d5f6e3f8.svg
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/list_view.cacc94c7.svg
+-rw-r--r--   0 root         (0) root         (0)      649 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/mini-terminal.f5a8e1d0.svg
+-rw-r--r--   0 root         (0) root         (0)     3222 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/new_vuln_modal_icon.033159cd.svg
+-rw-r--r--   0 root         (0) root         (0)      393 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/next.0e62ddad.svg
+-rw-r--r--   0 root         (0) root         (0)      283 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/next_arrow.407b029f.svg
+-rw-r--r--   0 root         (0) root         (0)      837 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/noun-help.a93b0458.svg
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/preferences_icons_Account.e0a4aa09.svg
+-rw-r--r--   0 root         (0) root         (0)      757 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/preferences_icons_Authentication.1b59fc92.svg
+-rw-r--r--   0 root         (0) root         (0)      390 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/prev.ecd34f23.svg
+-rw-r--r--   0 root         (0) root         (0)      851 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/reload.0d7f0f5c.svg
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/report_small.e8a3d444.svg
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/reports.f38dca7f.svg
+-rw-r--r--   0 root         (0) root         (0)      327 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/resize_bottom_right.eced93cf.svg
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/save_template.d74f944a.svg
+-rw-r--r--   0 root         (0) root         (0)     3621 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/services.0f83c980.svg
+-rw-r--r--   0 root         (0) root         (0)      399 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/shape.9ea9d3d6.svg
+-rw-r--r--   0 root         (0) root         (0)      482 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/sort.062a68ce.svg
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/star.8eb97b2c.svg
+-rw-r--r--   0 root         (0) root         (0)      674 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/status.660ac4e6.svg
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/tasks_icon.ba912fa5.svg
+-rw-r--r--   0 root         (0) root         (0)      842 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/template.bc90870d.svg
+-rw-r--r--   0 root         (0) root         (0)    16275 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_arachni.ac5b15cb.png
+-rw-r--r--   0 root         (0) root         (0)    11697 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_nessus.8ed3098d.png
+-rw-r--r--   0 root         (0) root         (0)    18860 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_nikto.9acc1459.png
+-rw-r--r--   0 root         (0) root         (0)    21908 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_nmap.9a81da35.png
+-rw-r--r--   0 root         (0) root         (0)    19674 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_openvas.88898507.png
+-rw-r--r--   0 root         (0) root         (0)    19425 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_w3af.221ef0f2.png
+-rw-r--r--   0 root         (0) root         (0)    14366 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_wpscan.92adc6c5.png
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/tool_trash.e6d04612.svg
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/tool_wheel.1b4bc890.svg
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/unknown_filetype.f6b0014d.svg
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/vulnerabilities.bc957e73.svg
+-rw-r--r--   0 root         (0) root         (0)     2873 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/warning-delete.33357364.svg
+-rw-r--r--   0 root         (0) root         (0)      813 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/wf_arrow_collapsed.51829f9b.svg
+-rw-r--r--   0 root         (0) root         (0)      905 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/wf_arrow_expand.06e6e9bd.svg
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ws-lock.5d1e24be.svg
+-rw-r--r--   0 root         (0) root         (0)     1233 2023-04-03 14:30:06.000000 faradaysec-4.3.5/faraday/server/www/static/media/ws-unlock.b7653513.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.369980 faradaysec-4.3.5/faraday/settings/
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3515 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/settings/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/settings/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/settings/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/settings/reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/settings/smtp.py
+-rw-rw-rw-   0 root         (0) root         (0)     6238 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/start_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.370980 faradaysec-4.3.5/faraday/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/utils/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5964 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/utils/faraday_openapi_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2023-04-12 22:34:29.000000 faradaysec-4.3.5/faraday/utils/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:34:58.372980 faradaysec-4.3.5/faradaysec.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7835 2023-04-12 22:34:58.000000 faradaysec-4.3.5/faradaysec.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16938 2023-04-12 22:34:58.000000 faradaysec-4.3.5/faradaysec.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 22:34:58.000000 faradaysec-4.3.5/faradaysec.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-04-12 22:34:58.000000 faradaysec-4.3.5/faradaysec.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-04-12 22:34:58.000000 faradaysec-4.3.5/faradaysec.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-12 22:34:58.000000 faradaysec-4.3.5/faradaysec.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-04-12 22:34:29.000000 faradaysec-4.3.5/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-04-12 22:34:29.000000 faradaysec-4.3.5/requirements_dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-04-12 22:34:58.373980 faradaysec-4.3.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    10462 2023-04-12 22:34:29.000000 faradaysec-4.3.5/setup.py
```

### Comparing `faradaysec-4.3.4/AUTHORS` & `faradaysec-4.3.5/AUTHORS`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/LICENSE` & `faradaysec-4.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/PKG-INFO` & `faradaysec-4.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faradaysec
-Version: 4.3.4
+Version: 4.3.5
 Summary: Open Source Collaborative Penetration Test and Vulnerability Management Platform https://www.faradaysec.com
 Home-page: https://github.com/infobyte/faraday
 Author: Faradaysec
 Author-email: devel@faradaysec.com
 Project-URL: Bug Reports, https://github.com/infobyte/faraday/issues
 Project-URL: Say Thanks!, http://saythanks.io/to/faradaysec
 Project-URL: Source, https://github.com/infobyte/faraday/
```

### Comparing `faradaysec-4.3.4/README.md` & `faradaysec-4.3.5/README.md`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/alembic.ini` & `faradaysec-4.3.5/faraday/alembic.ini`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/manage.py` & `faradaysec-4.3.5/faraday/manage.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/env.py` & `faradaysec-4.3.5/faraday/migrations/env.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/0409e696eeec_workspace_important_flag_and_risk_.py` & `faradaysec-4.3.5/faraday/migrations/versions/0409e696eeec_workspace_important_flag_and_risk_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/06c48492f587_reformat_jira_issue_fields_value.py` & `faradaysec-4.3.5/faraday/migrations/versions/06c48492f587_reformat_jira_issue_fields_value.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/085188e0a016_create_rules_tables.py` & `faradaysec-4.3.5/faraday/migrations/versions/085188e0a016_create_rules_tables.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/08d02214aedc_add_advanced_filter_to_executive_report_table.py` & `faradaysec-4.3.5/faraday/migrations/versions/08d02214aedc_add_advanced_filter_to_executive_report_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/0d216660da28_add_notification_table.py` & `faradaysec-4.3.5/faraday/migrations/versions/0d216660da28_add_notification_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/0ed0dab44def_add_tags_arguments_for_agent_schedule.py` & `faradaysec-4.3.5/faraday/migrations/versions/0ed0dab44def_add_tags_arguments_for_agent_schedule.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/1574fbcf72f5_disable_several_notifications_and_add_event_enabled_flag.py` & `faradaysec-4.3.5/faraday/migrations/versions/1574fbcf72f5_disable_several_notifications_and_add_event_enabled_flag.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/15d70093d262_severities_histogram_model.py` & `faradaysec-4.3.5/faraday/migrations/versions/15d70093d262_severities_histogram_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/18891ca61db6_add_cascade_delete_from_workspace.py` & `faradaysec-4.3.5/faraday/migrations/versions/18891ca61db6_add_cascade_delete_from_workspace.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/1b2533cc16fe_fix_custom_fields_display_name_was_used_.py` & `faradaysec-4.3.5/faraday/migrations/versions/1b2533cc16fe_fix_custom_fields_display_name_was_used_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/1d328f7bf643_planner_model.py` & `faradaysec-4.3.5/faraday/migrations/versions/1d328f7bf643_planner_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/1dbe9e8e4247_add_rule_execution_start_and_end_fields.py` & `faradaysec-4.3.5/faraday/migrations/versions/1dbe9e8e4247_add_rule_execution_start_and_end_fields.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/1e95dde5b9c8_cascade_on_kb.py` & `faradaysec-4.3.5/faraday/migrations/versions/1e95dde5b9c8_cascade_on_kb.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/20f3d0c2f71f_alter_table_executive_report_add_.py` & `faradaysec-4.3.5/faraday/migrations/versions/20f3d0c2f71f_alter_table_executive_report_add_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/247a90b029f2_fix_severities_ordering.py` & `faradaysec-4.3.5/faraday/migrations/versions/247a90b029f2_fix_severities_ordering.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/282ac9b6569f_add_agent_as_import_source_to_command.py` & `faradaysec-4.3.5/faraday/migrations/versions/282ac9b6569f_add_agent_as_import_source_to_command.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/2a0de6132377_add_searchfilter_table.py` & `faradaysec-4.3.5/faraday/migrations/versions/2a0de6132377_add_searchfilter_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/2db31733fb78_unique_field_name_in_customfield.py` & `faradaysec-4.3.5/faraday/migrations/versions/2db31733fb78_unique_field_name_in_customfield.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/384784872dc1_add_weight_column_in_role.py` & `faradaysec-4.3.5/faraday/migrations/versions/384784872dc1_add_weight_column_in_role.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/38bb251889e6_bulks.py` & `faradaysec-4.3.5/faraday/migrations/versions/38bb251889e6_bulks.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/3eb96406e88d_rename_important_with_importance_and_remove_check_constraint.py` & `faradaysec-4.3.5/faraday/migrations/versions/3eb96406e88d_rename_important_with_importance_and_remove_check_constraint.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/47e53ddc0308_add_cwe.py` & `faradaysec-4.3.5/faraday/migrations/versions/47e53ddc0308_add_cwe.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/4d7a8fdd94e4_rename_not_active_users.py` & `faradaysec-4.3.5/faraday/migrations/versions/4d7a8fdd94e4_rename_not_active_users.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/526aa91cac98_vulnerability_merge_model.py` & `faradaysec-4.3.5/faraday/migrations/versions/526aa91cac98_vulnerability_merge_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/5272b3f5a820_add_markdown_column_to_exectuive_reports.py` & `faradaysec-4.3.5/faraday/migrations/versions/5272b3f5a820_add_markdown_column_to_exectuive_reports.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/5658775e113f_add_command_id_to_agent_execution.py` & `faradaysec-4.3.5/faraday/migrations/versions/5658775e113f_add_command_id_to_agent_execution.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/581121b181d8_add_owasp_model.py` & `faradaysec-4.3.5/faraday/migrations/versions/581121b181d8_add_owasp_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/59bed5515407_vuln_external_id.py` & `faradaysec-4.3.5/faraday/migrations/versions/59bed5515407_vuln_external_id.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/5cf9660bba80_policyviolationvulnerabilityassociation_.py` & `faradaysec-4.3.5/faraday/migrations/versions/5cf9660bba80_policyviolationvulnerabilityassociation_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/5d7a930c439e_cve_many_to_many.py` & `faradaysec-4.3.5/faraday/migrations/versions/5d7a930c439e_cve_many_to_many.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/6471033046cb_added_delete_on_cascade_to_schedule.py` & `faradaysec-4.3.5/faraday/migrations/versions/6471033046cb_added_delete_on_cascade_to_schedule.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/699402156cf4_update_risk_value.py` & `faradaysec-4.3.5/faraday/migrations/versions/699402156cf4_update_risk_value.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/7dea3a6caf51_cascade_in_vuls_relation.py` & `faradaysec-4.3.5/faraday/migrations/versions/7dea3a6caf51_cascade_in_vuls_relation.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/84f266a05be3_add_tool_column_to_vuln.py` & `faradaysec-4.3.5/faraday/migrations/versions/84f266a05be3_add_tool_column_to_vuln.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/85aeb4185f98_refactor_cvss.py` & `faradaysec-4.3.5/faraday/migrations/versions/85aeb4185f98_refactor_cvss.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/877dd088c8cb_comment_ws_not_mandatory.py` & `faradaysec-4.3.5/faraday/migrations/versions/877dd088c8cb_comment_ws_not_mandatory.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/89115e133f0a_add_hosts_notifications.py` & `faradaysec-4.3.5/faraday/migrations/versions/89115e133f0a_add_hosts_notifications.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/8a10ff3926a5_2fa_columns.py` & `faradaysec-4.3.5/faraday/migrations/versions/8a10ff3926a5_2fa_columns.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/904a517a2f0c_create_executor_table.py` & `faradaysec-4.3.5/faraday/migrations/versions/904a517a2f0c_create_executor_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/905261860ad0_user_types_enum.py` & `faradaysec-4.3.5/faraday/migrations/versions/905261860ad0_user_types_enum.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/97a9348d0406_add_fields_to_report.py` & `faradaysec-4.3.5/faraday/migrations/versions/97a9348d0406_add_fields_to_report.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/99a740945c44_add_index_into_vulnerability.py` & `faradaysec-4.3.5/faraday/migrations/versions/99a740945c44_add_index_into_vulnerability.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/9c4091d1a09b_create_agent_table.py` & `faradaysec-4.3.5/faraday/migrations/versions/9c4091d1a09b_create_agent_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/a39a3a6e3f99_create_user_preferences_column.py` & `faradaysec-4.3.5/faraday/migrations/versions/a39a3a6e3f99_create_user_preferences_column.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/a4def820a5bb_alter_otp_secret_length_in_user.py` & `faradaysec-4.3.5/faraday/migrations/versions/a4def820a5bb_alter_otp_secret_length_in_user.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/a9fcf8444c79_add_notification_event_and_subscription_.py` & `faradaysec-4.3.5/faraday/migrations/versions/a9fcf8444c79_add_notification_event_and_subscription_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/aa56852fa76d_update_rule_fields.py` & `faradaysec-4.3.5/faraday/migrations/versions/aa56852fa76d_update_rule_fields.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/abb7ed8c56b4_add_workflow_models.py` & `faradaysec-4.3.5/faraday/migrations/versions/abb7ed8c56b4_add_workflow_models.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/b1d15a55556d_remove_ticketing_tools_credentials.py` & `faradaysec-4.3.5/faraday/migrations/versions/b1d15a55556d_remove_ticketing_tools_credentials.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/b31fa447f00c_add_analytics_monthly_graphs_model.py` & `faradaysec-4.3.5/faraday/migrations/versions/b31fa447f00c_add_analytics_monthly_graphs_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/b49d8efbd0c2_add_configuration_table.py` & `faradaysec-4.3.5/faraday/migrations/versions/b49d8efbd0c2_add_configuration_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/be1f942eba28_add_analytics_saved_graphics_model.py` & `faradaysec-4.3.5/faraday/migrations/versions/be1f942eba28_add_analytics_saved_graphics_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/be89aa03e35e_add_severities_column_to_executive_.py` & `faradaysec-4.3.5/faraday/migrations/versions/be89aa03e35e_add_severities_column_to_executive_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/cb25cf42bda7_remove_knowledge_base_aka_pasta_base.py` & `faradaysec-4.3.5/faraday/migrations/versions/cb25cf42bda7_remove_knowledge_base_aka_pasta_base.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/d3afdb4e0b11_add_enum_to_comment_model.py` & `faradaysec-4.3.5/faraday/migrations/versions/d3afdb4e0b11_add_enum_to_comment_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/d8f0b32a5c0e_cvss_model.py` & `faradaysec-4.3.5/faraday/migrations/versions/d8f0b32a5c0e_cvss_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/e61afb450465_add_custom_fields.py` & `faradaysec-4.3.5/faraday/migrations/versions/e61afb450465_add_custom_fields.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/ed403da439d4_agents_with_multiple_workspaces.py` & `faradaysec-4.3.5/faraday/migrations/versions/ed403da439d4_agents_with_multiple_workspaces.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/f00247a92a14_add_agent_execution_data.py` & `faradaysec-4.3.5/faraday/migrations/versions/f00247a92a14_add_agent_execution_data.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/f0439bf6688a_updating_to_a_role_model_to_use_faraday_.py` & `faradaysec-4.3.5/faraday/migrations/versions/f0439bf6688a_updating_to_a_role_model_to_use_faraday_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/f0a507afabd4_adding_fs_uniquifier_to_user_model.py` & `faradaysec-4.3.5/faraday/migrations/versions/f0a507afabd4_adding_fs_uniquifier_to_user_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/f20aa8756612_change_executivereport_field_to_text.py` & `faradaysec-4.3.5/faraday/migrations/versions/f20aa8756612_change_executivereport_field_to_text.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/f28eae25416b_fix_constraint_in_cve_association.py` & `faradaysec-4.3.5/faraday/migrations/versions/f28eae25416b_fix_constraint_in_cve_association.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/f6edb9a16479_add_type_to_reference_model.py` & `faradaysec-4.3.5/faraday/migrations/versions/f6edb9a16479_add_type_to_reference_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/f82a9136c408_remove_ws_from_agents_and_make_schedule_.py` & `faradaysec-4.3.5/faraday/migrations/versions/f82a9136c408_remove_ws_from_agents_and_make_schedule_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/f8a44acd0e41_add_new_user_role.py` & `faradaysec-4.3.5/faraday/migrations/versions/f8a44acd0e41_add_new_user_role.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/migrations/versions/fa12b8322112_update_workflow_modules.py` & `faradaysec-4.3.5/faraday/migrations/versions/fa12b8322112_update_workflow_modules.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/openapi/faraday_swagger.json` & `faradaysec-4.3.5/faraday/openapi/faraday_swagger.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9880952380952381%*

 * *Differences: {"'info'": "{'title': 'Faraday 4.3.5 API'}"}*

```diff
@@ -1552,15 +1552,15 @@
                 "scheme": "Basic",
                 "type": "http"
             }
         }
     },
     "info": {
         "description": "The Faraday REST API enables you to interact with [our server](https://github.com/infobyte/faraday).\nUse this API to interact or integrate with Faraday server. This page documents the REST API, with HTTP response codes and example requests and responses.",
-        "title": "Faraday 4.3.4 API",
+        "title": "Faraday 4.3.5 API",
         "version": "v3"
     },
     "openapi": "3.0.2",
     "paths": {
         "/change": {},
         "/config": {
             "get": {
```

### Comparing `faradaysec-4.3.4/faraday/requirements.txt` & `faradaysec-4.3.5/faraday/requirements.txt`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/base.py` & `faradaysec-4.3.5/faraday/server/api/base.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/activity_feed.py` & `faradaysec-4.3.5/faraday/server/api/modules/activity_feed.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/agent.py` & `faradaysec-4.3.5/faraday/server/api/modules/agent.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/agent_auth_token.py` & `faradaysec-4.3.5/faraday/server/api/modules/agent_auth_token.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/bulk_create.py` & `faradaysec-4.3.5/faraday/server/api/modules/bulk_create.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/commandsrun.py` & `faradaysec-4.3.5/faraday/server/api/modules/commandsrun.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/comments.py` & `faradaysec-4.3.5/faraday/server/api/modules/comments.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/credentials.py` & `faradaysec-4.3.5/faraday/server/api/modules/credentials.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/custom_fields.py` & `faradaysec-4.3.5/faraday/server/api/modules/custom_fields.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/export_data.py` & `faradaysec-4.3.5/faraday/server/api/modules/export_data.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/get_exploits.py` & `faradaysec-4.3.5/faraday/server/api/modules/get_exploits.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/global_commands.py` & `faradaysec-4.3.5/faraday/server/api/modules/global_commands.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/hosts.py` & `faradaysec-4.3.5/faraday/server/api/modules/hosts.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/info.py` & `faradaysec-4.3.5/faraday/server/api/modules/info.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/licenses.py` & `faradaysec-4.3.5/faraday/server/api/modules/licenses.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/preferences.py` & `faradaysec-4.3.5/faraday/server/api/modules/preferences.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/search_filter.py` & `faradaysec-4.3.5/faraday/server/api/modules/search_filter.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/services.py` & `faradaysec-4.3.5/faraday/server/api/modules/services.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/session.py` & `faradaysec-4.3.5/faraday/server/api/modules/session.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/settings.py` & `faradaysec-4.3.5/faraday/server/api/modules/settings.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/settings_dashboard.py` & `faradaysec-4.3.5/faraday/server/api/modules/settings_dashboard.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/settings_reports.py` & `faradaysec-4.3.5/faraday/server/api/modules/settings_reports.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/swagger.py` & `faradaysec-4.3.5/faraday/server/api/modules/swagger.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/token.py` & `faradaysec-4.3.5/faraday/server/api/modules/token.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/upload_reports.py` & `faradaysec-4.3.5/faraday/server/api/modules/upload_reports.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/vulnerability_template.py` & `faradaysec-4.3.5/faraday/server/api/modules/vulnerability_template.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/vulns.py` & `faradaysec-4.3.5/faraday/server/api/modules/vulns.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/websocket_auth.py` & `faradaysec-4.3.5/faraday/server/api/modules/websocket_auth.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/api/modules/workspaces.py` & `faradaysec-4.3.5/faraday/server/api/modules/workspaces.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/app.py` & `faradaysec-4.3.5/faraday/server/app.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/commands/app_urls.py` & `faradaysec-4.3.5/faraday/server/commands/app_urls.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/commands/change_password.py` & `faradaysec-4.3.5/faraday/server/commands/change_password.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/commands/change_username.py` & `faradaysec-4.3.5/faraday/server/commands/change_username.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/commands/custom_fields.py` & `faradaysec-4.3.5/faraday/server/commands/custom_fields.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/commands/faraday_schema_display.py` & `faradaysec-4.3.5/faraday/server/commands/faraday_schema_display.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/commands/import_vulnerability_template.py` & `faradaysec-4.3.5/faraday/server/commands/import_vulnerability_template.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/commands/initdb.py` & `faradaysec-4.3.5/faraday/server/commands/initdb.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/commands/manage_settings.py` & `faradaysec-4.3.5/faraday/server/commands/manage_settings.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/commands/nginx_config.py` & `faradaysec-4.3.5/faraday/server/commands/nginx_config.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/commands/reset_db.py` & `faradaysec-4.3.5/faraday/server/commands/reset_db.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/commands/templates/nginx_config.j2` & `faradaysec-4.3.5/faraday/server/commands/templates/nginx_config.j2`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/config.py` & `faradaysec-4.3.5/faraday/server/config.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/events.py` & `faradaysec-4.3.5/faraday/server/events.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/fields.py` & `faradaysec-4.3.5/faraday/server/fields.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/models.py` & `faradaysec-4.3.5/faraday/server/models.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/schemas.py` & `faradaysec-4.3.5/faraday/server/schemas.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/threads/ping_home.py` & `faradaysec-4.3.5/faraday/server/threads/ping_home.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/threads/reports_processor.py` & `faradaysec-4.3.5/faraday/server/threads/reports_processor.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/agents.py` & `faradaysec-4.3.5/faraday/server/utils/agents.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/bulk_create.py` & `faradaysec-4.3.5/faraday/server/utils/bulk_create.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/command.py` & `faradaysec-4.3.5/faraday/server/utils/command.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/cvss.py` & `faradaysec-4.3.5/faraday/server/utils/cvss.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/cwe.py` & `faradaysec-4.3.5/faraday/server/utils/cwe.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/daemonize.py` & `faradaysec-4.3.5/faraday/server/utils/daemonize.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/database.py` & `faradaysec-4.3.5/faraday/server/utils/database.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/debug.py` & `faradaysec-4.3.5/faraday/server/utils/debug.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/export.py` & `faradaysec-4.3.5/faraday/server/utils/export.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/filters.py` & `faradaysec-4.3.5/faraday/server/utils/filters.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/logger.py` & `faradaysec-4.3.5/faraday/server/utils/logger.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/reference.py` & `faradaysec-4.3.5/faraday/server/utils/reference.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/search.py` & `faradaysec-4.3.5/faraday/server/utils/search.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/utils/web.py` & `faradaysec-4.3.5/faraday/server/utils/web.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/web.py` & `faradaysec-4.3.5/faraday/server/web.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/websocket_factories.py` & `faradaysec-4.3.5/faraday/server/websocket_factories.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/websockets.py` & `faradaysec-4.3.5/faraday/server/websockets.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/asset-manifest.json` & `faradaysec-4.3.5/faraday/server/www/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/favicon.ico` & `faradaysec-4.3.5/faraday/server/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/index.html` & `faradaysec-4.3.5/faraday/server/www/index.html`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/precache-manifest.76e73c7b229a75e39d1b019b45394088.js` & `faradaysec-4.3.5/faraday/server/www/precache-manifest.76e73c7b229a75e39d1b019b45394088.js`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/service-worker.js` & `faradaysec-4.3.5/faraday/server/www/service-worker.js`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/css/2.b43efbd6.chunk.css` & `faradaysec-4.3.5/faraday/server/www/static/css/2.b43efbd6.chunk.css`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/css/2.b43efbd6.chunk.css.map` & `faradaysec-4.3.5/faraday/server/www/static/css/2.b43efbd6.chunk.css.map`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/css/main.bd546d28.chunk.css` & `faradaysec-4.3.5/faraday/server/www/static/css/main.bd546d28.chunk.css`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/css/main.bd546d28.chunk.css.map` & `faradaysec-4.3.5/faraday/server/www/static/css/main.bd546d28.chunk.css.map`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/js/2.ebd7c667.chunk.js` & `faradaysec-4.3.5/faraday/server/www/static/js/2.ebd7c667.chunk.js`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/js/2.ebd7c667.chunk.js.LICENSE.txt` & `faradaysec-4.3.5/faraday/server/www/static/js/2.ebd7c667.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/js/2.ebd7c667.chunk.js.map` & `faradaysec-4.3.5/faraday/server/www/static/js/2.ebd7c667.chunk.js.map`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/js/main.8be13664.chunk.js` & `faradaysec-4.3.5/faraday/server/www/static/js/main.8be13664.chunk.js`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/js/main.8be13664.chunk.js.map` & `faradaysec-4.3.5/faraday/server/www/static/js/main.8be13664.chunk.js.map`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/js/runtime-main.ea9693b3.js` & `faradaysec-4.3.5/faraday/server/www/static/js/runtime-main.ea9693b3.js`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/js/runtime-main.ea9693b3.js.map` & `faradaysec-4.3.5/faraday/server/www/static/js/runtime-main.ea9693b3.js.map`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/CentraNo2-Book.386f0594.otf` & `faradaysec-4.3.5/faraday/server/www/static/media/CentraNo2-Book.386f0594.otf`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/CentraNo2-Medium.63911e85.otf` & `faradaysec-4.3.5/faraday/server/www/static/media/CentraNo2-Medium.63911e85.otf`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/Checkbox.b83098ac.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/Checkbox.b83098ac.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/Checkbox_ok.52c5a6cc.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/Checkbox_ok.52c5a6cc.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/Sequel_Sans_Head_Bold.89985cf2.woff` & `faradaysec-4.3.5/faraday/server/www/static/media/Sequel_Sans_Head_Bold.89985cf2.woff`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/Sequel_Sans_Head_Book.b99ba59e.woff` & `faradaysec-4.3.5/faraday/server/www/static/media/Sequel_Sans_Head_Book.b99ba59e.woff`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/Sequel_Sans_Head_Medium.db87ffc9.woff` & `faradaysec-4.3.5/faraday/server/www/static/media/Sequel_Sans_Head_Medium.db87ffc9.woff`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/Sequel_Sans_Head_Roman.db35328c.woff` & `faradaysec-4.3.5/faraday/server/www/static/media/Sequel_Sans_Head_Roman.db35328c.woff`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/Sequel_Sans_Head_SemiBold.48873506.woff` & `faradaysec-4.3.5/faraday/server/www/static/media/Sequel_Sans_Head_SemiBold.48873506.woff`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/activity-dashboard.b37176e7.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/activity-dashboard.b37176e7.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/agent_small.d1a2c9fe.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/agent_small.d1a2c9fe.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/analytics.b5f3011a.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/analytics.b5f3011a.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/api_link.dcbdf06d.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/api_link.dcbdf06d.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/assets.581bf13b.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/assets.581bf13b.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/automation.a512d67b.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/automation.a512d67b.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/clear.26371e5f.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/clear.26371e5f.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/cog.6f2e860c.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/cog.6f2e860c.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/command.4ada7185.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/command.4ada7185.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/copy_link.852fb400.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/copy_link.852fb400.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/customAttributes.c7457305.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/customAttributes.c7457305.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/download-icon.eadbcf9c.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/download-icon.eadbcf9c.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/empty-feed.3ebce7f3.png` & `faradaysec-4.3.5/faraday/server/www/static/media/empty-feed.3ebce7f3.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/empty-vulns.1b2994f2.png` & `faradaysec-4.3.5/faraday/server/www/static/media/empty-vulns.1b2994f2.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/evidence-default.2dcc3b35.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/evidence-default.2dcc3b35.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/faraday-logo-nav.8385ead1.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/faraday-logo-nav.8385ead1.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/faraday_loadingbar.13bdbd54.gif` & `faradaysec-4.3.5/faraday/server/www/static/media/faraday_loadingbar.13bdbd54.gif`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/faraday_logo.3af44fcb.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/faraday_logo.3af44fcb.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/faraday_logo_product.57beba14.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/faraday_logo_product.57beba14.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ff_2fa.efd0850b.png` & `faradaysec-4.3.5/faraday/server/www/static/media/ff_2fa.efd0850b.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ff_analytics.b39bc4e5.png` & `faradaysec-4.3.5/faraday/server/www/static/media/ff_analytics.b39bc4e5.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ff_duplicates.46352b01.png` & `faradaysec-4.3.5/faraday/server/www/static/media/ff_duplicates.46352b01.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ff_ldap.e96f786d.png` & `faradaysec-4.3.5/faraday/server/www/static/media/ff_ldap.e96f786d.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ff_pipelines.165eec78.png` & `faradaysec-4.3.5/faraday/server/www/static/media/ff_pipelines.165eec78.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ff_planner.7afb07e6.png` & `faradaysec-4.3.5/faraday/server/www/static/media/ff_planner.7afb07e6.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ff_reporting.a9a7890d.png` & `faradaysec-4.3.5/faraday/server/www/static/media/ff_reporting.a9a7890d.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ff_saml.119fe76f.png` & `faradaysec-4.3.5/faraday/server/www/static/media/ff_saml.119fe76f.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ff_scheduler.b29ac5ec.png` & `faradaysec-4.3.5/faraday/server/www/static/media/ff_scheduler.b29ac5ec.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ff_tags.ccc5427b.png` & `faradaysec-4.3.5/faraday/server/www/static/media/ff_tags.ccc5427b.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ff_users.ea35eac5.png` & `faradaysec-4.3.5/faraday/server/www/static/media/ff_users.ea35eac5.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/generic_file.f9988671.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/generic_file.f9988671.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/grid_view.580f3d12.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/grid_view.580f3d12.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/help-sysreq.5680b8ff.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/help-sysreq.5680b8ff.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/help.61ace590.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/help.61ace590.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ico-web-shell.fc841a37.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/ico-web-shell.fc841a37.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-column.efe44a0e.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-column.efe44a0e.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-edit.a362c51d.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-edit.a362c51d.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-more.fd9db67e.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-more.fd9db67e.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-tags.c0f5d2b3.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-tags.c0f5d2b3.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-token.d7973c77.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-token.d7973c77.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-trash.b1589206.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-trash.b1589206.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-trigger-disabled.af2d2680.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-trigger-disabled.af2d2680.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-action-bar-trigger.f9c88d81.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-action-bar-trigger.f9c88d81.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-close-without-background.9b3b0c89.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-close-without-background.9b3b0c89.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-close.9a5cad5c.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-close.9a5cad5c.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-edit-enabled.a68d0409.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-edit-enabled.a68d0409.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-evidence.fdee90dd.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-evidence.fdee90dd.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-show-duplicates.79a1569d.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-show-duplicates.79a1569d.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-toolbar-confirmed-on.6c7a2996.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-toolbar-confirmed-on.6c7a2996.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon-trash-red.1ebe0df4.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon-trash-red.1ebe0df4.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon_clearsearch.e7b18936.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon_clearsearch.e7b18936.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon_close_error.459e6ef9.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon_close_error.459e6ef9.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon_drag.d52758c1.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon_drag.d52758c1.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon_edit.97c1ea04.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon_edit.97c1ea04.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon_filter_on.6de198fd.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon_filter_on.6de198fd.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon_help.1b34b217.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon_help.1b34b217.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon_loupe.663ddfdd.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon_loupe.663ddfdd.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon_severity.b2244c26.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon_severity.b2244c26.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon_upload.cd99484a.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon_upload.cd99484a.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/icon_users.0781ec97.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/icon_users.0781ec97.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/laptop_icon.21863406.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/laptop_icon.21863406.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/list_view.cacc94c7.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/list_view.cacc94c7.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/mini-terminal.f5a8e1d0.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/mini-terminal.f5a8e1d0.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/new_vuln_modal_icon.033159cd.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/new_vuln_modal_icon.033159cd.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/noun-help.a93b0458.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/noun-help.a93b0458.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/preferences_icons_Account.e0a4aa09.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/preferences_icons_Account.e0a4aa09.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/preferences_icons_Authentication.1b59fc92.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/preferences_icons_Authentication.1b59fc92.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/reload.0d7f0f5c.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/reload.0d7f0f5c.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/report_small.e8a3d444.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/report_small.e8a3d444.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/reports.f38dca7f.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/reports.f38dca7f.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/save_template.d74f944a.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/save_template.d74f944a.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/services.0f83c980.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/services.0f83c980.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/star.8eb97b2c.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/star.8eb97b2c.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/status.660ac4e6.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/status.660ac4e6.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/tasks_icon.ba912fa5.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/tasks_icon.ba912fa5.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/template.bc90870d.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/template.bc90870d.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_arachni.ac5b15cb.png` & `faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_arachni.ac5b15cb.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_nessus.8ed3098d.png` & `faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_nessus.8ed3098d.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_nikto.9acc1459.png` & `faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_nikto.9acc1459.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_nmap.9a81da35.png` & `faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_nmap.9a81da35.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_openvas.88898507.png` & `faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_openvas.88898507.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_w3af.221ef0f2.png` & `faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_w3af.221ef0f2.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/tool_logo_wpscan.92adc6c5.png` & `faradaysec-4.3.5/faraday/server/www/static/media/tool_logo_wpscan.92adc6c5.png`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/tool_trash.e6d04612.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/tool_trash.e6d04612.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/tool_wheel.1b4bc890.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/tool_wheel.1b4bc890.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/unknown_filetype.f6b0014d.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/unknown_filetype.f6b0014d.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/vulnerabilities.bc957e73.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/vulnerabilities.bc957e73.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/warning-delete.33357364.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/warning-delete.33357364.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/wf_arrow_collapsed.51829f9b.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/wf_arrow_collapsed.51829f9b.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/wf_arrow_expand.06e6e9bd.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/wf_arrow_expand.06e6e9bd.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ws-lock.5d1e24be.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/ws-lock.5d1e24be.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/server/www/static/media/ws-unlock.b7653513.svg` & `faradaysec-4.3.5/faraday/server/www/static/media/ws-unlock.b7653513.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/settings/__init__.py` & `faradaysec-4.3.5/faraday/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/settings/base.py` & `faradaysec-4.3.5/faraday/settings/base.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/settings/dashboard.py` & `faradaysec-4.3.5/faraday/settings/dashboard.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/settings/reports.py` & `faradaysec-4.3.5/faraday/settings/reports.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/settings/smtp.py` & `faradaysec-4.3.5/faraday/settings/smtp.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/start_server.py` & `faradaysec-4.3.5/faraday/start_server.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/utils/decorators.py` & `faradaysec-4.3.5/faraday/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/utils/faraday_openapi_plugin.py` & `faradaysec-4.3.5/faraday/utils/faraday_openapi_plugin.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faraday/utils/smtp.py` & `faradaysec-4.3.5/faraday/utils/smtp.py`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faradaysec.egg-info/PKG-INFO` & `faradaysec-4.3.5/faradaysec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faradaysec
-Version: 4.3.4
+Version: 4.3.5
 Summary: Open Source Collaborative Penetration Test and Vulnerability Management Platform https://www.faradaysec.com
 Home-page: https://github.com/infobyte/faraday
 Author: Faradaysec
 Author-email: devel@faradaysec.com
 Project-URL: Bug Reports, https://github.com/infobyte/faraday/issues
 Project-URL: Say Thanks!, http://saythanks.io/to/faradaysec
 Project-URL: Source, https://github.com/infobyte/faraday/
```

### Comparing `faradaysec-4.3.4/faradaysec.egg-info/SOURCES.txt` & `faradaysec-4.3.5/faradaysec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/faradaysec.egg-info/requires.txt` & `faradaysec-4.3.5/faradaysec.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/requirements.txt` & `faradaysec-4.3.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `faradaysec-4.3.4/setup.py` & `faradaysec-4.3.5/setup.py`

 * *Files identical despite different names*

