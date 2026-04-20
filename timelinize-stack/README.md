# timelinize-stack

Timeline tool — Timelinize

## Stack: timelinize-stack

### Services

```
  • timelinize
```

### Key Environment Variables

- `TLZ_ORIGIN`
- `TZ`
- `XDG_CONFIG_HOME`

### Volumes

- `/mnt/storagepool/apps_config/timelinize/repo`
- `/mnt/storagepool/apps_config/timelinize/config`
- `/mnt/storagepool/master/timelinize`
- `/mnt/storagepool/apps_config/Immich/data`

### Ports Exposed

- `12002`

### Deployment

```bash
cd timelinize-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
