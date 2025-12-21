# general_apps

## gotify

### Links

* Documentation: <https://gotify.net/>
* GitHub: <https://github.com/gotify/server>

### Notes

* Requires "user: UID:GID" field and does not support PUID and PGID environment variables.
* Setup reverse proxy for this app. Also add the default websocket fields.

## homepage

### Links

* Documentation: <https://gethomepage.dev/>
* GitHub: <https://github.com/gethomepage/homepage/>

### Notes

* Uses PUID and PGID environment variables to run rootless.
* This application does not have any built-in authentication and we'll use authentik to do so.
* Setup reverse proxy for this app, but point to the authentik port instead.

## homepage-socket-proxy

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-socket-proxy/>

### Notes

* Runs as root.

## librespeed

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-librespeed/>

### Notes

* Uses PUID and PGID environment variables to run rootless.

## theme-park

### Links

* Documentation: <https://docs.theme-park.dev/>
* GitHub: <https://github.com/themepark-dev/theme.park/>

### Notes

* Uses PUID and PGID environment variables to run rootless.
