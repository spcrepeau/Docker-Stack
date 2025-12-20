# plex_apps

## agregarr

### Links

* GitHub: <https://github.com/agregarr/agregarr>

## kometa

### Links

* Documentation: <https://kometa.wiki/en/latest/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-kometa/>

### Notes

* Uses PUID and PGID environment variables to run rootless.
* The KOMETA_PLEXURL value should be in the <https://#-#-#-#.##########.plex.direct:32400> format.
* Follow the kometa wiki for configuring any other connections.

#### Examples for how the config processes posters for movies, TV shows, and anime

![Movie Poster Example](https://github.com/spcrepeau/Docker-Stack/blob/main/.images/kometa_movie.jpg) ![TV Show Poster Example](https://github.com/spcrepeau/Docker-Stack/blob/main/.images/kometa_tv_show.jpg) ![Anime Poster Example](https://github.com/spcrepeau/Docker-Stack/blob/main/.images/kometa_anime.jpg)

## plexautolanguages

### Links

* GitHub: <https://github.com/JourneyDocker/Plex-Auto-Languages>

### Notes

* Requires "user: UID:GID" field and does not support PUID and PGID environment variables.

## quickstart

### Links

* GitHub: <https://github.com/Kometa-Team/Quickstart/>

### Notes

* Requires "user: UID:GID" field and does not support PUID and PGID environment variables.

## shinkro

### Links

* Documentation: <https://docs.shinkro.com/>
* GitHub: <https://github.com/varoOP/shinkro>

### Notes

* Requires "user: UID:GID" field and does not support PUID and PGID environment variables.
* Setup reverse proxy for this app.

## tautulli

### Links

* Documentation: <https://tautulli.com/>
* LinuxServer: <https://docs.linuxserver.io/images/docker-tautulli/>

### Notes

* Uses PUID and PGID environment variables to run rootless.
* Setup reverse proxy for this app if you're using remote apps like nzb360.
* Uses Plex SSO.
* To setup SMTP app password <https://support.google.com/mail/answer/185833?hl=en>
