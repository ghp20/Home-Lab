# dispatcharr-stack

Docker stack managed by Portainer

## Services

```
  • dispatcharr
  • gluetun-iptv
```

## Volumes

- `/dev/dri/renderD128`
- `/dev/dri/card0`
- `/dev/net/tun`

## Deployment

```bash
cd dispatcharr-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration