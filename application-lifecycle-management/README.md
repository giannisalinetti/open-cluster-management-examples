# Application Lifecycle Management examples

This folder contains example to test application lifecycle management features on
Open Cluster Management.

Before beginning, the `application-manager` add-on must be installed on the Hub and Managed clusters.

## Installing on the Hub cluster

To install on the Hub cluster using the `clusteradm` CLI:

```
$ clusteradm install addons --names application-manager --context <HUB_CLUSTER_CONTEXT>
```

This operation will deploy the `channel`, `placementrule`, `subscription` and `appsub-summary` controllers on the Hub cluster.

## Enabling managed clusters

Ensure the `open-cluster-management-agent-addon` exists on the target managed cluster(s).

Execute the following command on the Hub cluster to enable the add-on on the managed cluster(s).

```
$ clusteradm enable addons --names application-manager --clusters <MANAGED_CLUSTER_NAME> --context <HUB_CLUSTER_CONTEXT>
```

It is now possible to test the application examples on the managed clusters.