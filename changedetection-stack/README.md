# changedetection-stack

Website change detection

## Stack: changedetection-stack

### Services

```
  • changedetection
  • browser-sockpuppet-chrome
  • changedetection_net
```

### Key Environment Variables

- `BASE_URL`
- `FETCH_WORKERS`
- `HIDE_REFERER`
- `MAX_CONCURRENT_CHROME_PROCESSES`
- `MINIMUM_SECONDS_RECHECK_TIME`
- `PLAYWRIGHT_DRIVER_URL`
- `SCREEN_DEPTH`
- `SCREEN_HEIGHT`
- `SCREEN_WIDTH`
- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/changedetection/datastore`
- `/tmp`

### Ports Exposed

- `30159`

### Deployment

```bash
cd changedetection-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
