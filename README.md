# argocd-metrics-servicemonitors
Prometheus service monitors to automatic discovery and fetch argocd metrics

# How to deploy

Simply run the following commands to deploy it on kubernetes.
N.B prometheus-operator or kube-prometheus-stack must have to deployed before deploying the following commands.

`kubectl apply -f argocd-metrics.yml`

`kubectl apply -f argocd-server-metrics.yml`

`kubectl apply -f argocd-application-metrics.yml`

`kubectl apply -f argocd-repo-metrics.yml`

After deploying it, you can visualize the metrics by importing the following dashboard on Grafana

https://grafana.com/grafana/dashboards/14584-argocd/