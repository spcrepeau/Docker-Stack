# media_management

## audiobookrequest

### Links

* Documentation: <https://markbeep.github.io/AudioBookRequest/>
* GitHub: <https://github.com/markbeep/AudioBookRequest>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: Setup reverse proxy for this app.
* Notifications: Setup gotify.
* Authentication: To setup OAuth with authentik: <https://markbeep.github.io/AudioBookRequest/docs/tutorials/oidc/>

## lidarr

### Links

* Documentation: <https://lidarr.audio/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-lidarr/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: Setup reverse proxy for this app if you're using remote apps like nzb360, but point to the authentik port instead. <https://wiki.servarr.com/radarr/faq#forced-authentication>, <https://integrations.goauthentik.io/media/sonarr/>. Custom header: Upgrade=$http_upgrade, Connection=$http_connection
* Notifications: Setup gotify.
* Authentication: Create authentik app and proxy provider. In the authentik provider, edit the unauthenticated paths to include the regex ^/api/.* to allow nzb360 access to API.

## overseerr

### Links

* Documentation: <https://overseerr.dev/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-overseerr/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: Setup reverse proxy for this app.
* Notifications: Setup gotify. To setup SMTP app password <https://support.google.com/mail/answer/185833?hl=en>
* Authentication: Plex SSO.

## prowlarr

### Links

* Documentation: <https://prowlarr.com/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-prowlarr/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: Setup reverse proxy for this app if you're using remote apps like nzb360, but point to the authentik port instead. <https://wiki.servarr.com/radarr/faq#forced-authentication>, <https://integrations.goauthentik.io/media/sonarr/>. Custom header: Upgrade=$http_upgrade, Connection=$http_connection
* Notifications: Setup gotify.
* Authentication: Create authentik app and proxy provider. In the authentik provider, edit the unauthenticated paths to include the regex ^/api/.* to allow nzb360 access to API.

## radarr & radarr-4K

### Links

* Documentation: <https://radarr.video/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-prowlarr/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: Setup reverse proxy for this app if you're using remote apps like nzb360, but point to the authentik port instead. <https://wiki.servarr.com/radarr/faq#forced-authentication>, <https://integrations.goauthentik.io/media/sonarr/>. Custom header: Upgrade=$http_upgrade, Connection=$http_connection
* Notifications: Setup gotify.
* Authentication: Create authentik app and proxy provider. In the authentik provider, edit the unauthenticated paths to include the regex ^/api/.* to allow nzb360 access to API.

## recyclarr

### Links

* Documentation: <https://recyclarr.dev/wiki/>
* GitHub: <https://github.com/recyclarr/recyclarr>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: N/A
* Notifications: Connect to apprise API URL and then forward to gotify apprise formatted URL. <https://recyclarr.dev/reference/settings/notifications/>
* Authentication: N/A

* Manually run recyclarr sync with these commands:

```bash
# To enter the recyclarr container
sudo docker exec -it recyclarr bash
# Run the sync command in the recyclarr shell
recyclarr sync
```

### radarr.yaml and sonarr.yaml

* Old versions being maintained for when setting quality profiles through recyclarr is no longer desired.

## sabnzbd

### Links

* Documentation: <https://sabnzbd.org/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-sabnzbd/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: * Setup reverse proxy for this app if you're using remote apps like nzb360, but point to the authentik port instead. Disable authentication.
* Notifications: Setup gotify. Select Apprise and use URL <gotifys://gotify.mydomain.com/myToken>.
* Authentication: Create authentik app and proxy provider. In the authentik provider, edit the unauthenticated paths to include the regex ^/api.* to allow nzb360 access to API.

## slskd

### Links

* GitHub: <https://github.com/slskd/slskd>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: None
* Notifications: N/A
* Authentication: Built-in.

## sonarr & sonarr-anime

### Links

* Documentation: <https://sonarr.tv/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-sonarr/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: Setup reverse proxy for this app if you're using remote apps like nzb360, but point to the authentik port instead. <https://wiki.servarr.com/radarr/faq#forced-authentication>, <https://integrations.goauthentik.io/media/sonarr/>. Custom header: Upgrade=$http_upgrade, Connection=$http_connection
* Notifications: Setup gotify.
* Authentication: Create authentik app and proxy provider. In the authentik provider, edit the unauthenticated paths to include the regex ^/api/.* to allow nzb360 access to API.

## soularr

### Links

* GitHub: <https://github.com/mrusse/soularr>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: N/A
* Notifications: N/A
* Authentication: N/A

## custom format files

* These JSON files should be imported into every instance of sonarr and radarr. Recyclarr will build the rest.
* This folder and its files do not need to exists here and be be copied elsewhere or deleted once they've been imported.
