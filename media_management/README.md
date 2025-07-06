# media_management

## lidarr

### Links

* Documentation: <https://lidarr.audio/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-lidarr/>

### Notes

* Setup reverse proxy for this app.

## overseerr

### Links

* Documentation: <https://overseerr.dev/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-overseerr/>

### Notes

* Setup reverse proxy for this app.

## prowlarr

### Links

* Documentation: <https://prowlarr.com/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-prowlarr/>

### Notes

* Setup reverse proxy for this app.

## radarr & radarr-4K

### Links

* Documentation: <https://radarr.video/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-prowlarr/>

### Notes

* Setup reverse proxy for this app.

## recyclarr

### Links

* Documentation: <https://recyclarr.dev/wiki/>
* GitHib: <https://github.com/recyclarr/recyclarr>

### Notes

* Requires "user: UID:GID" field and does not support PUID and PGID environment variables.
* Manually run recyclarr sync with these commands:

```bash
# To enter the recyclarr container
sudo docker exec -it recyclarr bash
# Run the sync command in the recyclarr shell
recyclarr sync
```

#### secrets.yaml

* The *_base_url values should be in the <http://hostname:port> format

#### radarr.yaml and sonarr.yaml

* Old versions being maintained for when setting quality profiles through recyclarr is no longer desired.

## sabnzbd

### Links

* Documentation: <https://sabnzbd.org/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-sabnzbd/>

### Notes

* Setup reverse proxy for this app.

## sonarr & sonarr-anime

### Links

* Documentation: <https://sonarr.tv/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-sonarr/>

### Notes

* Setup reverse proxy for this app.

## custom format files

* These JSON files should be imported into every instance of sonarr and radarr. Recyclarr will build the rest.
* This folder and its files do not need to exists here and be be copied elsewhere or deleted once they've been imported.
