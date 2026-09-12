# Marktvergleich möglicher Produktgrenzen

## Entscheidungsfrage

Der Prototyp kann als Controller, als standardisiertes Komponentenpaket oder als betriebsfertig installiertes System vermarktet werden. Diese Varianten sind keine bloßen Verpackungsoptionen: Zielkunde, Wettbewerb, Preis, Haftung, Support und Skalierbarkeit ändern sich grundlegend.

Alle Preisbereiche in diesem Dokument sind Arbeitshypothesen aus sichtbaren Wettbewerbs- und Komponentenpreisen. Sie sind weder validierte Zahlungsbereitschaft noch Angebotsempfehlungen.

## Drei Produktgrenzen

| Kriterium | A – Controller/DIY-Kit | B – standardisiertes Einzonen-System | C – betriebsfertige Installation |
|---|---|---|---|
| typischer Lieferumfang | 12/24-VDC-Controller und offene Software; Kunde wählt Komponenten | Controller und Plug-and-play-Schnittstellen; geprüfte Komponenten wahlweise mitgeliefert oder transparent extern beschafft | vollständiges System einschließlich Aktoren, Netzanschluss, Verkabelung, Montage und Inbetriebnahme |
| primärer Kunde | technisch versierter Hobbyanwender / Maker | Premium-Hobbykunde oder kleiner Betrieb mit Elektriker-/Montagezugang | zahlungskräftiger Privatkunde oder kleiner Gewerbebetrieb mit Wunsch nach Gesamtverantwortung |
| nächster Wettbewerb | Home Assistant, ESPHome, OpenSprinkler und Eigenbau | Harvst, GrowControl/NIDO als angrenzende Produkte, Trellis als früher Marktindikator | regionale Gewächshaustechnik- und Automationsintegratoren |
| plausible interne Preishypothese | etwa 700–1.500 EUR | etwa 1.700–3.000 EUR zuzüglich klar abgegrenzter Montage | wahrscheinlich über 3.000 EUR, stark objektabhängig |
| stärkster Vorteil | niedriger Preis, einfacher Versand | klare Differenzierung durch Außenwetter, Fensterlogik und Standardisierung | größter Kundennutzen und höchste Systemverantwortung |
| größter Nachteil | Kunde trägt genau den Integrationsaufwand, den das Produkt lösen soll | Kompatibilität und Installationsgrenze müssen sehr sauber definiert sein | hoher Vor-Ort-Aufwand, regionale Skalierung, Gewährleistungs- und Haftungsrisiko |
| Preistransparenz | hoch | hoch bis mittel | niedrig, sobald jedes Objekt anders geplant wird |
| Skalierbarkeit | hoch, aber supportanfällig | potenziell hoch bei wenigen geprüften Varianten | zunächst niedrig |
| Marktfit des Prototyps | technisch möglich und als Community-Einstieg sinnvoll, aber supportanfällig | beste Übereinstimmung mit der identifizierten Marktlücke | widerspricht dem bevorzugten reinen Onlinehandel |

## Option A – Controller oder DIY-Kit

### Marktchance

Ein Preis im bisherigen Zielkorridor von 700–1.500 EUR wird am ehesten erreichbar, wenn Wetterstation, Antriebe, Leistungsstufen und Montage nicht vollständig enthalten sind. Der Kaufweg kann online und über Versand funktionieren.

### Strategisches Problem

Der Käufer muss kompatible Sensoren, Motoren und Mechanik selbst zusammenführen. Damit bleibt ein großer Teil des beobachteten Problems bestehen. Ein 12/24-VDC-Controller und ein externes zertifiziertes Netzteil reduzieren zwar die Netzspannungsgrenze, beseitigen aber nicht die Integrations- und Supportfrage.

### Eignung

Sinnvoll als:

- Entwickler-/Pilotversion für sehr technische Nutzer,
- klar gekennzeichnetes Integrationsprodukt,
- späteres OEM-Modul für Partner.

Weniger geeignet als primäres Premium-Hobbyangebot.

## Option B – Standardisiertes Einzonen-System

### Marktchance

Diese Produktgrenze passt am besten zur bisher erkannten Lücke. Das System löst nicht nur Software, sondern auch die kritische Komponentenauswahl. Gleichzeitig bleibt die Anlage kleiner und standardisierter als professionelle Projektsteuerung.

### Empfohlene Abgrenzung

Im festen Kernumfang:

- 12/24-VDC-Controller mit lokaler Bedienung,
- kein zwingend integriertes Netzgerät; definierte zertifizierte externe Netzgeräte,
- Innenfühler für Temperatur und Feuchte,
- Außenmessung für Temperatur, Wind und Regen,
- zwei definierte Motorachsen beziehungsweise geprüfte Motorinterfaces,
- Heizung als Freigabekontakt,
- ein Ventilatorausgang,
- vorkonfigurierte Schutzlogik,
- Ereignisprotokoll und Fernzugriff,
- verpolungssicherer Plug-and-play-Kabel-/Steckverbinderumfang,
- routerähnliche Inbetriebnahme drahtloser Erweiterungen,
- dokumentierte kompatible Antriebe und Installationsvoraussetzungen.

Objektspezifisch beziehungsweise optional:

- mechanische Anpassung der Fenster,
- Netzanschluss und Arbeiten an 230 V,
- zusätzliche Sensoren/Aktoren,
- zweite Zone,
- Bewässerung und Beschattung.

### Kritische Bedingung

„Standardisiert“ darf nicht nur für die Software gelten. Auch Kabelwege, Steckverbinder, Motorleistung, Endlagen, Schutzorgane und Inbetriebnahme müssen auf wenige geprüfte Kombinationen reduziert werden. Sonst wird Option B faktisch zu einem schlecht kalkulierten Projektgeschäft.

## Option C – Schlüsselfertiges System

### Marktchance

Ein vollständiges Angebot beseitigt Kundensorgen zu Auswahl, Installation und Verantwortung. Es erlaubt einen höheren Auftragswert und ist für nichttechnische Premiumkunden wahrscheinlich am verständlichsten.

### Strategisches Problem

Jedes abweichende Fenster, Fundament, Kabelweg oder vorhandene Heizgerät erzeugt Planungs- und Vor-Ort-Aufwand. Damit nähert sich das Geschäftsmodell den professionellen Integratoren. Ohne Montageprozess, regionale Partner, dokumentierte Abnahme und Rückstellung für Nacharbeit ist diese Variante nicht skalierbar.

### Eignung

Sinnvoll als:

- lokal begrenztes Pilotangebot,
- Premiumoption über einen Gewächshaushersteller,
- Lernkanal zur Entwicklung standardisierter Kits.

Nicht sinnvoll als sofortiges flächendeckendes DACH-Versprechen.

## Empfehlung

### Produktarchitektur auf Option B ausrichten

Das marktfähige Ziel sollte ein **offenes, standardisiertes Plug-and-play-System** sein. Der eigene Kern sind Controller, robuste Schnittstellen, Regelsoftware, Dokumentation und geprüfte Kompatibilität. Wetterstation, Sensoren und zertifiziertes Netzgerät können als Paket angeboten oder anhand einer exakten Liste transparent extern beschafft werden. „Bring your own“ erhält nur für geprüfte Fabrikate vollen Herstellersupport.

### Markteintritt stufenweise gestalten

1. Den bestehenden Prototyp intern auf den festen B-Umfang reduzieren.
2. Kompatibilitätsmatrix für wenige Antriebe, Lüfter und Heizungsinterfaces erstellen.
3. Herstellkosten und Montagezeit getrennt für Kernpaket und Objektarbeit erfassen.
4. Einen Online-Konfigurator und Installationscheck vor dem Verkauf entwerfen.
5. Das versendbare B-Paket einschließlich Dokumentation und Selbsttest entwickeln.
6. Option A als Community-/Maker-Pfad nur mit klarer Support- und Lizenzgrenze anbieten.

Dieser Pfad nutzt schlüsselfertige Pilotinstallationen als Lerninstrument, ohne das langfristige Geschäftsmodell auf individuelles Projektgeschäft festzulegen.

## Empfohlene Paketlogik

Die Namen sind Platzhalter; entscheidend ist die funktionale Trennung.

### Schutzkern

- eine Zone,
- Innenklima plus Außenwetter,
- zwei Lüftungsmotoren,
- Heizungssignal,
- vier Schutzmodi,
- lokale Bedienung, Alarm und Historie.

### Klima-Erweiterung

- zusätzlicher Umluft-/Abluftkanal,
- weitere Innenfühler,
- Feuchte-/Kondensationsstrategie,
- optional Beschattung.

### Wasser-Erweiterung

- Bodenfeuchte,
- Ventile/Pumpe,
- Durchfluss- oder Drucküberwachung,
- Leck-/Trockenlaufalarm.

### Mehrzonen-Erweiterung

- zweite Zone oder zweites Gewächshaus,
- klar getrennte Sensor-/Aktorzuordnung,
- gemeinsame Wetterstation,
- definierte Prioritäten bei gemeinsam genutzten Geräten.

Erdreichwärmetauscher und KI bleiben außerhalb dieser ersten Paketfamilie.

## Entscheidungskriterien für die Produktgrenze

Option B ist nur dann tragfähig, wenn nach technischer Inventur folgende Bedingungen plausibel sind:

- mindestens 80 % der Zielinstallationen lassen sich mit wenigen dokumentierten Varianten abdecken,
- die objektabhängige Arbeit kann vor Bestellung anhand von Fotos und Maßen bestimmt werden,
- Installations- und Supportgrenzen sind für Kunden eindeutig,
- ein Fehler an Internet oder optionalem Funk beeinträchtigt den Schutzkern nicht,
- der Deckungsbeitrag bleibt nach realistisch bewerteter Einrichtungs- und Supportzeit positiv,
- Konformitäts- und Dokumentationsanforderungen werden von Anfang an in die Architektur aufgenommen.

Die 80-%-Schwelle ist eine interne Arbeitsregel, keine aus einer Marktstudie abgeleitete Kennzahl.

## Noch nicht entscheidbar

Ohne technische Inventur und Stückliste kann die Desk Research nicht klären:

- ob der empfohlene B-Umfang mit der vorhandenen Hardware wirtschaftlich erreichbar ist,
- welche Antriebsvarianten ohne individuelle Konstruktion unterstützt werden können,
- welche externen 12/24-V-Netzgeräte offiziell unterstützt und gegebenenfalls mitverkauft werden,
- welcher Endpreis nach Montage, Garantie und Support wirtschaftlich ist.

Diese Fragen benötigen keine Kundenrekrutierung, aber konkrete Prototyp-, Bauteil- und Kostendaten.
