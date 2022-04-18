# Install ArgoCD
1. kubectl --kubeconfig="kubeconfig path" create namespace argocd
2. kubectl --kubeconfig="kubeconfig path" apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/v2.3.3/manifests/install.yaml
3. wait 5 min
4. kubectl --kubeconfig="kubeconfig path" delete all --all -n argocd
5. wait 5 min or create argocd-initial-admin-secret secret
6. kubectl --kubeconfig="kubeconfig path" apply -n argocd -f https://raw.githubusercontent.com/m-minasyan/argocd-arm64/main/install.yml
