# arr-stack

Media management stack — Prowlarr, Radarr, Sonarr, Bazarr, Lazylibrarian, CleanupArr

## Stack: arr-stack

### Services

```
  • options
  • arrnet
  • prowlarr
  • radarr
  • sonarr
  • bazarr
  • lazylibrarian
  • cleanuparr
```

### Key Environment Variables

- `PGID`
- `PUID`
- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/prowlarr/config`
- `/mnt/storagepool/apps_config/radarr/config`
- `/mnt/storagepool/master/Media/Movies`
- `/mnt/storagepool/master/Media/downloads`
- `/mnt/storagepool/master/Media/usenet/downloads`
- `/mnt/storagepool/apps_config/sonarr/config`

### Ports Exposed

- `9696`
- `7878`
- `8989`
- `6767`
- `5299`
- `11011`

### Deployment

```bash
cd arr-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
