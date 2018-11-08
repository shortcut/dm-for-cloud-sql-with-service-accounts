# dm-for-cloud-sql-with-service-accounts

This is a dummy Rails app with Postgres database that runs in a Kubernetes kluster at GCP.
Here you can see how to setup everything on GCP using Deployment Manager.


Use Deployment manger to setup
* Cloud SQL with an service account
Enable the API
Enable the Cloud SQL Admin API.
[ENABLE THE API](https://console.cloud.google.com/flows/enableapi?apiid=sqladmin&redirect=https://console.cloud.google.com&_ga=2.112788804.-1901542352.1539335125&_gac=1.142207494.1540974947.EAIaIQobChMIk-3V_6Kw3gIVC7nACh0EUgqnEAAYASAAEgKbZvD_BwE)


* Reserving a new static external IP address
```
gcloud compute addresses create pepper-staging --global
```
* SSL loadbalancer

Do what's described in https://cloud.google.com/sql/docs/postgres/connect-kubernetes-engine
