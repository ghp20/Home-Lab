# sample-plan-stack

Sample planning tool

## Stack: sample-plan-stack

### Services

```
  • backend
  • frontend
  • sample-plan-net
```

### Key Environment Variables

- `DATABASE_URL`

### Volumes

- `/mnt/storagepool/apps_config/sample-plan`

### Ports Exposed

- `8094`

### Deployment

```bash
cd sample-plan-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
