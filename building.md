# How to build

In your project directory, run:

`docker run --platform=linux/amd64 -it --rm -v $(pwd):/workspace adeel111/fprime-arm-custom:latest bash`

This will boot you into a docker container with all dependencies and toolchains setup.

Run:

`fprime-util generate aarch64-linux -f`
`fprime-util build`
`exit`

The container will shut down and your build will be in `/<project>/build-artifacts/aarch64-linux/<deployment name>/bin`