# Comparing `tmp/auth0-python-4.1.0.tar.gz` & `tmp/auth0-python-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth0-python-4.1.0.tar", last modified: Wed Mar 15 14:43:30 2023, max compression
+gzip compressed data, was "auth0-python-4.1.1.tar", last modified: Thu Apr 13 13:40:41 2023, max compression
```

## Comparing `auth0-python-4.1.0.tar` & `auth0-python-4.1.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.471216 auth0-python-4.1.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-03-15 14:43:30.000000 auth0-python-4.1.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-03-15 14:43:30.471216 auth0-python-4.1.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8039 2023-03-15 14:43:30.000000 auth0-python-4.1.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.459216 auth0-python-4.1.0/auth0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      169 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2776 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/asyncify.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.459216 auth0-python-4.1.0/auth0/authentication/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6779 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/async_token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2439 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2498 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/client_authentication.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/database.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1073 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/delegated.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/enterprise.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7732 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/get_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2268 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/passwordless.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      958 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/revoke_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1137 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/social.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15148 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1499 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/authentication/users.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      572 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/exceptions.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.463216 auth0-python-4.1.0/auth0/management/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1689 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7908 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/actions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1616 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/async_auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3762 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/attack_protection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2603 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/blacklists.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4670 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/branding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/client_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3447 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/client_grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5304 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/clients.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5595 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/connections.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2700 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/custom_domains.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3687 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/device_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2834 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/email_templates.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2831 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/emails.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2750 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5042 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/guardian.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5866 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/hooks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4551 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/jobs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/log_streams.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3742 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/logs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13772 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/organizations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2348 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/prompts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3473 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/resource_servers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7165 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/roles.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4877 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/rules.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2256 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/rules_configs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2039 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2228 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/tenants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/tickets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2608 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/user_blocks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18274 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/users.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2048 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/management/users_by_email.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10884 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4919 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/rest_async.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.463216 auth0-python-4.1.0/auth0/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.467216 auth0-python-4.1.0/auth0/test/authentication/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/authentication/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11856 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/authentication/test_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2446 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/authentication/test_database.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2052 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/authentication/test_delegated.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      789 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/authentication/test_enterprise.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7441 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/authentication/test_get_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3038 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/authentication/test_passwordless.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      936 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/authentication/test_revoke_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1301 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/authentication/test_social.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    32975 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/authentication/test_token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      433 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/authentication/test_users.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.471216 auth0-python-4.1.0/auth0/test/management/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8426 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_actions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_atack_protection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1578 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_blacklists.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4476 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_branding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1992 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_client_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3770 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_client_grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4428 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_clients.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5887 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_connections.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1989 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_custom_domains.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_device_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1674 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_email_endpoints.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_emails.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1449 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5181 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_guardian.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5649 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_hooks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3542 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_jobs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2781 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_log_streams.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1954 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_logs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15308 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_organizations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_prompts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2910 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_resource_servers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30831 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6515 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_roles.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4115 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_rules.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_rules_configs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1364 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_tenants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1236 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_tickets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_user_blocks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14460 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_users.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1398 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test/management/test_users_by_email.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.471216 auth0-python-4.1.0/auth0/test_async/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test_async/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2250 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test_async/test_async_auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10099 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test_async/test_async_token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6618 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/test_async/test_asyncify.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-15 14:43:30.471216 auth0-python-4.1.0/auth0_python.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0_python.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3750 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0_python.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0_python.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0_python.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-03-15 14:43:30.000000 auth0-python-4.1.0/auth0_python.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-03-15 14:43:30.471216 auth0-python-4.1.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2023-03-15 14:43:30.000000 auth0-python-4.1.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.585198 auth0-python-4.1.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-04-13 13:40:41.000000 auth0-python-4.1.1/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-04-13 13:40:41.585198 auth0-python-4.1.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8039 2023-04-13 13:40:41.000000 auth0-python-4.1.1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.569198 auth0-python-4.1.1/auth0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      169 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2776 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/asyncify.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.573198 auth0-python-4.1.1/auth0/authentication/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6779 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/async_token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2439 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2498 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/client_authentication.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/database.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1073 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/delegated.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/enterprise.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7777 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/get_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2268 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/passwordless.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      958 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/revoke_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1137 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/social.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15148 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1499 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/users.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      572 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/exceptions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.577198 auth0-python-4.1.1/auth0/management/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1689 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7908 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/actions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1672 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/async_auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3762 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/attack_protection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3910 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/blacklists.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4670 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/branding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/client_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3447 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/client_grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5304 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/clients.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5595 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/connections.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2700 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/custom_domains.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3687 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/device_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2834 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/email_templates.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2831 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/emails.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2750 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5042 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/guardian.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5866 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/hooks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4551 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/jobs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/log_streams.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3742 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/logs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13772 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/organizations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2348 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/prompts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3473 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/resource_servers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7165 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/roles.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4877 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/rules.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2256 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/rules_configs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2039 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/stats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2228 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/tenants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/tickets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2608 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/user_blocks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18274 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/users.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2048 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/users_by_email.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10884 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4919 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/rest_async.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.577198 auth0-python-4.1.1/auth0/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.581198 auth0-python-4.1.1/auth0/test/authentication/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11856 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2446 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_database.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2052 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_delegated.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      789 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_enterprise.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8225 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_get_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3038 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_passwordless.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      936 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_revoke_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1301 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_social.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    32975 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      433 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_users.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.585198 auth0-python-4.1.1/auth0/test/management/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8426 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_actions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_atack_protection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1578 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_blacklists.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4476 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_branding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1992 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_client_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3770 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_client_grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4428 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_clients.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5887 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_connections.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1989 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_custom_domains.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_device_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1674 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_email_endpoints.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_emails.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1449 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5181 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_guardian.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5649 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_hooks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3542 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_jobs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2781 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_log_streams.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1954 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_logs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15308 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_organizations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_prompts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2910 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_resource_servers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30831 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6515 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_roles.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4115 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_rules.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_rules_configs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1364 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_stats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_tenants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1236 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_tickets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_user_blocks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14460 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_users.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1398 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_users_by_email.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.585198 auth0-python-4.1.1/auth0/test_async/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test_async/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2250 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test_async/test_async_auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10099 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test_async/test_async_token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6618 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test_async/test_asyncify.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.585198 auth0-python-4.1.1/auth0_python.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0_python.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3750 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0_python.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0_python.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0_python.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0_python.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-13 13:40:41.585198 auth0-python-4.1.1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2023-04-13 13:40:41.000000 auth0-python-4.1.1/setup.py
```

### Comparing `auth0-python-4.1.0/LICENSE` & `auth0-python-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/PKG-INFO` & `auth0-python-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth0-python
-Version: 4.1.0
+Version: 4.1.1
 Summary: Auth0 Python SDK
 Home-page: https://github.com/auth0/auth0-python
 Author: Auth0
 Author-email: support@auth0.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auth0-python Version: 4.1.0 Summary: Auth0 Python
+Metadata-Version: 2.1 Name: auth0-python Version: 4.1.1 Summary: Auth0 Python
 SDK Home-page: https://github.com/auth0/auth0-python Author: Auth0 Author-
 email: support@auth0.com License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `auth0-python-4.1.0/README.md` & `auth0-python-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/asyncify.py` & `auth0-python-4.1.1/auth0/asyncify.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/authentication/async_token_verifier.py` & `auth0-python-4.1.1/auth0/authentication/async_token_verifier.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/authentication/base.py` & `auth0-python-4.1.1/auth0/authentication/base.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/authentication/client_authentication.py` & `auth0-python-4.1.1/auth0/authentication/client_authentication.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/authentication/database.py` & `auth0-python-4.1.1/auth0/authentication/database.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/authentication/delegated.py` & `auth0-python-4.1.1/auth0/authentication/delegated.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/authentication/enterprise.py` & `auth0-python-4.1.1/auth0/authentication/enterprise.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/authentication/get_token.py` & `auth0-python-4.1.1/auth0/authentication/get_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,42 +114,42 @@
             },
         )
 
     def login(
         self,
         username,
         password,
-        scope,
-        realm,
-        audience,
+        scope=None,
+        realm=None,
+        audience=None,
         grant_type="http://auth0.com/oauth/grant-type/password-realm",
     ):
         """Calls /oauth/token endpoint with password-realm grant type
 
 
         This is the OAuth 2.0 grant that highly trusted apps utilize in order
         to access an API. In this flow the end-user is asked to fill in credentials
         (username/password) typically using an interactive form in the user-agent
         (browser). This information is later on sent to the client and Auth0.
         It is therefore imperative that the client is absolutely trusted with
         this information.
 
         Args:
-            audience (str): The unique identifier of the target API you want to access.
-
             username (str): Resource owner's identifier
 
             password (str): resource owner's Secret
 
-            scope(str): String value of the different scopes the client is asking for.
+            scope(str, optional): String value of the different scopes the client is asking for.
             Multiple scopes are separated with whitespace.
 
-            realm (str): String value of the realm the user belongs.
+            realm (str, optional): String value of the realm the user belongs.
             Set this if you want to add realm support at this grant.
 
+            audience (str, optional): The unique identifier of the target API you want to access.
+
             grant_type (str, optional): Denotes the flow you're using. For password realm
             use http://auth0.com/oauth/grant-type/password-realm
 
         Returns:
             access_token, id_token
         """
```

### Comparing `auth0-python-4.1.0/auth0/authentication/passwordless.py` & `auth0-python-4.1.1/auth0/authentication/passwordless.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/authentication/revoke_token.py` & `auth0-python-4.1.1/auth0/authentication/revoke_token.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/authentication/social.py` & `auth0-python-4.1.1/auth0/authentication/social.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/authentication/token_verifier.py` & `auth0-python-4.1.1/auth0/authentication/token_verifier.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/authentication/users.py` & `auth0-python-4.1.1/auth0/authentication/users.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/exceptions.py` & `auth0-python-4.1.1/auth0/exceptions.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/__init__.py` & `auth0-python-4.1.1/auth0/management/__init__.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/actions.py` & `auth0-python-4.1.1/auth0/management/actions.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/async_auth0.py` & `auth0-python-4.1.1/auth0/management/async_auth0.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import aiohttp
 
 from ..asyncify import asyncify
-from .auth0 import modules
+from .auth0 import Auth0
 
 
 class AsyncAuth0:
     """Provides easy access to all endpoint classes
 
     Args:
         domain (str): Your Auth0 domain, for example 'username.auth0.com'
@@ -16,16 +16,16 @@
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(self, domain, token, rest_options=None):
         self._services = []
-        for name, cls in modules.items():
-            cls = asyncify(cls)
+        for name, attr in vars(Auth0(domain, token, rest_options=rest_options)).items():
+            cls = asyncify(attr.__class__)
             service = cls(domain=domain, token=token, rest_options=rest_options)
             self._services.append(service)
             setattr(
                 self,
                 name,
                 service,
             )
```

### Comparing `auth0-python-4.1.0/auth0/management/attack_protection.py` & `auth0-python-4.1.1/auth0/management/attack_protection.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/blacklists.py` & `auth0-python-4.1.1/auth0/management/blacklists.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/branding.py` & `auth0-python-4.1.1/auth0/management/branding.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/client_credentials.py` & `auth0-python-4.1.1/auth0/management/client_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/client_grants.py` & `auth0-python-4.1.1/auth0/management/client_grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/clients.py` & `auth0-python-4.1.1/auth0/management/clients.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/connections.py` & `auth0-python-4.1.1/auth0/management/connections.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/custom_domains.py` & `auth0-python-4.1.1/auth0/management/custom_domains.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/device_credentials.py` & `auth0-python-4.1.1/auth0/management/device_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/email_templates.py` & `auth0-python-4.1.1/auth0/management/email_templates.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/emails.py` & `auth0-python-4.1.1/auth0/management/emails.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/grants.py` & `auth0-python-4.1.1/auth0/management/grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/guardian.py` & `auth0-python-4.1.1/auth0/management/guardian.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/hooks.py` & `auth0-python-4.1.1/auth0/management/hooks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/jobs.py` & `auth0-python-4.1.1/auth0/management/jobs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/log_streams.py` & `auth0-python-4.1.1/auth0/management/log_streams.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/logs.py` & `auth0-python-4.1.1/auth0/management/logs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/organizations.py` & `auth0-python-4.1.1/auth0/management/organizations.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/prompts.py` & `auth0-python-4.1.1/auth0/management/prompts.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/resource_servers.py` & `auth0-python-4.1.1/auth0/management/resource_servers.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/roles.py` & `auth0-python-4.1.1/auth0/management/roles.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/rules.py` & `auth0-python-4.1.1/auth0/management/rules.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/rules_configs.py` & `auth0-python-4.1.1/auth0/management/rules_configs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/stats.py` & `auth0-python-4.1.1/auth0/management/stats.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/tenants.py` & `auth0-python-4.1.1/auth0/management/tenants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/tickets.py` & `auth0-python-4.1.1/auth0/management/tickets.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/user_blocks.py` & `auth0-python-4.1.1/auth0/management/user_blocks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/users.py` & `auth0-python-4.1.1/auth0/management/users.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/management/users_by_email.py` & `auth0-python-4.1.1/auth0/management/users_by_email.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/rest.py` & `auth0-python-4.1.1/auth0/rest.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/rest_async.py` & `auth0-python-4.1.1/auth0/rest_async.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/authentication/test_base.py` & `auth0-python-4.1.1/auth0/test/authentication/test_base.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/authentication/test_database.py` & `auth0-python-4.1.1/auth0/test/authentication/test_database.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/authentication/test_delegated.py` & `auth0-python-4.1.1/auth0/test/authentication/test_delegated.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/authentication/test_enterprise.py` & `auth0-python-4.1.1/auth0/test/authentication/test_enterprise.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/authentication/test_get_token.py` & `auth0-python-4.1.1/auth0/test/authentication/test_get_token.py`

 * *Files 7% similar despite different names*

```diff
@@ -160,14 +160,40 @@
                 "realm": "rlm",
                 "audience": "aud",
                 "grant_type": "gt",
             },
         )
 
     @mock.patch("auth0.rest.RestClient.post")
+    def test_login_simple(self, mock_post):
+        g = GetToken("my.domain.com", "cid", client_secret="clsec")
+
+        g.login(
+            username="usrnm",
+            password="pswd",
+        )
+
+        args, kwargs = mock_post.call_args
+
+        self.assertEqual(args[0], "https://my.domain.com/oauth/token")
+        self.assertEqual(
+            kwargs["data"],
+            {
+                "client_id": "cid",
+                "client_secret": "clsec",
+                "username": "usrnm",
+                "password": "pswd",
+                "realm": None,
+                "scope": None,
+                "audience": None,
+                "grant_type": "http://auth0.com/oauth/grant-type/password-realm",
+            },
+        )
+
+    @mock.patch("auth0.rest.RestClient.post")
     def test_refresh_token(self, mock_post):
         g = GetToken("my.domain.com", "cid", client_secret="clsec")
 
         g.refresh_token(
             refresh_token="rt",
             grant_type="gt",
             scope="s",
```

### Comparing `auth0-python-4.1.0/auth0/test/authentication/test_passwordless.py` & `auth0-python-4.1.1/auth0/test/authentication/test_passwordless.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/authentication/test_revoke_token.py` & `auth0-python-4.1.1/auth0/test/authentication/test_revoke_token.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/authentication/test_social.py` & `auth0-python-4.1.1/auth0/test/authentication/test_social.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/authentication/test_token_verifier.py` & `auth0-python-4.1.1/auth0/test/authentication/test_token_verifier.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_actions.py` & `auth0-python-4.1.1/auth0/test/management/test_actions.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_atack_protection.py` & `auth0-python-4.1.1/auth0/test/management/test_atack_protection.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_auth0.py` & `auth0-python-4.1.1/auth0/test/management/test_auth0.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_blacklists.py` & `auth0-python-4.1.1/auth0/test/management/test_blacklists.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_branding.py` & `auth0-python-4.1.1/auth0/test/management/test_branding.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_client_credentials.py` & `auth0-python-4.1.1/auth0/test/management/test_client_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_client_grants.py` & `auth0-python-4.1.1/auth0/test/management/test_client_grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_clients.py` & `auth0-python-4.1.1/auth0/test/management/test_clients.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_connections.py` & `auth0-python-4.1.1/auth0/test/management/test_connections.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_custom_domains.py` & `auth0-python-4.1.1/auth0/test/management/test_custom_domains.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_device_credentials.py` & `auth0-python-4.1.1/auth0/test/management/test_device_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_email_endpoints.py` & `auth0-python-4.1.1/auth0/test/management/test_email_endpoints.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_emails.py` & `auth0-python-4.1.1/auth0/test/management/test_emails.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_grants.py` & `auth0-python-4.1.1/auth0/test/management/test_grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_guardian.py` & `auth0-python-4.1.1/auth0/test/management/test_guardian.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_hooks.py` & `auth0-python-4.1.1/auth0/test/management/test_hooks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_jobs.py` & `auth0-python-4.1.1/auth0/test/management/test_jobs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_log_streams.py` & `auth0-python-4.1.1/auth0/test/management/test_log_streams.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_logs.py` & `auth0-python-4.1.1/auth0/test/management/test_logs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_organizations.py` & `auth0-python-4.1.1/auth0/test/management/test_organizations.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_prompts.py` & `auth0-python-4.1.1/auth0/test/management/test_prompts.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_resource_servers.py` & `auth0-python-4.1.1/auth0/test/management/test_resource_servers.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_rest.py` & `auth0-python-4.1.1/auth0/test/management/test_rest.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_roles.py` & `auth0-python-4.1.1/auth0/test/management/test_roles.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_rules.py` & `auth0-python-4.1.1/auth0/test/management/test_rules.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_rules_configs.py` & `auth0-python-4.1.1/auth0/test/management/test_rules_configs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_stats.py` & `auth0-python-4.1.1/auth0/test/management/test_stats.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_tenants.py` & `auth0-python-4.1.1/auth0/test/management/test_tenants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_tickets.py` & `auth0-python-4.1.1/auth0/test/management/test_tickets.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_user_blocks.py` & `auth0-python-4.1.1/auth0/test/management/test_user_blocks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_users.py` & `auth0-python-4.1.1/auth0/test/management/test_users.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test/management/test_users_by_email.py` & `auth0-python-4.1.1/auth0/test/management/test_users_by_email.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test_async/test_async_auth0.py` & `auth0-python-4.1.1/auth0/test_async/test_async_auth0.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test_async/test_async_token_verifier.py` & `auth0-python-4.1.1/auth0/test_async/test_async_token_verifier.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0/test_async/test_asyncify.py` & `auth0-python-4.1.1/auth0/test_async/test_asyncify.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/auth0_python.egg-info/PKG-INFO` & `auth0-python-4.1.1/auth0_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth0-python
-Version: 4.1.0
+Version: 4.1.1
 Summary: Auth0 Python SDK
 Home-page: https://github.com/auth0/auth0-python
 Author: Auth0
 Author-email: support@auth0.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auth0-python Version: 4.1.0 Summary: Auth0 Python
+Metadata-Version: 2.1 Name: auth0-python Version: 4.1.1 Summary: Auth0 Python
 SDK Home-page: https://github.com/auth0/auth0-python Author: Auth0 Author-
 email: support@auth0.com License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `auth0-python-4.1.0/auth0_python.egg-info/SOURCES.txt` & `auth0-python-4.1.1/auth0_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.0/setup.py` & `auth0-python-4.1.1/setup.py`

 * *Files identical despite different names*

