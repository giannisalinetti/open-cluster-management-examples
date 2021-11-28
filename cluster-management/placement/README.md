# Placement example

`Placement` API is used to select a set of managed clusters in one or multiple `ManagedClusterSets` so that the user’s workloads can be deployed to these clusters.

Before creating a `Placement`, users must create a `ManagedClusterSetBinding` to associate a `ManagedClusterSet` to a namespace, in order 
to make it bindable to the `Placement`.

The following example creates the `ManagedClusterSetBinding` and the `Placement` associated to the example `ManagedClusterSet` of this repo:

```
kubectl create -f 01-lab-manageclustersetbinding.yaml
kubectl create -f 02-lab-placement.yaml
```

The `Placement` API automatically generate a `PlacementDecision` resource that contains the selected clusters.
Please refer to the [Placement documentation](https://open-cluster-management.io/concepts/placement/) for more detailes about **Selectors** and
**Prioritzers** that can be used to filter out clusters in a more specific way.