# Yew tuto notes

Sources
  * [Yew getting started](https://yew.rs/getting-started/build-a-sample-app)

## Build image

```shell
cd docker-yew-app
docker build -t tuto/yew:0.0.1 .
````

## Run app

```shell
cd yew-sample-app
docker run --rm -v ${PWD}:/app -p8080:8080 -ti tuto/yew:0.0.1 /usr/local/cargo/bin/trunk serve
```