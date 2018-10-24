# tomcat-env

Spin up a Tomcat 8.5 environment with JRE8.

 - Already configured to work without the "only localhost" nonsense. (So you just access `localhost:8000` and it freaking works, just like it should be.)
 - Increased max size limits on WAR deployment (50mb max? Really? That's the base size of a Spring Boot deployment).
 - Includes a MySQL so you can use it in your deployments. (Just change the db image in `docker-compose.yml` if you need other one).

## Usage ##

```sh
docker-compose up -d --build # Be sure to always include the --build. The image might change and it'll use the cache anyways.
```

Then, login using user `tomcat` and password `s3cret`.

## License ##

MIT
