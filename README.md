# Local Kubernetes Runner

LKR, Local Kubernetes Runner.

Supported engines:
- `k3s`

Supported container engines:
- `docker`
- `podman`

## Get started

```
curl -Ls "https://raw.githubusercontent.com/nicoloboschi/local-kubernetes-runner/main/get-lkr.sh" | bash
```

```
lkr start
lkr kubectl get pods
lkr stop
```