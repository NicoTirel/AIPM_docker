# AIPM_docker
Install and use AIPowerMeter (https://github.com/GreenAI-Uppa/AIPowerMeter) throughout a docker container

## Requirements
RAPL and/or nvidia-smi available

Docker

## Build

```
sudo docker build -t aipm_test_01:latest .
```

## Run

Change path to the docker repository

```
sudo docker run --gpus all -it --rm --mount type=bind,src=/path/to/docker_repo,dst=/mnt IMAGE_NAME:TAG
```

## Show consumption

Open the PowerConsumption.ipynb and change the path to the docker repository

You can use docker-env/bin/python as a kernel for the notebook with all requirements needed