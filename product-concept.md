# Produktkonzept

## Status

Diese Datei beschreibt nur den aktuellen Rahmen. Technische Detailentwicklung ist derzeit nicht Schwerpunkt.

Die marktbasierte Bewertung und empfohlene Reduktion des Startumfangs stehen in [prototype-market-assessment.md](prototype-market-assessment.md). Die Empfehlungen sind noch keine Produktentscheidungen.

## Zielbereich

- Gewächshäuser ca. 10–100 m²
- zwei Zonen / zwei Gewächshäuser im verkabelten Grundsystem
- weitere Erweiterung über WLAN möglich

## Grundarchitektur

- Versorgung des Controllers mit 12 oder 24 VDC
- kein zwingend integriertes Netzgerät; zertifizierte externe Netzgeräte sind am Markt verfügbar
- lokale autonome Steuerung
- Internet nicht erforderlich für Kernfunktionen
- Fernüberwachung und Fernsteuerung möglich
- MQTT vorgesehen
- Touchbedienung am Gerät
- Webinterface
- zukünftige Plattform: ESP32
- Plug-and-play-Verkabelung für Sensoren und Aktoren
- Einrichtung drahtloser Komponenten mit dem Bedienniveau eines WLAN-Routers

## Schutzfunktionen

Bereits im Prototyp konzeptionell bzw. teilweise realisiert:

- Sturmschutz
- Frostschutz
- Sensorausfall / Ersatzsensoren
- Überhitzungsschutz
- Feuchteregelung
- lokale Wetterdaten

## Sensorik aus älterem Konzept

- Außen-Multisensor
  - Temperatur
  - Feuchte
  - Windstärke
  - Windrichtung
  - UV / Helligkeit
  - Regen
- bis zu 8 Innensensoren
- bis zu 8 Blattfeuchtesensoren
- bis zu 8 Bodenfeuchtesensoren
- bis zu 8 Bodentemperatursensoren

Die Anzahl von bis zu acht Sensoren wird derzeit durch die vorgesehene Wetterstation beziehungsweise deren Architektur geprägt. Sie ist kein aus dem Markt abgeleiteter Bedarf. Alternative Fabrikate kommen erst infrage, wenn neben Protokoll und Messqualität auch die mechanischen und klimatischen Qualitätsanforderungen erfüllt sind.

## Aktorik aus älterem Konzept

- Zirkulationsventilator
- Befeuchtung
- Heizlüfter / Heizung
- bis zu 4 Linearantriebe
- EWT-Ventilator

## Erdreichwärmetauscher

Der Erdreichwärmetauscher ist eine technische Differenzierungshypothese für Ganzjahresbetrieb und Energieoptimierung. Die bisherige Marktanalyse liefert dafür keine direkte Nachfrageevidenz; er wird daher nicht als Bestandteil des empfohlenen Kernpakets behandelt.

## Produktprinzip

> Verkabelte Kernfunktionen mit Plug-and-play-Anschlüssen für Zuverlässigkeit, drahtlose Erweiterungen mit routerähnlicher Einrichtung für Skalierbarkeit.

## Wasch- und Strahlwasserschutz

Nach Gründerangabe werden Gewächshäuser innen gelegentlich mit Gartenschlauch oder Hochdruckreiniger gereinigt. Der Umgebungsschutz soll deshalb nicht an ein zusätzliches, vom Kunden auszuwählendes Gehäuse delegiert werden.

Als marktbasierte Arbeitshypothese gilt:

- gesamte Feldinstallation für nasse Reinigung konzipieren,
- Gartenschlauchtauglichkeit als Mindestziel technisch definieren,
- IP66 nur nach Prüfung der vollständigen Anordnung bewerben,
- Hochdruckreinigung separat auf IPX9/IP69-Niveau prüfen,
- Steckverbinder, Schutzkappen, Kabel, Sensoren und Bedienelemente in die Systemprüfung einbeziehen,
- externes Netzgerät und 230-V-Verbindung außerhalb der Waschzone anordnen oder getrennt qualifizieren.

Details und Wettbewerbsbelege stehen in [washdown-protection-analysis.md](washdown-protection-analysis.md).

Die ältere Präsentation zeigt allerdings einen solar-/batteriebetriebenen Außen-Multisensor. Da Wind und Regen Schutzentscheidungen auslösen, muss diese Abweichung vor einer Produktentscheidung durch Verkabelung oder einen nachweisbar überwachten Fallback aufgelöst werden.
