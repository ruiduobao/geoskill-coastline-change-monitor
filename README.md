# geoskill-coastline-change-monitor

> Multi-temporal shoreline change rate analysis. Generates transects, computes Endpoint Rate (EPR) and Linear Regression Rate (LRR), and identifies erosion hotspots. Use when monitoring coastline retreat/accretion or identifying erosion-prone segments.

See [SKILL.md](SKILL.md) for full usage, inputs and outputs.

## Quick start

```bash
# Vector shorelines
python scripts/coastline_change_monitor.py \
  --shoreline-files shore_2015.geojson shore_018.geojson shore_2021.geojson \
  --years 2015 2018 2021

# Raster water masks
python scripts/coastline_change_monitor.py \
  --shoreline-files water_2015.tif water_2018.tif water_2021.tif \
  --years 2015 2018 2021 \
  --transect-spacing 50 --transect-length 300
```

## License

MIT
