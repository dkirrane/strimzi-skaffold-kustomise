

# This Works
```bash
kubectl apply -k ./kustomize/
kubectl delete -k ./kustomize/
```

# This doesn't work
```bash
skaffold deploy
skaffold delete
```

# Debug
```
skaffold deploy -v debug 2>&1 | grep -i 'Running command'
skaffold delete -v debug 2>&1 | grep -i 'Running command'
```