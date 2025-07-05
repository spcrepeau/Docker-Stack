# container_management

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

## socket-proxy-watchtower

### Links

* LSCR: <https://docs.linuxserver.io/images/docker-socket-proxy/>
