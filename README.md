## Learning Elasticsearch

This repo was setup to document the studies trying to use ElasticSearch.

## Running

To execute it, you need to have **Docker** and **docker compose** installed, then run:

```sh
docker compose up -d
```

This will start elasticsearch on https://localhost:9200 (accessible only via postman - see /postman dir to import a collection) and will start Kibana on http://localhost:5601/, where it's possible to execute all the queries and commands.

### Custom options

If you need to set custom options, create a `.env` file by running:

```sh
cp .env.example .env
```

And fill out the needed config.

### Populating the indices

To populate a sample index, you can execute the `Import data` in Postman, importing the configs from `postman/Elasticsearch.postman_collection.json`
