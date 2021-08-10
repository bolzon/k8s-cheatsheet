# k8s cheat sheet

This repo contains some useful commands to deal with kubernetes.

```sh
# list namespaces

$ kubectl get namespaces # simple
$ kubectl describe namespaces # detailed
```

```sh
# switch default namespace

$ kubectl config set-context --current --namespace=<namespace-name>
```

```sh
# list pods

$ kubectl get pods # current namespace

$ kubectl get pods -A # all namespaces
$ kubectl get pods --all-namespaces # all namespaces

$ kubectl get pods -n <namespace>
$ kubectl get pods --namespace <namespace>
```

```sh
# list pods (detailed)
# use "describe" instead of "get"

$ kubectl describe pods
```

```sh
# get contexts

$ kubectl config get-contexts
```

```sh
# set another context

$ kubectl config use-context <context-name>
```
