# claude-code-stack

Docker stack managed by Portainer

## Services

```
  • claude-code
```

## Volumes

- `/mnt/storagepool/apps_config/claude-code`
- `/mnt/storagepool/master/claude-code`

## Deployment

```bash
cd claude-code-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration