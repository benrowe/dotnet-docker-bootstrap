# Dockerised .net local dev

Simple bootstrap project to run/build a .net project via docker.

Locally runs a `donet watch run` command, mounts the current directory as a volume in docker and exposes port 800 to the host machine.

Build produces a local docker image complete with application and dependencies required to run application.

## Todo

- [ ] Complete `build` process
- [ ] Fix local port expose

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