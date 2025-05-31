# ksp-istio-sample

kubectl apply -f nginx-deployment.yaml
kubectl apply -f nginx-service.yaml
kubectl apply -f nginx-gateway.yaml
kubectl apply -f nginx-virtualservice.yaml


kubectl delete -f nginx-deployment.yaml
kubectl delete -f nginx-service.yaml
kubectl delete -f nginx-gateway.yaml
kubectl delete -f nginx-virtualservice.yaml


kubectl apply -f nginx-v1.yaml
kubectl apply -f nginx-v2.yaml
kubectl apply -f nginx-svc.yaml
kubectl apply -f nginx-gateway.yaml
kubectl apply -f nginx-destinationrule.yaml
kubectl apply -f nginx-virtualservice.yaml

nohup kubectl port-forward svc/nginx-sample-svc 80:80 --address <nodeip> &
[1] 18218
watch -n 1 'curl -H "Connection: close" http://<clusterip>:80'





