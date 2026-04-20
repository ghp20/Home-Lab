# syncthing-stack

File sync — Syncthing

## Stack: syncthing-stack

### Services

```
  • syncthing
```

### Volumes

- `/mnt/storagepool/master/Media/Movies`
- `/mnt/storagepool/master/Media/Tv`
- `/mnt/storagepool/apps_config/syncthing/config`

### Deployment

```bash
cd syncthing-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
