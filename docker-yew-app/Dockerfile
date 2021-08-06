FROM rust

WORKDIR /app
EXPOSE 8080/TCP

RUN apt-get update && apt-get upgrade -y  && rm -rf /var/lib/apt/lists/*
RUN cargo install trunk wasm-bindgen-cli
RUN rustup target add wasm32-unknown-unknown
