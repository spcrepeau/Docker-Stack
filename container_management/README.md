# container_management

## portainer

### Links

* Documentation: <https://docs.portainer.io/>
* GitHub: <https://github.com/portainer/portainer>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: Setup reverse proxy for this app.
* Notifications: Note at this time.
* Authentication: To setup OAuth with authentik: <https://integrations.goauthentik.io/hypervisors-orchestrators/portainer/>

## socket-proxy

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-socket-proxy/>

### Notes

* Rootless: Runs as root.
* Reverse Proxy: N/A
* Notifications: N/A
* Authentication: N/A

## wud

### Links

* Documentation: <https://getwud.github.io/wud/>
* GitHub: <https://github.com/getwud/wud>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: Setup reverse proxy for this app.
* Notifications: Setup gotify. To setup SMTP app password <https://support.google.com/mail/answer/185833?hl=en> and use in in wud <https://getwud.github.io/wud/#/configuration/triggers/smtp/>.
* Authentication: To setup OAuth with authentik: <https://integrations.goauthentik.io/monitoring/whats-up-docker/>. Requires reverse proxy setup for this app, as redirect will fail with local URL and port.
* WUD_AUTH_BASIC_MY_HASH: Each \$ character must be replaced with $$.
* WUD_AUTH_BASIC_MY_HASH__FILE: Leave the \$ as a single character.
