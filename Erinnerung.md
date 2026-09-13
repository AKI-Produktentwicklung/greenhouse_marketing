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
- Im Gewächshaus treten dauerhaft beziehungsweise regelmäßig sehr hohe Luftfeuchtigkeiten auf.
- Für den vorgesehenen Einsatz wird ein ungeschützter oder nur schwach geschützter Controller als ungeeignet betrachtet.

## Wichtige Präzisierung zur Schutzart

- IP67 ist der aktuelle Stand des Prototypengehäuses.
- Noch zu prüfen ist, ob IP67 für die vollständig bestückte Einheit gilt: Deckel, Dichtung, Display, Kabelverschraubungen, Steckverbinder, Schutzkappen und Montage.
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

## Nächste Entscheidungen und Prüfungen

### 1. Prototyp sichtbar und funktional erfassen

- [ ] Screenshot beziehungsweise Fotos des Prototyps bereitstellen: Displayansicht, geschlossener Deckel, geöffneter Deckel und Anschlüsse.
- [ ] Kurz markieren, welche Anzeigen und Bedienfunktionen bereits real funktionieren.
- [ ] Aktuelle Sensoren und Aktoren den sichtbaren Funktionen zuordnen.

### 2. Schutzversprechen festlegen

- [ ] Klären, ob IP67 nur für das Rohgehäuse oder für die vollständig bestückte Einheit nachgewiesen ist.
- [ ] Entscheiden, ob das Produkt Gartenschlauchreinigung, Hochdruckreinigung oder beides ausdrücklich erlauben soll.
- [ ] Prüfen, welche Bedienhandlungen bei geschlossenem Deckel möglich beziehungsweise sicherheitsrelevant sein müssen.
- [ ] Kondensationskonzept festlegen: Dichtung, Druckausgleichsmembran, Beschichtung, Entfeuchtung oder andere Maßnahme.

### 3. Kernprodukt abgrenzen

- [ ] Entscheiden, ob das erste kaufbare Grundsystem eine oder zwei Zonen enthält.
- [ ] Festlegen, welche Wetterstation und Sensorfabrikate offiziell unterstützt werden.
- [ ] Festlegen, welche Komponenten mitverkauft und welche transparent extern beschafft werden.

### 4. Sicherheitsverhalten beschreiben

- [ ] Für Sensorfehler, Aktorfehler, Kommunikationsausfall und Stromwiederkehr jeweils den sicheren Zustand definieren.
- [ ] Klären, welche Handbedienung ohne App und ohne Öffnen des Gehäuses erforderlich ist.
- [ ] Festlegen, wie Aktorpositionen oder Endlagen zuverlässig bestätigt werden.

### 5. Vollständigen Preis verstehen

- [ ] Stückliste des aktuellen Prototyps mit realen Einkaufspreisen ergänzen.
- [ ] Drei vollständige Beispielanlagen einschließlich Kabeln, Sensoren, Netzteil, Schnittstellen und Aktoren kalkulieren.
- [ ] Erst danach Zielpreis und Paketstruktur beurteilen.

## Später zu entscheiden

- Umfang der Open-Source-Freigabe
- bezahlte und kostenlose Software-/Cloudfunktionen
- genaue Inhalte des Online-Konfigurators
- EWT als Produktmodul oder ausschließlich als Wissens-/Berechnungsthema

