# Vorläufiges Market Sizing – DACH

## Status

Stand: 12. September 2026

Dieses Dokument ist ein erstes, bewusst konservativ dargestelltes Szenariomodell. Es ist noch **keine belastbare TAM-/SAM-/SOM-Schätzung**, weil zwei entscheidende private Marktquoten öffentlich nicht belegt sind:

1. Anteil der Gärten mit einem Gewächshaus.
2. Anteil dieser Gewächshäuser, der hochwertig genug ist und einen ausreichend starken Automationsbedarf besitzt.

Die Modellwerte sind deshalb Szenarien, keine Marktbehauptungen.

## Marktdefinition

### Privater Kernmarkt

- Region: Deutschland, Österreich und Schweiz
- Nutzer: private Besitzer hochwertiger Gewächshäuser, Selbstversorger und Ganzjahresnutzer
- Produkt: nachrüstbare autonome Steuerung für ungefähr 10–100 m²
- Messgröße: potenziell geeigneter Bestand, daraus abgeleitete jährliche Käufe und Hardwareumsatz
- betrachteter durchschnittlicher Verkaufspreis: 1.500–2.500 EUR je System als Szenario

### Gewerblicher Ergänzungsmarkt

- kleine Produzenten, Direktvermarkter, Zierpflanzenbetriebe und Bildungsanlagen
- amtliche Statistiken erfassen überwiegend deutlich größere beziehungsweise anders abgegrenzte Betriebe
- daher zunächst nur als Größenordnung und Rekrutierungspool, nicht als berechneter SAM

## Verifizierte Ausgangsdaten

| Eingangsgröße | Wert | Einordnung | Quelle |
|---|---:|---|---|
| Privathaushalte Deutschland 2025 | 41,126 Mio. | amtlicher Fakt | [Destatis](https://www.destatis.de/DE/Themen/Gesellschaft-Umwelt/Bevoelkerung/Haushalte-Familien/Tabellen/1-1-privathaushalte-haushaltsmitglieder.html) |
| Haushalte mit Garten in Deutschland | 60 % | repräsentative Befragung; Garten schließt Klein-/Schrebergärten ein | [KfW Research](https://www.kfw.de/%C3%9Cber-die-KfW/Newsroom/Aktuelles/Pressemitteilungen-Details_897472.html) |
| Zahl der Gärten in Deutschland | 17,2 Mio. | KfW-Hochrechnung | [KfW Research](https://www.kfw.de/%C3%9Cber-die-KfW/Newsroom/Aktuelles/Pressemitteilungen-Details_897472.html) |
| Privathaushalte Österreich 2025 | 4,182 Mio. | amtlicher Fakt | [Statistik Austria](https://www.statistik.at/statistiken/bevoelkerung-und-soziales/bevoelkerung/familien-haushalte-lebensformen/privathaushalte) |
| Privathaushalte Schweiz | rund 4,0 Mio. | amtliche, gerundete Angabe; Datenjahr der Publikation älter als 2025 | [Bundesamt für Statistik](https://www.bfs.admin.ch/bfsstatic/dam/assets/30489004/master) |
| Deutscher Gartenmarkt 2025 | 19,7 Mrd. EUR | breiter Gesamtmarkt, kein Gewächshaus- oder Automationsumsatz | [Industrieverband Garten](https://ivg.org/der-gartenmarkt/aktuelle-marktzahlen/) |
| Online-Umsatz deutscher Gartenmarkt 2025 | 1,28 Mrd. EUR | breiter Gesamtmarkt; Online-Anteil 6,5 % | [Industrieverband Garten](https://ivg.org/der-gartenmarkt/aktuelle-marktzahlen/) |

Der breite Gartenmarkt belegt wirtschaftliches Umfeld und Vertriebskanal, ist aber **kein geeigneter Nenner**, um den Gewächshausautomationsmarkt prozentual abzuleiten.

## Private Bottom-up-Modellierung

### Schritt 1: DACH-Gartenproxy

Für Österreich und die Schweiz fehlt bislang eine vergleichbare aktuelle Gartenbestandszahl. Als reine Proxy-Annahme wird deshalb die deutsche Zahl von 17,2 Mio. Gärten proportional zur Zahl der Haushalte hochgerechnet:

```text
DACH-Gartenproxy = 17,2 Mio. × (41,126 + 4,182 + 4,0) / 41,126
                  = 20,622 Mio. Gärten
```

Diese Hochrechnung unterstellt für Österreich und die Schweiz dieselbe Zahl von Gärten je Haushalt wie für Deutschland. Das ist unbestätigt und muss ersetzt werden, sobald nationale Daten verfügbar sind.

### Schritt 2: Szenarien

| Szenario | Gärten mit Gewächshaus* | Davon passend/premium* | Potenziell geeigneter Bestand | Jährliche Kaufquote* | Jährliche Systeme | Preis je System* | Jährlicher Hardware-Umsatz |
|---|---:|---:|---:|---:|---:|---:|---:|
| Eng | 2 % | 5 % | 20.622 | 5 % | 1.031 | 1.500 EUR | 1,55 Mio. EUR |
| Basis | 5 % | 10 % | 103.110 | 7 % | 7.218 | 2.000 EUR | 14,44 Mio. EUR |
| Weit | 8 % | 20 % | 329.952 | 10 % | 32.995 | 2.500 EUR | 82,49 Mio. EUR |

\* Nicht verifizierte Modellannahme.

Formeln:

```text
Geeigneter Bestand = DACH-Gartenproxy × Gewächshausquote × Passungsquote
Jährliche Systeme  = geeigneter Bestand × jährliche Kaufquote
Hardware-Umsatz    = jährliche Systeme × durchschnittlicher Systempreis
```

## Interpretation

### Was das Modell zeigt

- Bereits kleine Änderungen der Gewächshaus- und Passungsquote verändern das Ergebnis stark.
- Das Basisszenario von 14,44 Mio. EUR Jahresumsatz ist rechnerisch korrekt, aber wegen der unbelegten Quoten **niedrig belastbar**.
- Der private Markt kann plausibel groß genug für ein spezialisiertes kleines Unternehmen sein; die aktuelle Evidenz beweist das noch nicht.
- Der breite Gartenmarkt von 19,7 Mrd. EUR darf nicht als TAM bezeichnet werden. Greenhouse Assistant adressiert nur einen sehr kleinen, derzeit unbekannten Teil davon.

### Sensitivität

Die zwei stärksten Unsicherheiten wirken multiplikativ:

- Halbiert sich die angenommene Gewächshausquote, halbieren sich Bestand, Stückzahl und Umsatz.
- Halbiert sich die Passungsquote, gilt dasselbe.
- Beide Halbierungen gemeinsam reduzieren das Ergebnis auf ein Viertel.

Die Preisannahme verändert nur den Umsatz, nicht die Zahl potenzieller Käufer. Für die Marktvalidierung sind Gewächshausbestand und Passungsquote daher wichtiger als eine frühzeitige Feinoptimierung des Verkaufspreises.

## Gewerblicher Markt: belegte Randgrößen

Die verfügbaren Statistiken zeigen einen realen, aber nicht sauber auf 10–100 m² eingrenzbaren gewerblichen Markt:

| Region | Verifizierte Größe | Einschränkung |
|---|---|---|
| Deutschland | 2020 gab es 5.642 spezialisierte Gartenbaubetriebe. Rund 85 % von etwa 2.700 spezialisierten Zierpflanzenbetrieben und rund 46 % von etwa 740 spezialisierten Gemüsebetrieben produzierten überwiegend unter Glas. | „Überwiegend unter Glas“ sagt nichts über eine Zielgröße von 10–100 m²; Betriebe können bereits professionelle Systeme einsetzen. |
| Deutschland | 1.650 Betriebe bauten 2020 Gemüse auf knapp 1.300 ha unter hohen begehbaren Schutzabdeckungen an. | Andere Definition als „spezialisierte Betriebe“; Werte dürfen wegen möglicher Überschneidung nicht addiert werden. |
| Österreich | 2020 wurden 1.034 Gartenbaubetriebe und 529,88 ha Gewächshaus-/Folientunnelfläche erfasst; 684 Betriebe hatten insgesamt weniger als 1 ha gärtnerische Nutzfläche. | Nicht alle Betriebe besitzen Gewächshäuser; „unter 1 ha“ liegt weit über der Produktzielgröße. |
| Schweiz | 2023 bestanden rund 460 ha Gemüse-Gewächshausfläche; insgesamt gab es 803 spezialisierte Gemüsebaubetriebe. | Keine öffentlich belegte Zahl kleiner Gewächshausbetriebe; Zierpflanzenbetriebe fehlen in dieser Quelle. |

Diese Daten reichen aus, um gewerbliche Interviewpartner und Pilotkunden zu suchen. Für eine Umsatzschätzung reichen sie nicht aus.

## SOM als Kapazitätsszenario

Vor Kenntnis von Vertriebskanal, Installationszeit und Abschlussquote ist ein Marktanteils-SOM nicht seriös. Als operative Planungsgröße können zunächst drei Kapazitätsszenarien dienen:

| Auslieferungen pro Jahr* | Hardware-Umsatz bei 2.000 EUR* |
|---:|---:|
| 50 | 100.000 EUR |
| 150 | 300.000 EUR |
| 300 | 600.000 EUR |

\* Planungsannahmen, keine Marktprognose. Serviceumsätze, Umsatzsteuer, Rabatte, Installation und Hardwarekosten sind nicht berücksichtigt.

## Höchste Validierungsprioritäten

1. Jährliche Stückzahlen und installierte Basis von drei bis fünf Premium-Gewächshausherstellern oder Händlern ermitteln.
2. In einer qualifizierten Befragung feststellen, welcher Anteil der Besitzer tatsächlich ein Gewächshaus besitzt, mehr als etwa 5.000 EUR investiert hat und regelmäßig abwesend ist.
3. In Interviews die Passung mit konkreten Verhaltensdaten prüfen: Schäden, Kontrollfahrten, heutige Ausgaben und bereits gekaufte Automationskomponenten.
4. Abschlussquote bei zwei bis drei konkreten Preis-/Leistungspaketen testen.
5. Für den gewerblichen Markt Betriebe nach realer Gewächshausfläche, vorhandener Steuerung und jährlichem Verlust-/Arbeitszeitpotenzial segmentieren.

Bis diese Punkte geklärt sind, sollte das Basisszenario nicht für Finanzierungs- oder Investitionsentscheidungen verwendet werden.
