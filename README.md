# GPU-aware Tensorflow container

## Example `docker run` command
`docker run -it -d --runtime=nvidia --restart=unless-stopped --shm-size=1G --ulimit memlock=-1 --ulimit stack=67108864 --name [OPTIONAL_CONTAINER_NAME] --hostname [OPTIONAL_HOST_NAME] -p [TENSORBOARD_PORT]:6006 -v [HOST_MOUNT_POINT]:/workspace sleeepyjack/tensorflow:py3`

## Dependencies
* Linux
* CUDA-capable GPU (>= Kepler architecture is recommended)
* [NVIDIA driver](http://www.nvidia.de/Download/index.aspx)
* [Docker](https://docs.docker.com/install/)
* [nvidia-docker](https://github.com/NVIDIA/nvidia-docker)

## See project on [Docker Hub](https://hub.docker.com/r/sleeepyjack/tensorflow/)
