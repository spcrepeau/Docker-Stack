# media_management

## lidarr

## overseerr

## prowlarr

## radarr

## radarr-4K

## recyclarr

* Requires "user: UID:GID" field and does not support PUID and PGID environment variables.
* Manually run recyclarr sync with these commands:

```bash
# To enter the recyclarr container
sudo docker exec -it recyclarr bash
# Run the sync command in the recyclarr shell
recyclarr sync
```

### secrets.yaml

* The *_base_url values should be in the <http://hostname:port> format

### radarr.yaml and sonarr.yaml

* Old versions being maintained for when setting quality profiles through recyclarr is no longer desired.

## sabnzbd

## sonarr

## sonarr-anime

## custom format files

* These JSON files should be imported into every instance of sonarr and radarr. Recyclarr will build the rest.

* This folder and its files do not need to exists here and be be copied elsewhere or deleted once they've been imported.
