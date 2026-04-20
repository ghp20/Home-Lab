# anything_llm-stack

LLM chat interface — AnythingLLM

## Stack: anything_llm-stack

### Services

```
  • options
  • anything-llm
```

### Key Environment Variables

- `DATABASE_URL`
- `DISABLE_TELEMETRY`
- `ENCRYPTION_KEY`
- `JWT_SECRET`
- `SERVER_PORT`
- `STORAGE_DIR`

### Volumes

- `/mnt/storagepool/apps_config/anything_llm/data`
- `/mnt/storagepool/apps_config/anything_llm/data`

### Ports Exposed

- `30239`

### Deployment

```bash
cd anything_llm-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
