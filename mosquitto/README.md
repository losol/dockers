# Mosquitto

Eclipse Mosquitto is an open source (EPL/EDL licensed) message broker that implements the MQTT protocol versions 5.0, 3.1.1 and 3.1. Mosquitto is lightweight and is suitable for use on all devices from low power single board computers to full servers.

## Get started

Create a empty file in the config folder named `credentials`.

To add a user, get a container shell `docker exec -it mosquitto sh` and run
`mosquitto_passwd -c /mosquitto/config/credentials USERNAME`

## Read more

- [Mosquitto docs](https://mosquitto.org/documentation/)
