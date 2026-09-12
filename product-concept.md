# Produktkonzept

## Status

Diese Datei beschreibt nur den aktuellen Rahmen. Technische Detailentwicklung ist derzeit nicht Schwerpunkt.

## Zielbereich

- Gewächshäuser ca. 10–100 m²
- zwei Zonen / zwei Gewächshäuser im verkabelten Grundsystem
- weitere Erweiterung über WLAN möglich

## Grundarchitektur

- lokale autonome Steuerung
- Internet nicht erforderlich für Kernfunktionen
- Fernüberwachung und Fernsteuerung möglich
- MQTT vorgesehen
- Touchbedienung am Gerät
- Webinterface
- zukünftige Plattform: ESP32

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

## Aktorik aus älterem Konzept

- Zirkulationsventilator
- Befeuchtung
- Heizlüfter / Heizung
- bis zu 4 Linearantriebe
- EWT-Ventilator

## Erdreichwärmetauscher

Der Erdreichwärmetauscher ist ein wichtiger Differenzierungsansatz für Ganzjahresbetrieb und Energieoptimierung.

## Produktprinzip

> Verkabelte Kernfunktionen für Zuverlässigkeit, drahtlose Erweiterungen für Skalierbarkeit.
