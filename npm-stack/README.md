# npm-stack

Reverse proxy — Nginx Proxy Manager

## Services

```
  • npm
```

## Volumes

- `/mnt/storagepool/apps_config/npm/data`
- `/mnt/storagepool/apps_config/npm/certs`

## Ports

- `80`
- `443`
- `30020`

## Deployment

```bash
cd npm-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration