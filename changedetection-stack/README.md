# changedetection-stack

Docker stack managed by Portainer

## Services

```
  • changedetection
  • browser-sockpuppet-chrome
  • changedetection_net
```

## Volumes

- `/mnt/storagepool/apps_config/changedetection/datastore`
- `/tmp`

## Ports

- `30159`

## Deployment

```bash
cd changedetection-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration