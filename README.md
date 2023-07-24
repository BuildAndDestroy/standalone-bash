# standalone-bash
Compile standalone bash for CLI access on containers.

## Build

* The build process is done using Docker.
* Once the build is complete, run the image as a container and copy bash out to your host.
* Tested to run on Alpine and Debian builds.

```
cd build_bash/debian
docker build -t debian-bash-standalone .
docker run --rm -it debian-bash-standalone bash

# Using another container

docker container ls
docker cp <CONTAINER ID>::/opt/bash-5.2.15/bash .
```


