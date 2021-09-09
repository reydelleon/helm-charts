# Event Store DB

To install Event Store DB in the Kubernetes cluster with the default configuration, run the following commands in the root of this folder.

```
helm repo add eventstore https://eventstore.github.io/EventStore.Charts
helm repo update
helm install <your-release-name> eventstore/eventstore --set 'admin.password=<your-custom-password>'
```

The `values.yml` file in this directory can be used to customize the configuration of the Event Store DB instance. You can find all configurable values [here](https://github.com/EventStore/EventStore.Charts/blob/master/stable/eventstore/README.md#configuration)