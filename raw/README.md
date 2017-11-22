```
$ lhasa e rk-nihon-v1.lzh
$ ogr2ogr -f GeoJSON ryouseikoku.json rk-nihon-v1.shp
$ iconv -f WINDOWS-31J -t UTF8 ryouseikoku.json > ryouseikoku_utf8.json
$ geo2topo -p R_CODE -p name_local -p 国名 -p ID -o ryouseikoku_topo.json ryouseikoku_utf8.json
```
