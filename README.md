# pdok

Amsterdam MBTile with PDOK vector tiles

Source: https://geodata.nationaalgeoregister.nl/beta/topotiles-viewer/#8/52.33/5.19


## Unpack MBTiles

To unpack the MBTiles file you can use the command <A href="https://github.com/mapbox/mbutil">mb-util</a> as follows:

```
$ mb-util amsterdam.mbtiles tiles --image_format=pbf
```

## Offline Sample viewer

To run offline sample viewer with vector tiles:

1] Copy amsterdam.mbtiles to the samples directy

2] Unpack MBTiles

```
$ mb-util amsterdam.mbtiles tiles --image_format=pbf
```

3] run webserver

for example run <a href="https://caddyserver.com/">caddy server</a>

```
$ caddy
Activating privacy features... done.
http://:2015
```

4] View in browser

Go to http://localhost:2015/index.html to view the site 