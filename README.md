# n8n with PostgreSQL & worker, SSL, hosted as a subdomain

Starts n8n with PostgreSQL as database, the worker as a separate container,
running behind Caddy, as subdomain of the main host.

A combination of the existing [docker-caddy](https://github.com/n8n-io/n8n-hosting/tree/main/docker-caddy) and [withPostgresAndWorker](https://github.com/n8n-io/n8n-hosting/tree/main/docker-compose/withPostgresAndWorker) setups from the `n8n-hosting` repo, with a number of cleanups suggested by [docker-compose-linter](https://github.com/zavoloklom/docker-compose-linter)

## Configuration

- `cp EXAMPLE.env .env`
- Update `.env` with your configuration details

## Start

`docker-compose up -d`

To stop, run: `docker-compose stop`
