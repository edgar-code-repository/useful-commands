KUBERNETES COMMANDS
-----------------------------------------------------------------------

A few commands to watch and destroy some pods on Kubernetes.

-----------------------------------------------------------------------

**Listing pods, deployments and services:**

```

kubectl -n <namespace> get pods

kubectl -n <namespace> get pods | grep -i <search-pattern>

```

```

kubectl -n <namespace> get deployments

kubectl -n <namespace> get deployments | grep -i <search-pattern>

```

```

kubectl -n <namespace> get services

kubectl -n <namespace> get services | grep -i <search-pattern>

```

-----------------------------------------------------------------------


**Deleting pods, deployments and services:**

```

kubectl delete -n <namespace> <pod_name>

kubectl delete -n <namespace> deployments/<deployment_name>

kubectl delete -n <namespace> services/<service_name>

```

-----------------------------------------------------------------------
