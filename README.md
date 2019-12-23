# saltminion-docker

Dockered Salt Minion for asustor

# Folders

* Create a folder for salt-minion config file. (Example ~/salt)
* Copy minion over to ~/salt

# Execution

```
docker pull visago/salt-minion
docker stop salt-minion
docker rm salt-minion
docker run --restart=always --name=salt-minion -d \
  --pid=host --privileged --network=host \
  -v $(pwd):/etc/salt \
  visago/salt-minion
```
