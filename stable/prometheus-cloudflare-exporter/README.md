# prometheus-cloudflare-exporter

![Version: 0.0.2](https://img.shields.io/badge/Version-0.0.2-informational?style=flat-square) ![AppVersion: 1.2.0](https://img.shields.io/badge/AppVersion-1.2.0-informational?style=flat-square)

Cloudflare metrics exporter

**Homepage:** <https://github.com/wehkamp/docker-prometheus-cloudflare-exporter>

## How to install this chart

A simple install with default values, latest chart version and generated name:

```console
helm install --generate-name oci://ghcr.io/deliveryhero/helm-charts/prometheus-cloudflare-exporter
```

To install a specific version of this chart:

```console
helm install --generate-name oci://ghcr.io/deliveryhero/helm-charts/prometheus-cloudflare-exporter --version 0.0.2
```

To install the chart with the release name `my-release`:

```console
helm install my-release oci://ghcr.io/deliveryhero/helm-charts/prometheus-cloudflare-exporter
```

To install with some set values:

```console
helm install my-release oci://ghcr.io/deliveryhero/helm-charts/prometheus-cloudflare-exporter --set values_key1=value1 --set values_key2=value2
```

To install with custom values file:

```console
helm install my-release oci://ghcr.io/deliveryhero/helm-charts/prometheus-cloudflare-exporter -f values.yaml
```

## Source Code

* <https://github.com/wehkamp/docker-prometheus-cloudflare-exporter>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| cloudflare.auth_email | string | `"Change ME>"` |  |
| cloudflare.auth_key | string | `"<Change ME>"` |  |
| cloudflare.zone | string | `"<Change ME>"` |  |
| env | object | `{}` |  |
| extraLabels | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"osig/prometheus-cloudflare-exporter"` |  |
| image.tag | string | `"1.2.0"` |  |
| imagePullSecrets | list | `[]` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations."prometheus.io/path" | string | `"/metrics"` |  |
| podAnnotations."prometheus.io/port" | string | `"9199"` |  |
| podAnnotations."prometheus.io_scrape" | string | `"true"` |  |
| podLabels | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| service.create | bool | `false` |  |
| serviceAccountName | string | `""` | service account to be used by the containers |
| tolerations | list | `[]` |  |

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| javad-hajiani |  | <https://github.com/javad-hajiani> |

## Chart source and versions

Chart source: [github.com/deliveryhero/helm-charts/prometheus-cloudflare-exporter](https://github.com/deliveryhero/helm-charts/tree/master/stable/prometheus-cloudflare-exporter)

Older chart versions: [github.com/deliveryhero/helm-charts/pkgs/container/helm-charts/prometheus-cloudflare-exporter](https://github.com/deliveryhero/helm-charts/pkgs/container/helm-charts%2Fprometheus-cloudflare-exporter)
