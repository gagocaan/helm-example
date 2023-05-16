# helm-example

A Helm chart for Kubernetes

## Usage

```bash
helm repo add helm-example https://gagocaan.github.io/helm-example/
helm repo update
```

## Installing the Chart 📦

To install the chart with the release name `test` run:

```bash
helm install test helm-example
```

## Uninstalling the Chart 🗑️

To uninstall the `test` deployment:

```bash
helm uninstall test
```

The command removes all the Kubernetes components associated with the chart and deletes the release.

## Values

| Key | Type | Default | Description |
|---|---|---|---|
| replicaCount | int | 1 | Number of replicas |
| image.repository | string | nginx | The image repository to pull from |
| image.pullPolicy | string | IfNotPresent | The image pull policy |
| ... | ... | ... | ... |

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`.
