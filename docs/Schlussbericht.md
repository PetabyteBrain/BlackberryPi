Schlussbericht

|  |  |
| --- | --- |
| **Status** | **In Arbeit** / In Prüfung / Abgeschlossen |
| **Projektname** | Blackberry Pi |
| **Projektleiter** | Spyros Catéchis |
| **Auftraggeber** | Kurt Järmann |
| **Autoren** | Aram A., Nicolas A., Naomi B., Spyros C. |
| **Verteiler** | Kurt Järmann |

**Änderungskontrolle, Prüfung, Genehmigung**

|  |  |  |  |
| --- | --- | --- | --- |
| Version | Datum | Beschreibung, Bemerkung | Name oder Rolle |
| 1.0 | 25.04.2025 | Erstes befüllen | Naomi, Aram |
| 1.1 | 25.04.2025 | Raffinierung & ergänzende Infos | Naomi, Aram |
| 1.2 | 25.04.2025 | Prüfung | Spyros, Aram |
| 1.3 | 25.04.2025 | Überarbeitung | Nicolas, Aram |
| 2.0 | 25.04.2025 | Finale Abgabe | Spyros, Aram |

**Definitionen und Abkürzungen**

|  |  |
| --- | --- |
| Begriff / Abkürzung | Bedeutung |
|  |  |

**Referenzen**

|  |  |
| --- | --- |
| Referenz | Titel, Quelle |
| Projektreferenzen | GitHub Repository | [GitHub](https://github.com/PetabyteBrain/BlackberryPi) |

Inhalt

[Teil 1 4](#_Toc196486154)

[Management Abstract 4](#_Toc196486155)

[Aufgabenstellung 5](#_Toc196486156)

[1. Ausgangslage 5](#_Toc196486157)

[2. Projektziele 5](#_Toc196486158)

[3. Rahmenbedingungen 5](#_Toc196486159)

[4. Aufwand & Ressourcen 5](#_Toc196486160)

[5. Kostenübersicht (geschätzt) 5](#_Toc196486161)

[6. Kommunikation 6](#_Toc196486162)

[Deklaration 6](#_Toc196486163)

[1. Zu den vorkenntnissen 6](#_Toc196486164)

[2. Zu Vorarbeiten 7](#_Toc196486165)

[3. Zu Firmenstandards 7](#_Toc196486166)

[Zeitplan 7](#_Toc196486167)

[Arbeitsprotokoll 8](#_Toc196486168)

[Spyros 8](#_Toc196486169)

[Aram 9](#_Toc196486170)

[Naomi 10](#_Toc196486171)

[Nicolas 11](#_Toc196486172)

[Teil 2: 12](#_Toc196486173)

[Situationsanalyse 12](#_Toc196486174)

[Ausgangslage 12](#_Toc196486175)

[SystemZiele & Lösungsvorschläge 14](#_Toc196486176)

[Systemarchitektur 15](#_Toc196486177)

[Testkonzept & Testspezifikationen 16](#_Toc196486178)

[Testspezifikation 16](#_Toc196486179)

[Testprozedur 18](#_Toc196486180)

[Testprotokoll 19](#_Toc196486181)

[Benutzerdokumentation / Anleitung 21](#_Toc196486182)

[Systemübersicht 21](#_Toc196486183)

[Anwenderfunktionalität 21](#_Toc196486184)

[Projekterfahrung 22](#_Toc196486185)

[Teil 3 22](#_Toc196486186)

[Selber erstelle Listings und Skripte 22](#_Toc196486187)

[Literaturverzeichnis 22](#_Toc196486188)

[Hardware 22](#_Toc196486189)

[Software / OS 23](#_Toc196486190)

[Glossar 24](#_Toc196486191)

# Teil 1

## Management Abstract

Alles startete bei dem Ausflug ins Technikmuseum in Solothurn, dort wurde unser PO(Spyros) inspiriert, ein eigenes Blackberry-Telefon zu kreieren, einfach eines, welches mit den Standards von heute mithalten kann.

Nach dieser initialen Idee kam die Projektwoche näher und Spyros sammelte wie verrückt Quellen und konkretere Ideen. Während der Woche wurde unser Projekt mithilfe des Projektantrags und der Studie zum Leben erweckt. Nach dem November arbeiteten wir drei regelmässig an der Entwicklung unseres Telefons. Am 28. Februar stiess dann Nicolas zu unserem Projekt hinzu. Wir haben dann fleissig bis am Dienstag das Projekt fertig gemacht. Hier ist anzumerken, dass wir bis dahin noch kein Gehäuse gedruckt hatten.

Uns ist es sehr wichtig, ein gutes Open-Source-Produkt zu kreieren, somit haben wir darauf geachtet, dass das Telefon nicht lizenzierte Komponenten hat und für die meisten einfach zugänglich ist. Zudem waren die Hauptziele, dass das Telefon ein Touchdisplay hat, eine Tastatur, simple Startknöpfe, auf einem Raspberry Pi läuft und eine Batterie als Stromversorgung hat.

Dank unserer harten Arbeit haben wir gute Resultate erhalten. Wir haben ein funktionierendes Blackberry Pi Telefon, welches Sachen wie Discord oder WhatsApp-Web darauf laden kann oder sogar Spiele. Zudem haben wir eine Interne und externe Tastatur, obwohl die Interne per Default abgeschaltet ist. Das ganze Telefon hat eine LIPO Batterie, somit kann man dies gut ohne direkte Stromversorgung brauchen.

Natürlich kann ich hier nur für mich sprechen, jedoch würde ich sagen, es ist eine sehr lehrreiche Projektarbeit gewesen. Das gesamte Wissen in unserem Team über GPIO-Pins und dergleichen ist zumindest ein bisschen gestiegen. Persönlich habe ich sehr viel gelernt. Für das ganze Team war es auch eine gute Erfahrung und Übung für unsere IDPA und IPA, da diese ähnlich ablaufen werden.

## Aufgabenstellung

### 1. Ausgangslage

**Projektidee:** Ein ausgedientes BlackBerry-Smartphone wird mit einem Raspberry Pi und modernen Komponenten neu aufgebaut. Ziel ist ein Retro-Gerät mit aktuellem Funktionsumfang.
**Problem:** Physische Tastaturen verschwinden, Geräte werden grösser – dieses Projekt bietet eine kompakte Alternative für Liebhaber klassischer Eingabemethoden.
**Stand:** Erste Konzepte und technische Machbarkeitsstudien sind abgeschlossen.

### 2. Projektziele

* Einbau eines Raspberry Pi in ein BlackBerry-Gehäuse
* Funktionsfähige Hardware-Schnittstellen (Tastatur, Display)
* Erstellung eines Prototyps
* Entwicklung eines eigenen Betriebssystems (AOSP-basiert)

### 3. Rahmenbedingungen

* **Zeit:** Initialisierung bis 29.11.2024
* **Organisation:** Unterstützung durch Lehrkräfte, Online-Ressourcen
* **Methodik:** Hermes
* **Genehmigung & Planung:** durch Autoren

### 4. Aufwand & Ressourcen

**Aufwand:** ~70 Stunden für Planung, Bau, Test
**Technik:** Raspberry Pi, Display, Akku, Tastatur, Gehäuse
**Werkzeuge:** CAD-Software, Lötstation, 3D-Drucker
**Support:** Online-Recherche, Lehrkraft

### 5. Kostenübersicht (geschätzt)

| **Komponente** | **CHF** |
| --- | --- |
| Gehäuse & Tastatur | 29.60 |
| Touchscreen | 14.00 |
| PCB (via Onboard gratis) | 0.00 |
| Tastatur-Connector | 24.29 |
| Raspberry Pi | 20–80 |
| **Gesamt** | 87.89–147.89 |

### 6. Kommunikation

* Projektabstimmungen im Team & mit Auftraggeber
* Regelmässige Kurzprotokolle und Updates über Teams
* Zusammenfassungen für den Auftraggeber

**7. Risiken & Massnahmen**

| **Risiko** | **Eintritt** | **Auswirkung** | **Massnahme** |
| --- | --- | --- | --- |
| Unklare Aufgabenverteilung | Mittel | Mittel | Klare Kommunikation, tägliche Updates |
| Fehlender Zugang zu Infrastruktur | Gering | Hoch | Nutzung privater Räume, IT-Frühwarnung |
| Abstimmungsprobleme mit Auftraggeber | Mittel | Hoch | Regelmässige Rückmeldungen, direkte Kommunikation |
| Zeitliche Engpässe im Team | Mittel | Mittel | Frühzeitige Planung, Priorisierung |

## Deklaration

### 1. Zu den vorkenntnissen

Da wir vor allem mit Hardware-komponenten arbeiteten, mussten die einzigen Vorkenntnisse sein, wie man lötet, Kabel aufschneidet (Lötvorbereitung), wie GPIO-pins funktionieren. Zudem hatten drei Person Erfahrungen mit Raspberry Pi und eine davon viel Erfahrung mit Arduino. Das ganze Team hatte schon vorher ein ähnliches Projekt, ein GTTO-display; hier kam jedoch noch mehr programmieren vor als im Blackberry PI Projekt. Da es ein sehr simples Projekt war, brauchte und hatte niemand von uns eine Spezialisation oder ein relevantes Zertifikat.

### 2. Zu Vorarbeiten

Wir haben mit dem Projekt schon um den 20. September 2024 gestartet, dies waren ca. 4 bis 6 Stunden Arbeit bis wir dann offiziell in der Woche vom 23. – 27 November gestartet haben. In der Zeit zwischen der zu vorgenannten Woche und der Jetzigen waren wir wöchentlich mindestens 45 Minuten mit dem Projekt beschäftigt, dies beinhaltete Komponenten kaufen, planen von der Zusammensetzung, design-planung, Testing Einheiten von erfolgreichen Schritten.

### 3. Zu Firmenstandards

Wir haben mit dem Projekt schon um den 20. September 2024 gestartet, dies waren ca. 4 bis 6 Stunden Arbeit bis wir dann offiziell in der Woche vom 23. – 27 November gestartet haben. In der Zeit zwischen der zu vorgenannten Woche und der Jetzigen waren wir wöchentlich mindestens 45 Minuten mit dem Projekt beschäftigt, dies beinhaltete Komponenten kaufen, planen von der Zusammensetzung, design-planung, Testing Einheiten von erfolgreichen Schritten.

## Zeitplan

Der Zeitaufwand für das Projekt wird auf ungefähr **70 Stunden** geschätzt. Dies beinhaltet die folgenden Phasen:

* **Planung**: Recherche und Designphase, in der die Anforderungen und Spezifikationen festgelegt werden. Dazu gehört auch das Finden von geeigneten Hardware- und Softwarelösungen, die den Projektzielen entsprechen.
* **Aufbau und Implementierung**: Der praktische Teil des Projekts, bei dem die einzelnen Komponenten zusammengefügt werden. Hierzu zählen das Löten, die Verkabelung der Hardware, das Zusammenbauen des Gehäuses sowie das Installieren und Konfigurieren der Software.
* **Fehlerbehebung und Tests**: Nach der Implementierung wird eine Testphase durchgeführt, um sicherzustellen, dass alle Funktionen wie vorgesehen arbeiten. Dazu gehört das Debuggen von Softwareproblemen und die Optimierung der Hardware-Integration.

## Arbeitsprotokoll

### Spyros

Spyros war in mehrfacher Hinsicht ein wichtiger Teil des Teams. Bereits zu Beginn der Projektphase erklärte er sich bereit, die **Finanzierung** zu übernehmen. Er besorgte nicht nur die Bauteile, sondern kümmerte sich auch um die Logistik – also Bestellung, Lieferung und rechtzeitige Bereitstellung der Materialien. Diese Verantwortung übernahm er eigenständig, wodurch dem Team wertvolle Zeit für die technische Arbeit zur Verfügung stand.

Im technischen Bereich war seine grösste Leistung die Erstellung des **3D-Modells des Handy-Gehäuses**. Er nutzte hierfür spezialisierte Software und baute das Modell in enger Rücksprache mit Aram und Naomi schrittweise auf. Dabei achtete er auf eine präzise Umsetzung der vorgegebenen Masse und eine praxisnahe Anordnung der Bauteile. Sein Beitrag im Bereich der 3D-Modellierung war der umfangreichste im gesamten Team.

Auch in der **Script-Recherche** zeigte sich Spyros sehr engagiert. Er analysierte verschiedene Optionen, testete erste Umsetzungen und trug zur finalen Auswahl der Skripte bei, mit denen das Gerät betrieben wurde. In dieser Phase arbeitete er eng mit Aram zusammen, um praktikable und funktionierende Lösungen zu identifizieren.

Ein weiterer Beitrag lag in der **Mitarbeit an der logischen Planung** des Geräts. Spyros war stark darin, technische Zusammenhänge zu erfassen und Vorschläge zu machen, wie etwa Kabelverläufe optimiert oder Komponenten effizienter untergebracht werden könnten. Seine Einschätzungen waren oft sehr praxisorientiert und halfen dabei, mögliche Probleme im Aufbau frühzeitig zu erkennen.

In der **Dokumentation** brachte er sich zwar nur vereinzelt ein, lieferte aber technische Inhalte und unterstützte insbesondere Naomi bei der Formulierung technischer Abschnitte.

Spyros überzeugte durch technisches Geschick, Problemlösungsorientierung und einen hohen Grad an Eigenverantwortung, insbesondere in den Bereichen Finanzierung, 3D-Modellierung und technische Planung.

### Aram

Aram übernahm im Verlauf des Projekts eine zentrale Rolle und war in nahezu allen Bereichen aktiv eingebunden. Als Allrounder konnte er sich flexibel an die jeweiligen Anforderungen anpassen und übernahm Verantwortung für verschiedene Schlüsselaspekte der Projektarbeit.

Ein wesentlicher Teil seiner Arbeit bestand in der **Ausarbeitung der Präsentation**, mit der das Team das Projekt abschliessend vorstellte. Er kümmerte sich sowohl um den visuellen Aufbau als auch um die inhaltliche Ausformulierung der Präsentation, wobei er besonderen Wert auf Struktur, Verständlichkeit und Präzision legte.

Zusätzlich war Aram massgeblich an der **Recherche und Auswahl geeigneter Scripts** beteiligt. Diese Scripts bildeten die Grundlage für die Funktionsweise des Projekts und mussten sorgfältig analysiert, angepasst und integriert werden. Aram trug hier wesentlich dazu bei, passende Lösungen zu finden und funktionale Abläufe zu gewährleisten.

Auch die **logische Konzeption des Aufbaus des DIY-Handys** wurde in enger Abstimmung mit den anderen Teammitgliedern von ihm mitentwickelt. Aram behielt stets den Gesamtüberblick und sorgte dafür, dass alle Bauteile und Softwareelemente sinnvoll zusammenspielten.

Er engagierte sich stark beim **Löten der Hardwarekomponenten** und stellte sicher, dass die Verbindungen technisch einwandfrei und sauber ausgeführt wurden – eine wichtige Voraussetzung für die Funktionstüchtigkeit des Geräts.

Im gestalterischen Bereich übernahm er zusammen mit Spyros die Entwicklung des **3D-Modells des Handy-Gehäuses**. Aram lieferte eigene Ideen zur Form, Ergonomie und zum technischen Aufbau des Gehäuses, und arbeitete aktiv in der Modellierungsphase mit.

Auch bei der **Dokumentation** des Projekts brachte Aram sich umfassend ein. Er strukturierte die Inhalte mit und half dabei, technische Abläufe verständlich darzustellen. Insgesamt zeichnete sich Aram durch eine hohe Einsatzbereitschaft, Vielseitigkeit und Eigeninitiative aus, was für das Gelingen des Projekts wesentlich war.

### Naomi

Naomi war eine der tragenden Säulen des Projekts – sowohl im schriftlichen als auch im technischen Bereich. Ihre Hauptverantwortung lag bei der **Dokumentation**, die sie mit grosser Sorgfalt und Struktur erstellte. Sie investierte viel Zeit in die Ausformulierung der einzelnen Abschnitte, achtete auf klare Formulierungen, inhaltliche Genauigkeit sowie einheitliche Gestaltung. Besonders bei komplexen technischen Zusammenhängen verstand sie es, die Inhalte so zu formulieren, dass sie auch für Aussenstehende verständlich wurden.

Darüber hinaus war Naomi intensiv in die **logische Planung und Struktur des Aufbaus** des DIY-Handys eingebunden. Sie arbeitete eng mit Aram und Spyros zusammen und half bei der Entscheidung, wie die verschiedenen Hardware- und Software-Komponenten sinnvoll aufeinander abgestimmt werden können. Dabei zeigte sie ein gutes Verständnis für funktionale Abläufe und bewies ein gutes Gespür für die technische Umsetzung.

Auch im **3D-Modelling** war Naomi beteiligt. Obwohl der Grossteil von Spyros umgesetzt wurde, leistete sie inhaltliche Zuarbeit, brachte Verbesserungsvorschläge ein und übernahm kleinere Modellierungsaufgaben. Besonders im Bereich der Detailgestaltung – wie z.B. der Platzierung bestimmter Bauteile im Gehäuse – lieferte sie hilfreiche Inputs, die zur finalen Qualität des Modells beitrugen.

Zusätzlich war Naomi eine konstante und verlässliche Teamplayerin, die sich proaktiv einbrachte, den Überblick über wichtige Arbeitsschritte behielt und die Zusammenarbeit im Team mit ihrer strukturierten Art positiv beeinflusste. Ihr Beitrag war durchgehend bedeutend und inhaltlich vielseitig.

### Nicolas

Nicolas kam im späteren Verlauf des Projekts zum Team und fand sich rasch in die bestehende Arbeitsstruktur ein. Obwohl er nicht von Beginn an involviert war, bemühte er sich, sich konstruktiv einzubringen und übernahm gezielt Aufgaben, die das Team entlasteten. Sein Beitrag war zwar nicht so umfassend wie der der anderen Teammitglieder, dennoch war seine Unterstützung in bestimmten Bereichen hilfreich und wertvoll.

Ein Schwerpunkt seiner Tätigkeit lag im Bereich der **praktischen Umsetzung**, insbesondere beim **Löten**. In dieser technisch sensiblen Phase half er bei der Verbindung einzelner Komponenten und unterstützte dabei, dass die Hardware korrekt miteinander verschaltet wurde. Auch wenn er diese Tätigkeit nicht hauptverantwortlich übernahm, war seine Unterstützung bei der Durchführung und Vorbereitung der Lötarbeiten eine spürbare Entlastung für das Team.

Darüber hinaus beteiligte sich Nicolas auch an der **Erstellung der Projektdokumentation**. In Abstimmung mit Naomi und Aram ergänzte er bestehende Texte, überarbeitete kleinere Abschnitte und half bei der Korrektur von Formulierungen und technischen Beschreibungen. Dabei zeigte er eine sorgfältige Herangehensweise, mit dem Ziel, die Dokumentation sprachlich zu verfeinern und inhaltlich zu vervollständigen.

Nicolas war auch bei mehreren Teamtreffen präsent, wo er sich aktiv in Gespräche über technische Abläufe und gestalterische Entscheidungen einbrachte. Besonders bei der Planung kleinerer Details – etwa der Platzierung von Bauteilen oder organisatorischen Aufgaben – lieferte er hin und wieder hilfreiche Anmerkungen. Er zeigte Interesse an den technischen Prozessen und stellte Fragen, um die Zusammenhänge besser zu verstehen und gegebenenfalls mitarbeiten zu können.

Auch wenn sein Beitrag im Vergleich zu den anderen Teammitgliedern punktueller war, war seine Bereitschaft zur Mitarbeit deutlich spürbar. In den ihm übertragenen Aufgabenbereichen arbeitete er gewissenhaft und trug dazu bei, das Gesamtprojekt zu unterstützen.

Seine Rolle kann als **ergänzend und unterstützend** beschrieben werden – weniger im konzeptionellen oder gestalterischen Bereich, aber umso mehr im praktischen Mitwirken, wo er durch seine ruhige und konzentrierte Arbeitsweise half, Aufgaben effizient abzuschliessen.

# Teil 2:

## Situationsanalyse

### Ausgangslage

Die Telefone von BlackBerry waren einst die unangefochtenen Marktführer im Smartphone-Bereich und besonders beliebt bei Geschäftskunden, da sie eine physische Tastatur, hohe Sicherheit und effiziente E-Mail-Verwaltung boten. Mit der Einführung des iPhones und der Touchscreen-Revolution durch Apple verschob sich der Fokus der Nutzer jedoch weg von Tastaturen hin zu grossen, interaktiven Displays. BlackBerry verpasste es, sich schnell genug anzupassen, und verlor schliesslich seinen Platz als Marktführer.

Heute ähneln sich die meisten Smartphones in Design und Funktionalität, was die Vielfalt am Markt stark eingeschränkt hat. In dieser homogenen Welt sehen wir eine Chance, BlackBerry neu zu interpretieren und etwas Einzigartiges zu schaffen.

Die bewährte BlackBerry-Architektur und die physische Tastatur bieten weiterhin viele Vorteile, insbesondere für Nutzer, die ein Gerät mit einer "echten" Tasteneingabe bevorzugen. Durch den Einsatz eines Raspberry Pi als Kern können wir die klassische Hardware mit moderner Technik kombinieren und ein Smartphone kreieren, das sowohl funktional als auch innovativ ist. Dieses neue Gerät vereint das Beste aus zwei Welten: Die Retro-Ästhetik und Haptik eines BlackBerry mit der Flexibilität und Leistungsfähigkeit eines Raspberry Pi – und bringt endlich wieder ein „neues Format“ auf den Smartphone-Markt.

#### Stärken

* Da die meisten Handys heutzutage ähnlich aussehen, hätten wir mit der Ästhetik des Blackberrys und der Tastatur einen Vorteil, da es anders als das Produkt der Konkurrenz ist. Dieses aussehen kann einen attraktiven Verkaufspunkt für Blackberry Enthusiasten sein.
* Dazu haben wir den Vorteil, dass wir unser Produkt Open Source behalten und deswegen jeder Nutzer genau wissen kann, was es beinhaltet und was er eingeht beim Gebrauch unserer Software.
* Kosteneffiziente Hardware, Beispiel Raspberry Pi. Der Vorteil davon ist, dass die Reparaturen einfach vom Nutzer / einem Dienst gemacht werden können und günstiger wären als andere moderne Handys.
* Das Blackberry Pi kann auch mit anderen Betriebssystemen laufen, solange es mit den Drivern und Hardware kompatibel ist.
* Da es Open Source ist, kann es die Möglichkeit geben, Anpassungen am Gerät zu führen, um diese Benutzerspezifisch zu gestalten und zu entwickeln.

#### Schwächen

#### Hohe Abhängigkeit von proprietärer Software:

Viele Nutzer sind auf geschlossene OS (z.B. iOS, Android) angewiesen. Ein offenes, anpassbares System basierend auf Raspberry Pi kann die Abhängigkeit reduzieren.

#### Hohe Kosten moderner Smartphones:

Premium-Smartphones sind oft sehr teuer. Ein DIY-Handy auf Basis eines Raspberry Pi bietet eine kostengünstige Alternative, insbesondere für technikaffine Nutzer.

#### Komplizierte Reparierbarkeit:

Viele aktuelle Smartphones sind schwierig zu reparieren (z.B. durch verklebte Komponenten). Unser Projekt kann durch ein modulares Design mit leicht austauschbaren Teilen punkten.

#### Mangelnde Software-Upgrades bei älteren Geräten:

Hersteller unterstützen ältere Modelle oft nicht mehr mit Updates, was Sicherheitsrisiken birgt. Ein offenes System erlaubt langfristige Pflege und Updates durch die Community.

#### Eingeschränkte Anpassbarkeit:

Nutzer können Design, Funktionen und Hardware ihrer Smartphones nur begrenzt anpassen. Mit einem Raspberry Pi sind massgeschneiderte Anpassungen möglich.

## SystemZiele & Lösungsvorschläge

#### Freie OS Wahl:

Mit einer freien resp. unabhängigen OS Wahl ist die Bandbreite des Blackberrys viel besser und man kann.

#### Kosten & Marken:

Solange man nicht nur für die Marke bezahlt ist ein Smartphone schon sehr viel billiger, wenn wir dies mit simpler Technologie verknüpfen, bekommen wir ein einfaches Telefon und faires Preis-Leistung Verhältnis.

#### Simple Technologie:

Da wir unser Blackberry Pi mit einem Raspberry Pi ausstatten, ein Screen und noch eine Tastatur hinzufügen ist das ganze Telefon sehr simpel und wenn ein Natel simpel ist, ist es auch simpel zum Reparieren. Was vor allem für ein kostengünstiges design ein Schlüsselziel ist.

#### Sicherstellung langfristiger Software-Upgrades durch ein offenes System:

Das Projekt BlackBerry Pi zielt darauf ab, ein Smartphone mit einem offenen Betriebssystem zu entwickeln, das von der Community unterstützt werden kann. Dadurch wird es Nutzern ermöglicht, regelmässig Sicherheitsupdates und neue Funktionen zu erhalten, unabhängig von der Herstellerunterstützung. Dies reduziert Sicherheitsrisiken und verlängert die Nutzungsdauer des Geräts erheblich.

#### Personalisierung:

Durch die simple Technologie und die freie OS-wahl ist das Natel individualisierbar. Das heisst der Nutzer kann alles personalisieren, eigene teile zum Telefon zusammenstellen. Wenn der Nutzer sehr viel Technik wissen hat, könnte er sogar zuhause sein Handy personalisieren.

## Systemarchitektur


<img src=„Images/design.component.view..png“></img>

## Testkonzept & Testspezifikationen

### Testspezifikation

#### Kritikalität der Funktionseinheit

|  |  |  |
| --- | --- | --- |
| **Funktionseinheit** | **Kritikalität** | **Begründung** |
| Recheneinheit (Raspberry Pi) | Hoch | Ohne funktionierende Recheneinheit ist keine Systemfunktion möglich. |
| Stromversorgung (Akku) | Hoch | Das System ist ohne Stromversorgung nicht betriebsbereit. |
| Betriebssystem / Root-Zugriff | Hoch | Notwendig für alle weiteren Software-Tests und Anpassungen. |
| Tastatur (Hardware-Eingabe) | Mittel | Grundlegende Eingabe notwendig, jedoch durch Bildschirm ggf. ergänzbar. |
| WLAN | Mittel | Essentiell für viele Anwendungen, aber Systemstart auch offline möglich. |
| Gehäuse (3D-Druck) | Niedrig | Physisch wichtig, aber nicht kritisch für Softwarefunktionen. |

#### Testanforderungen

Tests mit Normal-, Grenz- und Fehlerwerten.

Tests unter Ausnahmebedingungen (z. B. Akkuwechsel im Betrieb).

Alle Testergebnisse werden protokolliert.

#### Testverfahren

Vorbereitung:

Komponenten anschliessen, OS installieren, Stromversorgung sichern.

Durchführung:

Durchführung gemäss Testfalltabellen, manuell.

Auswertung:

Vergleich von Ist- mit Sollverhalten, Bewertung als „Bestanden / Nicht bestanden“.

#### Testkriterien

Abdeckungsgrad: Mindestens ein Test pro Anforderung.

Checklisten: Alle Modul- und Systemfunktionen abgedeckt.

Ende-Kriterien: Keine Fehler in hochkritischen Modulen, System vollständig funktionsfähig.

#### Testfälle

|  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- |
| **Nr.** | **AFo-Nr.** | **Anwendungsfall**  **(ggf. orientiert an Use Cases)** | **Ausgangssituation** | **Eingabedaten** | **erwartetes Ergebnis** | **Bemerkungen, Prüfergebnis** |
| T1 | A5 | Akku ausstecken | Gerät ist ausgeschaltet | Akku entfernen und wieder einsetzen | Gerät startet wie erwartet | Es funktioniert wie erwartet |
| T2 | A6 | Gehäuse prüfen (3D-Druck) | Gehäuseteile vorhanden | Zusammenbauen | Teile passen genau, Gerät sitzt fest |  |
| T3 | A7 | WLAN-Verbindung testen | WLAN verfügbar | SSID + Passwort eingeben | Verbindung bleibt stabil | Wlan lässt sich verbinden und es bleibt verbunden |
| T4 | A2 | Tastatureingabe testen | System betriebsbereit | Text eingeben | Zeichen werden korrekt dargestellt | Tastatur funktioniert |
| T5 | A8 | Konfigurationsdatei ändern | config.yaml geladen | Parameter ändern | Änderung zeigt Auswirkungen im Verhalten | Dies funktioniert |
| T6 | A9 | Budgetprüfung | Komponentenliste vorhanden | Preise eintragen | Gesamtkosten ≤ 250 € |  |
| T7 | A10 | Nachbau mit Doku | Nur Dokumentation vorhanden | Gerät nach Anleitung bauen | Gerät funktioniert wie geplant |  |

### Testprozedur

#### Vorbereitung

OS-Installation auf SD-Karte abgeschlossen

Alle Module verbunden (ohne Kamera & Audio)

WLAN-SSID & Passwort bekannt

Voraussetzungen:
Alle Komponenten liegen vor und sind überprüft.

Tools zur Durchführung sind verfügbar.

Dokumentation für Referenztests ist vollständig und zugänglich.

Konfiguration:
Raspberry Pi in 3D-gedrucktem Gehäuse eingebaut.

Display, Tastatur und Akku korrekt verbunden.

Alle verwendeten Konfigurationsdateien befinden sich auf dem System.

Testumgebung: stabile Stromversorgung, lokales Netzwerk, stabile Tischunterlage für Gehäusetests.

#### Durchführung

Initialisierung: System einschalten oder vorbereiten (z. B. Komponenten einsetzen).

Durchführung: Entsprechend des Testfalls Eingaben tätigen, Komponenten prüfen, Funktionen aufrufen oder physikalische Veränderungen vornehmen.

Beobachtung: Reaktion des Systems oder Moduls beobachten.

Vergleich: Ergebnis mit dem erwarteten Resultat aus der Testspezifikation vergleichen.

Dokumentation: Testausgang (Erfolg, Fehler, Besonderheiten) direkt erfassen.

#### Nachbearbeitung

Auswertung der Resultate:

Das Ergebnis wird direkt nach jedem Testschritt dokumentiert (z. B. Tabelle oder digitales Protokoll).

Wenn nötig, werden Screenshots, Fotos oder Log-Dateien als Beleg gesichert.

Fehlermeldungen:

Auffälligkeiten (z. B. keine Reaktion, Bootfehler) werden mit Uhrzeit und Beschreibung festgehalten.

Bei Abweichung vom Soll: Testwiederholung und Prüfung der Fehlerquelle.

Protokollierung:

Ergebnisse werden in der Testprotokoll-Tabelle eingetragen (siehe 4.3.2).

Jede Abweichung wird auch im Abschnitt Testauswertung (4.3.3) kommentiert.

### Testprotokoll

#### Testobjekt

Testobjekt: Raspberry-Pi-basiertes System mit modularer Bauweise (Version: v1.0)

Testfall: T1 – Akku entfernen und wieder einsetzen

Tester: Nicolas Ammeter

Ort: Innovationlab

Datum: 23.04.2025

Uhrzeit: 14:10 – 14:15 Uhr

#### Testresultate

|  |  |  |  |
| --- | --- | --- | --- |
| **Zeitpunkt** | **Handlung** | **Beobachtung** | **Bewertung** |
| 14:10 Uhr | System ist ausgeschaltet | Keine Aktivität sichtbar | Erwartungsgemäss |
| 14:11 Uhr | Akku entnommen | Kein Widerstand, Stecker gut gelöst | Erwartungsgemäss |
| 14:12 Uhr | Akku wieder eingesetzt | Verbindung sitzt fest | Erwartungsgemäss |
| 14:13 Uhr | Gerät eingeschaltet (Power-Button) | LED leuchtet, System startet korrekt | **Bestanden** |

Erwartetes Ergebnis laut Spezifikation: Gerät startet nach Akkueinbau fehlerfrei → erfüllt

Zwischenergebnisse: Keine Zwischenstörungen, keine Verzögerung beim Boot

#### Testauswertung

Abweichungen zur Spezifikation: Keine

Einfluss auf Funktionalität: Keine Einschränkung festgestellt. System funktioniert einwandfrei nach Akku-Wiedereinbau.

Mögliche Fehlerursachen: Keine aufgetreten

Trendbeobachtung: Keine Häufung ähnlicher Fehler – Test zeigt, dass die modulare Stromversorgung zuverlässig funktioniert.

## Benutzerdokumentation / Anleitung

### Systemübersicht

Unser Hauptziel ist es, ein portables, austauschbares, open source Telefon zu kreieren. Unser Telefon basiert auf einem Raspberry Pi, welches in ein Blackberry integriert wird. Die einzige externe Schnittstelle ist ein USB-Type-C-Kabel-Port, dieser wird gebraucht, um das Telefon aufzuladen. Da wir nicht mit Daten und sonstigen Informationen arbeiten, haben wir weder verschiedene Nutzer noch Schutzmassnahmen implementiert. Da unser Projekt open source ist, ist es in der Verantwortung jeden Users, sich selbst zu schützen.

### Anwenderfunktionalität

Das Telefon ist ein recht simples Ding, es kann sich jedoch mit dem Internet verbinden, hat einen Touchscreen und hat trotzdem eine echte Tastatur. Um das Telefon zu benutzen, muss man es nur zusammensetzen, es aufladen, danach kann man es schon versklaven. Damit wir das alles testen können, ist die simpelste Aufgabe, ein Wortspiel im Browser zu öffnen und dies danach zuspielen. Somit sollte man in den Browser kommen, das Spiel mittels der Tastatur spielen und das alles ohne Probleme. Um das Telefon abzuschalten, muss man ins Menu gehen und dort auf Shutdown klicken. Um es danach wieder zu starten, muss man nur auf den Button am Case drücken und es schaltet sich ein. Wir haben keine Software verbundenen Fehlermeldungen, die nicht von Raspberry Pi kommen, und für diese gibt es ein eigenes [Handbuch](https://www.raspberrypi.com/documentation/). Somit gibt es nicht wirkliche Software-Recovery-Plans von unserer Seite, für die Hardware-Recovery kann man das Supporthandbuch, Kapitel 3.3.2, konsultieren.

## Projekterfahrung

Wir haben schlussendlich alle unsere Grundziele erreicht. Wir haben ein funktionierendes Blackberry-Phone, welches auf der Basis eines Raspberry Pis läuft, mit einem Touchscreen, einer Tastatur und Buttons, um das Telefon zu bedienen. Unser Design war nicht wirklich ein Grundziel, jedoch war es ein sehr wichtiger Bestandteil unseres Projekts.

Für unsere Gruppe war dieses Projekt eine Bereicherung an Praxisbezug in unserem Feld. Die Teamarbeit war gut und die Kommunikation lief immer sehr offen. Zeitprobleme hatten wir nie. Die einzige Verspätung war wegen eines Drucks und wir haben es schnell wieder aufgearbeitet.

Nächstes mal probieren wir, schon früher mit dem 3D-drucken zu starten, einfach damit wir nie in Zeitdruck geraten.

Die Zukunft für dieses Projekt sieht gut aus, denn wir haben noch etwa 4 Weiterentwicklungsmöglichkeiten gefunden. Diese wären: Display-Orientierungserkennung, eine SIM-Karten-Integration, damit es zu einem wahrhaftigen Telefon wird, weitere externe Ports und eine Kameraanbindung.

Somit ist unser Telefon zwar kommunikations- und funktionsfähig, jedoch hat es noch viel Verbesserungspotenzial, welches diese Gruppe in Zukunft angehen will.

# Teil 3

## Selber erstelle Listings und Skripte

Die sind alle im Github aufzufinden.

## Literaturverzeichnis

### Hardware

#### Keyboard

* [Blackberry Keyboard with Arduino](https://forum.arduino.cc/t/interfacing-blackberry-q10-keypad-to-arduino-and-the-oled-typewriter/342989)
* [Blackberry Keyboard eevblog](https://www.eevblog.com/forum/beginners/how-to-connect-to-a-very-very-challanging-blackberry-q10-keyboard-connector/msg735622/)
* [Adafruit Blog Blackberry Keyboard](https://blog.adafruit.com/2019/01/14/interfacing-a-blackberry-q10-keyboard-into-your-microcontroller-project-blackberry-arduino-microcontroller/)
* [BBQ10KBD arturo182](https://github.com/arturo182/BBQ10KBD/tree/master)
* [Blackberry tastatur mit Bluetooth/ usb c](https://github.com/wallComputer/bbq20kbd_hw)
* [Adapter PCB keyboard to usb-C](https://github.com/Dakkaron/Fairberry)
* [Update Firmware of UsbASP programmer](https://www.electronics-lab.com/project/usbasp-firmware-update-guide/)
* [Keyboard project github](https://github.com/ZitaoTech/BBQ10-USB_BLE_Keyboard)

#### Other

* [2.8 inch Display](https://www.waveshare.com/wiki/2.8inch_DPI_LCD)
* [Compute module 5 lite, 16gb ram, wifi](https://www.welectron.com/Raspberry-Pi-Compute-Module-CM5116000-Lite-16-GB-RAM-WiFi)
* [Nano Base Board (A)](https://www.berrybase.ch/nano-base-board-a-fuer-raspberry-pi-compute-module-4?c=2410)

### Software / OS

#### AOSP

* [Android Open Source Project (AOSP)](https://source.android.com/)
* [AOSP adapted for Raspberry pi](https://konstakang.com/devices/rpi5/)
* [Raspberry pi Vanilla](https://github.com/raspberry-vanilla)
* [Android install instructions](https://www.xda-developers.com/how-to-install-android-on-a-raspberry-pi/)

#### Other OS

* [Lineage OS](https://lineageos.org/)
* [Sailfish OS](https://sailfishos.org/)
* [Plasma mobile](https://plasma-mobile.org/)
* [Mobian](https://mobian-project.org/)
* [Manjaro](https://manjaro.org/products/download/arm)
* [Postmarket OS](https://postmarketos.org/)

#### Extra / Other

* [Pi Zero 2w + blackberry case + e-ink](https://www.reddit.com/r/RASPBERRY_PI_PROJECTS/comments/1ddj94n/pi_zero_2w_blackberry_case_eink_would_this_work/)

## Glossar

|  |  |
| --- | --- |
| Begriff | Erklärung |
|  |  |
| Blackberry | Eine alte Telefonmarke, die lange Marktführer war vor Apple |
| Raspberry Pi | Ein mini Computer Apparat ist, welches selbst ansteuerbar ist |
| 3D-Druck | Ein Model das durch Filament und ein spezieller Drucker erstellt wird |
| Scripts | Code Dateien welche z.B.: der Tastatur sagt, wie sie ansteuerbar ist |
| GPIO | **G**eneral-**p**urpose **I**nput / **O**utput 🡪Schnittstelle von Base Boards u. ä. |
| LIPO | **L**ithium **p**olymer Batterie |