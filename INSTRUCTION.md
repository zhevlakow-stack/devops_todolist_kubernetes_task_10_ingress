# Validation Instructions

## 1. Deploy Environment

Run the bootstrap script to provision the cluster, install the NGINX Ingress Controller, and deploy the application components.

```bash
sh bootstrap.sh
```

## 2. Validate Infrastructure
2.1 Check Ingress Controller

Ensure the NGINX controller pods are running in their dedicated namespace.

```bash
kubectl get pods -n ingress-nginx
```

2.2 Check Ingress Resource

Verify that your Ingress rule has been created and has acquired an address (localhost).