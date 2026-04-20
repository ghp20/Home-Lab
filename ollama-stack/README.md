# ollama-stack

Local LLM inference — Ollama

## Stack: ollama-stack

### Services

```
  • ollama
  • homelab
```

### Key Environment Variables

- `CUDA_VISIBLE_DEVICES`
- `GID`
- `NVIDIA_DRIVER_CAPABILITIES`
- `NVIDIA_VISIBLE_DEVICES`
- `OLLAMA_CONFIG`
- `OLLAMA_CONTEXT_LENGTH`
- `OLLAMA_HOST`
- `OLLAMA_KEEP_ALIVE`
- `OLLAMA_MODELS`
- `UID`

### Volumes

- `/mnt/storagepool/apps_config/ollama/config`
- `/mnt/storagepool/apps_config/ollama/data`
- `/mnt/nvmepool/appsconfig/ollama/models`

### Deployment

```bash
cd ollama-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
