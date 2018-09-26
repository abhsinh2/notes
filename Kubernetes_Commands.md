kubectl get pods -v=9

curl http://127.0.0.1:8001/api/v1/namespaces/default/pods

### Show PODs with labels

`kubectl get pods --show-labels`

`kubectl get pods -Lapp`

### Show PODs with label app=foo

`kubectl get pods -l app=foo`

kubectl label pods <POD> foo=<> app=<> --overwrite

### Show endpoints

kubectl get endpoints

### Scale deployments

kubectl scale deployments <NAME> --replica 3

### Query JSON

```
kubectl get pods -l app=foo -o json | jq -r

kubectl get pods -l app=foo -o json | jq -r .items[].status.podIP
```
