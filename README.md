# Development Framework in Equinor Radix



## Running locally

```bash
docker-compose up

docker-compose run --rm dmss reset-app
# There is a bug in dm which causes blob uploads to fail. Only import the "DMT" package
docker-compose run --rm dmt dm -u http://dmss:5000 ds import-all apps/data_sources
docker-compose run --rm dmt dm -u http://dmss:5000 pkg delete DMT DMT
docker-compose run --rm dmt dm -u http://dmss:5000 pkg import apps/data/DMT/DMT DMT
docker-compose run --rm dm-job dm -u http://dmss:5000 reset app
```