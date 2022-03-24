# openpose-docker
A docker build file for CMU openpose with Python API support

## Requirements
- Nvidia Docker runtime: https://github.com/NVIDIA/nvidia-docker#quickstart
- CUDA 11.2 or higher on your host, check with `nvidia-smi`

## Build

```
cd openpose-docker/
docker build -t haleyai/openpose .
```

## Example

```
docker run -it --rm --gpus all -e NVIDIA_VISIBLE_DEVICES=0 haleyai/openpose
```

The Openpose repo is in `/openpose`
