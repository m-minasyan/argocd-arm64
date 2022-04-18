# Install ArgoCD
kubectl --kubeconfig=C:/Users/minas/.kube/kubeconfig create namespace argocd
kubectl --kubeconfig=C:/Users/minas/.kube/kubeconfig apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/v2.3.3/manifests/install.yaml
## wait 5 min
kubectl --kubeconfig=C:/Users/minas/.kube/kubeconfig delete all --all -n argocd
## wait 5 min or create argocd-initial-admin-secret secret
kubectl --kubeconfig=C:/Users/minas/.kube/kubeconfig apply -n argocd -f https://raw.githubusercontent.com/m-minasyan/argocd-arm64/main/install.yml
