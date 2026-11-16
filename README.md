GHANA MINING AND RESTORATION ATLAS
Research snapshot | 16 November 2026

Open Ghana_Mining_Atlas.html in Chrome, Firefox or Edge after extracting
the archive. The map and its data run offline. Linked sources need internet.
Use the zoom buttons and checkboxes to inspect individual datasets. Turn on
Annual gold conversion and move its slider to browse 2007–2017.
The full research brief is available separately as Ghana_Mining_Research_Brief.pdf.

QGIS
Open Ghana_Mining.gpkg via Layer > Add Layer > Add Vector Layer. Select the
layers to add. In the GeoPackage, review these first:

  ghana_gold_extent_to_2019
    Barenblitt, Payton and Lagomasino (2021), DOI 10.17632/s4rfcckr39.1.
    7,622 features. MineType 1 is artisanal, 2 industrial. The archive’s
    mapped AreaM2 values total about 29,212 and 5,019 ha, respectively.
    The article’s estimate of about 47,000 ± 2,218 ha of conversion to
    artisanal mining is a separate statistic. It cannot be reproduced by
    summing this file’s mapped features. CC BY 4.0. Geometry promoted to
    MultiPolygon for GeoPackage export.

  ghana_gold_conversion_2007_2017
    Same source and licence. 53,793 polygon records. detection_year is
    source classifica + 2000. source_count preserves the input attribute.
    Use the annual CSV for raw sums of mapped polygon areas reprojected
    to EPSG:6933. Those sums are not probability-adjusted area estimates.
    The atlas displays annual layers rasterized at 0.001 degrees, so small
    polygons can disappear there. Use original vectors for close analysis.

  mining_footprint_2019_maus_v2
    Maus et al. (2022), DOI 10.1594/PANGAEA.942325. Ghana extract from the
    ArcGIS public mirror (service item 5dff30ba5d1b4fa6b6b64c5ac156d257).
    Verified against the original published per-country count and area.
    577 features. area_km2 is the source field. Covers diverse mining
    infrastructure interpreted from a 2019 Sentinel-2 mosaic near
    known mine coordinates. Scale, legal status and closure status are
    unknown. CC BY-SA 4.0 applies to this layer and its adaptations.

  site_references
    38 source-linked orientation points, many at district level. Filter
    by category. Check geometry_reference and read the source_ids before
    using a point. A district reference is placed within the district;
    it is not a mine location or the location of a reported pit.

  damang_tender_2026_indicative
    Digitized from all 88 angular coordinates in MLNR’s published
    Annexure A. The published notice does not specify a datum. The
    plot assumes WGS84 only for display and approximates the stated
    4,042 ha. This is the tender area, not the operative current lease.
    Use the official geometry and known datum to match boundaries.

  regions_geoboundaries_2021; districts_geoboundaries_2019
    16 regions and 260 districts in the source vintage. CC BY 4.0.
    Verify current districts with Ghana Statistical Service as needed.
    These reference layers have simplified boundaries.

  lake_volta_natural_earth
    Cartographic orientation from Natural Earth. Public domain.

Tinga_Sentinel2_comparison.jpg shows the same location on 27 January 2018
and 28 January 2026. Contains modified Copernicus Sentinel data 2018 and
2026, distributed by Element 84 Earth Search. Scene URLs are in Sources.csv.

The three footprint files overlap. Do not add their areas. The package
contains no complete historical concession dataset, comprehensive
current mining delineation, engineered rehabilitation design or lab
clearance. Disturbance mapped from imagery does not establish who mined
it, whether permission was valid, when work stopped or whether land is safe.
Latest independent change alerts and official sources are linked in
Sources.csv. The current cadastre was not available as a verified
bulk export for ingestion. See the research brief for acquisition steps.

Map interface uses Leaflet 1.9.4, BSD 2-Clause, see Leaflet-LICENSE.txt.
