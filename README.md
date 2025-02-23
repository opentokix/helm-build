# Simple helm chart

This is a simple helm chart that is essentially a helm create example1 that is then built using github actions and published into a github pages site..

## To install the chart

This will add a helm repo and name it "opentokix-helm-build" and then install the chart into a namespace called "helm-test".
example1 is the name of the chart.


```bash
helm repo add opentokix-helm-build https://opentokix.github.io/helm-build/
helm install example1 opentokix-helm-build/example1 -n helm-test --create-namespace
```
## To uninstall the chart

```bash
helm uninstall example1 -n helm-test
```


