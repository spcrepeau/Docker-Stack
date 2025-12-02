# container_management

## portainer

### Links

* Documentation: <https://docs.portainer.io/>
* GitHub: <https://github.com/portainer/portainer>

### Notes

* Setup reverse proxy for this app.
* To setup OAuth with authentik: <https://integrations.goauthentik.io/hypervisors-orchestrators/portainer/>

## socket-proxy

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-socket-proxy/>

## wud

### Links

* Documentation: <https://getwud.github.io/wud/>
* GitHub: <https://github.com/getwud/wud>

### Notes

* WUD_AUTH_BASIC_MY_HASH: Each \$ character must be replaced with $$.
* WUD_AUTH_BASIC_MY_HASH__FILE: Leave the \$ as a single character.
* Requires "user: UID:GID" field and does not support PUID and PGID environment variables.
* To setup OAuth with authentik: <https://integrations.goauthentik.io/monitoring/whats-up-docker/>. Requires reverse proxy setup for this app, as redirect will fail with local URL and port.
