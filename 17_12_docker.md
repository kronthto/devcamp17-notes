## Docker from sketch

### AUFS
* FS in stacks
+ Every FS stack (hash) -> image/template
* `docker run` spawns Container (from image?)

### Docker registry
* Ex: Dockerhub
* Image Upload/Download

### Alpine vs Ubuntu
* Alpine 5-7 MB (w/o glibc) vs. several 100MB Ubuntu

### Dockerfile
* FROM <existing image>
* RUN Commands/Changes
* Entrypoint
* Every command => Own stack => Lots of inline and cleanup (e.g. `rm -rf /var/lib/apt/lists/`)

### docker-compose
* Problem: Often need for multiple containers that interact with each other (Apache/MySQL)
* Defines images that start together, ports, hosts, ...


### random notes
* ssh'ing in an changing things would be a concept fraction
* `-v` mount volume (even /tmp/x11socket possible lol)

### vs. vagrant / ansible
* Vagrant full VM with OS etc
* Docker process runs on host system

### Alternatives
* rkt
