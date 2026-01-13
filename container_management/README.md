# container_management

## dockhand

### Links

* Documentation: <https://dockhand.pro/manual/#>
* GitHub: <https://github.com/Finsys/dockhand>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: Setup reverse proxy for this app.
* Notifications: Setup gotify and use URL <gotifys://gotify.mydomain.com/myToken>.
* Authentication: To setup OAuth with authentik: <https://dockhand.pro/manual/#appendix-oidc>. The Issuer URL format is <https://authentik.mydomain.com/application/o/dockhand/>.

## dockhand_socket-proxy

### Links

* LinuxServer: <https://docs.linuxserver.io/images/docker-socket-proxy/>

### Notes

* Rootless: Runs as root.
* Reverse Proxy: N/A
* Notifications: N/A
* Authentication: N/A
