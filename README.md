# Dockerized Centos8

Base container with systed
-----------

* $ docker build -t centos8-systemd .
* $ docker run -it --tmpfs /run --tmpfs /tmp -v /sys/fs/cgroup:/sys/fs/cgroup:ro centos8-systemd

Container with systed and nginx inside. Nginx from base repo centos8.
-----------

* $ docker build -t centos8-nginx .
* $ docker run -d -it --tmpfs /run --tmpfs /tmp -v /sys/fs/cgroup:/sys/fs/cgroup:ro -p80:80 centos8-nginx:latest

