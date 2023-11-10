# kepler.gl in a box

* [http://kepler.gl](http://kepler.gl)
* [https://github.com/uber/kepler.gl](https://github.com/uber/kepler.gl)

## Build
Clone the repo. Go to Root of the dir and run the followings
```bash
docker build . -t keplergl
```

# Run: pass your mapbox access token to the container
docker run  --name keplergl -p 8080:80 \
	-e MapboxAccessToken="yourMapboxAccessToken" -d keplergl
```
Some modules need to be build at startup. Therefore, it will a take a minute until the container is ready to use
at [http://localhost:8080](http://localhost:8080).

