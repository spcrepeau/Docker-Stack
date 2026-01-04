# access_management

## authentik_database (postgres)

### Links

* GitHub: <https://hub.docker.com/layers/library/postgres/16-alpine/>

### Notes

* Rootless: Runs as root
* Reverse Proxy: N/A
* Notifications: N/A
* Authentication: N/A

## authentik_server

### Links

* Documentation: <https://docs.goauthentik.io/>
* GitHub: <https://github.com/goauthentik/authentik>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: Setup reverse proxy for this app in DSM.
* Notifications:
  * SMTP: To setup SMTP app password <https://support.google.com/mail/answer/185833?hl=en> then use in in authentik <https://docs.goauthentik.io/install-config/email/>.
  * Gotify: Use gotify-webhook-mapping-body.txt to create a webhook property mapping. Then create a notification transport for a generic webhook, URL in format <https://gotify.domain.com/message?token=api_key>, and select the newly created mapping for the body. Create a notification rule, select the newly created transport, select send notification to event user, and severity to warning. Expand the rule and create and event matcher policy binding, and select login failed for the action.
* Authentication: Uses itself.

## authentik_worker

### Links

* Documentation: <https://docs.goauthentik.io/>
* GitHub: <https://github.com/goauthentik/authentik>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: N/A
* Notifications: N/A
* Authentication: N/A

## wizarr

### Links

* Documentation: <https://docs.wizarr.dev/>
* GitHub: <https://github.com/wizarrrr/wizarr/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: Setup reverse proxy for this app, but point to the authentik port instead. <https://docs.wizarr.dev/using-wizarr/single-sign-on-sso#authentik-other>
* Notifications: Setup gotify. Select Apprise and use URL <gotifys://gotify.mydomain.com/myToken>.
* Authentication: Create authentik app and proxy provider. In the authentik provider, edit the unauthenticated paths to include the regex exceptions in the above URL. Remove the dash and quotes from each line.
