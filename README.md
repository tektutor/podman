# podman

## Installing Podman in Ubuntu
```
sudo apt-get -y install podman
```

## Checking Podman version
```
podman --version
podman info
```

## Container Runtime Overview
<pre>
- is a low-level software that is used to manage containers and container images
- it is not user-friendly, hence end-users like will not use the container runtime directly
- Examples
  - runc is a Container Runtime
  - CRI-O is a container Runtime
</pre>

## Container Engine Overview
<pre>
- is a high-level software that can manage containers and container images
- is user-friendly, hence without knowing how the container technology is enabled by Linux kernel we can easily manage images and containers
- container engine internally depends on Container Runtimes to manage images and containers
- Examples
  - Docker is a Container Engine which internally depends on containerd, containerd internally depends on runC container runtime
  - Podman is a Container Engine which internally depends on CRI-O Container Runtime
</pre>
