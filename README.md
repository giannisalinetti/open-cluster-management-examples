# Open Cluster Management examples

This repository contains examples to be applied to an Open Cluster Management lab.
Materials inside this repository are intended for demo purposes, not production.

The examples in this repository are based on the official Open Cluster Management [documentation](https://open-cluster-management.io/concepts/).

## Application Lifecycle Management

Open Cluster Management enables a GitOps-based approach to manage applications over
clusters. The following examples are available:

- [nginx-app](application-lifecycle-management/nginx-app): a basic Nginx deployment and service created on clusters that match label-based PlacementRule.

## Cluster Management

This folder contains practical example of multi-cluster-management:

- [ManagedClusterSets](cluster-management/managedclustersets): an example of a `ManagedClusterSet` creation.
- [ManifestWork](cluster-management/manifestwork): a sample `ManifestWork` that can be created on managed clusters.

### Maintainers
Gianni Salinetti <gsalinet@redhat.com>