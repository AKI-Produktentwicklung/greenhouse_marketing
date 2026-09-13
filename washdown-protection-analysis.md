# Wasch- und Strahlwasserschutz als Produktpositionierung

## Kurzfazit

Die Recherche stützt die Beobachtung, dass viele naheliegende Controller für die tatsächliche Nassreinigung eines Gewächshauses ungeeignet oder zumindest nicht nachweislich geeignet sind. Das eröffnet eine belastbare Differenzierungsmöglichkeit:

> Greenhouse Assistant wird nicht nur „für feuchte Räume“, sondern als dokumentiert waschbares Feldsystem entwickelt.

Das ist noch kein Nachweis, dass genügend Kunden dafür mehr bezahlen. Es ist aber ein deutlich konkreteres und überprüfbareres Produktmerkmal als allgemeine Aussagen wie „robust“ oder „für Gewächshäuser geeignet“.

## Was die Herstellerangaben belegen

| Produkt / Quelle | Dokumentierte Aussage | Einordnung für Reinigung |
|---|---|---|
| GrowControl GrowBase | IP42 | Schutz gegen Tropf-/Sprühwasser in begrenzter Richtung; kein Wasserstrahl- oder Hochdrucknachweis. |
| NIDO ONE V2 | Gerät von Spritzwasser fernhalten und nur mit feuchtem Tuch reinigen | Für direktes Abspritzen ausdrücklich ungeeignet. |
| Home Assistant Green | nur Innenraum, trocken und nicht kondensierend | Als Geschäftsmodellvergleich brauchbar, als Gewächshaus-Feldgerät ungeeignet. |
| OpenSprinkler | Hersteller-Supportforum: Gehäuse nicht wasserdicht, für außen zusätzliches Schutzgehäuse nötig | Das Produkt delegiert den Umgebungsschutz an die Installation. |
| Harvst WaterMate | externes wasserdichtes 12-V-Netzteil; kein gefundener Schutzartnachweis für die komplette Steuereinheit | Einzelne Komponente geschützt, Waschbarkeit des Gesamtsystems nicht belegt. |
| Senmatic LCC1 | IP65, 0–95 % rF ohne Kondensation | Gegen Wasserstrahlen geprüft; kein Nachweis für Hochdruck-/Heißwasserreinigung. |

Die Stichprobe ist nicht vollständig. „Keine Schutzart gefunden“ bedeutet nicht „nicht geschützt“, sondern nur, dass aus den geprüften Primärquellen kein belastbares Produktversprechen ableitbar ist.

Eine plausible Erklärung ist, dass professionelle Anbieter den Controller in einem geschützten Bereich oder zusätzlichen Schaltschrank montieren und den Umgebungsschutz damit an Planung und Installation delegieren. Das ist nicht automatisch schlechte Technik, passt aber schlecht zu einem online verkauften Nachrüstprodukt, dessen Käufer eine eindeutige und vollständige Aussage erwartet.

## Gartenschlauch und Hochdruckreiniger sind zwei verschiedene Anforderungen

Nach der IP-Systematik bezeichnet die zweite Ziffer:

- IPX5: Schutz gegen Wasserstrahlen,
- IPX6: Schutz gegen starke Wasserstrahlen,
- IPX9 beziehungsweise IP69/IP69K: Schutz bei Hochdruck-/Heißwasser-Strahlreinigung unter definierten Prüfbedingungen.

Ein IP66-Gehäuse ist daher nicht automatisch hochdruckreinigerfest. Umgekehrt erlaubt auch IP69 keine beliebige Reinigung aus jeder Entfernung mit jedem Druck, Reinigungsmittel und jeder Temperatur. Das spätere Produktversprechen muss die zulässigen Bedingungen ausdrücklich nennen.

## Die Schutzart gehört dem vollständigen System

Ein gutes Gehäuse allein reicht nicht. Für ein waschbares Feldsystem müssen gemeinsam betrachtet und geprüft werden:

- Gehäuse und Deckeldichtung,
- Display, Tasten und sonstige Bedienöffnungen,
- Steckverbinder im gesteckten Zustand,
- Schutzkappen unbenutzter Anschlüsse,
- Kabel und Kabelverschraubungen,
- Sensoren und Aktoren,
- Druckausgleich gegen Kondensation,
- Montageausrichtung und Wasserablauf,
- Alterung durch UV-Licht, Dünger, Pflanzenschutz- und Reinigungsmittel.

Stecker sind häufig die Schwachstelle. Industrielle M12-Steckverbinder und Sensoren sind bis IP69K erhältlich; das belegt technische Machbarkeit, nicht automatisch die Schutzart einer daraus aufgebauten Gesamtanlage.

## Empfohlene Produktgrenze

### Basisversprechen

- Controller und alle Feldanschlüsse mindestens für kräftiges Abspritzen mit einem Gartenschlauch auslegen.
- Das konkrete Ziel – beispielsweise IP66 – erst nach Prüfung der vollständigen betriebsfertigen Anordnung bewerben.
- Ungesteckte Buchsen nur mit verriegelten Schutzkappen als geschützt behandeln.
- Externes Netzgerät und 230-V-Verbindung außerhalb der Waschzone anordnen oder separat dafür qualifizieren.

### Differenzierende Premiumanforderung

- Eine Hochdruckreinigungsvariante auf IPX9/IP69-Niveau technisch und wirtschaftlich prüfen.
- Wash-down-taugliche Steckverbinder, Kabel und Sensoren als zusammenhängende Produktfamilie auswählen.
- Zulässigen Druck, Abstand, Temperatur, Winkel, Dauer und Reinigungsmittel dokumentieren.
- Reinigung als geführten Betriebsmodus vorsehen: Aktoren sichern, Alarme unterdrücken, danach Sensor-/Steckertest und Ereigniseintrag.

## Marktpositionierung

Eine mögliche verständliche Positionierung lautet:

> Der Gewächshaus-Controller, der im Gewächshaus bleiben darf, wenn gereinigt wird.

Vor einem solchen Claim ist eine Prüfung zwingend. Bis dahin sollte die interne Arbeitsformulierung „wash-down-fähiges Feldsystem“ lauten.

Die Robustheit passt besonders gut zur bisherigen Position zwischen DIY und professioneller Automatisierung:

- gegenüber DIY: weniger Schutzgehäuse-, Stecker- und Abdichtungsarbeit,
- gegenüber Consumer-/Grow-Controllern: für die reale Gewächshausumgebung qualifiziert,
- gegenüber professionellen Systemen: robuste Feldtechnik ohne individuellen Schaltschrankbau.

## Noch offene Entscheidungen

1. Was ist der reale Reinigungsfall: Gartenschlauch, Hochdruckreiniger oder beides?
2. Welche maximalen Drücke, Abstände und Wassertemperaturen sollen erlaubt sein?
3. Werden Reiniger, Dünger oder Desinfektionsmittel eingesetzt?
4. Muss der Controller selbst in der Waschzone sitzen oder kann nur ein dezentrales I/O-Modul dort verbleiben?
5. Welcher Mehrpreis entsteht für Gehäuse, Steckverbinder, Kabel, Sensoren und Prüfung?
6. Ist die gesamte Basisausführung wash-down-fähig oder entsteht eine Premiumvariante?

Die Punkte 1–4 benötigen später konkrete Prototyp- und Nutzungsangaben. Sie erfordern aktuell keine Kundenkontakte.
