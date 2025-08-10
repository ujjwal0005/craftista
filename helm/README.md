# Craftista Helm Chart

## Installation

### Development Environment
```bash
helm install craftista-dev ./craftista -f craftista/values/dev.yaml
```

### Staging Environment
```bash
helm install craftista-staging ./craftista -f craftista/values/staging.yaml
```

### Production Environment
```bash
helm install craftista-prod ./craftista -f craftista/values/prod.yaml
```

## Upgrade
```bash
helm upgrade craftista-dev ./craftista -f craftista/values/dev.yaml
```

## Uninstall
```bash
helm uninstall craftista-dev
```

## Configuration

| Parameter | Description | Default |
|-----------|-------------|---------|
| `global.registry` | Container registry | `ghcr.io` |
| `global.repository` | Repository name | `craftista/craftista` |
| `global.tag` | Image tag | `latest` |
| `frontend.replicaCount` | Frontend replicas | `2` |
| `frontend.ingress.enabled` | Enable ingress | `true` |
| `frontend.ingress.host` | Ingress hostname | `craftista.local` |