# lidarr-tak
[![lidarr-tak](https://snapcraft.io/lidarr-tak/badge.svg)](https://snapcraft.io/lidarr-tak)
![snap arch](https://badgen.net/snapcraft/architecture/lidarr-tak)
![snap size](https://badgen.net/snapcraft/size/lidarr-tak/amd64/stable)

## Snap Description
Canonical Snap for Lidarr\
https://snapcraft.io/lidarr-tak

## Lidarr Description
<img src="/icon.svg" width="100">
Lidarr is a music collection manager for Usenet and BitTorrent users.
It can monitor multiple RSS feeds for new tracks from your favorite artists 
and will grab, sort and rename them. It can also be configured 
to automatically upgrade the quality of files already downloaded 
when a better quality format becomes available.

See https://lidarr.audio for more details.

## Information

The web interface is accessible by default at http://localhost:8686

Lidarr Release 2+\
Core20 is still required for dependencies\
Service is restarted on any condition.

Post install commands required to access media folders and see resources :
```
sudo snap connect lidarr-tak:removable-media
sudo snap connect lidarr-tak:mount-observe
```

**!!! Files can only be written in a directory owned by 'root' !!!**\
**!!! Home base directory content is not readable !!!**

This is due to current behavior and restrictions of snaps by Canonical.\
Check common doc in FAQ if you want to setup data in /home directory.

## FAQ
See my common doc about [FAQ](https://github.com/TehAppKiller/Snapcraft-common-doc/tree/main#FAQ).

## Building
The snap requires Core20 for .NET source dependencies.\
See my common doc about [building a snap](https://github.com/TehAppKiller/Snapcraft-common-doc/tree/main#Building).
## Versionning
See my common doc about [versionning](https://github.com/TehAppKiller/Snapcraft-common-doc/tree/main#Versionning).
