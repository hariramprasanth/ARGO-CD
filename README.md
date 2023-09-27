# ARGOCD
1. Create a namespace for argocd `kubectl create namespace argocd`
2. Run `kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml`

## ARGOCD Apps
1. To install Argocd Apps Run `kubectl apply -f nginx-app.yaml`
2. The nginx-app file have the declartive config for the argocd app
3. It has the source configs which refers to the github repo where the manifest files are stored

Note: For helm based app do `hard refresh`

https://argo-cd.readthedocs.io/en/stable/core_concepts/
src <--Refresh / Hard refresh--> argocd <--sync--> k8 manifest