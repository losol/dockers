# Curated list of software running in docker

For some software and services.

- Grafana: port `3000`
- Home assistant: port `8123`
- InfluxDB: port `8086`
- Mosquitto: ports `1883` and `9001`
- Nginx Proxy manager: port `81`
- Node-red: port `1880`
- PgAdmin: port `5050`
- Posgres: port `5432`
- Strapi: port `1337`
- Wordpress: port `8000`

## Upgrade to latest image

To upgrade to the latest image of all services in a docker-compose just pull a fresh image, and restart:

```
docker-compose pull
docker-compose restart
```
