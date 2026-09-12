# Pain Points

## Ziel

Nicht Funktionen sammeln, sondern Probleme finden, für deren Lösung Kunden tatsächlich Geld bezahlen.

Bewertungskriterien:

- Häufigkeit
- wirtschaftlicher Schaden
- Zeitverlust
- Stress / Bindung an den Standort
- Dringlichkeit
- heutige Lösungsqualität
- Zahlungsbereitschaft

## Aktuelle Kern-Pain-Points

### 1. Gewächshaus kann nicht unbeaufsichtigt bleiben
Der Besitzer muss bei Wetteränderungen oder kritischen Zuständen erreichbar und oft physisch vor Ort sein.

Nutzen einer Lösung:
- Freiheit
- Urlaub
- Berufstätigkeit
- weniger Kontrollfahrten

### 2. Überhitzung bei plötzlicher Sonneneinstrahlung
Temperaturen können schnell kritische Bereiche erreichen.

Nutzen:
- Schutz vor Pflanzenschäden
- stabileres Klima
- weniger manuelle Lüftung

### 3. Sturm bei geöffneten Lüftungen
Offene Fenster oder Klappen können bei starkem Wind beschädigt werden.

Nutzen:
- Schutz von Gewächshaus und Antrieben
- automatische Reaktion auch bei Abwesenheit

### 4. Frost
Nächtliche Temperaturabfälle können Pflanzen und Kulturen schädigen.

Nutzen:
- automatische Schutzmaßnahmen
- höhere Ertragssicherheit

### 5. Zu hohe Luftfeuchtigkeit / Kondensation / Schimmelrisiko
Probleme entstehen nicht nur durch Temperatur, sondern durch das Zusammenspiel mehrerer Klimagrößen.

Nutzen:
- gesündere Pflanzen
- weniger Krankheitsdruck
- kontrolliertes Lüften / Heizen / Umluft

### 6. Bewässerungsfehler
Zu wenig oder zu viel Wasser kann schnell Schäden verursachen.

Nutzen:
- konstante Versorgung
- Alarm bei Ausfall
- spätere Erweiterbarkeit um Bodenfeuchte und Bewässerungslogik

### 7. Einzelne Geräte arbeiten nicht als System
Thermostate, Lüfter, Fensteröffner, Pumpen und Sensoren arbeiten getrennt.

Nutzen:
- koordinierte Entscheidungen
- weniger widersprüchliche Aktionen
- zentrale Bedienung

### 8. Ausfälle werden zu spät erkannt
Sensoren, Antriebe, Pumpen oder Heizungen können ausfallen, ohne dass der Nutzer es sofort bemerkt.

Nutzen:
- Fehlererkennung
- Ersatzsensoren / Fallback
- Alarmierung
- definierter Safe Mode

### 9. Ganzjahresbetrieb ist energieintensiv
Heizung, Lüftung und Entfeuchtung können unnötig Energie verbrauchen.

Nutzen:
- intelligentere Betriebsstrategien
- Nutzung eines Erdreichwärmetauschers
- spätere Energieoptimierung

### 10. Automation ist technisch zu kompliziert
Viele bestehende Lösungen verlangen Eigenbau, Programmierung oder Smart-Home-Know-how.

Nutzen:
- fertiges Gesamtsystem
- steckbare Komponenten
- Ansprechpartner
- Updates und Support

## Zusätzliche Pain-Points

### 11. Keine belastbare Datenhistorie
Ohne Logging ist schwer nachvollziehbar, warum eine Kultur besser oder schlechter lief.

### 12. Mehrere Gewächshäuser erhöhen den Kontrollaufwand
Mit jeder weiteren Zone steigt der Aufwand überproportional.

### 13. Wetterprognosen werden nicht genutzt
Bestehende einfache Regler reagieren nur auf aktuelle Sensorwerte.

### 14. Fehlende Fernüberwachung
Der Nutzer weiß unterwegs nicht, ob das Gewächshaus in einem sicheren Zustand ist.

## Aktuelle Priorisierung

Besonders relevant erscheinen derzeit:

1. Abwesenheit / Standortbindung
2. Überhitzung
3. Sturm
4. Frost
5. Ausfallerkennung
6. stabile Klimabedingungen
7. Zeitersparnis im gewerblichen Betrieb
8. einfaches Gesamtsystem statt DIY

## Erste Voice-of-Customer-Stichprobe - 12. September 2026

Diese erste Stichprobe umfasst acht öffentlich zugängliche Community-Diskussionen aus 2025 und 2026. Sie ist qualitativ und nicht repräsentativ. Einzelne Aussagen belegen, dass ein Problem vorkommt; sie erlauben noch keine Aussage über Häufigkeit, Marktgröße oder Zahlungsbereitschaft.

| Beobachtetes Problem | Konkretes Signal aus der Stichprobe | Betroffene Hypothese | Quellen |
|---|---|---|---|
| Überhitzung während Abwesenheit | Ein Nutzer kann morgens wegen Frost nicht öffnen; bei Sonne würde das Gewächshaus vor seiner Rückkehr etwa 90 °F erreichen. Andere berichten trotz passiver Öffner von 85-90 °F. | Abwesenheit plus schnelle Wetteränderung ist plausibel kaufrelevant. | [Automatische Öffner funktionieren nicht](https://www.reddit.com/r/Greenhouses/comments/1quhz10/has_anyone_ever_used_these_before/), [Fragen zu automatischen Öffnern](https://www.reddit.com/r/Greenhouses/comments/1vsmjsj/automatic_vent_questions/) |
| Konflikt zwischen Hitzeschutz und Sturm | Passive Öffner reagieren auf Temperatur, können aber bei plötzlich aufkommendem Wind nicht aktiv schließen. Nutzer improvisieren Verriegelungen oder bevorzugen elektrische Antriebe. | Sturmschutz ist nicht bloß Zusatzfunktion, sondern löst einen Zielkonflikt einfacher Automatisierung. | [Fragen zu automatischen Öffnern](https://www.reddit.com/r/Greenhouses/comments/1vsmjsj/automatic_vent_questions/), [Feuchtegesteuerter Lüfter](https://www.reddit.com/r/Greenhouses/comments/1irpp5y/humidity_controlled_fan_setup_first_time/) |
| Begrenzte Haltbarkeit und langsame Reaktion passiver Öffner | Erfahrungen reichen von Defekten nach ein bis zwei Saisons bis zu mehrjährig gutem Betrieb; die Öffnung kann rund 20 Minuten benötigen. | Zuverlässigkeit ist relevant, aber die Produktklasse ist nicht pauschal schlecht. | [Automatische Fensteröffner](https://www.reddit.com/r/Greenhouses/comments/1rf1ioe/automatic_vent_openers/) |
| Klima erfordert koordinierte Regelung | Ein Nutzer hält Temperatur und Feuchte trotz Abluft, Umluft und zeitgesteuerter Vernebelung nicht stabil; nach kurzer Kühlung steigen die Werte wieder. | Einzelne Thermostate und Timer können bei gekoppelten Klimagrößen unzureichend sein. | [Temperatur-/Feuchteregelung](https://www.reddit.com/r/greenhouse/comments/1ui8t7w/greenhouse_temperaturehumidity_control/) |
| Wunsch nach einfacher Fertiglösung | Ein technisch interessierter Neueinsteiger sucht ausdrücklich eine einfachere, vorgefertigte Lösung für feuchte-/temperaturgesteuerte Ventilatoren. | "Technikoffen, aber kein Integrator" ist ein plausibles Kundensegment. | [Feuchtegesteuerter Lüfter](https://www.reddit.com/r/Greenhouses/comments/1irpp5y/humidity_controlled_fan_setup_first_time/) |
| DIY-Lösungen werden schnell zu Systemprojekten | Aktuelle Home-Assistant-Projekte kombinieren Temperatur-/Feuchtesensoren, Außenwetter, Motoren, Pumpen, Magnetventile, Smart Plugs, Bewässerung und Prognosen. | Der Integrationsaufwand ist real; zugleich ist DIY für versierte Anwender eine starke Alternative. | [Automatisiertes Gewächshaus 2026](https://www.reddit.com/r/homeassistant/comments/1uo8m4z/automated_greenhouse/), [Smart-Greenhouse-Projekt 2026](https://www.reddit.com/r/Greenhouses/comments/1vfe8hk/my_first_smart_greenhouse_project/) |
| Sensorik und Funk im Außenbereich sind störanfällig | Ein Nutzer berichtet von ausgefallenen beziehungsweise instabilen Zigbee-Außensensoren; eine weitere Diskussion nennt Fehlalarme einfacher Regensensoren durch Kondensation. | Verkabelte Kernsensorik und Sensor-Plausibilisierung können echte Differenzierungsmerkmale sein. | [Home-Assistant-Gewächshaus](https://www.reddit.com/r/homeassistant/comments/1s0cs9l/ha_greenhouse/), [Zigbee-Regensensor](https://www.reddit.com/r/homeassistant/comments/1u83jeg/rain_sensor_zigbee/) |
| Beschattung bleibt oft manuell | Ein aktuelles DIY-Projekt automatisiert bereits Lüfter, Wasser und Nebel, sucht aber noch eine automatisch einziehbare Beschattung. | Beschattung ist ein sinnvoller Ausbaupfad, vermutlich nicht zwingend Teil des kleinsten Einstiegspakets. | [Automatisiertes Gewächshaus 2026](https://www.reddit.com/r/homeassistant/comments/1uo8m4z/automated_greenhouse/) |

### Vorläufige Verdichtung

Die stärkste qualitative Problemkette lautet derzeit:

> Sonne erzeugt während Abwesenheit schnell Überhitzung; passive Öffner können bei Sturm nicht sicher schließen; elektrische Eigenlösungen erfordern mehrere Sensoren, Aktoren und Regeln; Funk- und Sensorfehler erhöhen wiederum das Risiko.

Diese Kette stützt die Positionierung "zuverlässige Autonomie und Schutz" stärker als ein allgemeines Komfortversprechen. Zahlungsbereitschaft und Häufigkeit sind damit noch nicht validiert.
