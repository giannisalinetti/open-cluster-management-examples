# ManifestWork example

In OCM a `ManifestWork` is a resource that groups Kubernetes resources to be applied to a managed cluster.
The `klusterlet-work-agent` in the managed cluster is responsible to enforce the status of the object.
If the objects are abailable the Work Agent returns an `Available` state, and returns an `Applied` 
state in case of creation of the objects.

The example `hello-work-manifestwork.yaml` must be created in the namespace of the target cluster.
The example uses a `cluster` namespace in the Hub cluster to address the resource creation to the
cluster named `cluster1`.
