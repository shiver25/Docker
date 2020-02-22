# Docker

Centos8
-----------

* $ docker build -t centos8-systemd .
* $ docker run -it --tmpfs /run --tmpfs /tmp -v /sys/fs/cgroup:/sys/fs/cgroup:ro centos8-systemd
