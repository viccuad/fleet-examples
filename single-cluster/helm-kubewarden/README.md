# Helm Multi-Chart Example

This example will deploy Kubewarden packaged as Helm charts from the Kubewarden
Helm repo, https://charts.kubewarden.io, into the `cattle-fleet-system`
namespace.

```yaml
kind: GitRepo
apiVersion: fleet.cattle.io/v1alpha1
metadata:
  name: helm
  namespace: fleet-local
spec:
  repo: https://github.com/viccuad/fleet-examples
  paths:
  - single-cluster/helm-kubewarden
```
