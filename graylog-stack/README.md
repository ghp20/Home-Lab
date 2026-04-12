# graylog-stack

Docker Compose stack for **graylog-stack**.

## Services

Services:   graylog_net,  mongodb,  datanode,  graylog,

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
