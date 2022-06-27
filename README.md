# Istio Bookinfo Helm chart

- Based on [Bookinfo Sample Application](https://github.com/istio/istio/tree/master/samples/bookinfo)
- Adopted to use in OpenShift
- Tested on OpenShift version 4.7-4.9

## Prerequirements

[Helm](https://github.com/helm/helm/releases) version 3.x.z

## Installation

```bash
git clone git@github.com:vbelouso/bookinfo-helm-chart.git
helm upgrade --install bookinfo --namespace bookinfo --create-namespace bookinfo-helm-chart/bookinfo/
```

## Uninstall

```bash
helm uninstall bookinfo -n bookinfo
```

## Improvements

- Add global values for configurable services (tags, images).
- Make services disabled/enabled.
