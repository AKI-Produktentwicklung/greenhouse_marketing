# Online- und Open-Source-Strategie

## Kurzempfehlung

Die stärkste derzeit plausible Position ist kein steckerfertiger Klimacomputer und kein loses DIY-Board, sondern ein **offenes Plug-and-play-System für hochwertige kleine Gewächshäuser**:

- 12/24-VDC-Controller als eigener Produktkern,
- keine zwingend integrierte Netzspannungsversorgung,
- robuste, verpolungssichere Steckverbindungen,
- offiziell geprüfte Sensor-, Wetterstations-, Netzteil- und Aktorkombinationen,
- lokale Regelung ohne Cloudpflicht,
- sehr einfache Funk-Inbetriebnahme,
- transparenter Online-Kaufweg mit vollständigem Konfigurationspreis.

Diese Position ist eine strategische Hypothese. Die Desk Research zeigt passende Problem- und Produktmuster, aber noch keine validierte Nachfragegröße.

## Warum die fehlende direkte Konkurrenz ambivalent ist

Die bisher betrachteten professionellen Anbieter sind vor allem Funktions- und Robustheitsbenchmarks. Der Zielkunde vergleicht realistischerweise mit manueller Bedienung, passiven Fensteröffnern, Thermostaten, einem Home-Assistant-Eigenbau oder einem angrenzenden kleinen System wie Harvst.

Dass kein etablierter DACH-Anbieter exakt dieselbe Position besetzt, kann bedeuten:

1. Es gibt eine unbesetzte Lücke zwischen DIY und Projektanlage.
2. Die Nachfrage ist zu klein, zu saisonal oder zu supportintensiv.
3. Die individuelle Gewächshausmechanik verhindert bisher ein skalierbares Paket.
4. Käufer lösen das Problem ausreichend gut mit günstigeren Einzelprodukten.

Die Existenz von Harvst, Trellis, OpenSprinkler sowie umfangreichen DIY-Lösungen stützt die erste Erklärung, entscheidet aber nicht zwischen diesen Möglichkeiten.

## Empfohlenes Erlösmodell

### Eigener bezahlter Wert

- Controller und robuste I/O-/Funk-Schnittstellen
- Plug-and-play-Kabel und Adapter
- getestete Kompatibilität
- stabile Releases, Updates und Wiederherstellung
- vorkonfigurierte Sicherheitslogik
- Dokumentation, Diagnose und klar definierter Support
- optionale Komfort- oder Fernzugriffsdienste ohne Cloudpflicht für den Grundbetrieb

### Transparentes Fremdzubehör

Bei Wetterstation, Standardsensoren und zertifiziertem Netzteil ist keine Marge um jeden Preis notwendig. Transparenz kann Vertrauen erzeugen und Lager-/Gewährleistungsrisiken senken. Sie funktioniert aber nur mit drei Supportklassen:

1. **Offiziell unterstützt:** exakt getestetes Fabrikat und Version, voller Support.
2. **Community/experimentell:** dokumentierte Schnittstelle, keine Funktionsgarantie.
3. **Nicht unterstützt:** bekannte elektrische, mechanische oder qualitative Unverträglichkeit.

Eine Wetterstation darf nicht allein wegen Protokollkompatibilität freigegeben werden. Gehäuse, UV-/Feuchtebeständigkeit, Befestigung, Kabel, Ersatzteilverfügbarkeit und Messverhalten gehören in dieselbe Prüfung.

## Open-Source-Varianten

| Variante | Vorteil | Hauptrisiko | Vorläufige Eignung |
|---|---|---|---|
| vollständig Open Source | maximales Vertrauen und DIY-Reichweite | Nachbauten, Variantenfragmentierung und hoher Community-Support | möglich, aber Lizenz-/Markenstrategie zuerst klären |
| Open Core | Community-Version offen; produktisierte Funktionen und Dienste differenziert | Grenze kann künstlich oder unfair wirken | prüfenswert, wenn bezahlter Mehrwert klar ist |
| offene Schnittstellen und Integrationen | Fremdkomponenten und Home Assistant möglich, Kernsoftware bleibt kontrolliert | geringerer Community-Sog | risikoärmster Start |

OpenSprinkler belegt das Muster „offene Software/Hardware plus verkaufte Spezialhardware und Zubehör“. Home Assistant belegt „freie Software plus offizielle Plug-and-play-Hardware und optionale Dienste“. Beide sind Analogien, kein Nachweis für Gewächshausnachfrage.

## Was Online-first zwingend erfordert

Ein reiner Onlinehandel verschiebt Beratung in das Produkt und die Website. Vor dem Verkauf müssen daher mindestens verfügbar sein:

- Konfigurator mit vollständig sichtbarem Warenkorb,
- Foto-/Maß-basierter Installationscheck,
- Kompatibilitätsmatrix,
- verständliche Installationsgrenzen für Mechanik und Netzspannung,
- vollständige technische Dokumentation und kurze Aufbauvideos,
- automatischer Anschluss- und Gerätetest,
- Ferndiagnose und exportierbares Ereignisprotokoll,
- Ersatzteil- und Updateversprechen,
- klare Rückgabe-, Garantie- und Supportbedingungen.

Wissensartikel, EWT-/Lüftungsrechner und Erfahrungsberichte können als organischer Vertriebskanal wirken. Ihr Wert liegt nicht nur in Reichweite: Sie qualifizieren Käufer und reduzieren falsche Erwartungen. Ob damit genügend DACH-Kunden wirtschaftlich gewonnen werden, bleibt zu modellieren.

## Nächste Marktanalyse ohne Kontakte

1. Drei reale Beispielkonfigurationen für 10, 30 und 100 m² mit vollständigem Endpreis bilden.
2. Die Komponenten nach Marge, Supportlast und Differenzierungswert klassifizieren.
3. Open-Source-, Open-Core- und Open-API-Modell wirtschaftlich und lizenzrechtlich vergleichen.
4. Einen Online-Konfigurator als Entscheidungsbaum entwerfen und alle Fälle markieren, die individuelle Beratung auslösen.
5. Für Harvst, OpenSprinkler und Home Assistant Kaufweg, Dokumentation, Supportgrenzen, Updates und Zubehörlogik systematisch vergleichen.

