kubectl create namespace argocd

kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

kubectl get ns

kubectl port-forward svc/argocd-server -n argocd 8080:443

kubectl get secret -n argocd

kubectl get secret argocd-initial-admin-secret -n argocd -o yaml

echo <VALUE> | base64 -d; echo



After the application is defined, apply application.yaml to the cluster
kubectl apply -f application.yaml
