Minikube start
```
minikube start
```

Create Namespace
```
kubectl create ns odoo 
```
Apply Postgres
```
cd postgres
kubectl apply -f . -n odoo
```
Apply Odoo
```
cd odoo
kubectl apply -f . -n odoo
```
Port Forwarding
```
kubectl get pods -n odoo
kubectl port-forward <pod-name> -n odoo 8069:8069
```
