# openSUSE and NodeJS6 image

This project builds an openSUSE-based image which includes NodeJS version 6. It can be used as a base image by projects which require NodeJS6.

### Tini
[Tini](https://github.com/krallin/tini) is pre-installed in the container.  If the image entrypoint is not overwritten then it will be automatically used.

### Startup Scripts
Any executable scripts added to the `/startup/startup.d/` directory will be automatically run each time the container is started (assuming the image entrypoint is not overwritten).

### Certificate Installation
The image comes pre-installed with several startup scripts which provide a mechanism to extend the CA certificates which should be trusted.
