# Erinnerung

Diese Datei sammelt kleine Produktdetails, Korrekturen und noch nicht weit genug entwickelte Gedanken. Sie dient als Kurzzeitgedächtnis für spätere Analysen.

Größere bestätigte Richtungsentscheidungen gehören weiterhin in [decisions.md](decisions.md). Die Präsentation wird nicht wegen jedes neuen Details geändert, sondern erst, wenn mehrere Punkte eine relevante Aussage verändern.

## Bestätigte Prototypdetails

Stand: 13. September 2026 – Angaben des Gründers, noch nicht unabhängig geprüft.

- Die Prototypengehäuse sind IP67.
- Das Gehäuse besitzt einen transparenten Frontdeckel.
- Das Display bleibt bei geschlossenem Deckel gut ablesbar.
- Für die lokale Bedienung muss der Deckel geöffnet werden.
- Alternativ ist die Bedienung über die App möglich.
- IP67 gilt nach Gründerangabe für den vollständig aufgebauten Controller einschließlich seiner Anschlüsse.
- Die Außensensoren sind wetterfest; die Innensensoren sind mindestens gegen Regen geschützt.
- Aktuell eingebunden ist eine Ecowitt Wittboy GW2001. Die Systemansicht zeigt das zugehörige Gateway als GW2000A im 868-MHz-Band.
- Als neuere mögliche Nachfolgeplattform wurde die Ecowitt Wittboy GW3001 identifiziert. Sie besteht laut Hersteller aus GW3000-Gateway und WS90-Außensensor; sie ist noch nicht als Produktentscheidung oder bereits integrierte Komponente zu behandeln.
- M01 und M02 bilden Zone beziehungsweise Gewächshaus 1; M03 und M04 bilden Zone beziehungsweise Gewächshaus 2.
- Sämtliche auf den bereitgestellten Screenshots dargestellten Funktionen laufen nach Gründerangabe seit drei Jahren im realen Gewächshausbetrieb.
- Reinigung mit dem Gartenschlauch ist ein zugesagtes Produktmerkmal. Hochdruckreinigung bleibt davon getrennt und ist noch nicht zugesagt.
- Im Gewächshaus treten dauerhaft beziehungsweise regelmäßig sehr hohe Luftfeuchtigkeiten auf.
- Für den vorgesehenen Einsatz wird ein ungeschützter oder nur schwach geschützter Controller als ungeeignet betrachtet.

## Wichtige Präzisierung zur Schutzart

- IP67 ist nach Gründerangabe der aktuelle Stand des vollständig aufgebauten Controllers samt Anschlüssen.
- Offen bleibt der formale Nachweis für das spätere Serienprodukt und dessen konkrete Steckverbinder-, Kabel- und Montagekonfiguration.
- IP67 belegt zeitweiliges Untertauchen, aber nicht automatisch starke Wasserstrahlen oder Hochdruckreinigung. Für das spätere Produktversprechen sind gegebenenfalls kombinierte Prüfungen wie IP66/IP67 oder zusätzlich IP69 erforderlich.
- Das Öffnen des Deckels in feuchter Luft kann Feuchtigkeit in das Gehäuse bringen. Kondensation, Druckausgleich und das Bedienkonzept müssen deshalb getrennt betrachtet werden.

## Korrekturen und Abgrenzungen

- **Home Assistant Green ist kein Gewächshausprodukt.** „Green“ bezeichnet lediglich die grüne Hardware beziehungsweise den Produktnamen.
- Home Assistant wird in der Recherche nur als DIY-Alternative, Integrationsplattform und Geschäftsmodellvergleich für Open Source plus offizielle Hardware betrachtet.
- Home Assistant Green darf nicht als direkter Wettbewerber oder Gewächshauscontroller dargestellt werden.

## Arbeitsweise für neue Details

1. Kleine Information zunächst hier festhalten.
2. Als Gründerangabe, Hypothese, offene Frage oder Entscheidung kennzeichnen.
3. Erst bei strategischer Relevanz in Fachanalyse, `decisions.md` oder Präsentation übernehmen.
4. Überholte Einträge nicht still löschen, sondern datiert korrigieren oder als erledigt markieren.

## Aus den Prototypbildern ablesbarer Funktionsstand

Stand: 13. September 2026 – Sichtprüfung der vom Gründer bereitgestellten Fotos und Screenshots. Die Bilder belegen Bedienoberflächen und sichtbare Hardware. Der dreijährige Echtbetrieb aller dargestellten Funktionen sowie die Schutz- und Zonenaussagen sind Gründerangaben und noch nicht unabhängig geprüft.

- Übersichtsseite mit Innen- und Außenklima, Wind, Regen, Solarstrahlung, Luftdruck, EWT-Temperatur, vier Motorpositionen und Aktorstatus
- automatische Schutz- und Regelfunktionen für Sturm, starken Wind, Temperatur, Luftfeuchte, Tau-/Kondensationsschutz, Befeuchtung, Frostschutz und Heizung
- EWT-Betriebsarten zum Laden und Entladen sowie einstellbare Ventilatorleistung
- manuelle Bedienung von vier Motoren sowie Zirkulation, Befeuchtung, Heizung und EWT
- Konfiguration von Sensoren, Aktoren, Motlaufzeiten, Schwellwerten und Hysteresen
- lokale Systemdiagnose, Softwareaktualisierung, Neustart und WLAN-Einrichtung
- Controller im transparenten Schutzgehäuse mit lokalem Display und physischen Tasten
- sichtbar angeschlossene beziehungsweise eingesetzte Komponenten: Linearantriebe, Umluftventilator, EWT-/Rohrventilator, Wittboy-Außenstation und mehrere Ecowitt-Innen-/Fühlersensoren

Eine strukturierte Zuordnung steht in [prototype-inventory.md](prototype-inventory.md). Gerätekennungen, Zugangscodes und lokale Netzwerkadressen aus der Systemansicht werden nicht in die Dokumentation übernommen.

## Nächste Entscheidungen und Prüfungen

### 1. Prototyp sichtbar und funktional erfassen

- [x] Screenshots und Fotos des Prototyps bereitgestellt: Bedienoberfläche, geschlossener und geöffneter Controller sowie Feldkomponenten.
- [x] Sichtbaren Funktionsumfang und Hardwarebestand in einer ersten Prototypinventur erfasst.
- [x] Vom Gründer bestätigt: Alle auf den Screenshots dargestellten Funktionen laufen seit drei Jahren im Echtbetrieb.
- [x] Motorkanäle zugeordnet: M01/M02 = Zone beziehungsweise Gewächshaus 1; M03/M04 = Zone beziehungsweise Gewächshaus 2.
- [ ] Noch nicht eindeutige Sensorrollen und die jeweilige Funktion der beiden Motoren innerhalb einer Zone zuordnen.

### 2. Schutzversprechen festlegen

- [x] Nach Gründerangabe geklärt: IP67 gilt für den vollständig aufgebauten Controller samt Anschlüssen.
- [ ] Prüfgrundlage beziehungsweise Nachweis der Schutzart und Übertragbarkeit auf das Serienprodukt dokumentieren.
- [x] Gartenschlauchreinigung als zugesagtes Produktmerkmal festgelegt.
- [ ] Entscheiden, ob zusätzlich direkte Hochdruckreinigung erlaubt und zugesagt werden soll.
- [ ] Prüfen, welche Bedienhandlungen bei geschlossenem Deckel möglich beziehungsweise sicherheitsrelevant sein müssen.
- [ ] Kondensationskonzept festlegen: Dichtung, Druckausgleichsmembran, Beschichtung, Entfeuchtung oder andere Maßnahme.

### 3. Kernprodukt abgrenzen

- [ ] Entscheiden, ob das erste kaufbare Grundsystem eine oder zwei Zonen enthält.
- [ ] Festlegen, welche Wetterstation und Sensorfabrikate offiziell unterstützt werden.
- [ ] GW2001 und GW3001 praktisch vergleichen: lokale Schnittstelle, Datenlatenz, Ausfallerkennung, Winterbetrieb, Funküberwachung und Integrationsaufwand.
- [ ] Prüfen, ob beim WS90 für sicherheitsrelevante Windmessung die optionale 12-V-Versorgung mit Heizung verpflichtender Bestandteil der unterstützten Installation sein muss.
- [ ] Festlegen, welche Komponenten mitverkauft und welche transparent extern beschafft werden.

### 4. Sicherheitsverhalten beschreiben

- [ ] Für Sensorfehler, Aktorfehler, Kommunikationsausfall und Stromwiederkehr jeweils den sicheren Zustand definieren.
- [ ] Klären, welche Handbedienung ohne App und ohne Öffnen des Gehäuses erforderlich ist.
- [ ] Festlegen, wie Aktorpositionen oder Endlagen zuverlässig bestätigt werden.

### 5. Vollständigen Preis verstehen

- [ ] Stückliste des aktuellen Prototyps mit realen Einkaufspreisen ergänzen.
- [ ] Drei vollständige Beispielanlagen einschließlich Kabeln, Sensoren, Netzteil, Schnittstellen und Aktoren kalkulieren.
- [ ] Erst danach Zielpreis und Paketstruktur beurteilen.

Status: Die Kalkulation wird vom Gründer nachgeholt; bis dahin bleiben Preis- und Margenaussagen ausdrücklich vorläufig.

## Später zu entscheiden

- Umfang der Open-Source-Freigabe
- bezahlte und kostenlose Software-/Cloudfunktionen
- genaue Inhalte des Online-Konfigurators
- EWT als Produktmodul oder ausschließlich als Wissens-/Berechnungsthema
