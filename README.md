# mysql-node-on-kybernetes
steps:
1.create a namespace
2.set the current namespace to the one you created
3.create db-secret
4.create configmap
5.create deployment
6.create service

code for the steps:
kubectl create namespace demo
kubectl config set-context --current --namespace=demo
kubectl create -f secret.yaml
kubectl create -f configmap.yaml
kubectl create -f db-deploymet.yaml
kubectl get pods --watch
