# plex-stack

Media server — Plex

## Stack: plex-stack

### Services

```
  • plex
```

### Key Environment Variables

- `PGID`
- `PLEX_CLAIM`
- `PUID`
- `TZ`
- `VERSION`

### Volumes

- `/mnt/storagepool/apps_config/plex/config`
- `/mnt/storagepool/apps_config/plex/transcode`
- `/mnt/storagepool/master/Media`
- `/dev/dri`

### Ports Exposed

- `32400`

### Deployment

```bash
cd plex-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
