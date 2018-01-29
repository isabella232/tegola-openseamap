# tegola-openseamap
OpenSeaMap implementation using Tegola

This repo houses instructions and configuration files to aid with standing up a [tegola](https://github.com/terranodo/tegola)-based vector tile server that mimics the OpenSeaMap project. It builds on [earlier work with OpenStreetMap data](https://github.com/terranodo/tegola-osm).

## Repo config files

- imposm3.json - an [imposm3](https://github.com/omniscale/imposm3) mapping file for the OSM PBF file.
- tegola.toml - a [tegola](https://github.com/terranodo/tegola) configuration file for the OSM import produced by imposm3.

## Dependencies

- [PostgreSQL](https://www.postgresql.org/) server with [PostGIS](http://www.postgis.net) enabled.
- imposm3 ([download binaries for linux](https://imposm.org/static/rel/) or [see the Go Go Go section](http://erictheise.com/blog/2017/11/13/hello-tegola#go-go-go) for a homebrew-ish OS X installation)
- tegola ([download](https://github.com/terranodo/tegola/releases))
- [gdal](http://www.gdal.org/) - required for Natural Earth import

## Resources

* [OpenSeaMap](http://openseamap.org/index.php?id=openseamap&L=1)
* [Symbology](https://github.com/OpenSeaMap/renderer/tree/master/searender/symbols)
* [seamark tag usage](https://taginfo.openstreetmap.org/search?q=seamark)
* [vectortiles-generator](https://github.com/OpenSeaMap/vectortiles-generator/blob/master/src/import-osm/mapping.yml) from OpenSeaMap project
* [renderer implemented in c](https://github.com/OpenSeaMap/renderer/tree/master/searender)
* [INT-1 styling](https://github.com/OpenSeaMap/josm/blob/master/INT1_MapCSS.mapcss)