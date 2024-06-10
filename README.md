# Minikube Cluster with Helm and ArgoCd


# Usage
- Checkout helm branch:
    ```bash
    git checkout helm
    ```
- Expose the ArgoCD Service:
    ```bash
    kubectl port-forward service/argocd-server -n argocd 8080:443
    ```
- To access wordpress:
    ```bash
    minikube service wordpress --url
    ```
- To upgrade helm chart:
    ```bash
    cd helm
    helm upgrade wordpress ./wordpress
    ```