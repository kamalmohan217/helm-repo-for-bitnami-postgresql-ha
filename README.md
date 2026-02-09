```
helm upgrade --install postgresql bitnami/postgresql-ha/ -f bitnami/postgresql-ha/values.yaml --create-namespace --namespace postgresql --set postgresql.replicaCount=3,persistence.enabled=true,persistence.size=1Gi,global.defaultStorageClass=standard-rwo,service.type=ClusterIP,postgresql.username=postgres,postgresql.password=Dexter123,postgresql.database=dexter --kube-context=gke_wise-trainer-244916_us-central1_awx-gke-cluster
```
