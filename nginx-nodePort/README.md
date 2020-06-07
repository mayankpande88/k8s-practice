# Example for nodePort service

How to deploy on k8s
```
kubectl apply -f my-app-deployment.yml
```

Visit http://localhost:30007 you will see

```
Server address: 10.1.3.9:80

Server name: my-app-79f768d4f4-79s4v

Date: 07/Jun/2020:16:39:56 +0000

URI: /

Request Id: c7e9c41102f5c0896def80ca76ed9067
```

For cleanup execute below commands
```
kubectl delete deployment my-app
kubectl delete configmap my-app-config
kubectl delete service my-app-service
```
