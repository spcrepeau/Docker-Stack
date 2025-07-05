# media_management

## lidarr

### Links

* Documentation: <https://lidarr.audio/>
* LSCR: <https://docs.linuxserver.io/images/docker-lidarr/>

## overseerr

### Links

* Documentation: <https://overseerr.dev/>
* LSCR: <https://docs.linuxserver.io/images/docker-overseerr/>

## prowlarr

### Links

* Documentation: <https://prowlarr.com/>
* LSCR: <https://docs.linuxserver.io/images/docker-prowlarr/>

## radarr & radarr-4K

### Links

* Documentation: <https://radarr.video/>
* LSCR: <https://docs.linuxserver.io/images/docker-prowlarr/>

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
* LSCR: <https://docs.linuxserver.io/images/docker-sabnzbd/>

## sonarr & sonarr-anime

### Links

* Documentation: <https://sonarr.tv/>
* LSCR: <https://docs.linuxserver.io/images/docker-sonarr/>

## custom format files

* These JSON files should be imported into every instance of sonarr and radarr. Recyclarr will build the rest.
* This folder and its files do not need to exists here and be be copied elsewhere or deleted once they've been imported.
