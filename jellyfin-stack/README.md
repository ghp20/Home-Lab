# jellyfin-stack

Media server — Jellyfin

## Stack: jellyfin-stack

### Services

```
  • jellyfin
```

### Key Environment Variables

- `NVIDIA_DRIVER_CAPABILITIES`
- `NVIDIA_VISIBLE_DEVICES`
- `PGID`
- `PUID`
- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/jellyfin/config`
- `/mnt/storagepool/apps_config/jellyfin/cache`
- `/mnt/storagepool/apps_config/jellyfin/transcode`
- `/mnt/storagepool/master/Media`

### Ports Exposed

- `8096`
- `8920`

### Deployment

```bash
cd jellyfin-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
