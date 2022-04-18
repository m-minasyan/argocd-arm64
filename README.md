# How to install ArgoCD on ARM64
1. kubectl --kubeconfig="kubeconfig path" create namespace argocd
2. kubectl --kubeconfig="kubeconfig path" apply -n argocd -f https://raw.githubusercontent.com/m-minasyan/argocd-arm64/main/install.yml
