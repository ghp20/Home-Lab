# Graylog

## What this stack is for

Centralized logging stack for collecting, searching, and managing logs.

## Included services

- `mongodb` — `mongo`
- `datanode` — `graylog-datanode`
- `graylog` — `graylog`

## Deploy with Portainer

1. In Portainer, open **Stacks** and choose **Add stack**.
2. Use the folder name from this repo as the stack name, then paste or upload the `docker-compose.yaml` from this directory.
3. Replace placeholders such as `changeme`, `/path/to/your/data`, `your-*`, and any `${ENV_VAR}` values.
4. Create any required bind-mount paths, datasets, secrets, and external Docker networks before deployment.
5. Deploy the stack, then check **Container logs**, **Health**, and published ports in Portainer.

## Warnings & gotchas

- Replace all placeholders (`changeme`, `/path/to/your/data`, `your-*`, `${...}`) before deploying.
- Deploy the whole stack together in Portainer; the services depend on each other.

## Exposed ports

12201:12201/udp, 12201:12201/tcp, 5140:5140/udp, 5140:5140/tcp, 8999:8999, 9000:9000/tcp

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
