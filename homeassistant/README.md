# Home Assistant Docker Setup

This repository contains the Docker Compose setup for running Home Assistant in a Docker container.

## Configuration

The `docker-compose.yml` file sets up Home Assistant with the necessary ports and volumes:

- **Service Name**: `homeassistant`
- **Image**: `homeassistant/home-assistant:stable`
- **Ports**: `8123` is exposed for web interface access.
- **Volumes**: Local configurations are stored in `./config`, and the container's timezone is synchronized with the host.

## Managing the Container

To control your Home Assistant container, you can use the following Docker Compose commands:

## Updating Home Assistant
For updating to the latest version of Home Assistant:

```sh
docker compose pull homeassistant
docker compose up -d
```