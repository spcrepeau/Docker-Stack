# Docker-Stack

* Please see the Wiki for all information
* env and secrets files have been stripped of all personal information, edit REPLACE_ME in each to reflect your environment.
* When using wud to update your containers, change the lscr.io in the image field to ghcr.io.

## To-Do's

* romm authentik SSO broken. Temp fix: <https://github.com/rommapp/romm/issues/2626>
* Waiting on OIDC/Proxy login for gotify
* Waiting on chaptarr, the readarr replacement to release.
* Remove calibre-web? Is ABS a good replacement>
* Explore other DNS servers?
* romm-db change?
* recyclarr gotify support

## Projects

* [access_management](https://github.com/spcrepeau/Docker-Stack/tree/main/access_management)
  * authentik_database (postgres)
  * authentik_server
  * authentik_worker
  * wizarr
* [container_management](https://github.com/spcrepeau/Docker-Stack/tree/main/container_management)
  * portainer
  * socket-proxy
  * wud/whatsupdocker
* [general_apps](https://github.com/spcrepeau/Docker-Stack/tree/main/general_apps)
  * apprise
  * gotify
  * homepage
  * homepage-socket-proxy
  * librespeed
  * theme-park
* [media_apps](https://github.com/spcrepeau/Docker-Stack/tree/main/media_apps)
  * audiobookshelf
  * calibre
  * calibre-web
  * romm
  * romm-db (mariadb)
* [media_management](https://github.com/spcrepeau/Docker-Stack/tree/main/media_management)
  * audiobookrequest
  * lidarr
  * overseerr
  * prowlarr
  * radarr
  * radarr-4K (radarr)
  * recyclarr
  * sabnzbd
  * sonarr
  * sonarr-anime (sonarr)
* [network_apps](https://github.com/spcrepeau/Docker-Stack/tree/main/network_apps)
  * pihole
* [plex_apps](https://github.com/spcrepeau/Docker-Stack/tree/main/plex_apps)
  * agregarr
  * kometa
  * plexautolanguages
  * quickstart
  * shinkro
  * tautulli

## VSCode Extensions

* Code Spell Checker by Street Side Software
* indent-rainbow by oderwat
* json by ZainChen
* Markdown Preview Enhanced by Yiyi Wang
* markdownlint by David Anson
* Notepad++ keymap by Microsoft
* PowerShell by Microsoft
* YAML by Red Hat

## Icon Repos

* Dashboard Icons <https://dashboardicons.com/>, <https://github.com/homarr-labs/dashboard-icons>
* Material Design Icons <https://pictogrammers.com/library/mdi/>
* Simple Icons <https://simpleicons.org/?q=agenda>
* Self-Hosted Dashboard Icons <https://selfh.st/icons/>
* Font Awesome Icon <https://fontawesome.com/>
