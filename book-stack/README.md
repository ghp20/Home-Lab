# book-stack

Docker stack managed by Portainer

## Services

```
  • books_net
  • bookshelf
  • calibre
  • calibre-web
  • audiobookshelf
  • calibre-importer
```

## Volumes

- `/mnt/storagepool/apps_config/bookshelf/config`
- `/mnt/storagepool/master/Media/downloads`
- `/mnt/storagepool/master/Media/usenet/downloads`
- `/mnt/storagepool/master/Media/Books/ebooks`
- `/mnt/storagepool/master/Media/Books/audiobooks`
- `/mnt/storagepool/apps_config/calibre/config`

## Ports

- `8787`

## Deployment

```bash
cd book-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration