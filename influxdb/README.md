# InfluxDB

InfluxDB is an open-source time series database. Excellent for operations monitoring, application metrics, and all my Internet of Things sensor data.

After spinning up the docker, it will be available in your browser at `localhost:8086`. Just setup your installation, and start real time analyzing.

To use the InfluxDB CLI, just spin up a shell in the container: `docker exec -it influxdb /bin/bash`.

Remember to export env variables: `TELEGRAF_INFLUXDB_TOKEN`, `TELEGRAF_MQTT_PASSWORD` and `TELEGRAF_MQTT_PASSWORD`

## Read more:

- [InfluxDB documentation](https://docs.influxdata.com/influxdb/v2.3/)
- [InfluxDB Docker docs](https://hub.docker.com/_/influxdb)
