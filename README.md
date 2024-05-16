# Paketo Noble Buildpackless Tiny Builder

## `paketobuildpacks/builder-noble-buildpackless-tiny`

This builder uses the [Paketo Noble Tiny Stack](https://github.com/paketo-buildpacks/noble-tiny-stack) (Ubuntu Noble Numbat 
build image, distroless-like run image) and contains **no buildpacks
nor order groups**. To use this builder, you must specify buildpacks at build
time using whatever mechanisms your CNB platform of choice offers.

For example, with the `pack` CLI, use `--buildpack` as follows:
```
pack build go-with-buildpackless-builder \
           --buildpack gcr.io/paketo-buildpacks/go \
           --builder paketobuildpacks/builder-noble-buildpackless-tiny:latest
```

To see which versions of build and run images and the lifecycle are in a given
builder version, see the
[Releases](https://github.com/paketo-buildpacks/builder-noble-buildpackless-tiny/releases)
on this repository. This information is also available in the `builder.toml`.

For more information about this builder and how to use it, visit the [Paketo
builder documentation](https://paketo.io/docs/builders/).  To learn about the
stack included in this builder, visit the [Paketo stack
documentation](https://paketo.io/docs/stacks/) and the [Paketo noble Tiny Stack
repo](https://github.com/paketo-buildpacks/noble-tiny-stack).
