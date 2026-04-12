# qdrant-stack

Docker Compose stack for **qdrant-stack**.

## Services

| Service | Image |
|---------|-------|
| qdrant | `qdrant/qdrant:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `QDRANT__SERVICE__GRPC_PORT` — see compose for default
- `QDRANT__SERVICE__HTTP_PORT` — see compose for default
- `QDRANT__STORAGE__WAL_CAPACITY_MB` — see compose for default
- `QDRANT__STORAGE__WAL_SEGMENTS_AHEAD` — see compose for default

## Volumes

- /mnt/nvmepool/appsconfig/qdrant/storage
- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
