### This instalation is for Kubernetes <=1.21, fdrom 1.22 the CustomResourceDefition api is not compatible with operator instalation (apiextensions.k8s.io/v1beta1)

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