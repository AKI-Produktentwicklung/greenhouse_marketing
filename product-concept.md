# Produktkonzept

## Status

Diese Datei beschreibt nur den aktuellen Rahmen. Technische Detailentwicklung ist derzeit nicht Schwerpunkt.

Die marktbasierte Neubewertung und empfohlene Paketlogik stehen in [prototype-market-assessment.md](prototype-market-assessment.md). Die Empfehlungen sind noch keine Produktentscheidungen.

## Zielbereich

- Gewächshäuser ca. 10–100 m²
- zwei Zonen / zwei Gewächshäuser im verkabelten Grundsystem
- weitere Erweiterung über WLAN möglich

## Grundarchitektur

- Versorgung des Controllers mit 12 oder 24 VDC
- vorgesehene 12-V-Versorgung der Wetterstation über den Controller; genaue elektrische Auslegung noch zu dokumentieren
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

Seit drei Jahren im Prototyp im realen Gewächshausbetrieb:

- Sturmschutz
- Frostschutz
- Sensorausfall / Ersatzsensoren
- Überhitzungsschutz
- Feuchteregelung
- lokale Wetterdaten

## Dokumentierter Prototypstand

Fotos und Screenshots zeigen einen deutlich breiteren bereits angelegten Funktionsumfang: vier Motorkanäle, Umluft, Befeuchtung, Heizung, EWT, Wind- und Sturmschutz sowie temperatur-, feuchte- und taupunktbezogene Regelung. M01/M02 sind Zone beziehungsweise Gewächshaus 1, M03/M04 Zone beziehungsweise Gewächshaus 2. Sämtliche dargestellten Funktionen laufen nach Gründerangabe seit drei Jahren im realen Gewächshausbetrieb. Die derzeit eingebundene Wetterstation ist eine Ecowitt Wittboy GW2001.

Der aufgebaute Controller samt Anschlüssen ist nach Gründerangabe IP67. Die Außensensoren sind wetterfest, die Innensensoren mindestens regengeschützt. Sichtbare Komponenten und noch offene Zuordnungen sind in [prototype-inventory.md](prototype-inventory.md) dokumentiert.

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

Die offizielle Beschreibung der neueren Ecowitt Wittboy GW3001 bestätigt diese Plattformlogik: Das GW3000-Gateway unterstützt laut Hersteller unter anderem jeweils bis zu acht Blattfeuchte-, Temperaturfühler- und kombinierte Temperatur-/Feuchtekanäle sowie bis zu 16 Bodensensoren. Ethernet, WLAN, lokale Micro-SD-Speicherung, WebUI und HTTP-API passen grundsätzlich zur lokal autonomen Architektur. Das ist noch keine Festlegung auf die GW3001; Integrationsverhalten, Ausfallerkennung und mechanische Eignung müssen praktisch geprüft werden.

Der im GW3001-Paket enthaltene WS90-Außensensor ist laut Hersteller IPX5. Für Frost und Schnee wird eine optionale 12-V-Versorgung mit Heizfunktion empfohlen. Da Winddaten Schutzentscheidungen auslösen, ist diese Winterkonfiguration nicht nur Zubehörfrage, sondern Teil der späteren Zuverlässigkeitsbewertung.

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

Als Produktanforderung beziehungsweise marktbasierte Arbeitshypothese gilt:

- gesamte Feldinstallation für nasse Reinigung konzipieren,
- Gartenschlauchreinigung als zugesagtes Produktmerkmal technisch eindeutig definieren und für die vollständige relevante Anordnung nachweisen,
- IP66 nur nach Prüfung der vollständigen Anordnung bewerben,
- Hochdruckreinigung separat auf IPX9/IP69-Niveau prüfen,
- Steckverbinder, Schutzkappen, Kabel, Sensoren und Bedienelemente in die Systemprüfung einbeziehen,
- externes Netzgerät und 230-V-Verbindung außerhalb der Waschzone anordnen oder getrennt qualifizieren.

Die IP67-Angabe zum aktuellen Controller ist damit ein wichtiger Prototypvorteil. Für die zugesagte Gartenschlauchreinigung muss dennoch der zulässige Strahl, Abstand, Winkel und Betriebszustand der vollständigen relevanten Anordnung eindeutig beschrieben und geprüft werden. Direkte Hochdruckreinigung bleibt ein separates, derzeit nicht zugesagtes Schutzziel.

Details und Wettbewerbsbelege stehen in [washdown-protection-analysis.md](washdown-protection-analysis.md).

Die ältere Präsentation zeigt allerdings einen solar-/batteriebetriebenen Außen-Multisensor. Da Wind und Regen Schutzentscheidungen auslösen, muss diese Abweichung vor einer Produktentscheidung durch Verkabelung oder einen nachweisbar überwachten Fallback aufgelöst werden.
