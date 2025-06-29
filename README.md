# nginx-configmap Helm Chart

This Helm chart deploys an NGINX container that serves a customizable `index.html` page via a ConfigMap.

## Usage

```bash
helm install my-nginx ./nginx-configmap
```

## Customize the HTML

Edit `values.yaml`:

```yaml
indexHtml: |
  <html><body><h1>Custom Page</h1></body></html>
```

## Fleet Integration

Use with Rancher Fleet by referencing this chart in your GitRepo resource or in a `fleet.yaml`.
