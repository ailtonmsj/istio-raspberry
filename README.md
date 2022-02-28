### This instalation is for Kubernetes >= 1.21, from 1.22 the CustomResourceDefition api is not compatible with operator instalation in version <= 1.13.0 (apiextensions.k8s.io/v1beta1)
<br/>

# To install Istio and Addons

Install istioctl in version >= 1.13.0 (arm64 version)

```bash
istioctl operator init --hub=docker.io/querycapistio --tag=1.13.0
```

### Apply files in istio-operator folder

```bash
kubectl apply -f istio-operator/
```

### Install prometheus

```bash
kubectl apply -f addons/prometheus/
```

### Install grafana

```bash
kubectl apply -f addons/grafana/
```

### Install jaeger

```bash
kubectl apply -f addons/jaeger/
```

### Install kiali

```bash
kubectl apply -f addons/kiali/
```