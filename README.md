# kepler.gl in a box

* [http://kepler.gl](http://kepler.gl)
* [https://github.com/uber/kepler.gl](https://github.com/uber/kepler.gl)

## Run

```bash
docker run --name kepler.gl -p 8080:80 -d kepler

# Optional: pass your mapbox access token to the container
docker run  --name kepler.gl -p 8080:80 \
	-e MapboxAccessToken="yourMapboxAccessToken" -d /kepler
```

Some modules need to be build at startup. Therefore, it will a take a minute until the container is ready to use
at [http://localhost:8080](http://localhost:8080).

## Build

```bash
docker build -t docker-keplergl  https://github.com/ankush-ksharma/docker-kepler.git
```

