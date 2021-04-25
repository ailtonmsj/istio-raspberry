### To access the Kubernetes dashboard use:

#### https://DNS-OR-NGINX-INGRESS-IP:NGINX-HTTPS-PORT/

#### Example:

#### https://teste.com.br:31410/

### To get the dashboard token:

#### kubectl -n kubernetes-dashboard get secret KUBERNETES-DASHBOARD-TOKEN-NAME -o jsonpath={.data.token} | base64 --decode

#### kubectl -n kubernetes-dashboard get secret kubernetes-dashboard-token-vzfmr -o jsonpath={.data.token} | base64 --decode