
## Installing dependencies
```bash
python3 -m pip install -r requirements.txt
```

## Getting map data
Don't wanna package the data with the repo, so if you wanna reproduce, here you go:
```bash
curl -LO https://international.ipums.org/international/resources/gis/IPUMSI_world_release2024.zip
curl -LO https://earthworks.stanford.edu/download/file/stanford-bh326sc0899-shapefile.zip
curl -LO https://stacks.stanford.edu/file/druid:sg048gr3784/data.zip
curl -LO "https://ourworldindata.org/grapher/democracy-index-eiu.csv?v=1&csvType=full&useColumnShortNames=true"

mv democracy-index-eiu.csv data/
unzip data.zip -d data/
unzip IPUMSI_world_release2024.zip -d data/
unzip stanford-bh326sc0899-shapefile.zip -d data/
```
