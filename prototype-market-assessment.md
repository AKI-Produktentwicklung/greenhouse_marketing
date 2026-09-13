# Marktbasierte Standortbestimmung des Prototyps

## Kurzfazit

Der vorhandene Greenhouse-Assistant-Prototyp ist **kein technischer Demonstrator mehr**, sondern ein seit drei Jahren real betriebenes, zweizoniges Schutz- und Klimasystem. Er besetzt funktional bereits die gesuchte Brücke: lokale Steuerung, Außenwetter, vier motorische Lüftungen, Heizung, Feuchtefunktionen, manuelle Bedienung und Fernzugriff für kleine Gewächshäuser.

Die wichtigste marktbasierte Änderung ist deshalb weder das Hinzufügen noch das Entfernen bereits funktionierender Regeln. Der vorhandene Funktionskern sollte in wenige klar bepreisbare, nachweisbar robuste Lieferpakete übersetzt werden:

> Nachrüstbares, lokal autonomes und gartenschlauchtaugliches Schutz- und Klimasystem für ein oder zwei hochwertige kleine Gewächshäuser – online kaufbar, mit aktiver Lüftung, Außenwetter und verständlichem Betriebszustand.

Der Prototyp liefert starke Felderfahrung. Für ein verkaufsfähiges Produkt fehlen vor allem standardisierter Lieferumfang, dokumentierte Prüf- und Fehlerfälle, Installationsgrenze, Konformitätsplanung und eine Stückkostenrechnung je Paket.

## Evidenzbasis und Grenzen

### Vom Gründer bereitgestellte beziehungsweise intern dokumentierte Informationen

- Alle auf den bereitgestellten Screenshots dargestellten Funktionen laufen nach Gründerangabe seit drei Jahren im realen Gewächshausbetrieb.
- M01/M02 steuern Zone beziehungsweise Gewächshaus 1, M03/M04 Zone beziehungsweise Gewächshaus 2.
- Der aufgebaute Controller samt Anschlüssen ist nach Gründerangabe IP67; Gartenschlauchreinigung ist zugesagtes Produktmerkmal.
- Die Fotos und Screenshots zeigen Außenwetter, Innenklima, vier Motorkanäle, Heizung, Umluft, Befeuchtung, Erdreichwärmetauscher, lokale Bedienung sowie Sturm-, Wind-, Frost-, Hitze-, Feuchte- und Kondensationslogik.

Diese Angaben sind wertvolle Produktinformationen, aber keine unabhängig geprüften Leistungs-, Sicherheits- oder Dauerhaltbarkeitsnachweise.

### Verifizierte Marktevidenz

- Professionelle Systeme von Ridder, Senmatic, RAM und MABEG verbinden bereits Klima, Außenwetter und Schutzfunktionen. Sturm-, Frost- und Regenschutz allein sind daher keine einzigartige Erfindung.
- Einfach kaufbare Produkte um etwa 1.000–1.500 EUR konzentrieren sich häufig auf Indoor-Klima oder Fertigation und belegen keine vollständige Kombination aus Außenwetter und sicherer Fenstersteuerung.
- Schon unvollständige Vergleichswarenkörbe liegen öffentlich bei rund 1.700 EUR beziehungsweise 2.600 USD, noch ohne funktionsgleichen Installationsumfang.
- Die qualitative Voice-of-Customer-Stichprobe stützt wiederholt Überhitzung bei Abwesenheit, den Konflikt zwischen Lüftung und Sturm, Integrationsaufwand sowie Sensor-/Funkprobleme. Sie belegt weder Häufigkeit noch Zahlungsbereitschaft.

## Position im Wettbewerbsfeld

| Marktklasse | Typisches Angebot | Stärke | Schwäche | Position des Prototyps |
|---|---|---|---|---|
| einfache Einzelgeräte | passive Öffner, Thermostate, Timer, Smart Plugs | günstig und leicht erhältlich | Geräte arbeiten unkoordiniert; wenig Diagnose und Außenwetter | funktional klar überlegen |
| DIY / Smart Home | Home Assistant, ESP32, Node-RED, Funk-Sensoren | flexibel und preiswert bei eigener Arbeitszeit | hoher Integrations- und Wartungsaufwand; keine Systemverantwortung | ähnliche technische Flexibilität, aber Chance auf standardisiertes Gesamtsystem |
| kompakte Grow-/Fertigationscontroller | GrowControl, NIDO, TrolMaster | kaufbar, App, Sensorik, modulare Erweiterung | meist Indoor-/Bewässerungsfokus; klassische Gewächshausmotorik nicht der Kern | Außenwetter und Lüftungsmotorik sind ein relevanter Vorteil |
| professionelle Gewächshaussteuerung | Ridder, Senmatic, RAM, MABEG, Priva | bewährte Funktionsbreite, Projektierung und Service | für kleine private Häuser komplex, schwer vergleichbar und meist ohne öffentlichen Komplettpreis | funktional darunter, bei Einfachheit und Nachrüstung potenziell attraktiver |

### Strategische Position

Der Prototyp steht **zwischen DIY und professioneller Projektanlage**. Genau dort ist eine plausible Lücke erkennbar. Sie ist jedoch schmaler als ursprünglich angenommen: Mehrere professionelle Anbieter besitzen lokale und wetterabhängige Schutzfunktionen bereits. Differenzierung muss aus der Kombination von Zielgröße, einfacher Nachrüstung, transparentem Paket, lokaler Robustheit und verständlicher Bedienung entstehen.

## Funktions-Fit des aktuellen Konzepts

Die Bewertung „hoch/mittel/niedrig“ ist eine strategische Einschätzung aus Wettbewerbs- und Problemsignalen, keine gemessene Nachfrage.

| Merkmal des Prototyps | Marktfit | Begründung | Empfehlung |
|---|---|---|---|
| lokale Autonomie | hoch | Grundvoraussetzung für Schutz bei Internetstörung; von einigen Wettbewerbern ebenfalls erfüllt | zwingend beibehalten und nachweisbar testen |
| Außenwetter mit Wind und Regen | hoch | löst den dokumentierten Zielkonflikt zwischen Lüftung, Hitze und Sturm | in den Kernumfang aufnehmen |
| motorische Fenstersteuerung | hoch | klare Abgrenzung zu Indoor-Controllern und passiven Öffnern | Kernfunktion, aber mit Positions-/Fehlerdiagnose |
| Frost- und Überhitzungsschutz | hoch | häufig verständlicher direkter Nutzen | beibehalten; Schutzzustände sichtbar machen |
| manuelle Tasten am Gerät | hoch | wichtig bei Einrichtung, Wartung und Kommunikationsausfall | beibehalten; sichere Prioritätslogik definieren |
| Web-/Smartphone-Zugriff | mittel bis hoch | marktübliche Erwartung und nützlich bei Abwesenheit, aber kein Alleinstellungsmerkmal | beibehalten, nicht als Hauptbotschaft verwenden |
| Touchscreen am Gerät | mittel | lokale Transparenz ist wichtig; ein großer Touchscreen erhöht Kosten und Fehlerfläche | einfache Statusanzeige plus robuste Tasten zunächst bevorzugen |
| zwei Zonen im Controller | mittel bis hoch | die vier Motorkanäle und Zonenzuordnung sind bereits drei Jahre in Betrieb; zwei Zonen erhöhen den adressierbaren Anlagenumfang ohne neue Controllerplattform | Controller standardmäßig zweizonenfähig lassen; Ein- und Zweizonenpaket über Sensoren, Antriebe und Kabel unterscheiden |
| bis zu acht Sensoren je Sensortyp | nicht als Marktbedarf belegt | die Zahl ist durch die Ecowitt-Plattform technisch nachvollziehbar, aber weiterhin kein belegter Kundenbedarf; alternative Fabrikate müssen auch mechanische und klimatische Qualitätsanforderungen erfüllen | Kapazität als Erweiterbarkeit behandeln, nicht als Basispaket; GW2001/GW3001 und Alternativen anhand einer Qualitäts- und Kompatibilitätsmatrix prüfen |
| Blattfeuchtesensorik | mittel bis niedrig | kann Krankheitsrisiko unterstützen, ist in der Stichprobe kein dominanter Kaufgrund | optionale spätere Erweiterung |
| Bodenfeuchte/Bewässerung | mittel | reales Problem und starker bestehender Markt, würde den Startumfang jedoch verbreitern | Schnittstelle vorsehen, Regelung erst nach Klimakern |
| Erdreichwärmetauscher | niedrig für den Markteintritt | derzeit keine belastbare Nachfrageevidenz; erfordert Bauarbeit und erweitert Haftung/Projektierung | aus dem Kernprodukt entfernen und als separates Innovationsmodul behandeln |
| Wetterprognose und KI | niedrig für den Markteintritt | Wettbewerber bieten Prognosen bereits; Kernprobleme benötigen zunächst robuste aktuelle Messung und Regeln | zurückstellen, bis lokale Schutzlogik und Datenqualität bewiesen sind |

## Empfohlene erste Paketfamilie

Dies ist eine marktbasierte Empfehlung, noch keine Produktentscheidung.

### Gemeinsamer Controllerkern

- ein IP67-Controller samt Anschlüssen,
- 12/24-VDC-Versorgung und vorgesehene 12-V-Speisung der Wetterstation,
- vier Motorkanäle für zwei Zonen,
- lokale Bedienung und autonomer Betrieb,
- vorbereitete Schnittstellen für alle bereits real betriebenen Funktionen.

### Referenzpaket: eine Zone / ein Gewächshaus

- lokale Steuerung ohne Internet,
- ein kombinierter Innenfühler für Temperatur und Feuchte,
- verkabelte oder anderweitig nachweisbar zuverlässige Außenmessung für Temperatur, Wind und Regen,
- Steuerung von zwei motorischen Lüftungen,
- Freigabekontakt für eine vorhandene Heizung,
- ein Ausgang für Umluft- oder Abluftventilator,
- Sturm-, Regen-, Frost- und Überhitzungslogik,
- manuelle lokale Bedienung,
- klarer Normal-, Warn-, Fehler- und Handbetrieb,
- Ereignisprotokoll, Alarme und optionaler Fernzugriff.

### Zweizonenpaket

- derselbe Controllerkern,
- zwei Innenklimasensoren,
- vier motorische Lüftungen,
- gemeinsame Wetterstation,
- erweiterter Standard-Kabelsatz.

### Optionen statt verpflichtender Grundausstattung

- weitere Innenfühler,
- Bodenfeuchte und Bewässerung,
- Beschattung,
- Blattfeuchte,
- Befeuchtung/Entfeuchtung,
- Erdreichwärmetauscher,
- Prognose- und Optimierungsfunktionen.

Diese Aufteilung nutzt den vorhandenen Prototyp, ohne jeden Kunden zum Kauf sämtlicher Feldkomponenten zu zwingen. Standardisiert werden vor allem Lieferumfang, Kabelsatz und unterstützte Einbausituationen – nicht die bereits funktionierende Regelung künstlich entfernt.

## Konkrete Änderungen am bisherigen Konzept

### 1. Produktbotschaft von Funktionsbreite auf Schutzwirkung ändern

Nicht mit „moderner Micro-Controller“ oder möglichst vielen Sensoren beginnen. Die stärkste evidenzgestützte Problemkette ist:

> Das Gewächshaus bleibt bei Sonne, Sturm, Regen und Frost auch während Abwesenheit in einem definierten sicheren Zustand.

Klimaoptimierung und Komfort sind zweite Nutzenebenen. „Smart“, Cloud und KI sind austauschbare Begriffe und sollten nicht die Positionierung tragen.

### 2. Einen Controller, aber zwei klare Anlagenpakete anbieten

Die Zweizonenfähigkeit ist bereits vorhanden und real erprobt. Ein Rückbau würde keinen Marktbeleg schaffen. Sinnvoller ist ein gemeinsamer, zweizonenfähiger Controller mit zwei verständlichen Warenkörben: Einzonen-Referenzanlage und Zweizonenanlage. Der Unterschied liegt in Innenfühlern, Antrieben und Kabeln. Die Kapazität von bis zu acht Sensoren bleibt eine technische Eigenschaft der Wetterstationsarchitektur und darf nicht mit acht im Basispaket benötigten Sensoren verwechselt werden.

### 3. Sicherheits- und Diagnoseumfang vor weiteren Klimafunktionen ausbauen

Der Prototyp nennt bereits Sensor-Fallbacks. Für eine belastbare Produktposition sollten zusätzlich definiert und getestet werden:

- Plausibilitätsgrenzen und Abweichungserkennung zwischen Sensoren,
- Verhalten bei unterbrochenem oder festhängendem Sensor,
- Erkennung von Aktorbewegung, Endlage oder Zeitüberschreitung,
- Verhalten bei Stromwiederkehr,
- Priorität von Sturm, Frost, Hitze und manueller Bedienung,
- sicherer Zustand bei widersprüchlichen Anforderungen,
- lokale Ereignis- und Fehlerhistorie,
- sichtbarer Unterschied zwischen „Befehl gesendet“ und „Zustand bestätigt“.

Der Marktwert entsteht nicht aus mehr Regeln, sondern aus Vertrauen, dass bekannte Fehler beherrscht werden.

### 4. Außenwetter nicht von einer unbewiesenen Funkstrecke abhängig machen

Die Präsentation zeigt einen solar-/batteriebetriebenen Außen-Multisensor, während das Produktprinzip verkabelte Kernfunktionen verspricht. Auch die neuere GW3001 verwendet zwischen WS90 und Gateway eine Funkstrecke; Ethernet und lokale Speicherung des Gateways beseitigen dieses letzte Funkrisiko nicht. Da Wind und Regen sicherheitsrelevant sind, braucht die unterstützte Wetterstation eine nachweisbare Verbindungsüberwachung, definierte Ersatzlogik und einen sicheren Zustand bei veralteten oder fehlenden Daten. Für den WS90 sollte außerdem geprüft werden, ob die vom Hersteller empfohlene 12-V-Winterversorgung mit Heizung verpflichtend wird.

### 5. Lokale Bedienung vereinfachen

Die ältere Hardware mit physischen Aktortasten und Info-Display passt zur Robustheitsposition besser als ein zwingender großer Touchscreen. Konfiguration und Historie können im Webinterface liegen; sichere Handbedienung und Status müssen ohne Browser möglich bleiben.

### 6. Preis immer an einen Lieferumfang binden

Der frühere Zielbereich von 700–1.500 EUR ist höchstens als unterer Controllerpreis plausibel, aber für ein komplettes System mit Wetterstation, Motoren, Kabeln und Anschlüssen zu niedrig. Öffentlich sichtbare Teilwarenkörbe stützen diese Vorsicht, belegen aber keinen eigenen Verkaufspreis.

Künftig getrennt kommunizieren:

- Controller-/Kernhardware,
- Sensor- und Aktorpaket,
- Montage/Elektroinstallation,
- optionale Module,
- optionale Fern-/Datendienste.

Die neue vorläufige Preisarchitektur lautet deshalb 1.690 EUR für den Controllerkern, 2.990 EUR für eine standardisierte Einzonen-Schutzanlage und 3.990 EUR für zwei Zonen. Diese Werte sind marktlogische Testanker, keine Angebote. Die Kalkulation muss zeigen, ob nach Hardware, Fertigung, Versand, Gewährleistung und Support genügend Deckungsbeitrag verbleibt.

### 7. Erdreichwärmetauscher entkoppeln

Der EWT ist technisch interessant, vergrößert aber Bau-, Hygiene-, Kondensations-, Dimensionierungs- und Installationsfragen. In den ausgewerteten Kundenproblemen erscheint er nicht als gesuchte Lösung. Er sollte die Vermarktung des Kernsystems nicht verzögern und später als separates Modul oder Referenzprojekt bewertet werden.

### 8. Produktkonformität früh als Architekturthema behandeln

Mit 230-V-Ausgängen, Funk, vernetzten Funktionen und motorischen Antrieben ist Konformität kein nachträgliches Etikett. Welche EU-Regelwerke tatsächlich greifen, muss fachkundig für die endgültige Produktgrenze geprüft werden. Als offensichtliche Prüffelder gelten mindestens elektrische Sicherheit, elektromagnetische Verträglichkeit, Funk, Maschinen-/Antriebsintegration und Cybersicherheit.

Nach Gründerangabe gilt IP67 für den aufgebauten Controller einschließlich Anschlüsse. Für das Serienprodukt bleiben Prüfgrundlage, konkrete Stecker-/Kabelkonfiguration und Übertragbarkeit zu dokumentieren. IP67 und Gartenschlauchreinigung sind getrennte Aussagen: Für den Reinigungsclaim müssen Strahl, Abstand, Winkel und Betriebszustand festgelegt und geprüft werden.

### 9. Waschbarkeit als Systemmerkmal entwickeln

Nach Gründerangabe wird ein Gewächshaus innen gelegentlich mit Gartenschlauch oder Hochdruckreiniger gereinigt. Die geprüften nahen Produkte sind dafür vielfach ungeeignet oder liefern keinen entsprechenden Nachweis: GrowBase nennt IP42, NIDO ONE V2 soll ausdrücklich von Spritzwasser ferngehalten werden und OpenSprinkler benötigt für Außeneinsatz ein separates Schutzgehäuse. Senmatic LCC1 erreicht IP65, weist aber keinen Hochdruckreinigungsnachweis aus.

Damit ist eine gartenschlauchtaugliche Gesamtinstallation eine plausible und bereits gewählte Differenzierung. Sie muss als Systemanforderung für Gehäuse, Bedienung, Steckverbinder, Schutzkappen, Kabel, Sensoren und Aktoren behandelt werden. Gartenschlauch und Hochdruckreiniger sind getrennte Prüf- und Produktversprechen; direkte Hochdruckreinigung ist derzeit nicht zugesagt. Die Mehrzahlungsbereitschaft für dieses Merkmal ist noch nicht validiert.

## Noch offene Dokumentationspunkte

Vor einer weiteren Markt- oder Produktkommunikation sollte ein eindeutiger Ist-Stand hergestellt werden:

| Thema | Aktuelle Angaben | Klärung |
|---|---|---|
| lokale Bedienung | Präsentation: Info-Display und physische Aktortasten; Produktkonzept: Touchbedienung | Ist-Prototyp, Zielprodukt und optionale Bediengeräte getrennt beschreiben |
| Kernverkabelung | Produktprinzip: verkabelter Kern; Präsentation: solar-/batteriebetriebener Außen-Multisensor | Kommunikationsweg, Ausfallüberwachung und Fallback der Wetterstation festhalten |
| Zonen | geklärt: M01/M02 = Zone 1, M03/M04 = Zone 2 | Funktion der beiden Motoren innerhalb jeder Zone noch benennen |
| Blattfeuchte | Präsentation ordnet Sensoren 1/2 und 3/4 beide „Zone 1“ zu | mutmaßlichen Dokumentationsfehler prüfen, nicht ungeprüft übernehmen |
| Schutzart | Gründerangabe: IP67 für aufgebauten Controller samt Anschlüssen | Prüfgrundlage und Serienübertragbarkeit dokumentieren |
| EWT-Ventilator | Präsentation vermischt in „Max. 280Pa m³/h“ Druck- und Volumenstromeinheit | korrekte Kennwerte und Betriebspunkt dokumentieren |

Diese Punkte beweisen keinen technischen Fehler des Prototyps. Sie zeigen, dass Produktversprechen, vorhandene Hardware und geplante Architektur derzeit nicht ausreichend getrennt dokumentiert sind.

## Priorisierte Produkt-Roadmap aus Marktsicht

### Jetzt beibehalten und härten

1. lokale autonome Regelung,
2. Außenwetter und aktive Lüftung,
3. Sturm-, Regen-, Frost- und Überhitzungsschutz,
4. robuste lokale Handbedienung,
5. Fehlererkennung, bestätigte Aktorzustände und Ereignisprotokoll,
6. ein gemeinsamer zweizonenfähiger Controller mit klar definiertem Ein- und Zweizonenpaket.

### Danach modular ergänzen

1. Bewässerung und Bodenfeuchte,
2. Beschattung,
3. zusätzliche Klima-/Blattfeuchtesensorik,
4. Partnerinstallation und vorkonfigurierte Hauspakete.

### Vorerst nicht priorisieren

1. Erdreichwärmetauscher als Standardbestandteil,
2. zusätzliche Sensorfabrikate ohne bestandene mechanische, klimatische und elektrische Qualitätsprüfung,
3. KI als Verkaufsargument,
4. komplexe Mehrzonenoberfläche,
5. großer Touchscreen, sofern Statusanzeige und Handbedienung anders robust lösbar sind.

## Marktbasierte Go-/No-Go-Einschätzung

### Was die Desk Research stützt

- Das technische Problem existiert.
- Einfache Einzelgeräte lösen die Kombination aus Hitze und Sturm nicht vollständig.
- Professionelle Technik deckt die Funktionen ab, ist für kleine Anlagen aber komplex und preislich wenig transparent.
- Der Prototyp enthält bereits einen relevanten Teil des gesuchten Funktionskerns.
- Ein klar abgegrenztes Nachrüstsystem zwischen DIY und Projektanlage ist plausibel.

### Was nicht bewiesen ist

- wie viele passende DACH-Kunden existieren,
- ob der Nutzen einen Gesamtpreis von mehr als 1.000 EUR trägt,
- ob Käufer Selbstinstallation oder Fachmontage erwarten,
- wie hoch Garantie-, Support- und Akquisitionskosten werden,
- ob Premium-Hobby oder kleiner Gewerbebetrieb der bessere erste Markt ist.

### Entscheidung für die nächste Entwicklungsphase

Aus reiner Marktsicht ist ein Abbruch nicht begründet. Der dreijährige Echtbetrieb macht auch einen funktionalen Scope-Reset unattraktiv. Sinnvoll ist ein **Packaging-Reset auf einen gemeinsamen zweizonenfähigen Controller sowie klar definierte Ein- und Zweizonenpakete**, gefolgt von dokumentierter Prüfung und einer belastbaren Stück-/Installationskostenrechnung. Neue Komfort-, Bewässerungs- oder KI-Funktionen sollten erst danach Entwicklungszeit erhalten.

## Nächste analysierbare Entscheidungen ohne Rekrutierung

1. Ein- und Zweizonen-Warenkorb aus der vorhandenen Prototypinventur eindeutig abgrenzen.
2. Stückliste und Herstellkosten für Controllerkern, Einzonen- und Zweizonenpaket berechnen.
3. Sicherheitszustände und Prioritätslogik als prüfbare Anforderungen dokumentieren.
4. Produktgrenze festlegen: Controller/Komponentenkit oder betriebsfertiges System mit Aktoren und Installation.
5. Für beide Produktgrenzen Preis- und Margenszenarien rechnen.

Diese Schritte benötigen keine Kundenkontakte, aber teilweise technische und kaufmännische Informationen, die nicht aus öffentlichen Marktquellen ableitbar sind.

Der detaillierte Marktvergleich der drei realistischen Liefermodelle und die Empfehlung für ein standardisiertes Ein-/Zweizonensystem stehen in [product-boundary-options.md](product-boundary-options.md).
