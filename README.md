# prometheus-operator test

This repo is capturing the required config files to test prometheus-operator

## k8s cluster
- create the cluster using kind
- `kind create cluster --config kind-config.yaml`

## jsonnet

The prometheus-operator manifests have been built using the upstream compiling docs from [kube-prometheus](https://github.com/prometheus-operator/kube-prometheus#compiling)

Use `build.sh` to rebuild the yaml manifests after you've modified `example.jsonnet`

Use `kubectl apply ...` to apply the yaml manifests to the cluster.
