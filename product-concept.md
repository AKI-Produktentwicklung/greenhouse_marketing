# Produktkonzept

## Status

Diese Datei beschreibt nur den aktuellen Rahmen. Technische Detailentwicklung ist derzeit nicht Schwerpunkt.

Die marktbasierte Bewertung und empfohlene Reduktion des Startumfangs stehen in [prototype-market-assessment.md](prototype-market-assessment.md). Die Empfehlungen sind noch keine Produktentscheidungen.

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

Der Erdreichwärmetauscher ist eine technische Differenzierungshypothese für Ganzjahresbetrieb und Energieoptimierung. Die bisherige Marktanalyse liefert dafür keine direkte Nachfrageevidenz; er wird daher nicht als Bestandteil des empfohlenen Kernpakets behandelt.

## Produktprinzip

> Verkabelte Kernfunktionen für Zuverlässigkeit, drahtlose Erweiterungen für Skalierbarkeit.

Die ältere Präsentation zeigt allerdings einen solar-/batteriebetriebenen Außen-Multisensor. Da Wind und Regen Schutzentscheidungen auslösen, muss diese Abweichung vor einer Produktentscheidung durch Verkabelung oder einen nachweisbar überwachten Fallback aufgelöst werden.
