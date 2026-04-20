# stirling-pdf-stack

PDF toolkit — Stirling-PDF

## Services

```
  • stirling-pdf
```

## Volumes

- `/mnt/storagepool/apps_config/stirlingpdf/tesseract_data`
- `/mnt/storagepool/apps_config/stirlingpdf/config`
- `/mnt/storagepool/apps_config/stirlingpdf/files_storage`
- `/mnt/storagepool/apps_config/stirlingpdf/logs`
- `/mnt/storagepool/apps_config/stirlingpdf/pipeline`

## Deployment

```bash
cd stirling-pdf-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration