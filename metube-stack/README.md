# metube-stack

YouTube downloader — MeTube

## Stack: metube-stack

### Services

```
  • metube
```

### Key Environment Variables

- `DOWNLOAD_DIR`
- `GID`
- `STATE_DIR`
- `UID`
- `YTDL_OPTIONS`

### Volumes

- `/mnt/storagepool/master/Media/youtube`
- `/mnt/storagepool/apps_config/metube/state`
- `/mnt/storagepool/master/Media/youtube/metube-config/cookies.txt`

### Ports Exposed

- `8086`

### Deployment

```bash
cd metube-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
