# saltminion-docker

Dockered Salt Minion for asustor

# Folders

* Create a folder for salt-minion config file. (Example ~/salt)
* Copy minion over to ~/salt

# Execution

```
docker run -d --name=salt \
   --privileged --pid=host
   -v ~/salt:/etc/salt visago/saltminion 
```
