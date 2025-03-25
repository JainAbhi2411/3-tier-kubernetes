# 3-tier-kubernetes

kubectl apply -f ./frontend/frontend.yml
kubectl apply -f ./backend/backend-kube-app.yml
kubectl apply -f ./database/postgres-config.yml
kubectl apply -f ./database/postgres-pvc-pv.yml


kubectl exec -it [pod-name] --  psql -h localhost -U admin --password -p 5432 postgresdb
