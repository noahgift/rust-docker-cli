[![Clippy](https://github.com/noahgift/rust-docker-cli/actions/workflows/lint.yml/badge.svg)](https://github.com/noahgift/rust-docker-cli/actions/workflows/lint.yml)



# rust command-line tool in Docker container
An example of a tiny Rust command-line tool in a Docker container.
About 83.8MB in size.

## Usage

To build the container and run the application:
```bash
docker build -t marco-polo .
docker run --rm -it marco-polo --help 
```

You can see full invocation here:

```bash
➜  rust-docker-cli git:(main) ✗ docker run --rm -it marco-polo play --name Marco
Polo
```

To find the size of the application:

```bash
docker image ls | grep marco-polo
```

```bash
marco-polo                                                                   latest                                                                       7da8a3444176   15 minutes ago   83.8MB
```

## References

* [rust-cli-template](https://github.com/kbknapp/rust-cli-template)
* [Simplify Rust Deploy](https://www.docker.com/blog/simplify-your-deployments-using-the-rust-official-image/)
