# k8s cheat sheet

This repo contains some useful commands to deal with kubernetes.

```sh
# list namespaces

$ kubectl get namespaces # simple
$ kubectl describe namespaces # detailed
```

```sh
# list pods

$ kubectl get pods # current namespace

$ kubectl get pods -A # all namespaces
$ kubectl get pods --all-namespaces # all namespaces

$ kubectl get pods -n X # namespace "X"
$ kubectl get pods --namespace X # namespace "X"
```

```sh
# list pods (detailed)
# use "describe" instead of "get"

$ kubectl describe pods
```

```sh
# switch default namespace

$ kubectl config set-context --current --namespace=another-namespace
```