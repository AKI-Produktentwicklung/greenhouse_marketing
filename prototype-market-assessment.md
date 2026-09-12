# Marktbasierte Standortbestimmung des Prototyps

## Kurzfazit

Der vorhandene Greenhouse-Assistant-Prototyp ist **kein einfacher Smart-Home-Regler mehr**, aber auch **noch kein marktreifes professionelles Steuerungssystem**. Er besetzt technisch bereits die gesuchte Brücke: lokale Steuerung, Außenwetter, motorische Lüftung, Heizung, Feuchtefunktionen, manuelle Bedienung und Fernzugriff in einem System für kleine Gewächshäuser.

Die wichtigste marktbasierte Änderung ist deshalb nicht das Hinzufügen weiterer Funktionen. Das Konzept sollte auf einen kleineren, klar bepreisbaren und nachweisbar sicheren Kern reduziert werden:

> Nachrüstbares, lokal autonomes Schutz- und Klimasystem für ein hochwertiges kleines Gewächshaus – mit aktiver Lüftung, Außenwetter und verständlichem Betriebszustand.

Der Prototyp ist ein starker technischer Demonstrator. Für ein Produkt fehlen vor allem standardisierter Lieferumfang, belastbare Fehlerreaktionen, Installationskonzept, Konformitätsplanung und ein klarer Preisbezug je Anlagenumfang.

## Evidenzbasis und Grenzen

### Vom Gründer bereitgestellte beziehungsweise intern dokumentierte Informationen

- Der Node-RED-Prototyp läuft laut README seit etwa drei Jahren in einem realen Gewächshaus.
- Die ältere Präsentation beschreibt Außenwetter, bis zu acht Innen-, Blattfeuchte-, Bodenfeuchte- und Bodentemperatursensoren, bis zu vier Linearantriebe, Heizung, Umluft/Befeuchtung, Erdreichwärmetauscher und Smartphone-Bedienung.
- Lokale Sturm-, Frost- und Überhitzungslogik sowie ein teilweiser Sensor-Fallback sind als bereits vorhanden beschrieben.

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
| zwei Zonen im Grundsystem | mittel | für 10–100 m² teilweise nützlich, erhöht aber sofort I/O-, UI- und Testkomplexität | eine Zone als Basis, zweite Zone als klar bepreiste Erweiterung |
| bis zu acht Sensoren je Sensortyp | nicht als Marktbedarf belegt | die Zahl ist derzeit durch die vorgesehene Wetterstation geprägt; alternative Fabrikate müssen auch mechanische und klimatische Qualitätsanforderungen erfüllen | vorhandene Architektur nicht vorschnell verwerfen; Alternativen anhand einer Qualitäts- und Kompatibilitätsmatrix prüfen |
| Blattfeuchtesensorik | mittel bis niedrig | kann Krankheitsrisiko unterstützen, ist in der Stichprobe kein dominanter Kaufgrund | optionale spätere Erweiterung |
| Bodenfeuchte/Bewässerung | mittel | reales Problem und starker bestehender Markt, würde den Startumfang jedoch verbreitern | Schnittstelle vorsehen, Regelung erst nach Klimakern |
| Erdreichwärmetauscher | niedrig für den Markteintritt | derzeit keine belastbare Nachfrageevidenz; erfordert Bauarbeit und erweitert Haftung/Projektierung | aus dem Kernprodukt entfernen und als separates Innovationsmodul behandeln |
| Wetterprognose und KI | niedrig für den Markteintritt | Wettbewerber bieten Prognosen bereits; Kernprobleme benötigen zunächst robuste aktuelle Messung und Regeln | zurückstellen, bis lokale Schutzlogik und Datenqualität bewiesen sind |

## Empfohlenes erstes Produktpaket

Dies ist eine marktbasierte Empfehlung, noch keine Produktentscheidung.

### Kernsystem: eine Zone / ein Gewächshaus

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

### Erweiterungen statt Grundumfang

- zweite Zone,
- weitere Innenfühler,
- Bodenfeuchte und Bewässerung,
- Beschattung,
- Blattfeuchte,
- Befeuchtung/Entfeuchtung,
- Erdreichwärmetauscher,
- Prognose- und Optimierungsfunktionen.

Diese Aufteilung reduziert Varianten, Testfälle und Installationsaufwand, ohne die langfristige modulare Architektur aufzugeben.

## Konkrete Änderungen am bisherigen Konzept

### 1. Produktbotschaft von Funktionsbreite auf Schutzwirkung ändern

Nicht mit „moderner Micro-Controller“ oder möglichst vielen Sensoren beginnen. Die stärkste evidenzgestützte Problemkette ist:

> Das Gewächshaus bleibt bei Sonne, Sturm, Regen und Frost auch während Abwesenheit in einem definierten sicheren Zustand.

Klimaoptimierung und Komfort sind zweite Nutzenebenen. „Smart“, Cloud und KI sind austauschbare Begriffe und sollten nicht die Positionierung tragen.

### 2. Eine Zone zum Standard machen

Zwei Zonen im Grundsystem führen in Richtung professioneller Komplexität, bevor der private Kernnutzen belegt ist. Die zweite Zone sollte technisch vorbereitet, aber kommerziell als Erweiterung behandelt werden. Die Kapazität von bis zu acht Sensoren ist hingegen zunächst eine technische Eigenschaft der vorgesehenen Wetterstationsarchitektur und darf nicht mit acht im Basispaket benötigten Sensoren verwechselt werden.

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

Die Präsentation zeigt einen solar-/batteriebetriebenen Außen-Multisensor, während das Produktprinzip verkabelte Kernfunktionen verspricht. Da Wind und Regen sicherheitsrelevant sind und die Voice-of-Customer-Stichprobe instabile Außensensorik nennt, sollte die Kern-Wetterstation entweder verkabelt sein oder einen nachweisbaren lokalen Fallback mit Verbindungsüberwachung besitzen.

### 5. Lokale Bedienung vereinfachen

Die ältere Hardware mit physischen Aktortasten und Info-Display passt zur Robustheitsposition besser als ein zwingender großer Touchscreen. Konfiguration und Historie können im Webinterface liegen; sichere Handbedienung und Status müssen ohne Browser möglich bleiben.

### 6. Preis immer an einen Lieferumfang binden

Der frühere Zielbereich von 700–1.500 EUR ist als Controllerpreis plausibel, aber für ein komplettes System mit Wetterstation, I/O, Schaltschrank, Motoren und Installation wahrscheinlich zu niedrig. Öffentlich sichtbare Teilwarenkörbe stützen diese Vorsicht, belegen aber keinen eigenen Verkaufspreis.

Künftig getrennt kommunizieren:

- Controller-/Kernhardware,
- Sensor- und Aktorpaket,
- Montage/Elektroinstallation,
- optionale Module,
- optionale Fern-/Datendienste.

Der erste marktlogische Testkorridor bleibt deshalb 990 EUR, 1.790 EUR und 2.990 EUR als Reaktionsanker für dieselbe neutrale Konzeptbeschreibung; er ist keine Preisentscheidung. Beschlossene Angebote müssten später jeweils einen klaren Lieferumfang besitzen.

### 7. Erdreichwärmetauscher entkoppeln

Der EWT ist technisch interessant, vergrößert aber Bau-, Hygiene-, Kondensations-, Dimensionierungs- und Installationsfragen. In den ausgewerteten Kundenproblemen erscheint er nicht als gesuchte Lösung. Er sollte die Vermarktung des Kernsystems nicht verzögern und später als separates Modul oder Referenzprojekt bewertet werden.

### 8. Produktkonformität früh als Architekturthema behandeln

Mit 230-V-Ausgängen, Funk, vernetzten Funktionen und motorischen Antrieben ist Konformität kein nachträgliches Etikett. Welche EU-Regelwerke tatsächlich greifen, muss fachkundig für die endgültige Produktgrenze geprüft werden. Als offensichtliche Prüffelder gelten mindestens elektrische Sicherheit, elektromagnetische Verträglichkeit, Funk, Maschinen-/Antriebsintegration und Cybersicherheit.

Die Präsentationsangabe „IP66 (10 h tauchbar)“ muss korrigiert oder durch einen konkreten Prüfbericht belegt werden: IP66 bezeichnet Schutz gegen starke Wasserstrahlen, nicht gegen Untertauchen. Zeitweiliges Untertauchen wird über IP67 beschrieben. Außerdem gilt die Schutzart nur für die geprüfte vollständige Anordnung einschließlich Kabelverschraubungen und Bedienöffnungen, nicht automatisch für ein unbearbeitetes Einzelgehäuse.

## Widersprüche in der heutigen Produktbeschreibung

Vor einer weiteren Markt- oder Produktkommunikation sollte ein eindeutiger Ist-Stand hergestellt werden:

| Thema | Aktuelle Angaben | Klärung |
|---|---|---|
| lokale Bedienung | Präsentation: Info-Display und physische Aktortasten; Produktkonzept: Touchbedienung | Ist-Prototyp, Zielprodukt und optionale Bediengeräte getrennt beschreiben |
| Kernverkabelung | Produktprinzip: verkabelter Kern; Präsentation: solar-/batteriebetriebener Außen-Multisensor | Kommunikationsweg, Ausfallüberwachung und Fallback der Wetterstation festhalten |
| Zonen | Produktkonzept: zwei Zonen; Präsentation: unterschiedliche Paar-/Zonenzuordnungen je Sensortyp | eine konsistente Kanal- und Zonenmatrix erstellen |
| Blattfeuchte | Präsentation ordnet Sensoren 1/2 und 3/4 beide „Zone 1“ zu | mutmaßlichen Dokumentationsfehler prüfen, nicht ungeprüft übernehmen |
| Schutzart | Gehäuse und Antrieb: „IP66 (10 h tauchbar)“ | Herstellerdaten und Schutzart der vollständigen Baugruppe prüfen |
| EWT-Ventilator | Präsentation vermischt in „Max. 280Pa m³/h“ Druck- und Volumenstromeinheit | korrekte Kennwerte und Betriebspunkt dokumentieren |

Diese Punkte beweisen keinen technischen Fehler des Prototyps. Sie zeigen, dass Produktversprechen, vorhandene Hardware und geplante Architektur derzeit nicht ausreichend getrennt dokumentiert sind.

## Priorisierte Produkt-Roadmap aus Marktsicht

### Jetzt beibehalten und härten

1. lokale autonome Regelung,
2. Außenwetter und aktive Lüftung,
3. Sturm-, Regen-, Frost- und Überhitzungsschutz,
4. robuste lokale Handbedienung,
5. Fehlererkennung, bestätigte Aktorzustände und Ereignisprotokoll,
6. ein klar definiertes Einzonen-Kernpaket.

### Danach modular ergänzen

1. zweite Zone,
2. Bewässerung und Bodenfeuchte,
3. Beschattung,
4. zusätzliche Klima-/Blattfeuchtesensorik,
5. Partnerinstallation und vorkonfigurierte Hauspakete.

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

Aus reiner Marktsicht ist ein Abbruch nicht begründet. Ebenso wenig ist ein breiter Produktbau begründet. Sinnvoll ist ein **Scope-Reset des vorhandenen Prototyps auf ein standardisiertes Einzonen-Schutzpaket**, gefolgt von technischer Härtung und einer belastbaren Stück-/Installationskostenrechnung. Neue Komfort-, EWT-, KI- oder Mehrzonenfunktionen sollten erst danach Entwicklungszeit erhalten.

## Nächste analysierbare Entscheidungen ohne Rekrutierung

1. Bestehenden Prototyp gegen den empfohlenen Einzonen-Umfang inventarisieren: vorhanden, teilweise vorhanden, fehlt.
2. Stückliste und Herstellkosten für genau dieses Kernpaket berechnen.
3. Sicherheitszustände und Prioritätslogik als prüfbare Anforderungen dokumentieren.
4. Produktgrenze festlegen: Controller/Komponentenkit oder betriebsfertiges System mit Aktoren und Installation.
5. Für beide Produktgrenzen Preis- und Margenszenarien rechnen.

Diese Schritte benötigen keine Kundenkontakte, aber teilweise technische und kaufmännische Informationen, die nicht aus öffentlichen Marktquellen ableitbar sind.

Der detaillierte Marktvergleich der drei realistischen Liefermodelle und die Empfehlung für ein standardisiertes Einzonen-System stehen in [product-boundary-options.md](product-boundary-options.md).
