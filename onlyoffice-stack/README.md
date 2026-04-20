# onlyoffice-stack

Online office — OnlyOffice

## Services

```
  • onlyoffice-document-server
```

## Volumes

- `/mnt/storagepool/apps_config/onlyoffice/data`
- `/mnt/storagepool/apps_config/onlyoffice/logs`

## Ports

- `8082`

## Deployment

```bash
cd onlyoffice-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration