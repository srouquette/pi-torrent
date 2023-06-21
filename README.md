## Explanations

Torrents are downloaded into downloads, then moved into their appropriate directory.

Directory setup:

/Elements
    /series
    /movies
    /anime
    /downloads
        /series
        /movies
        /anime
        /untracked
    /torrent: watch dir if you want to download a .torrent file

## What to update

### docker-compose.yml

WHITELIST=127.0.0.1,192.168.1.*,192.168.2.*,172.18.0.*,172.20.0.*

### config/tranmission/settings.json

```
"download-dir": "/Elements/downloads/series",
"incomplete-dir": "/Elements",
"watch-dir": "/Elements/torrent",
```

### config/flexget/secrets.yml

 everything in it