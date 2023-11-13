## Installs ArgoCD application on K8s cluster
### Deploy using 
``` kubectl apply -f argocd/application/argocd.yaml ```

### Port forward service to port 8082
```
  kubectl port-forward svc/argocd-server -n argocd 8082:443
```
### Locally accessible at:
``` localhost:8082 ```

### TODO:
```- Implement ingress so that ArgoCD can be accessed via DNS name that points to k8s service```
