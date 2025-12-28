# plex_apps

## agregarr

### Links

* GitHub: <https://github.com/agregarr/agregarr>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: None.
* Notifications: N/A
* Authentication: Plex SSO.

## kometa

### Links

* Documentation: <https://kometa.wiki/en/latest/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-kometa/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: N/A
* Notifications: N/A
* Authentication: N/A
* The KOMETA_PLEXURL value should be in the <https://#-#-#-#.##########.plex.direct:32400> format.
* Follow the kometa wiki for configuring any other connections.

#### Examples for how the config processes posters for movies, TV shows, and anime

![Movie Poster Example](https://github.com/spcrepeau/Docker-Stack/blob/main/.images/kometa_movie.jpg) ![TV Show Poster Example](https://github.com/spcrepeau/Docker-Stack/blob/main/.images/kometa_tv_show.jpg) ![Anime Poster Example](https://github.com/spcrepeau/Docker-Stack/blob/main/.images/kometa_anime.jpg)

## plexautolanguages

### Links

* GitHub: <https://github.com/JourneyDocker/Plex-Auto-Languages>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: N/A
* Notifications: N/A
* Authentication: N/A

## quickstart

### Links

* GitHub: <https://github.com/Kometa-Team/Quickstart/>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: N/A
* Notifications: N/A
* Authentication: N/A

## shinkro

### Links

* Documentation: <https://docs.shinkro.com/>
* GitHub: <https://github.com/varoOP/shinkro>

### Notes

* Rootless: Uses "user: UID:GID".
* Reverse Proxy: Setup reverse proxy for this app in DSN.
* Notifications: Setup gotify.
* Authentication: Built-in.

## tautulli

### Links

* Documentation: <https://tautulli.com/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-tautulli/>

### Notes

* Rootless: Uses PUID and PGID environment variables.
* Reverse Proxy: Setup reverse proxy for this app if you're using remote apps like nzb360.
* Notifications: Setup gotify. To setup SMTP app password <https://support.google.com/mail/answer/185833?hl=en>
* Authentication: Plex SSO.
