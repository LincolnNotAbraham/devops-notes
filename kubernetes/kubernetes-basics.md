# Kubernetes Basics

## Comandos Essenciais

```bash
# Listar pods
kubectl get pods

# Listar servicos
kubectl get svc

# Ver logs do pod
kubectl logs pod_name

# Entrar no pod
kubectl exec -it pod_name -- /bin/bash

# Aplicar manifesto
kubectl apply -f manifest.yaml

# Deletar recurso
kubectl delete -f manifest.yaml
```

## Estrutura Basica de um Pod

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: meu-pod
spec:
  containers:
  - name: meu-container
    image: nginx:latest
    ports:
    - containerPort: 80
```
