# Sonekart v2 – 30 soner

Kopi av [Sonekart-ColliXL](https://mikkelnikolaievensen.github.io/Sonekart-ColliXL/)
oppdatert fra 24 til 30 soner. Det opprinnelige repoet er urørt.

Filer:

- `index.html`
- `map_export_forslag_sonekart.csv`
- `postnummer_sonekart_forslag.geojson`
- `priser_amo.json`
- `kjoredager.json`
- `kontrollrapport_sonekart.csv`

Aktiver GitHub Pages: Settings → Pages → Deploy from branch → main → /root

## Innhold
- Postnummer i sonekartet: 1133 (var 1027)
- Soner: 30 (var 24)
- Flater i GeoJSON: 1194, dekker 1128 av 1133 postnummer
- Postnummer uten flate: 1393, 1520, 1521, 1522, 1527 (postboks-/serviceområder
  uten flate i Kartverkets postnummerområder – de er korrekt sonesatt)

## Endringer fra v1
- Sone 9 er splittet: 9 Nedre Glomma (Fredrikstad/Sarpsborg), 25 E6-nord/Mosseaksen,
  26 Indre Østfold, 27 Halden. Alle beholder kjøredag 4.
- Ny dekning: 28 Larvik/Stavern, 29 Skien/Siljan, 30 Porsgrunn/Bamble.
  Kjøredag er ikke fastsatt for disse.
- Geometrien er bygget på nytt fra Kartverkets
  `Basisdata_0000_Norge_25833_Postnummeromrader` (EPSG:25833 → WGS84),
  slik at Grenland og Larvik faktisk tegnes.
- Prisene kommer fra `Prismatrise_18.08.26_30_soner_v4.xlsx` (30x30 per tjeneste
  og volumtrinn).

## Kilder
- Soner: `Sonekart 30.csv`
- Priser: `Prismatrise_18.08.26_30_soner_v4.xlsx`
- Kjøredager: app.collixl.no `/api/internal_ui_data/delivery-intervals-internal` (06.08.2026)
