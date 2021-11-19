# Ejercicio 2

### 1. ¿Cúal sería el comando que utilizarías para escalar el número de replicas a 10?

```bash
kubectl scale --replicas=10 rs rs-nginx
```

### 2. Si necesito tener una replica en cada uno de los nodos de Kubernetes, ¿qué objeto se adaptaría mejor?

- **DaemonSet**: Un DaemonSet garantiza que todos los nodos ejecuten una copia de un Pod. Conforme se añade más nodos al clúster, nuevos Pods son añadidos a los mismos. Conforme se elimina nodos del clúster, dichos Pods se destruyen. Al eliminar un DaemonSet se limpian todos los Pods que han sido creados.
