# helm-umbrella

This is a helm umbrella chart that can be used to deploy multiple helm charts in a single command.
Chart versions can be found at https://artifacthub.io/packages/helm/bitnami

## Usage

To deploy all the charts in this umbrella chart, run the following command:

```bash
helm dependency build
helm install my-chart . --namespace amit --create-namespace
```

To upgrade all the charts in this umbrella chart, run the following command:

```bash
helm dependency update
helm upgrade my-chart . --namespace amit
```

To delete all the charts in this umbrella chart, run the following command:

```bash
helm uninstall my-chart --namespace amit
```

