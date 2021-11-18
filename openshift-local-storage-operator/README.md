### Introduction

This folder installs the Red Hat Local Storage operator into a cluster.

### Install with Kustomize

To install the operator and instance using kustomize, first install the operator as follows:

```
oc apply -k openshift-local-storage-operator/operator/overlays/latest
```

Once the operator is running in `openshift-operators` you can then install a logical volume with the following command:

```
oc apply -k openshift-local-storage-operator/logical-volumes/overlays
```
