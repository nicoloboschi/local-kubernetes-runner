# Local Kubernetes Runner

LKR, Local Kubernetes Runner.

Supported engines:
- `k3s`

## Requirements
- Docker

## Get started

```
curl -Ls "https://raw.githubusercontent.com/nicoloboschi/local-kubernetes-runner/main/get-lkr.sh" | bash
```


## Cluster lifecycle
To start the kubernetes cluster:

```
lkr start
# lkr logs
# lkr stop
```

To load images to the cluster from the host:

```
lkr load <myimage>
```

To debug the node: 

```
lkr shell
```

## Working with applications

LKR doesn't change your local kube config.
In order to deploy and monitor applications in LKR, you need to prepend your commands with `lkr`.

```
lkr kubectl get pods
lkr helm install
```

`lkr` also introduces shortcuts for the most common tools.


### Kubectl

```
lkr k get pods
```

### K9s

```
lkr 9
```



