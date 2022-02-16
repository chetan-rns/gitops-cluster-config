# gitops-cluster-config
GitOpsify your OpenShift cluster configurations using the OpenShift GitOps operator. OpenShift GitOps allow admins to manage cluster configurations of their OpenShift clusters. Admins can enable Argo CD instances to manage cluster configurations by setting the environment variable “ARGOCD_CLUSTER_CONFIG_NAMESPACES”. The OpenShift GitOps operator will generate all the necessary permissions to manage cluster configuration resources like Identity Providers, Registries, Builds, Operators, etc.

### Usage

Create an Argo CD Application for a cluster config resource by running the below command:

```bash
oc apply -f <cluster-config-dir>/argocd
```