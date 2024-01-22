# app-of-apps

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.16.0](https://img.shields.io/badge/AppVersion-1.16.0-informational?style=flat-square)

An application that launches other applications.

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Andrew Linzie | <caerulescens.github@proton.me> |  |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| applications.argocd.enabled | bool | `false` | argocd enable: 'true', 'false' |
| applications.argocd.namespace | string | `"argocd"` | argocd namespace |
| applications.argocd.revision | string | `"5.49.0"` | argocd version |
| applications.argocd.wave | int | `-120` |  |
| applications.certManager.enabled | bool | `false` | cert-manager enable: 'true', 'false' |
| applications.certManager.namespace | string | `"cert-manager"` | cert-manager namespace |
| applications.certManager.revision | string | `"1.13.2"` | cert-manager version |
| applications.certManager.wave | int | `-190` |  |
| applications.istio.base.namespace | string | `"istio-system"` | istio-base namespace |
| applications.istio.base.wave | int | `-220` |  |
| applications.istio.enabled | bool | `false` | istio enable: 'true', 'false' |
| applications.istio.gateway.namespace | string | `"istio-ingress"` | gateway namespace |
| applications.istio.gateway.wave | int | `-200` |  |
| applications.istio.istiod.namespace | string | `"istio-system"` | istiod namespace |
| applications.istio.istiod.wave | int | `-210` |  |
| applications.istio.revision | string | `"1.18.0"` | istio version |
| applications.kiali.enabled | bool | `false` | kiali enable: 'true', 'false' |
| applications.kiali.namespace | string | `"kiali-operator"` | kiali namespace |
| applications.kiali.revision | string | `"1.70.0"` | kiali version |
| applications.kiali.wave | int | `-130` |  |
| applications.knative.enabled | bool | `false` | knative enable: 'true', 'false' |
| applications.knative.eventing.namespace | string | `"knative-eventing"` | knative eventing namespace |
| applications.knative.eventing.version | string | `"1.11.0"` | knative eventing version |
| applications.knative.eventing.wave | int | `-90` |  |
| applications.knative.operator.namespace | string | `"default"` | knative operator namespace |
| applications.knative.operator.version | string | `"1.11.0"` | knative operator version |
| applications.knative.operator.wave | int | `-110` |  |
| applications.knative.serving.namespace | string | `"knative-serving"` | knative serving namespace |
| applications.knative.serving.version | string | `"1.11.0"` | knative serving version |
| applications.knative.serving.wave | int | `-100` |  |
| applications.loki.enabled | bool | `true` | loki enable: 'true', 'false' |
| applications.loki.namespace | string | `"loki"` | loki namespace |
| applications.loki.revision | string | `"0.69.16"` | loki version |
| applications.loki.wave | int | `-60` |  |
| applications.mongodb.enabled | bool | `true` | mongodb enable: 'true', 'false' |
| applications.mongodb.namespace | string | `"mongodb"` | mongodb namespace |
| applications.mongodb.revision | string | `"0.9.0"` | mongodb version |
| applications.mongodb.wave | int | `-10` |  |
| applications.mysql.enabled | bool | `true` | mysql enable: 'true', 'false' |
| applications.mysql.namespace | string | `"mysql-operator"` | mysql namespace |
| applications.mysql.revision | string | `"2.1.1"` | mysql version |
| applications.mysql.wave | int | `-20` |  |
| applications.prometheus.enabled | bool | `false` | prometheus enable: 'true', 'false' |
| applications.prometheus.namespace | string | `"kube-prometheus"` | prometheus namespace |
| applications.prometheus.revision | string | `"48.1.1"` | prometheus version |
| applications.prometheus.wave | int | `-80` |  |
| applications.promtail.enabled | bool | `true` | promtail enable: 'true', 'false' |
| applications.promtail.namespace | string | `"promtail"` | promtail namespace |
| applications.promtail.revision | string | `"6.11.5"` | promtail version |
| applications.promtail.wave | int | `-50` |  |
| applications.rook.enabled | bool | `false` | rook enable: 'true', 'false' |
| applications.rook.namespace | string | `"rook-ceph"` | rook namespace |
| applications.rook.revision | string | `"v1.13.2"` | rook version |
| applications.rook.wave | int | `-70` |  |
| applications.strimzi.enabled | bool | `true` | strimzi enable: 'true', 'false' |
| applications.strimzi.namespace | string | `"kafka"` | strimzi namesapce |
| applications.strimzi.revision | string | `"0.35.1"` | strimzi version |
| applications.strimzi.wave | int | `-30` |  |
| applications.tempo.enabled | bool | `true` | tempo enable: 'true', 'false' |
| applications.tempo.namespace | string | `"tempo"` | tempo namespace |
| applications.tempo.revision | string | `"1.4.8"` | tempo version |
| applications.tempo.wave | int | `-40` |  |
| fullnameOverride | string | `""` | string to fully override `"app-of-apps.fullname"` |
| logs.enabled | bool | `true` | logs enable: 'true', 'false' |
| logs.format | string | `"json"` | logs format: 'json' |
| logs.level | string | `"info"` | logs level: 'trace', 'debug', 'info', 'warn', 'error', 'critical' |
| metrics.enabled | bool | `true` | metrics enable: 'true', 'false' |
| nameOverride | string | `"app-of-apps"` | provide a name in place of 'app-of-apps' |
| network.enabled | bool | `true` | network enable: 'true', 'false' |
| network.issuer | string | `"selfsigned"` | network issuer: 'selfsigned', 'acme' |
| network.mode | string | `"istio"` | network mode: 'istio' |
| project.branch | string | `"HEAD"` | project gitops branch |
| project.description | string | `"application that launches other applications"` | project description |
| project.domain | string | `"generic-infrastructure.org"` | project cluster domain |
| project.environment | string | `"development"` | project environment: 'development', 'staging', 'production' |
| project.name | string | `"default"` | project name |
| project.organization | string | `"generic-infrastructure"` | project organization |
| project.platform | string | `"minikube"` | project cluster platform: 'minikube', 'gke' |
| project.profile | string | `"demo"` | project cluster profile: 'demo', 'default' |
| project.region | string | `"local"` | project region: 'local', ... |
| project.repository | string | `"git@github.com:generic-infrastructure/terragrunt-devops.git"` | project gitops repository |
| traces.enabled | bool | `true` | traces enable: 'true', 'false' |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.12.0](https://github.com/norwoodj/helm-docs/releases/v1.12.0)
