# beszel-stack

Server monitoring — Beszel

## Stack: beszel-stack

### Services

```
  • beszel
  • beszel-agent
```

### Key Environment Variables

- `HUB_URL`
- `KEY`
- `LISTEN`
- `TOKEN`
- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/beszel/hub-data`
- `/mnt/storagepool/apps_config/beszel/socket`
- `/mnt/storagepool/apps_config/beszel/agent-data`
- `/mnt/storagepool/apps_config/beszel/socket`
- `/var/run/docker.sock`

### Ports Exposed

- `8097`

### Deployment

```bash
cd beszel-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
