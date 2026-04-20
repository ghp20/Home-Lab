# dashapp-stack

Docker stack managed by Portainer

## Services

```
  • dashapp
```

## Volumes

- `/mnt/storagepool/apps_config/dashapp`

## Ports

- `8050`

## Deployment

```bash
cd dashapp-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration