# multi-node-elasticsearch-cluster

The vm.max_map_count kernel setting must be set to at least 262144 for production use.

How you set vm.max_map_count depends on your platform.

For Linux & macOS
```
sysctl -w vm.max_map_count=262144
```

Windows and macOS with Docker Desktop
```
docker-machine ssh
sudo sysctl -w vm.max_map_count=262144
```