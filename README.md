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
