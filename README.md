# sre-k8s
K8s deployment files

To Deploy app, ensure you've got Kubernetes installed locally or have a cluster you can test on

Run the following:

kubectl apply -f secret.yaml
kubectl apply -f env-variables.yaml
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl apply -f ingress.yaml

Future work - wrap this in a Helm chart

To get the URL run:
kubectl describe service stocks-service
combine LoadBalancer Ingress (localhost for me) and NodePort (30001)

If using docker-desktop with k8s go to http://localhost:30001
