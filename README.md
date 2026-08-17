# Jottem Open Data

De open-data-landingspagina van het [Jottem-platform](https://github.com/inside-out-time-machines/jottem),
in deze fase gepubliceerd op **https://data.dev.iotm.nl/** (bij livegang: data.iotm.nl).

De pagina toont, per organisatie en project, alle open-data-uitgangen van het
platform (datasetbeschrijving, RDF-datadump, SPARQL, IIIF Presentation en Change
Discovery, W3C Web Annotations, RSS), de publieke API als Swagger UI en de
broncoderepo's. De projectgegevens komen client-side uit de publieke API
(`GET /organisaties`); de API-specificatie wordt geladen van
[design.iotm.nl/openapi.yaml](https://design.iotm.nl/openapi.yaml).

Statische site, geen buildstap. Swagger UI staat gevendored in
`assets/swagger-ui/` (swagger-ui-dist 5.17.14, Apache-2.0); fonts en logo komen
uit de [merkgids](https://github.com/inside-out-time-machines/brand).

Deployment: working copy op de dev-server, geserveerd door de `datapagina`-service
(nginx) uit `deploy/docker-compose.yml` in de jottem-repo; bijwerken = `git pull`.
