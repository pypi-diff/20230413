# Comparing `tmp/magnum_cluster_api-0.5.2.tar.gz` & `tmp/magnum_cluster_api-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnum_cluster_api-0.5.2.tar", max compression
+gzip compressed data, was "magnum_cluster_api-0.5.3.tar", max compression
```

## Comparing `magnum_cluster_api-0.5.2.tar` & `magnum_cluster_api-0.5.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0    10142 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/LICENSE
--rw-r--r--   0        0        0     2795 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/README.md
--rw-r--r--   0        0        0        0 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/.gitkeep
--rw-r--r--   0        0        0      349 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
--rw-r--r--   0        0        0      437 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
--rw-r--r--   0        0        0    29122 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/README.md
--rw-r--r--   0        0        0    14987 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
--rw-r--r--   0        0        0      827 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
--rw-r--r--   0        0        0     4034 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
--rw-r--r--   0        0        0     2982 2023-04-13 03:28:01.079157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
--rw-r--r--   0        0        0      534 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
--rw-r--r--   0        0        0    13204 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
--rw-r--r--   0        0        0      508 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
--rw-r--r--   0        0        0      972 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
--rw-r--r--   0        0        0      758 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
--rw-r--r--   0        0        0      564 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1807 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
--rw-r--r--   0        0        0      527 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
--rw-r--r--   0        0        0      989 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
--rw-r--r--   0        0        0     1180 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
--rw-r--r--   0        0        0      528 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      960 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
--rw-r--r--   0        0        0      663 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
--rw-r--r--   0        0        0    18003 2023-04-13 03:28:01.023157 magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
--rw-r--r--   0        0        0      843 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/clients.py
--rw-r--r--   0        0        0        0 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/cmd/__init__.py
--rw-r--r--   0        0        0     4019 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/cmd/image_builder.py
--rw-r--r--   0        0        0     4182 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/cmd/image_loader.py
--rw-r--r--   0        0        0      956 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/cmd/proxy.py
--rw-r--r--   0        0        0     1778 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/conf.py
--rw-r--r--   0        0        0    10862 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/driver.py
--rw-r--r--   0        0        0     2155 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/helm.py
--rw-r--r--   0        0        0     3171 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/image_utils.py
--rw-r--r--   0        0        0     1116 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/images.py
--rw-r--r--   0        0        0        0 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/__init__.py
--rw-r--r--   0        0        0     4941 2023-04-13 03:27:57.671137 magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/audit/policy.yaml
--rw-r--r--   0        0        0   235191 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/calico/v3.24.2.yaml
--rw-r--r--   0        0        0      623 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
--rw-r--r--   0        0        0     1430 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
--rw-r--r--   0        0        0     2263 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
--rw-r--r--   0        0        0     4506 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     4009 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml
--rw-r--r--   0        0        0      609 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     3297 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml
--rw-r--r--   0        0        0      194 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/csi/csi-cinder-driver.yaml
--rw-r--r--   0        0        0     1526 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/monitor.py
--rw-r--r--   0        0        0     2880 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/objects.py
--rw-r--r--   0        0        0      828 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/privsep/__init__.py
--rw-r--r--   0        0        0     1333 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/privsep/haproxy.py
--rw-r--r--   0        0        0    11719 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/proxy/manager.py
--rw-r--r--   0        0        0     3616 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/proxy/structs.py
--rw-r--r--   0        0        0      580 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
--rw-r--r--   0        0        0     1511 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/proxy/utils.py
--rw-r--r--   0        0        0    74957 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/resources.py
--rw-r--r--   0        0        0     1492 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/service.py
--rw-r--r--   0        0        0     3445 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/tests/test_helm.py
--rw-r--r--   0        0        0     1598 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/tests/test_image_utils.py
--rw-r--r--   0        0        0     2759 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/tests/test_images.py
--rw-r--r--   0        0        0     7554 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/magnum_cluster_api/utils.py
--rw-r--r--   0        0        0     1186 2023-04-13 03:27:57.675137 magnum_cluster_api-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 magnum_cluster_api-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2795 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/.gitkeep
+-rw-r--r--   0        0        0      349 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
+-rw-r--r--   0        0        0      437 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
+-rw-r--r--   0        0        0    29122 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/README.md
+-rw-r--r--   0        0        0    14987 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
+-rw-r--r--   0        0        0      827 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
+-rw-r--r--   0        0        0     4034 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2982 2023-04-13 21:21:56.335576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
+-rw-r--r--   0        0        0      534 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
+-rw-r--r--   0        0        0    13204 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
+-rw-r--r--   0        0        0      508 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
+-rw-r--r--   0        0        0      972 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
+-rw-r--r--   0        0        0      758 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
+-rw-r--r--   0        0        0      564 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1807 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
+-rw-r--r--   0        0        0      527 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
+-rw-r--r--   0        0        0      989 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
+-rw-r--r--   0        0        0     1180 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
+-rw-r--r--   0        0        0      528 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      960 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0      663 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
+-rw-r--r--   0        0        0    18003 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
+-rw-r--r--   0        0        0      843 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/clients.py
+-rw-r--r--   0        0        0        0 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/__init__.py
+-rw-r--r--   0        0        0     4019 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/image_builder.py
+-rw-r--r--   0        0        0     4182 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/image_loader.py
+-rw-r--r--   0        0        0      956 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/proxy.py
+-rw-r--r--   0        0        0     1778 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/conf.py
+-rw-r--r--   0        0        0    10862 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/driver.py
+-rw-r--r--   0        0        0     2155 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/helm.py
+-rw-r--r--   0        0        0     3171 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/image_utils.py
+-rw-r--r--   0        0        0     1116 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/images.py
+-rw-r--r--   0        0        0        0 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/__init__.py
+-rw-r--r--   0        0        0     4941 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/audit/policy.yaml
+-rw-r--r--   0        0        0   235191 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/calico/v3.24.2.yaml
+-rw-r--r--   0        0        0      623 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
+-rw-r--r--   0        0        0     1430 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
+-rw-r--r--   0        0        0     2263 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
+-rw-r--r--   0        0        0     4506 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     4034 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml
+-rw-r--r--   0        0        0      609 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     3307 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      194 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/csi-cinder-driver.yaml
+-rw-r--r--   0        0        0     1526 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/monitor.py
+-rw-r--r--   0        0        0     2880 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/objects.py
+-rw-r--r--   0        0        0      828 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/privsep/__init__.py
+-rw-r--r--   0        0        0     1333 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/privsep/haproxy.py
+-rw-r--r--   0        0        0    11719 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/manager.py
+-rw-r--r--   0        0        0     3616 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/structs.py
+-rw-r--r--   0        0        0      580 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
+-rw-r--r--   0        0        0     1511 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/utils.py
+-rw-r--r--   0        0        0    74957 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/resources.py
+-rw-r--r--   0        0        0     1492 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/service.py
+-rw-r--r--   0        0        0     3445 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/tests/test_helm.py
+-rw-r--r--   0        0        0     1731 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/tests/test_image_utils.py
+-rw-r--r--   0        0        0     2759 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/tests/test_images.py
+-rw-r--r--   0        0        0     7554 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/utils.py
+-rw-r--r--   0        0        0     1186 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 magnum_cluster_api-0.5.3/PKG-INFO
```

### Comparing `magnum_cluster_api-0.5.2/LICENSE` & `magnum_cluster_api-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/README.md` & `magnum_cluster_api-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/README.md` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/charts/cluster-autoscaler/values.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/values.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/clients.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/clients.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/cmd/image_builder.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/image_builder.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/cmd/image_loader.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/image_loader.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/cmd/proxy.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/proxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/conf.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/conf.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/driver.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/driver.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/helm.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/image_utils.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/images.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/audit/policy.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/audit/policy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/calico/v3.24.2.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/calico/v3.24.2.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       - args:
         - --csi-address=$(ADDRESS)
         - --timeout=3m
         - --leader-election=true
         env:
         - name: ADDRESS
           value: /var/lib/csi/sockets/pluginproxy/csi.sock
-        image: k8s.gcr.io/sig-storage/csi-attacher:v3.4.0
+        image: registry.k8s.io/sig-storage/csi-attacher:v3.4.0
         imagePullPolicy: IfNotPresent
         name: csi-attacher
         volumeMounts:
         - mountPath: /var/lib/csi/sockets/pluginproxy/
           name: socket-dir
       - args:
         - --csi-address=$(ADDRESS)
@@ -44,54 +44,54 @@
         - --default-fstype=ext4
         - --feature-gates=Topology=true
         - --extra-create-metadata
         - --leader-election=true
         env:
         - name: ADDRESS
           value: /var/lib/csi/sockets/pluginproxy/csi.sock
-        image: k8s.gcr.io/sig-storage/csi-provisioner:v3.1.0
+        image: registry.k8s.io/sig-storage/csi-provisioner:v3.1.0
         imagePullPolicy: IfNotPresent
         name: csi-provisioner
         volumeMounts:
         - mountPath: /var/lib/csi/sockets/pluginproxy/
           name: socket-dir
       - args:
         - --csi-address=$(ADDRESS)
         - --timeout=3m
         - --extra-create-metadata
         - --leader-election=true
         env:
         - name: ADDRESS
           value: /var/lib/csi/sockets/pluginproxy/csi.sock
-        image: k8s.gcr.io/sig-storage/csi-snapshotter:v6.0.1
+        image: registry.k8s.io/sig-storage/csi-snapshotter:v6.0.1
         imagePullPolicy: Always
         name: csi-snapshotter
         volumeMounts:
         - mountPath: /var/lib/csi/sockets/pluginproxy/
           name: socket-dir
       - args:
         - --csi-address=$(ADDRESS)
         - --timeout=3m
         - --handle-volume-inuse-error=false
         - --leader-election=true
         env:
         - name: ADDRESS
           value: /var/lib/csi/sockets/pluginproxy/csi.sock
-        image: k8s.gcr.io/sig-storage/csi-resizer:v1.4.0
+        image: registry.k8s.io/sig-storage/csi-resizer:v1.4.0
         imagePullPolicy: IfNotPresent
         name: csi-resizer
         volumeMounts:
         - mountPath: /var/lib/csi/sockets/pluginproxy/
           name: socket-dir
       - args:
         - --csi-address=$(ADDRESS)
         env:
         - name: ADDRESS
           value: /var/lib/csi/sockets/pluginproxy/csi.sock
-        image: k8s.gcr.io/sig-storage/livenessprobe:v2.7.0
+        image: registry.k8s.io/sig-storage/livenessprobe:v2.7.0
         name: liveness-probe
         volumeMounts:
         - mountPath: /var/lib/csi/sockets/pluginproxy/
           name: socket-dir
       - args:
         - /bin/cinder-csi-plugin
         - --endpoint=$(CSI_ENDPOINT)
```

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml` & `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -27,25 +27,25 @@
           value: /csi/csi.sock
         - name: DRIVER_REG_SOCK_PATH
           value: /var/lib/kubelet/plugins/cinder.csi.openstack.org/csi.sock
         - name: KUBE_NODE_NAME
           valueFrom:
             fieldRef:
               fieldPath: spec.nodeName
-        image: k8s.gcr.io/sig-storage/csi-node-driver-registrar:v2.5.1
+        image: registry.k8s.io/sig-storage/csi-node-driver-registrar:v2.5.1
         imagePullPolicy: IfNotPresent
         name: node-driver-registrar
         volumeMounts:
         - mountPath: /csi
           name: socket-dir
         - mountPath: /registration
           name: registration-dir
       - args:
         - --csi-address=/csi/csi.sock
-        image: k8s.gcr.io/sig-storage/livenessprobe:v2.7.0
+        image: registry.k8s.io/sig-storage/livenessprobe:v2.7.0
         name: liveness-probe
         volumeMounts:
         - mountPath: /csi
           name: socket-dir
       - args:
         - /bin/cinder-csi-plugin
         - --endpoint=$(CSI_ENDPOINT)
```

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/monitor.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/monitor.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/objects.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/objects.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/privsep/__init__.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/privsep/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/privsep/haproxy.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/privsep/haproxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/proxy/manager.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/manager.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/proxy/structs.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/structs.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/proxy/templates/haproxy.cfg.j2` & `magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/proxy/utils.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/resources.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/resources.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/service.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/service.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/tests/test_helm.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/tests/test_image_utils.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/tests/test_image_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,26 +13,35 @@
 # under the License.
 
 import glob
 import os
 import uuid
 
 import pkg_resources
+import pytest
 import yaml
 
 from magnum_cluster_api import image_utils
 
 
-def test_update_manifest_images_for_calico():
+@pytest.mark.parametrize(
+    "glob_path",
+    [
+        "calico/*.yaml",
+        "ccm/*.yaml",
+        "csi/*.yaml",
+    ],
+)
+def test_update_manifest_images(glob_path):
     manifests_path = pkg_resources.resource_filename("magnum_cluster_api", "manifests")
     repository = "quay.io/test"
 
     cluster_uuid = str(uuid.uuid4())
 
-    for manifest_file in glob.glob(os.path.join(manifests_path, "calico/*.yaml")):
+    for manifest_file in glob.glob(os.path.join(manifests_path, glob_path)):
         data = image_utils.update_manifest_images(
             cluster_uuid,
             manifest_file,
             repository=repository,
         )
 
         for doc in yaml.safe_load_all(data):
```

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/tests/test_images.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/magnum_cluster_api/utils.py` & `magnum_cluster_api-0.5.3/magnum_cluster_api/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.2/pyproject.toml` & `magnum_cluster_api-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnum-cluster-api"
-version = "0.5.2"
+version = "0.5.3"
 description = "Cluster API driver for Magnum"
 authors = ["Mohammed Naser <mnaser@vexxhost.com>"]
 readme = "README.md"
 packages = [{include = "magnum_cluster_api"}]
 include = ["magnum_cluster_api/charts/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `magnum_cluster_api-0.5.2/PKG-INFO` & `magnum_cluster_api-0.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnum-cluster-api
-Version: 0.5.2
+Version: 0.5.3
 Summary: Cluster API driver for Magnum
 Author: Mohammed Naser
 Author-email: mnaser@vexxhost.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

