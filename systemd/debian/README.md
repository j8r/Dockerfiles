# Debian image with systemd enabled

You can use this image as a base container to run systemd services inside.

## Supported tags
 - `sid`
 - `latest`, `10`
 - `9`
 - `8`

## Usage

Run the container as a daemon

`docker run -d --name systemd-debian --cap-add SYS_ADMIN -v /sys/fs/cgroup:/sys/fs/cgroup:ro jrei/systemd-debian`

Enter to the container

`docker exec -it systemd-debian bash`

Remove the container

`docker rm -f systemd-debian`
