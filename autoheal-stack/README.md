# autoheal-stack

Container auto-heal watcher

## Stack: autoheal-stack

### Services

```
  • autoheal
```

### Key Environment Variables

- `AUTOHEAL_INTERVAL`
- `AUTOHEAL_START_PERIOD`

### Volumes

- `/var/run/docker.sock`

### Deployment

```bash
cd autoheal-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
