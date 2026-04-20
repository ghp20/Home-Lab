# wireguard-us-server-stack

Docker stack managed by Portainer

## Services

```
  • options
  • wireguard-us-server
```

## Volumes

- `/mnt/storagepool/apps_config/wireguard/server_config`
- `/lib/modules`

## Ports

- `22`
- `443`

## Deployment

```bash
cd wireguard-us-server-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration