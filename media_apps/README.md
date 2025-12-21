# media_apps

## audiobookshelf

### Links

* Documentation: <https://www.audiobookshelf.org/>
* GitHub: <https://github.com/advplyr/audiobookshelf>

### Notes

* Requires "user: UID:GID" field and does not support PUID and PGID environment variables.
* Container will error out if running as non-root user and trying to bind to port 80. Change the default port to anything besides 80 with a PORT variable.
* Setup reverse proxy for this app. Also add the default websocket fields.
* To setup OAuth with authentik <https://www.audiobookshelf.org/guides/oidc_authentication/>
  * Subfolder for Redirect URLs: None
  * Match existing users by: Match by username

## calibre

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-calibre/>

## calibre-web

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-calibre-web/>

### Notes

* Setup reverse proxy for this app.

## romm

### Links

* Documentation: <https://romm.app/>
* GitHub: <https://github.com/rommapp/romm/>

### Notes

* Setup reverse proxy for this app.
* Requires "user: UID:GID" field and does not support PUID and PGID environment variables.
* To setup OAuth with authentik <https://docs.romm.app/latest/OIDC-Guides/OIDC-Setup-With-Authentik/>

## romm-db (MariaDB)

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-mariadb/>

### Notes

* Uses PUID and PGID environment variables to run rootless.
