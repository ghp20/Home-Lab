# monitoring-stack

Infrastructure monitoring

## Stack: monitoring-stack

### Services

```
  • prometheus
  • grafana
  • monitoring-net
```

### Key Environment Variables

- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/monitoring/prometheus/config/prometheus.yml`
- `/mnt/storagepool/apps_config/monitoring/prometheus/data`
- `/mnt/storagepool/apps_config/monitoring/grafana/data`

### Ports Exposed

- `9090`
- `3002`

### Deployment

```bash
cd monitoring-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
