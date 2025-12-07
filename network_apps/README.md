# network_apps

## authentik_database (postgres)

### Links

* GitHub: <https://hub.docker.com/layers/library/postgres/16-alpine/>

## authentik_server

### Links

* Documentation: <https://docs.goauthentik.io/>
* GitHub: <https://github.com/goauthentik/authentik>

### Notes

* Setup reverse proxy for this app.
* Requires "user: UID:GID" field and does not support PUID and PGID environment variables.
* To setup SMTP app password <https://support.google.com/mail/answer/185833?hl=en>

## authentik_worker

### Links

* Documentation: <https://docs.goauthentik.io/>
* GitHub: <https://github.com/goauthentik/authentik>

### Notes

* Requires "user: UID:GID" field and does not support PUID and PGID environment variables.

## pihole

### Links

* Documentation: <https://pi-hole.net/>
* GitHub: <https://github.com/pi-hole/pi-hole>

### Notes

* Requires use of PIHOLE_UID and PIHOLE_GID environment variables and does not support PUID and PGID environment variables.
