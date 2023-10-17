# Dockerised .net local dev

Simple bootstrap project to run/build a .net project via docker

## How to use

### Local Dev

You must have docker installed correctly before continuing

```sh
make dev-start
```

If you need to access the .net tooling (`dotnet`), you can do it within the workspace, which is accessed via

```sh
make dev-workspace
```

## Building

```sh
make build
```

This will build an image called `dotnet-build`