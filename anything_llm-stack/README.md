# anything_llm-stack

LLM chat — AnythingLLM

## Services

```
  • options
  • anything-llm
```

## Volumes

- `/mnt/storagepool/apps_config/anything_llm/data`
- `/mnt/storagepool/apps_config/anything_llm/data`

## Ports

- `30239`

## Deployment

```bash
cd anything_llm-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration