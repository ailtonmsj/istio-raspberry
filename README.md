### To install istio
```bash
istioctl operator init --hub=docker.io/querycapistio --tag=1.9.2
```

### Apply files in istio-operator folder
```bash
kubectl apply -f istio-operator/
```

### Install kiali
```bash
kubectl apply -f kiali/
```

### Install grafana
```bash
kubectl apply -f grafana/
```

### Install jaeger
```bash
kubectl apply -f jaeger/
```

### Install prometheus
```bash
kubectl apply -f prometheus/
```