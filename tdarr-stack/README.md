# tdarr-stack

Media transcoding — Tdarr

## Stack: tdarr-stack

### Services

```
  • tdarr
  • tdarr-node
```

### Key Environment Variables

- `PGID`
- `PUID`
- `TZ`
- `UMASK`

### Volumes

- `/mnt/storagepool/apps_config/tdarr/server`
- `/mnt/storagepool/apps_config/tdarr/config`
- `/mnt/storagepool/apps_config/tdarr/log`
- `/mnt/nvmepool/appsconfig/tdarr/temp`
- `/mnt/storagepool/master/Media/`
- `/mnt/storagepool/master/Media/Movies`

### Ports Exposed

- `8265`
- `8266`

### Deployment

```bash
cd tdarr-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
