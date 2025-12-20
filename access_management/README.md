# access_management

## authentik_database (postgres)

### Links

* GitHub: <https://hub.docker.com/layers/library/postgres/16-alpine/>

### Notes

* Runs as root

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

## wizarr

### Links

* Documentation: <https://docs.wizarr.dev/>
* GitHub: <https://github.com/wizarrrr/wizarr/>

### Notes

* Uses PUID and PGID environment variables to run rootless.
* Setup reverse proxy for this app, but point to the authentik port instead. <https://docs.wizarr.dev/using-wizarr/single-sign-on-sso#authentik-other>
* In the authentik provider, edit the unauthenticated paths to include the regex exceptions in the above URL. Remove the dash and quotes from each line.
