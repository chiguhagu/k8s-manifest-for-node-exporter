# k8s-manifest-for-node-exporter

This repository contains a manifest that uses Prometheus to monitor k8s Nodes.

## How To Use

### 1. Apply manifests

```shell
kubectl apply -f node-exporter.yaml
kubectl apply -f prometheus.yaml
kubectl port-forward service/prometheus 9090:9090 -n monitoring
```

### 2. Access Prometheus

http://localhost:9090
