### Create a https nginx application running in a kubernetes cluster

```sh
$ kubectl create configmap nginxconf --from-file=cm/nginx.conf --from-file=cm/prometheus.lua -oyaml --dry-run | kubectl apply -f -

$ kubectl create configmap nginxconfd --from-file=cm/default.conf --dry-run -oyaml | kubectl apply -f -
```