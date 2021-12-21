# Deployment Examples

Install helm repository using:

```bash 
helm repo add deployment-charts https://akanthos.github.io/deployment-charts/
helm repo list
helm repo update
helm search repo deployment-charts
```

Show all repositories:
```bash 
helm repo list
```

Update repositories (in case new chart versions are available):
```bash 
helm repo update
```

List all charts in repository:
```bash 
helm search repo deployment-charts
```

To install an app with a specific chart version and specific environment values:

```bash 
helm upgrade --install quarkus-app1 -f values-test.yaml deployment-charts/quarkus-chart --version 0.2.0
```

