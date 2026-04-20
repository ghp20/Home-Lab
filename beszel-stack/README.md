# beszel-stack

Server monitoring — Beszel

## Services

```
  • beszel
  • beszel-agent
```

## Volumes

- `/mnt/storagepool/apps_config/beszel/hub-data`
- `/mnt/storagepool/apps_config/beszel/socket`
- `/mnt/storagepool/apps_config/beszel/agent-data`
- `/mnt/storagepool/apps_config/beszel/socket`
- `/var/run/docker.sock`

## Ports

- `8097`

## Deployment

```bash
cd beszel-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration