# pgAdmin

pgAdmin is the most popular and feature rich Open Source administration and development platform for PostgreSQL.

## Set up ssl for localhost

To enable ssl, pgAdmin expects the files `/certs/server.cert` and `/certs/server.key`.

To make these files, run the commands below in the `./certs` folder.

```sh
openssl req -x509 -nodes -sha256 -newkey rsa:2048 -out server.pem -keyout server.key -subj '/CN=localhost'
openssl x509 -outform pem -in server.pem -out server.cert
```

Useful links:

- [pgAdmin docs: Container Deployment](https://www.pgadmin.org/docs/pgadmin4/latest/container_deployment.html). More info on environment variables and folders used by pgAdmin.
