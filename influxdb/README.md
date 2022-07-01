# InfluxDB

**InfluxDB** is an open-source time series database. Excellent for operations monitoring, application metrics, and all my Internet of Things sensor data.

**Telegraf** is an agent for collecting metrics and writing them to InfluxDB or other outputs.

## Get started

### InfluxDB

After spinning up the docker, it will be available in your browser at `localhost:8086`. Just setup your installation, and start real time analyzing.

To use the InfluxDB CLI, just spin up a shell in the container: `docker exec -it influxdb /bin/bash`.

### Telegraf

To get Telegraf running you need to set ut some environment variables:

- `TELEGRAF_INFLUXDB_TOKEN`
- `TELEGRAF_INFLUXDB_ORG`
- `TELEGRAF_INFLUXDB_BUCKET`
- `INFLUX_MQTT_USER` - defaults to `mqtt`
- `INFLUX_MQTT_PASSWORD` - defaults to `mqtt`

On a mac, the easiest way is to add this permanently to zsh env:

```sh
echo 'export TELEGRAF_INFLUXDB_TOKEN=token_here' >> ~/.zshenv
echo 'export TELEGRAF_INFLUXDB_ORG=orgname' >> ~/.zshenv
echo 'export TELEGRAF_INFLUXDB_BUCKET=bucketname' >> ~/.zshenv
```

## Read more:

- [InfluxDB documentation](https://docs.influxdata.com/influxdb/v2.3/)
- [InfluxDB Docker docs](https://hub.docker.com/_/influxdb)
- [Telegraf Docker docs](https://hub.docker.com/_/telegraf)
