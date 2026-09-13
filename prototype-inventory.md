# Prototypinventur

## Zweck und Evidenzstatus

Diese Datei beschreibt den am 13. September 2026 fotografisch dokumentierten Prototyp. Sie trennt sichtbare Befunde von Gründerangaben und noch offenen Zuordnungen. Eine Sichtprüfung ersetzt weder einen Funktionstest noch eine Schutzartprüfung.

## Systemüberblick

| Bereich | Sichtbarer beziehungsweise angegebener Stand | Evidenz |
|---|---|---|
| Controller | Schutzgehäuse mit transparentem Frontdeckel, lokalem Display, physischen Tasten und Kabeleinführungen beziehungsweise Anschlüssen | auf Fotos sichtbar |
| Umgebungsschutz | IP67 für den aufgebauten Controller einschließlich Anschlüsse | Gründerangabe |
| Versorgung | Controller arbeitet mit 12 oder 24 VDC | Gründerangabe aus der bisherigen Dokumentation |
| Bedienung | lokale Bedienung bei geöffnetem Deckel sowie Bedienung über App/Weboberfläche | Fotos, Screenshots und Gründerangabe |
| Wetterstation | Ecowitt Wittboy GW2001; Systemansicht bezeichnet das Gateway als GW2000A, 868 MHz | Gründerangabe und Screenshot |
| Außenumgebung | Außensensoren wetterfest | Gründerangabe |
| Innenumgebung | Innensensoren mindestens regengeschützt | Gründerangabe |
| Kosten | aktuelle Stück- und Gesamtkalkulation noch nicht vorhanden | Gründerangabe |
| Felderfahrung | alle auf den Screenshots dargestellten Funktionen laufen seit drei Jahren im realen Gewächshausbetrieb | Gründerangabe |
| Reinigung | Gartenschlauchreinigung ist zugesagtes Produktmerkmal; Hochdruckreinigung ist davon nicht umfasst | Gründerangabe/Produktentscheidung |

## Sichtbare Hardware

| Komponente | Beobachtung | Zuordnungssicherheit |
|---|---|---|
| Controllergehäuse | transparenter, verriegelbarer Deckel; innen Montageplatte, Display-/Tastenfeld und Ecowitt-Gateway | hoch |
| Lokale Bedienung | kleines Display und zehn sichtbare Bedientasten | hoch; konkrete Tastenbelegung noch offen |
| Linearantriebe | mindestens zwei fotografierte Antriebe; M01/M02 steuern Zone beziehungsweise Gewächshaus 1, M03/M04 Zone beziehungsweise Gewächshaus 2 | Hardware teilweise sichtbar, Vierkanalsteuerung per Screenshot sowie Zonenzuordnung per Gründerangabe belegt |
| Umluftventilator | großer Ventilator im Gewächshaus | Funktion als Zirkulation plausibel, genaue elektrische Zuordnung noch zu bestätigen |
| EWT-/Rohrventilator | Ventilator beziehungsweise Rohranschluss im EWT-Bereich | Funktion aus Oberfläche und Installation plausibel, genaue Zuordnung noch zu bestätigen |
| Wittboy-Außenstation | kompakte Außen-Multisensorstation an Mast | hoch |
| Innenklimasensor | Ecowitt-Sensor im Gewächshaus sichtbar | hoch; exaktes Modell und Messstellenrolle offen |
| Fühlersensor im Beet | Ecowitt-Fühler, auf dem Gerät als WN34AS bezeichnet, im Erd-/Pflanzbereich eingesetzt | Modellbeschriftung sichtbar; konkrete Messgröße im System noch zu bestätigen |
| weitere Fühler/Adapter | mehrere kleine Bauteile und Halterungen neben einem Antrieb fotografiert | nicht eindeutig identifizierbar |

## Sichtbarer Software- und Funktionsumfang

### Überwachung

- Innen- und Außentemperatur
- relative Luftfeuchte innen und außen
- Windgeschwindigkeit, Spitzenwert und Richtung
- Regenmenge
- Solarstrahlung und UV-Index
- Luftdruck
- EWT-Temperatur
- Position beziehungsweise Status von vier Motoren
- Status von Heizung, Umluft, Befeuchtung und EWT

### Automatik und Schutz

- Sturmschutz mit Schwellwert und Rückstellzeit
- Schutz bei starkem Wind mit begrenzter Öffnungsposition
- temperaturgeführte Lüftung
- feuchtegeführte Lüftung
- zusätzliche Umluft bei Hitze
- Umluft zur Feuchte- und Taupunkt-/Kondensationsbeherrschung
- Befeuchtung mit Schwellwert und Hysterese
- EWT-Laden und -Entladen mit Hysteresen und Bodentemperaturgrenze
- Frostschutz und Heizung mit Schwellwerten und Hysteresen

### Manuelle Bedienung und Einrichtung

- vier Motoren einzeln öffnen, stoppen und schließen
- Umluft, Befeuchtung, Heizung und EWT ein- beziehungsweise ausschalten
- Drehzahlvorgaben für Umluft und EWT
- Motorlaufzeiten und Freigaben konfigurieren
- Standardwerte laden
- WLAN einrichten
- Controller- und Wetterstationsstatus ansehen
- Anwendung aktualisieren und Komponenten neu starten

## Bestätigter Betriebsstand

Nach Gründerangabe laufen alle auf den Screenshots dargestellten Überwachungs-, Automatik-, Schutz-, Bedien- und Einrichtungsfunktionen seit drei Jahren im realen Gewächshausbetrieb. Für die Marktpositionierung ist das eine belastbare Felderfahrung, bleibt aber bis zu einer strukturierten Betriebsdokumentation eine Gründerangabe.

## Noch zu bestätigen

- Welche konkrete Funktion hat jeweils der erste und zweite Motor innerhalb einer Zone, beispielsweise Dachfenster, Seitenfenster oder Tür?
- Welche Modelle und Messgrößen haben die einzelnen Innen- und Fühlersensoren?
- Welche Steckverbinder werden aktuell verwendet, und sind unbenutzte Anschlüsse ebenfalls IP67 geschützt?
- Welche Aktoren werden direkt geschaltet und welche über zusätzliche Leistungsstufen oder Relais?
- Wie verhält sich das System bei Sensorfehler, Kommunikationsausfall, blockiertem Antrieb und Stromwiederkehr?
- Welche Bestandteile gehören später zum Lieferumfang, welche nur zur offiziell unterstützten Fremdbeschaffung?

## Datenschutz bei den Bilddateien

Eine Systemansicht enthält Gerätekennungen, einen Zugangscode und lokale Netzwerkdaten. Diese Werte werden nicht textlich übernommen. Vor einer Veröffentlichung der Bilder in einem öffentlichen oder geteilten Repository sollte die betreffende Ansicht redigiert werden.
