Rancher-Demo-App Chart
----------------------------------------------


| Type | Chart Version | App Version |
| ---- | ------------- | ----------- |
| application | `1.0.0` | `1.0.0` |

## Installing the Chart
```bash
helm install -n 
```
```bash
helm status -n 
```

## Uninstalling the Chart
```bash
helm uninstall -n 
```

## Configuration

The following table lists the configurable parameters of the Rancher-demo-app chart and their default values.

| Parameter | Default | Description |
| --------- | ------- | ----------- |
| `replicaCount` | `6` |  |
| `image.repository` | `"zackbradys/rancher-demo-app"` |  |
| `image.tag` | `"1.0.0"` |  |
| `image.pullPolicy` | `"IfNotPresent"` |  |
| `imagePullSecrets` | `[]` |  |
| `nameOverride` | `""` |  |
| `fullnameOverride` | `""` |  |
| `app.localization.title` | `"Rancher Federal Demo"` |  |
| `app.localization.pets` | `"cows"` | available pets include 'cows' and 'chameleons' and possibly 'cowmeleons' |
| `app.localization.color` | `"black"` | container background color (any color name from the CSS pallete) |
| `service.type` | `"ClusterIP"` |  |
| `service.port` | `80` |  |
| `service.nodePort` | `""` |  |
| `ingress.enabled` | `true` |  |
| `ingress.annotations` | `{}` |  |
| `ingress.paths` | `[]` |  |
| `ingress.host` | `"rancher-demo.7310hargrove.court"` |  |
| `ingress.tls` | `[]` |  |
| `resources` | `{}` |  |
| `nodeSelector` | `{}` |  |
| `tolerations` | `[]` |  |
| `affinity` | `{}` |  |

