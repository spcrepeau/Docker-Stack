# media_apps

## audiobookshelf

### Links

* Documentation: <https://www.audiobookshelf.org/>
* GitHub: <https://github.com/advplyr/audiobookshelf>

### Notes

* Rootless: Uses "user: UID:GID". Container will error out if running as non-root user and trying to bind to port 80. Change the default port to anything besides 80 with a PORT variable.
* Reverse Proxy: Setup reverse proxy for this app. Also add the default websocket fields.
* Notifications: None at this time.
* Authentication: To setup OAuth with authentik <https://www.audiobookshelf.org/guides/oidc_authentication/>
  * Subfolder for Redirect URLs: None
  * Match existing users by: Match by username

## calibre

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-calibre/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: None.
* Notifications: N/A
* Authentication: None

## calibre-web

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-calibre-web/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: Setup reverse proxy for this app.
* Notifications: N/A
* Authentication: Built-in.

## romm

### Links

* Documentation: <https://romm.app/>
* GitHub: <https://github.com/rommapp/romm/>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: Setup reverse proxy for this app.
* Notifications: None at this time.
* Authentication: To setup OAuth with authentik <https://docs.romm.app/latest/OIDC-Guides/OIDC-Setup-With-Authentik/>

## romm-db (MariaDB)

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-mariadb/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: N/A
* Notifications: N/A
* Authentication: N/A
