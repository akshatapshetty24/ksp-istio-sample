# ksp-istio-sample

kubectl apply -f nginx-deployment.yaml
kubectl apply -f nginx-service.yaml
kubectl apply -f nginx-gateway.yaml
kubectl apply -f nginx-virtualservice.yaml


kubectl delete -f nginx-deployment.yaml
kubectl delete -f nginx-service.yaml
kubectl delete -f nginx-gateway.yaml
kubectl delete -f nginx-virtualservice.yaml
