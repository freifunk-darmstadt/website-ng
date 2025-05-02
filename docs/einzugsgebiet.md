# Einzugsgebiet
Freifunk ist Dezentral und wird von vielen verschiedenen Communities betrieben.
Nur Knoten innerhalb der gleichen Community können miteinander meshen.

## Domains
Das Darmstädter Freifunk-Netz wird aktuell in mehrere unabhängige Domains aufgeteilt.
Du wirst daher bei der Einrichtung eines neuen Freifunk-Knotens im Konfigurationsmodus nach deiner Domain gefragt.

Beachte bitte, dass Knoten nur meshen können, falls sie sich innerhalb der gleichen oder einer benachbarten Domain mit der gleichen Farbe befinden.

<div id="map" class="box" style="height: 40em;"></div>

<!-- map foo -->
<link rel="stylesheet" href="/css/leaflet.css" />
<script src="/javascripts/leaflet.js"></script>
<script src="/javascripts/domains.js"></script>
<script>
	function onEachFeature(feature, layer) {
		if (feature.properties && feature.properties.pretty_name) {
			layer.bindPopup(feature.properties.pretty_name);
			layer.setStyle({opacity: 0.5, fillOpacity: 0.3, color: feature.properties.color, fillColor: feature.properties.color});
		}
	}

	function mapinit() {
		var map = L.map('map').setView([49.857906725, 8.743057251], 9);

		L.tileLayer('https://tiles.darmstadt.freifunk.net/{z}/{x}/{y}.png', {
			attribution: '&copy; <a href="http://osm.org/copyright">OpenStreetMap</a> contributors'
		}).addTo(map);

		L.geoJSON(domains, {onEachFeature: onEachFeature}).addTo(map);
	}
	mapinit();
</script>

!!! note "Karte"
    Wir haben auch eine [Karte mit allen Freifunk-Knoten in Darmstadt](https://meshviewer.darmstadt.freifunk.net).

## Nachbarn
Falls du außerhalb des Darmstädter Freifunk-Netzes bist, wende dich bitte an eine Community in deiner Nähe.

- [Freifunk Frankfurt](https://www.ffm.freifunk.net/)
- [Freifunk Wiesbaden](https://www.wiesbaden.freifunk.net/)
- [Freifunk Rhein-Neckar](https://www.freifunk-rhein-neckar.de/)

Auf der [Karte von freifunk.net](https://freifunk.net/wie-mache-ich-mit/community-finden/) fiendest du alle Freifunk-Communities in Deutschland.

