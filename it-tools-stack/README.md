# it-tools-stack

Docker stack managed by Portainer

## Services

```
  • it-tools
```

## Volumes

- `/mnt/storagepool/apps_config/it-tools`

## Ports

- `8088`

## Deployment

```bash
cd it-tools-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration