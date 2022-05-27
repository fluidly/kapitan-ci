Kapitan-CI
==========

The `kapitan:ci` image was [removed from Docker Hub](https://github.com/kapicorp/kapitan/issues/803) but we were using it extensively in our CI pipelines 😢

This docker image is based directly from the version kapitan [used to have in their repository](https://github.com/kapicorp/kapitan/blob/a632eca5ec914063743d463f5fac7b1018b9a434/Dockerfile.ci), except we are installing kapitan via `pip` than from source.
It is also available on [Docker Hub](https://hub.docker.com/r/fluidlydev/kapitan-ci).

For now, we're keeping it as it is, but we may refactor it to ensure there are tests and it stays up to date and remove some tools which are not necessary. (We only require `kapitan` and `google-cloud-sdk`.)
