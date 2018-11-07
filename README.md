# dm-for-cloud-sql-with-service-accounts

This is a dummy Rails app with Postgres database that runs in a Kubernetes kluster at GCP.
Here you can see how to setup everything on GCP using Deployment Manager.


Use Deployment manger to setup
* Cloud SQL with an service account
* Reserving a new static external IP address
```
gcloud compute addresses create [ADDRESS_NAME] \
    [--region [REGION] | --global ] \
    [--ip-version [IPV4 | IPV6]]
```
* SSL loadbalancer

Do what's described in https://cloud.google.com/sql/docs/postgres/connect-kubernetes-engine
