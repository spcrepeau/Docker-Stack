# container_management

## portainer

### Links

* Documentation: <https://docs.portainer.io/>
* GitHub: <https://github.com/portainer/portainer>

## socket-proxy

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-socket-proxy/>

## watchtower

### Links

* Documentation: <https://containrrr.dev/watchtower/>
* GitHub: <https://github.com/containrrr/watchtower>

### Notes

* Manually run watchtower with this command:

```bash
# This will create a new watchtower container, run it once, and then remove the container
sudo docker run --rm -v /var/run/docker.sock:/var/run/docker.sock containrrr/watchtower --run-once
```
