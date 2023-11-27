# docker-node-rust
Docker Rust development images built on node:lts-bullseye and node:current-bullseye.

## Motivation

Base development image for Rust web applications that also want to build JS/TS code alongside their Rust code.

The Node images were selected as the base image simply because the Rust Dockerfile code was less complicated and therefore theoretically easier to maintain.

## Usage

### Docker command line example

```bash
docker pull ghcr.io/johnbcodes/docker-node-rust:1.74.0
```

## Entrypoint / Command

The entrypoint/command of running either Node or a system command has been overridden to just run Bash.

## Updates

I will attempt to add images for new Rust/Rustup versions as they arrive. Otherwise, please submit an issue.

## Acknowledgments

The Node base images were created by the [Node.js project](https://nodejs.org/).

The Dockerfile code for Rust installation was created by the [Rust community](https://rust-lang.org/).

The Github Action CI, publishing of the ghcr.io image, and documentation was created by myself.
