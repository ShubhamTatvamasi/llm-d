# llm-d


llm-d Router — Standalone Mode
```bash
helm upgrade -i llm-d-router \
  oci://ghcr.io/llm-d/charts/llm-d-router-standalone \
  --version v0 \
  --namespace llm-d \
  --create-namespace
```

llm-d Router — Gateway Mode
```bash
helm upgrade -i llm-d-router-gateway \
  oci://ghcr.io/llm-d/charts/llm-d-router-gateway \
  --version v0 \
  --namespace llm-d \
  --create-namespace \
  --set 'router.modelServers.matchLabels.app=vllm' \
  --set 'router.resources=null' \
  --set 'router.epp.resources=null'
```
