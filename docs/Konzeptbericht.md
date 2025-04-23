# Konzeptbericht

| **Status** | In Arbeit / In Prüfung / **Abgeschlossen** |
| --- | --- |
| **Projektname** | BlackBerry Pi |
| **Projektleiter** | Spyros Catéchis |
| **Auftraggeber** | Kurt Järmann |
| **Autoren** | Aram A., Nicolas A., Naomi B., Spyros C. |
| **Verteiler** | K. Järmann |

**Änderungskontrolle, Prüfung, Genehmigung**

|  |  |  |  |
| --- | --- | --- | --- |
| Version | Datum | Beschreibung, Bemerkung | Name oder Rolle |
| 1.0 | 22.04.2025 | Erste Ausfüllung | Aram, Naomi, Nicolas |
| 1.1 | 22.04.2025 | Raffinierung | Aram, Naomi |
| 1.2 | 22.04.2025 | Prüfung | Spyros |
| 1.3 | 22.04.2025 | Überarbeitung | Naomi |
| 2.0 | 22.04.2025 | Finale Abgabe | Spyros |

**Definitionen und Abkürzungen**

|  |  |
| --- | --- |
| Begriff / Abkürzung | Bedeutung |
| Pi | Raspberry Pi |
| AOSP | Android Open Source Projekt |
| BS | Betriebssystem |
| CAD | Computer Aided Design |
| BlackBerry Pi | Umbauprojekt: BlackBerry mit Raspberry Pi als Herzstück |

**Referenzen**

|  |  |
| --- | --- |
| Referenz | Titel, Quelle |
| Projektreferenzen | GitHub Repository | [GitHub-BlackBerryPi](https://github.com/PetabyteBrain/BlackberryPi) |

**Inhaltsverzeichnis**

[1 Zusammenfassung 3](#_Toc196211344)

[2 Systemanforderungen 3](#_Toc196211345)

[2.1 Anforderungen an die Funktionalität 3](#_Toc196211346)

[2.2 Anforderungen an die Informationssicherheit und den Datenschutz 4](#_Toc196211347)

[3 Systemarchitektur 4](#_Toc196211348)

[3.1 Gliederung der Lösung in Module 4](#_Toc196211349)

[3.2 Schnittstellen 4](#_Toc196211350)

[4 Testkonzept 5](#_Toc196211351)

[5 Weiterführung der Projektplanung 7](#_Toc196211352)

[5.1 Abgleich von Planung und tatsächlichem Verlauf der Phase Konzept 7](#_Toc196211353)

[5.2 Aktualisierung der Risikosituation 7](#_Toc196211354)

[5.3 Planung der nächsten Phase 8](#_Toc196211355)

# Zusammenfassung

In den folgenden Kapiteln wird die Konzeptualisierung des Projekts "Blackberry Pi Phone" detailliert behandelt. Dabei werden wesentliche Aspekte wie die benötigten Ressourcen für die Umsetzung des Projekts sowie die Vorgehensweise beim Testing thematisiert. Ziel ist es, eine klare und strukturierte Übersicht zu bieten, die die notwendigen Schritte und Überlegungen für die erfolgreiche Realisierung des Projekts darstellt.

# Systemanforderungen

## Anforderungen an die Funktionalität

Verfeinerte Anforderungen:

|  |  |  |  |
| --- | --- | --- | --- |
| **Anforderung** | **Bezeichnung** | **Beschreibung** | **Ziel(e)** |
| Modularität | A1 | Das System muss vollständig modular aufgebaut sein (Display, Akku, Recheneinheit, Eingabegeräte). | Z1 |
| Hardware-Eingabegerät | A2 | |  | | --- | |  |  |  | | --- | | Es muss ein Hardware-Eingabegerät vorhanden sein (z. B. physische Tastatur). | | Z3 |
| Open Source | A3 | Das Betriebssystem muss Open Source sein und Root-Zugriff ermöglichen. | Z1 |
| Austauschbarkeit | A4 | Alle Hardwarekomponenten müssen dokumentiert, öffentlich zugänglich und austauschbar sein. | Z2 |
| Stromversorgung (Akku) | A5 | Die Stromversorgung muss über einen austauschbaren Akku realisiert werden. | Z5 |
| Reparierbar/Reproduzierbar (3D-Druck) | A6 | Das Gehäuse muss reparierbar und z. B. durch 3D-Druck reproduzierbar sein. | Z5 |
| Grundlegende Funktionen | A7 | Das Gerät muss grundlegende Smartphone-Funktionen bieten (z. B. WLAN, Browser, Touchscreen). | Z4 |
| Softwaremodifizierbarkeit | A8 | Die Software muss leicht modifizierbar sein (z. B. durch Konfig-Dateien oder offene Quellcodes). | Z2 |
| Kostengünstig | A9 | Die Lösung muss kostengünstig realisierbar sein (< 250 CHF Gesamtbudget). | Z2 |
| Technische Dokumentation | A10 | Es muss eine ausführliche technische Dokumentation des Systems erstellt werden. | Z6 |

Systemaufgaben zur Erfüllung der Anforderungen:

|  |  |  |
| --- | --- | --- |
| **Aufgaben** | **Systemaufgabe** | **Bezug zu Anforderung(en)** |
| S1 | Auswahl, Beschaffung und Integration modularer Hardwarekomponenten (Display, Pi, Akku, Tastatur etc.) | A1, A4, A5 |
| S2 | Entwicklung oder Anpassung eines offenen Betriebssystems mit vollem Root-Zugriff | |  | | --- | |  |   A3, A7, A8 |
| S3 | |  | | --- | |  |   Design eines individuellen, 3D-druckbaren Gehäuses inkl. Öffnungen für Ports und Kühlung | A6, A1 |
| S4 | Test der Systemfunktionen: WLAN, Touchscreen, Browser | A7 |
| S5 | Implementierung einer physischen Eingabe (z. B. Mini-QWERTZ-Keyboard) | A2 |
| S6 | Detaillierte Dokumentation aller verwendeten Komponenten, Softwarestände und Konfigurationsschritte | A4, A10 |
| S7 | Kostenplanung, Preisvergleich und Budgetkontrolle während der Entwicklung | A9 |
| S8 | |  | | --- | |  |   Einrichtung einer Entwicklungsumgebung für Softwaremodifikationen | A3, A8 |

## Anforderungen an die Informationssicherheit und den Datenschutz

In unserem Projekt wird nicht mit Informationen und Personendaten gehandelt. Somit sind unsere Anforderungen eher schlicht ausfallend. Für unser Team jedoch brauchen wir die folgenden Anforderungen.

1. Datenintegrität: Regelmässige Backups für Fortschritte zu abspeichern.
2. Dokumentation: Regelmässig Fortschritte mit einem Markup File dokumentieren.
3. Überprüfung: Regelmässig Testfälle überprüfen, um sicher zu stellen, das alles funktioniert.

# Systemarchitektur

## Gliederung der Lösung in Module

|  |  |  |
| --- | --- | --- |
| **Modul Nr.** | **Modulbezeichnung** | **Beschreibung** |
| M1 | Raspberry Pi | Zentrale Recheneinheit, die das Betriebssystem ausführt und die Kommunikation zwischen den Modulen steuert. |
| M2 | Touchscreen-Display | Anzeigeeinheit für die Benutzeroberfläche, ermöglicht die Interaktion durch Touch-Eingaben. |
| M3 | Physische Tastatur | Eingabemodul zur Text- und Befehlsübertragung über physische Tasten. |
| M4 | Gehäuse | Schutz und Halterung für alle Module, individuell gestaltbar. |
| M5 | Akku | Stromversorgung des gesamten Geräts. |
| M6 | Betriebssystem | Offenes Betriebssystem, das auf dem Raspberry Pi läuft und die Softwareumgebung bereitstellt. |
| M7 | Benutzeroberfläche | Anpassbare UI-Elemente, die die Interaktion mit dem Betriebssystem ermöglichen. |

## Schnittstellen

System – Extern

|  |  |  |  |
| --- | --- | --- | --- |
| Schnittstelle | Beschreibung | Datenübertragung | Konfiguration |
| S1 | WLAN/Bluetooth | Datenübertragung für Internet und Kommunikation | Über BS |
| S2 | USB-Schnittstelle | Verbindung zu externen Geräten | Über USB-C |

System – Intern

|  |  |  |  |
| --- | --- | --- | --- |
| S3 | GPIO-Schnittstelle | Steuerung und Kommunikation zwischen Modulen | Über BS |
| S4 | I2C-Schnittstelle | Kommunikation zwischen Display und Pi | Über BS |

# Testkonzept

|  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- |
| Systemaufgabe | Test-ID | Testbeschreibung | Testmethode / Eingabe | Erwartetes Ergebnis | Bezug zu Anforderung(en) |
| S1 – Modulare Hardwareintegration | S1-TF1 | Display einbauen und prüfen | Bildschirmmodul anschliessen | Bild wird angezeigt | A1 |
|  | S1-TF2 | Akku tauschen | Ersatzakku einsetzen | Gerät startet ohne Fehler | A5 |
|  | S1-TF3 | Recheneinheit gegen baugleiche tauschen | Austauschmodul einsetzen | System bootet korrekt | A4 |
|  | S1-TF4 | Tastatur austauschen | Physische Tastatur wechseln | Tasteneingabe funktioniert | A2, A4 |
| S2 – Open Source OS & Softwaremodifikation | S2-TF1 | Root-Zugriff aktivieren | Terminalzugang testen | Root-Shell verfügbar | A3 |
|  | S2-TF2 | Quellcode ändern & kompilieren | Funktion im Code modifizieren | Systemverhalten ändert sich korrekt | A8 |
|  | S2-TF3 | WLAN & Kamera mit OS nutzen | Verbindung + Kamerafunktion prüfen | Funktionen laufen stabil | A7 |
| S3 – 3D-druckbares Gehäuse | S3-TF1 | Gehäuse drucken nach STL-Datei | 3D-Drucker | Bauteil passt perfekt | A6 |
|  | S3-TF2 | Passgenauigkeit Gehäuse | Hardware einbauen | Alle Komponenten passen | A1, A6 |
|  | S3-TF3 | Stabilitätstest | Falltest aus 1 m Höhe | Kein Bruch / minimale Beschädigung | A6 |
| S4 – Grundfunktionen testen | S4-TF1 | WLAN-Verbindung prüfen | SSID + Passwort eingeben | Verbindung bleibt > 5 Min. | A7 |
|  | S4-TF2 | Kamera öffnen und Bild speichern | Foto aufnehmen | Bild erscheint in Galerie | A7 |
|  | S4-TF3 | Browserseite laden | URL eingeben | Website wird korrekt dargestellt | A7 |
| S5 – Eingabegerät | S5-TF1 | Tasteneingabe testen | Text eintippen | Text erscheint korrekt | A2 |
|  | S5-TF2 | Elektrisches Signal prüfen | Tastendruck + Multimeter | Signal wird übertragen | A2 |
| S6 – Technische Dokumentation prüfen | S6-TF1 | Doku auf Vollständigkeit prüfen | Dokumentenreview | Alle Komponenten & Schritte enthalten | A10 |
|  | S6-TF2 | Doku-gestützter Nachbau durch Dritte | Gerät nach Anleitung bauen | Gerät funktioniert wie geplant | A10, A4 |
| S7 – Budgetkontrolle & Vergleich | S7-TF1 | Einzelpreise auflisten & summieren | Kostenaufstellung | Gesamt ≤ 250 € | A9 |
|  | S7-TF2 | Preisvergleich mit Marktgeräten | Vergleichsprodukte recherchieren | ≤ 50 % vom Durchschnittspreis | A9 |
| S8 – Softwareentwicklung & Modifikation | S8-TF1 | Entwicklungsumgebung einrichten | Toolchain installieren | Projekte bauen ohne Fehler | A3 |
|  | S8-TF2 | Konfigurationsdateien ändern | z. B. config.yaml anpassen | Änderungen wirken im System | A8 |

# Weiterführung der Projektplanung

## Abgleich von Planung und tatsächlichem Verlauf der Phase Konzept

Wir kamen gut voran müssen nur noch Modul Gehäuse abarbeiten und unsere Präsentation / Dokumentation anfertigen.
Wir hatten keine Zeitliche oder zwischenmenschliche Probleme. Das grösste Risiko war die Kompatibilität respektiv die Inkompatibilität der Hardware miteinander, vor allem war dies ein Störfaktor beim Display. Dies ist jedoch nur eine leichte Verzögerung und stellt keine Gefahr für die Abschliessung des Projektes dar.

## Aktualisierung der Risikosituation

* **1. Unklare Aufgabenverteilung oder Kommunikationsprobleme im Team**
* **Aktualisierung:** Die interne Kommunikation im Team ist sehr gut strukturiert und effizient. Es bestehen klare Absprachen, die regelmässig über Teams und in Meetings aktualisiert werden.
* **Risikoeinschätzung:**
  + *Eintretenswahrscheinlichkeit:* Gering
  + *Auswirkungen:* Mittel
* **Massnahmen in der Konzeptphase:**
  + Beibehaltung der bestehenden Kommunikationswege.
  + Weiterhin Nutzung von Kanban und regelmässigen Abstimmungen.
* **2. Unzureichende Ressourcen (Räumlichkeiten, IT-Infrastruktur)**
* **Aktualisierung:** Aktuell stehen die notwendigen Räumlichkeiten und IT-Ressourcen ohne Einschränkungen zur Verfügung.
* **Risikoeinschätzung:**
  + *Eintretenswahrscheinlichkeit:* Gering
  + *Auswirkungen:* Hoch
* **Massnahmen in der Konzeptphase:**
  + Regelmässiger Check der Infrastruktur.
  + Vorhalten eines alternativen Arbeitsplatzes bei Störungen.
* **3. Fehlende Abstimmung mit dem Auftraggeber**
* **Aktualisierung:** Erste Rücksprachen mit dem Auftraggeber fanden statt. Dennoch bleibt die Gefahr bestehend, dass Anforderungen missverstanden werden.
* **Risikoeinschätzung:**
  + *Eintretenswahrscheinlichkeit:* Mittel
  + *Auswirkungen:* Hoch
* **Massnahmen in der Konzeptphase:**
  + Regelmässige Feedbackrunden mit dem Auftraggeber.
  + Detaillierte Dokumentation aller Anforderungen und Rückmeldungen.
* **4. Zeitliche Engpässe im Team**
* **Aktualisierung:** Die Zeitplanung wurde realistisch gestaltet, und bisher konnten alle Aufgaben im vorgesehenen Rahmen erledigt werden.
* **Risikoeinschätzung:**
  + *Eintretenswahrscheinlichkeit:* Gering
  + *Auswirkungen:* Mittel
* **Massnahmen in der Konzeptphase:**
  + Fortführung der aktuellen Arbeitsplanung.
  + Beibehaltung von Pufferzeiten für unvorhergesehene Aufgaben

**5. Technische Komplexität der Hardwareintegration**

* **Beschreibung:** Die Verbindung verschiedener Hardwarekomponenten könnte zu unerwarteten technischen Schwierigkeiten führen.
* **Eintretenswahrscheinlichkeit:** Sehr gering
* **Auswirkungen:** Hoch
* **Massnahmen:**
  + Frühzeitige Prototyp-Tests.
  + Klare Dokumentation von Schnittstellen und Konfigurationen.

## Planung der nächsten Phase

Da wir fast fertig mit unserem Projekt sind, bleiben nur noch das Modul Gehäuse (wie oben beschrieben) und die formale Angaben/ die Dokumentationen. Dies Teilen wir uns im Team ca. wie unten beschrieben auf. Natürlich gibt es Interaktionen im Team, auch wenn der Plan anderes aussagt.

|  |  |  |  |
| --- | --- | --- | --- |
| WER | Di. 22. April | Mi 23. April | Fr. 25.April |
| Spyros | CAD-Modeling | Modeling 2.0 | PP | Präsentation & Demo |
| Aram | Konzept Doc | Realisierung Doc |PP | Abschluss Doc |
| Naomi | Konzept Doc | Realisierung Doc |PP | Abschluss Doc |
| Nicolas | CAD-Modeling | Modeling 2.0 | PP | Präsentation & Demo |