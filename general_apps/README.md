# general_apps

## apprise

### Links

* GitHub: <https://github.com/caronc/apprise-api>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: None.
* Notifications: None.
* Authentication: None.

## gotify

### Links

* Documentation: <https://gotify.net/>
* GitHub: <https://github.com/gotify/server>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: Setup reverse proxy for this app in DSM and also add the default websocket fields.
* Notifications: Connect to mobile app.
* Authentication: Built-in.
* To get Gotify working with Synology:
  * Go to Control Panel > System > Notification > Webhooks > Add
  * Custom, use one of their rules or create your own.
  * Provider name: Gotify, Webhook URL: <https://gotifydomain/message?token=yoursecrettoken>
  * HTTP Method: POST, Content-Type: application/json, HTTP Body: {"message": "@@TEXT@@"}

## homepage

### Links

* Documentation: <https://gethomepage.dev/>
* GitHub: <https://github.com/gethomepage/homepage/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: Setup reverse proxy for this app, but point to the authentik port instead.
* Notifications: N/A
* Authentication: This application does not have any built-in authentication and we'll use an authentik proxy provider to do so.

## homepage-socket-proxy

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-socket-proxy/>

### Notes

* Rootless: Runs as root.
* Reverse Proxy: N/A
* Notifications: N/A
* Authentication: N/A

## librespeed

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-librespeed/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: None.
* Notifications: N/A
* Authentication: N/A

## theme-park

### Links

* Documentation: <https://docs.theme-park.dev/>
* GitHub: <https://github.com/themepark-dev/theme.park/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: None.
* Notifications: N/A
* Authentication: N/A
