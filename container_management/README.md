# container_management

## watchtower

* Manually run watchtower with this command:

```bash
# This this create a new watchtower container, run it once, and them remove the container
sudo docker run --rm -v /var/run/docker.sock:/var/run/docker.sock containrrr/watchtower --run-once
```

## socket-proxy-watchtower
