# ManagedClusterSet example

To join the `ManagedCluster` named `lab` to a `ManagedClusterSet` add the following label under `ManagedCluster.metadata.labels` of 
a ManagedCluster resource:

```
apiVersion: cluster.open-cluster-management.io/v1
kind: ManagedCluster
metadata:
  labels:
    cluster.open-cluster-management.io/clusterset: lab
```

The ManagedCluster will be automatically joined to the cluster set.

`ManagedClusterSets` can be used to organize clusters by role (lab, prod, test, dev, etc) or by region (US-East, Europe-Central, etc).

