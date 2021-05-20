### To install istio

#### istioctl operator init --hub=docker.io/querycapistio --tag=1.9.2

### Apply files in istio-operator folder
#### kubectl apply -f istio-operator/
#### kubectl apply -f gateway/

### Install kiali
#### kubectl apply -f kiali/

### Install grafana
#### kubectl apply -f grafana/

### Install jaeger
#### kubectl apply -f jaeger/

### Install prometheus
#### kubectl apply -f prometheus/