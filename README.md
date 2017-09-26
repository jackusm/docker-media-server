Installed docker containers:
- linuxserver/radarr [ URL: https://radarr.yourdomain.com ]
- linuxserver/plex  [ URL: https://plex.yourdomain.com ]
- linuxserver/jackett  [ URL: https://jackett.yourdomain.com ]
- linuxserver/hydra  [ URL: https://hydra.yourdomain.com ]
- linuxserver/sonarr  [ URL: https://sonarr.yourdomain.com ]
- linuxserver/deluge  [ URL: https://deluge.yourdomain.com ]
- linuxserver/headphones  [ URL: https://headphones.yourdomain.com ]
- linuxserver/plexpy  [ URL: https://plexpy.yourdomain.com ]
- linuxserver/nzbget  [ URL: https://nzbget.yourdomain.com ]
- linuxserver/libresonic  [ URL: https://music.yourdomain.com ]
- rogueosb/ombi  [ URL: https://plexrequests.yourdomain.com ]
- drlogout/caddy
- jwilder/docker-gen

Notes:
- Open docker-compose.yml, find and replace FOLDERYOUWANTSTUFF for the folder you want (eg. mine is /home/seedbox) and YOURDOMAIN for your domain (eg. google.com)
- Plex configuration will need to be completed with an SSH tunnel if the server is on a remote network. See https://support.plex.tv/hc/en-us/articles/200288586-Installation.
- Have to manually restart caddy "docker restart caddy" when containers are modified/created etc, this isn't often so haven't put in the time to look into why it's not doing it automatically. 