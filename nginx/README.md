# nginx HTTP web server

1. `sysctl net.ipv4.ip_unprivileged_port_start=80`
2. Edit `nginx.conf` file
3. Edit `compose.yaml` file and mount needed directories
4. `podman compose up -d`
