# dispatcharr-stack

Media request dispatcher

## Stack: dispatcharr-stack

### Services

```
  • dispatcharr
  • gluetun-iptv
```

### Key Environment Variables

- `CELERY_BROKER_URL`
- `DISPATCHARR_ENV`
- `DISPATCHARR_LOG_LEVEL`
- `DJANGO_SECRET_KEY`
- `DNS_ADDRESS`
- `DOT`
- `OPENVPN_PASSWORD`
- `OPENVPN_USER`
- `REDIS_HOST`
- `SERVER_CITIES`
- `SERVER_COUNTRIES`
- `SERVER_SELECTION`
- `TZ`
- `VPN_SERVICE_PROVIDER`
- `VPN_TYPE`

### Volumes

- `/mnt/storagepool/apps_config/dispatcharr/data`
- `/dev/dri/renderD128`
- `/dev/dri/card0`
- `/dev/net/tun`
- `/mnt/storagepool/apps_config/gluetun-iptv`

### Deployment

```bash
cd dispatcharr-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
