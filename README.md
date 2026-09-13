# llm-d


llm-d Router — Standalone Mode
```bash
helm install llm-d-router \
  oci://ghcr.io/llm-d/charts/llm-d-router-standalone \
  --namespace llm-d \
  --create-namespace
```

llm-d Router — Gateway Mode
```bash
helm install llm-d-router-gateway \
  oci://ghcr.io/llm-d/charts/llm-d-router-gateway \
  --namespace llm-d \
  --create-namespace
```
