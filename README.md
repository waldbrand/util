# Waldbrand utilities

**This repository is outdated, please use
[waldbrand/website](https://github.com/waldbrand/website) instead**

## Preparing OSM data

The tools in this repository work with OSM data stored at
`~/github/waldbrand/osm-data`.

Scripts for downloading and extracting data are currently
located in the [website](https://github.com/waldbrand/website)
repository, where from the `project` directory, you need to run
the following scripts in this order:

    ./scripts/download-osm-data
    ./scripts/extract-region-data
    ./scripts/extract-osm-data

Doing that will:

* download data from Geofabrik's download
  server to `~/github/waldbrand/osm-data`,
* extract Brandenburg from the Berlin-Brandenburg file,
* extract relevant OSM data from the Brandenburg file.

## Data packaging

Create assets for Android app and copy them to the app repository:

    ./scripts/create-database.sh
    ./scripts/create-mapfile.sh
    ./scripts/create-mapfile-waldbrand
    ./scripts/copy-assets.sh
