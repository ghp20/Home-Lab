# dispatcharr-stack

Docker stack managed by Portainer

## Services

```
  • dispatcharr
  • gluetun-iptv
```

## Volumes

- `/mnt/storagepool/apps_config/dispatcharr/data`
- `/dev/dri/renderD128`
- `/dev/dri/card0`
- `/dev/net/tun`
- `/mnt/storagepool/apps_config/gluetun-iptv`

## Deployment

```bash
cd dispatcharr-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration