# [PGO](https://github.com/CrunchyData/postgres-operator), Crunchy [Postgres Operator](https://github.com/CrunchyData/postgres-operator) Examples

This repository contains examples for deploying PGO, the Postgres Operator from Crunchy Data, using a variety of examples.

The examples are grouped by various tools that can be used to deploy them.

The best way to get started is to fork this repository and experiment with the examples.

Each of the examples has its own README that guides you through the process of deploying it.

You can find the full [PGO documentation](https://access.crunchydata.com/documentation/postgres-operator/v5/) for the project here:

[https://access.crunchydata.com/documentation/postgres-operator/v5/](https://access.crunchydata.com/documentation/postgres-operator/v5/)

You can find out more information about [PGO](https://github.com/CrunchyData/postgres-operator), the [Postgres Operator](https://github.com/CrunchyData/postgres-operator) from [Crunchy Data](https://www.crunchydata.com) at the project page:

[https://github.com/CrunchyData/postgres-operator](https://github.com/CrunchyData/postgres-operator)

---
## Instalation
### Step 1: Download the Examples
```
git clone

cd postgres-operator-examples
```
### Step 2: Install PGO, the Postgres Operator
```
kubectl apply -k kustomize/install/namespace
kubectl apply --server-side -k kustomize/install/default
```
### Step 3: Create a Postgres Cluster
```
kubectl apply -k kustomize\high-availability
```
### Step 4: Install PGO Monitoring
```
kubectl apply -k kustomize/monitoring
```
---
## Initation PGO K3S Lab
- [x] hippo cluster
- [x] hippo ha
- [x] pgAdmin
- [x] pgo monitoring
- [x] pgadmin hippo cluster
- [x] pgadmin hippo-ha cluster
- [x] keycloak hippo cluster
- [ ] keycloak hippo-ha cluster (bouncer)
- [x] backup manual and scheduler minIO
- [x] patroni hippo-ha cluster
- [ ] tunning
- [x] multiple backup
- [x] test user from pgBouncer
- [ ] restore configuration
- [ ] test chaos
