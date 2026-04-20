# monitoring-stack

Docker stack managed by Portainer

## Services

```
  • prometheus
  • grafana
  • monitoring-net
```

## Volumes

- `/mnt/storagepool/apps_config/monitoring/prometheus/config/prometheus.yml`
- `/mnt/storagepool/apps_config/monitoring/prometheus/data`
- `/mnt/storagepool/apps_config/monitoring/grafana/data`

## Ports

- `9090`
- `3002`

## Deployment

```bash
cd monitoring-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration