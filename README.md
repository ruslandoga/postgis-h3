Based on https://github.com/postgis/docker-postgis/blob/master/16-3.4/alpine/Dockerfile and https://github.com/zachasme/h3-pg/discussions/150.

```console
$ docker run -d -e POSTGRES_PASSWORD=postgres -p 5432:5432 --name postgis_h3 -v postgis_h3_data:/var/lib/postgres/data ghcr.io/ruslandoga/postgis-h3:latest
```

Can be used for migrating from PostGIS to Uber H3.
