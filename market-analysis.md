# Marktanalyse

## Leitfrage

Gibt es im DACH- bzw. europäischen Markt genügend Kunden, die für eine autonome Gewächshaussteuerung im Bereich von etwa 1.000–3.000 EUR oder mehr bezahlen?

## Arbeitshypothese

Zwischen zwei Marktenden scheint eine Lücke zu bestehen:

### Unteres Ende
DIY- und Smart-Home-Lösungen:

- ESP32 / Arduino
- Home Assistant
- Node-RED
- WLAN-Steckdosen
- Einzelthermostate
- einfache Grow-Controller

Vorteile:
- günstig
- flexibel

Nachteile:
- hoher Eigenaufwand
- fehlende Systemverantwortung
- oft keine echte Ausfallsicherheit
- unterschiedliche Hersteller und Apps
- für normale Anwender schwer wartbar

### Oberes Ende
Professionelle Gartenbauautomation:

- Klima-Computer
- professionelle Bewässerungs- und Fertigationssysteme
- industrielle Sensorik und Aktorik
- Service- und Integrationsleistungen

Vorteile:
- robust
- bewährt
- skalierbar

Nachteile:
- teuer
- oft überdimensioniert
- für kleine Gewächshäuser zu komplex
- häufig Installations- und Serviceabhängigkeit

## Vermutete Marktlücke

Zielbereich:

> Hochwertige kleine Gewächshäuser und kleine gewerbliche Anlagen, die mehr Zuverlässigkeit und Autonomie benötigen als Smart-Home-Lösungen bieten, aber keine klassische professionelle Gewächshausautomation rechtfertigen.

## Relevante Marktsegmente

Priorität 1:
- ambitionierte private Gewächshausbesitzer
- Selbstversorger mit hochwertigem Gewächshaus
- Besitzer von Ganzjahresgewächshäusern

Priorität 2:
- kleine Direktvermarkter
- Market Farmer
- kleine Gemüsebaubetriebe

Weitere mögliche Segmente:
- Gastronomie / Farm-to-table
- Schulen, Bildung, Demonstrationsanlagen
- kleine Spezialkulturen
- hochwertige Wintergärten bzw. Sonderanwendungen

## Marktannahmen, die validiert werden müssen

1. Kunden mit Gewächshäusern ab ca. 5.000 EUR akzeptieren zusätzliche Investitionen in Automation.
2. Ein Systempreis von ca. 1.000–3.000 EUR ist für einen Teil des Marktes plausibel.
3. Abwesenheit und Risikoschutz sind stärkere Kaufargumente als reine Komfortfunktionen.
4. Kleine gewerbliche Betriebe bewerten Arbeitszeitersparnis und Ertragssicherheit höher als private Nutzer.
5. Kunden wünschen eher ein funktionierendes Gesamtsystem als eine Sammlung einzelner Smart-Home-Komponenten.
6. Service, Fernwartung und Support erhöhen die Zahlungsbereitschaft.
7. Wiederkehrende Erlöse über Cloud-/Servicefunktionen sind akzeptabel, wenn der Grundbetrieb lokal und ohne Abo möglich bleibt.

## Verbleibende Evidenzlücken nach der Desk Research

Öffentliche Quellen haben typische Gewächshaus- und Controllerpreise, relevante Wettbewerber, qualitative Beschwerden und einen breiten DACH-Basisnenner geliefert. Nicht belastbar öffentlich bestimmbar sind weiterhin:

- der Anteil der Gärten mit eigenem Gewächshaus,
- der Anteil hochwertiger kleiner Gewächshäuser im Zielprofil,
- aktuelle DACH-Stückzahlen der Premiumhersteller,
- vollständig installierte Preise direkt vergleichbarer Steuerungen,
- tatsächliche Kaufquote und Zahlungsbereitschaft der Zielkunden,
- Support-, Installations- und Akquisitionskosten eines eigenen Angebots.

Diese Lücken benötigen Primärinterviews, Hersteller-/Händlerauskünfte oder eigene Pilotdaten. Weitere allgemeine Websuche würde vor allem zusätzliche Proxys liefern, aber die entscheidenden Modellparameter nicht validieren.

## Erstbefund Wettbewerbsmarkt - 12. September 2026

Die primärquellenbasierte Wettbewerbsrecherche umfasst inzwischen 23 Systeme beziehungsweise Produktfamilien. Davon sind 21 als aktuell verfügbar dokumentiert. Bartlett ClimateBoss ist eingestellt; Trellis One befindet sich noch in Entwicklung. Details und Einzelquellen stehen in [competitors.md](competitors.md) und [sources.md](sources.md).

### Verifizierte Fakten

- Mehrere ernsthafte Controller werden öffentlich für etwa 1.000-1.500 EUR angeboten: Link4 Pearl (1.499 USD zuzüglich ausgewiesenem Hardwareaufschlag), GrowControl GrowBase Pro WiFi (1.049 EUR inklusive Umsatzsteuer) und NIDO ONE V2 (1.489,99 EUR inklusive Umsatzsteuer). Bartlett ClimateBoss lag mit zuletzt 1.015 USD ebenfalls in diesem Bereich, ist laut Hersteller aber eingestellt und daher nur ein historischer Preisanker.
- Diese Preise sind nicht direkt vergleichbar. Lieferumfang, Netzspannung, Sensoren, I/O, Wetterstation, Motorsteuerung, Installation und Umsatzsteuer unterscheiden sich.
- Vollständige Gewächshausfunktionen einschließlich Wind-/Regenschutz und motorischer Lüftung sind bei professionellen Systemen wie Senmatic LCC1, RAM CC600 und MABEG nachgewiesen. Öffentliche Komplettpreise fehlen dort.
- Bei einfach online kaufbaren Produkten liegt der Schwerpunkt häufig auf Indoor-Grow oder Fertigation. Die geprüften Produktseiten belegen dort keine vollständige Kombination aus Außenwetter, Sturmreaktion und Fensterantrieben.
- Ridder Hortimax Go belegt, dass ein professionelles Einstiegssystem bereits Klima, Bewässerung sowie Sturm-, Frost- und Regenschutz verbinden kann. NIDO ONE V2 und Argus Axia belegen lokalen Weiterbetrieb bei Internetausfall. Diese Merkmale allein sind daher keine einzigartige Positionierung.
- Aktuelle DACH-Angebote bestätigen, dass private Gewächshauskäufer mehrere Tausend Euro investieren: Vitavia bietet ein 10,2-m²-Set mit Heizung, Beleuchtung und automatischen Dachlüftern ab 3.799,90 EUR an; Selfkant Wolters nennt für direkt kaufbare Modelle 3,8-14,7 m² und einen Einstieg ab 3.095 EUR; die WAMA-Preisliste 2026 enthält Profi-Konfigurationen von rund 7.300 EUR bis über 30.000 EUR.
- Aus öffentlichen Einzelpreisen gebildete, noch unvollständige Warenkörbe liegen bereits bei 1.667,14 EUR inklusive Umsatzsteuer für NIDO ONE V2 mit insgesamt vier Smart Plugs und bei 2.572,83 USD für Link4 Pearl mit einem 4-Relais-/4-Analog-Modul inklusive des ausgewiesenen Hardwareaufschlags. Beide Beträge enthalten noch keine funktionsgleiche Kombination aus Außenwetter, sicherer Motorsteuerung und Installation.

### Vorläufige Interpretation

Die Marktchance liegt wahrscheinlich nicht in "Gewächshausautomation gibt es noch nicht", sondern in einer anders verpackten Kombination bestehender Fähigkeiten:

- kleiner Anlagenumfang statt professionellem Gewächshauskomplex,
- lokaler, sicherer Grundbetrieb statt Cloud-Abhängigkeit,
- echte Außenwetter- und Schutzlogik statt Indoor-Klimaregelung,
- nachrüstbares System statt individuell geplantem Schaltschrank,
- verständlicher Kauf- und Installationspfad statt Projektvertrieb.

Diese Interpretation ist eine Hypothese. Sie muss durch Preise vollständiger Vergleichsanlagen und durch Kundenaussagen validiert werden.

Die erweiterte Community-Stichprobe in [voice-of-customer.md](voice-of-customer.md) stützt besonders den kombinierten Problemfall aus Überhitzung während Abwesenheit, geöffneten Lüftungen bei Sturm und hohem DIY-Integrationsaufwand. Sie ist nicht repräsentativ und belegt keine Zahlungsbereitschaft.

### Konsequenz für TAM / SAM / SOM

Ein erstes transparentes Szenariomodell steht in [market-sizing.md](market-sizing.md). Es zeigt eine sehr breite Spanne von rund 1,55 bis 82,49 Mio. EUR möglichem jährlichem Hardwareumsatz. Diese Spanne ist ausdrücklich keine belastbare Marktschätzung, sondern macht sichtbar, wie stark das Ergebnis von zwei noch unbelegten Quoten abhängt.

Für eine belastbare Marktgrößenrechnung müssen zwei Nenner geklärt werden:

1. Zahl hochwertiger kleiner Gewächshäuser beziehungsweise relevante jährliche Neuverkäufe in DACH.
2. Anteil der Besitzer, für die Abwesenheit, Wetterschutz und koordinierte Automation einen Kauf von mindestens etwa 1.000 EUR auslösen.

Bis diese Größen aus belastbaren Daten oder Primärinterviews gestützt sind, bleiben Marktvolumen und erreichbare Stückzahlen ausdrücklich offen. Der deutsche Garten-Gesamtmarkt von 19,7 Mrd. EUR eignet sich nur als Kontext und darf nicht als TAM für Gewächshausautomation verwendet werden.
