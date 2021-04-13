# argocd install 

Bootstrap a cluster with this kustomize application.

We also have the "Application of applications" pattern which will refer to other apps hosted in other git repos.


e.g.

1. create your GKE cluster using terraform
2. last step:

   ```
   kustomize build overlays/dev-central1 | kubectl apply -f -
   ```

   to install argocd and have it deploy everything and sync itself.


