# Realisierungsbericht

| **Status** | In Arbeit / In Prüfung / **Abgeschlossen** |
| --- | --- |
| **Projektname** | Blackberry Pi |
| **Projektleiter** | Spyros Catéchis |
| **Auftraggeber** | Kurt Järmann |
| **Autoren** | Aram A., Nicolas A., Naomi B., Spyros C. |
| **Verteiler** | Kurt Järmann |

**Änderungskontrolle, Prüfung, Genehmigung**

|  |  |  |  |
| --- | --- | --- | --- |
| Version | Datum | Beschreibung, Bemerkung | Name oder Rolle |
| 1.0 | 22.04.2025 | Erstes befüllen | Naomi, Nicolas |
| 1.1 | 23.04.2025 | Raffinierung & ergänzende Infos | Naomi, Nicolas | Aram |
| 1.2 | 23.04.2025 | Prüfung | Spyros |
| 1.3 | 23.04.2025 | Überarbeitung | Naomi |
| 2.0 | 23.04.2025 | Finale Abgabe | Spyros |

**Definitionen und Abkürzungen**

|  |  |
| --- | --- |
| Begriff / Abkürzung | Bedeutung |
| PMH | Power Management Hat |
| A Female | USB type A Female port |

**Referenzen**

|  |  |
| --- | --- |
| Referenz | Titel, Quelle |
| Projektreferenzen | GitHub Repository | [GitHub](https://github.com/PetabyteBrain/BlackberryPi) |

**Inhaltsverzeichnis**

[1 Zusammenfassung 3](#_Toc196311217)

[2 Technische Detailspezifikation 3](#_Toc196311218)

[2.1 Systemdesign 3](#_Toc196311219)

[2.1.1 Struktur 3](#_Toc196311220)

[2.1.2 Beschreibung der Elemente 3](#_Toc196311221)

[2.2 Schnittstellendefinitionen 4](#_Toc196311222)

[2.3 Sicherheit (ISDS) 4](#_Toc196311223)

[2.4 Anforderungszuordnung 4](#_Toc196311224)

[3 Systemdokumentation 4](#_Toc196311225)

[3.1 Konfigurations-Dokumentation 4](#_Toc196311226)

[3.2 Benutzerhandbuch 5](#_Toc196311227)

[3.2.1 Systemübersicht 5](#_Toc196311228)

[3.2.2 Anwenderfunktionalität 5](#_Toc196311229)

[3.3 Supporthandbuch 5](#_Toc196311230)

[3.3.1 Massnahmen bei Benutzerproblemen 5](#_Toc196311231)

[3.3.2 Massnahmen bei technischen Problemen 5](#_Toc196311232)

[3.3.3 Anhang zum Supporthandbuch 5](#_Toc196311233)

[4 Systemtest 5](#_Toc196311234)

[4.1 Testspezifikation 5](#_Toc196311235)

[4.1.1 Kritikalität der Funktionseinheit 5](#_Toc196311236)

[4.1.2 Testanforderungen 6](#_Toc196311237)

[4.1.3 Testverfahren 6](#_Toc196311238)

[4.1.4 Testkriterien 6](#_Toc196311239)

[4.1.5 Testfälle 6](#_Toc196311240)

[4.2 Testprozedur 7](#_Toc196311241)

[4.2.1 Vorbereitung 7](#_Toc196311242)

[4.2.2 Durchführung 7](#_Toc196311243)

[4.2.3 Nachbearbeitung 7](#_Toc196311244)

[4.3 Testprotokoll 8](#_Toc196311245)

[4.3.1 Testobjekt 8](#_Toc196311246)

[4.3.2 Testresultate 8](#_Toc196311247)

[4.3.3 Testauswertung 8](#_Toc196311248)

[5 Weiterführung der Projektplanung 8](#_Toc196311249)

[5.1 Abgleich von Planung und tatsächlichem Verlauf der Phase Konzept 8](#_Toc196311250)

[5.2 Aktualisierung der Risikosituation 8](#_Toc196311251)

[5.3 Planung der nächsten Phase 8](#_Toc196311252)

**Abbildungsverzeichnis**

Abb.1. Systemdesign Grafik / Autor: Naomi Bächler

# Zusammenfassung

In den folgenden Kapiteln wird die Realisierung des Projekts "Blackberry Pi Phone" detailliert aufgeführt. Dabei werden wesentliche Aspekte wie die tatsächliche Umsetzung des Projekts sowie die Resultate der Testing Fälle und unser weiteres Vorgehen. Das Ziel dieses Berichtes ist es, die gesamte Realisierung offen darzulegen und rückblickend zu urteilen, was wir besser machen konnte und was wir gut umsetzen.

# Technische Detailspezifikation

## Systemdesign

### Struktur

![Image of the Systemdesign](Images/design.components.view.png)
Abb. 1. Systemdesign Grafik

### Beschreibung der Elemente

* Raspberry Pi Compute Module 5
* Blackberry Tastatur Tastatur aus einem alten Blackberry
* Waveshare Display 4.3inch DSI LCD
* Lipo Batterie 3.7V 5000mAh
* Side Fan DC12V - 0.18A Model: JD4512M12
* Nano Base Board Type A für Raspberry Pi Compute Module 5
* 3D-Gehäuse Die Druckpläne sind auf unserem [GitHub](https://github.com/PetabyteBrain/BlackberryPi/blob/main/README.md#3d-plans).

## Schnittstellendefinitionen

In der Oberen Abbildung ist auf allen wichtigen Pfeilen eine Art der Schnittstelle gekennzeichnet, hier eine Erläuterung:

* Tastatur: USB type A. Auf dem Base Board ist ein A Female, welcher die Tastatur entgegennimmt.
* Display: Ribbon Cable. Auf dem Base Board ist eine Ribbon Schnittstelle.
* Base Board: Board to Board 🡪 Das Raspberry und Base Board sind via mini Pins direkt verbunden.
* PMH: GPIO Pins 🡪 Base Board wird via GPIO Kabel und Jumper Wires (für länge) verbunden.
  + Batterie Conector 🡪 typischer Conector der mit Batterien kommt.
  + Jumper wires 🡪 Verlängerungskabel.

## Sicherheit (ISDS)

Wir achteten uns immer darauf, dass unsere Quellen glaubwürdig sind. Da unser Projekt open source ist, liegt es sehr offen und klar beim User, was er sich kauft, um das Projekt nachzustellen. Somit sind wir dort nicht verantwortlich für allgemeine Datenverschwendung.

## Anforderungszuordnung

|  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **AFo.-Nr.** | **Anforderung (Stichwort)** | **1** | **2** | **3** | **4** | **5** | **6** | **7** | **8** | **5** | **6** | **7** | **8** | **9** | **10** | **11** | **12** |
| 1 | Modularität |  |  |  |  |  |  |  |  |  |  |  |  |  | **x** |  |  |
| 2 | Hardware-Eingabegerät |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | **x** |
| 3 | Open Source |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | **x** |
| 4 | Austauschbarkeit |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | **x** |
| 5 | Stromversorgung (Akku) |  |  |  |  |  |  |  |  |  |  |  |  |  |  | **x** |  |
| 6 | Reparierbar/Reproduzierbar (3D-Druck) |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | **x** |
| 7 | Grundlegende Funktionen |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | **x** |
| 8 | Softwaremodifizierbarkeit |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | **x** |
| 9 | Kostengünstig |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | **x** |
| 10 | Technische Dokumentation |  |  |  |  |  |  |  |  |  |  |  |  | **x** |  |  |  |

# Systemdokumentation

## Konfigurations-Dokumentation

Die im Kapitel 2.1 aufgelisteten Elemente sind alle Hardwarekomponenten unseres Projektes, Software haben wir noch Scripts, welche jedoch schon vorgeschrieben sind. Um unser Projekt umzusetzen, braucht man vorinstalliert nur Raspberry Imager und den Raspberry Mass Storage Gadget. Die jeweiligen Ports, die wir nutzen, sind auch im Kapitel 2.2 aufgelistet. Die angesprochenen Scripts findet man im [GitHub](https://github.com/PetabyteBrain/BlackberryPi/blob/main/README.md#scripts).

## Benutzerhandbuch

### Systemübersicht

Unser Hauptziel ist es, ein portables, austauschbares, open source Telefon zu kreieren. Unser Telefon basiert auf einem Raspberry Pi, welches in ein Blackberry integriert wird. Die einzige externe Schnittstelle ist ein USB-Type-C-Kabel-Port, dieser wird gebraucht, um das Telefon aufzuladen. Da wir nicht mit Daten und sonstigen Informationen arbeiten, haben wir weder verschiedene Nutzer noch Schutzmassnahmen implementiert. Da unser Projekt open source ist, ist es in der Verantwortung jeden Users, sich selbst zu schützen.

### Anwenderfunktionalität

Das Telefon ist ein recht simples Ding, es kann sich jedoch mit dem Internet verbinden, hat einen Touchscreen und hat trotzdem eine echte Tastatur. Um das Telefon zu benutzen, muss man es nur zusammensetzen, es aufladen, danach kann man es schon versklaven. Damit wir das alles testen können, ist die simpelste Aufgabe, ein Wortspiel im Browser zu öffnen und dies danach zuspielen. Somit sollte man in den Browser kommen, das Spiel mittels der Tastatur spielen und das alles ohne Probleme. Um das Telefon abzuschalten, muss man ins Menu gehen und dort auf Shutdown klicken. Um es danach wieder zu starten, muss man nur auf den Button am Case drücken und es schaltet sich ein. Wir haben keine Software verbundenen Fehlermeldungen, die nicht von Raspberry Pi kommen, und für diese gibt es ein eigenes [Handbuch](https://www.raspberrypi.com/documentation/). Somit gibt es nicht wirkliche Software-Recovery-Plans von unserer Seite, für die Hardware-Recovery kann man das Supporthandbuch, Kapitel 3.3.2, konsultieren.

## Supporthandbuch

### Massnahmen bei Benutzerproblemen

Wir haben nicht wirkliche Benutzerprobleme, jedoch sind hier ein paar Stolpersteine.

* Noch keine SIM-Karte integriert
* Der Akku ist nicht lange andauernd

### Massnahmen bei technischen Problemen

Hier sind gefährliche technische Probleme und ihre Lösungen.

* Kabel reissen innert dem Telefon Neues Kabelbestellen und alte ersetzen
* Batterie Leer Neue Batterie kaufen und alte ersetzen
* Batterie ausgelaufen Telefon neu kreieren, sonst sehr gefährlich
* Lüfter defekt / überhitzt Neuer Lüfter kaufen und alter ersetzen
* Display defekt Neuer Display kaufen und alten ersetzen
* Tastatur Neue Tastatur /PCB/Kabel kaufen & ersetzen
* Boards kaputt (sehr unwahrscheinlich) Neue Boards kaufen oder gesamtes Telefon neu aufsetzen

### Anhang zum Supporthandbuch

Momentan haben wir noch keine Anhänge für das Supporthandbuch, da wir zum Beispiel keine Fehlermeldungen haben oder auch kein Glossar kreiert haben. Jedoch könnten in der Zukunft noch technische Erläuterungen oder sogar technische Übersichten angefügt werden. Wenn dies der Fall ist, werden wir dies in unserem Readme.md auf dem [GitHub](https://github.com/PetabyteBrain/BlackberryPi/blob/main/README.md) ergänzen!

# Systemtest

## Testspezifikation

### Kritikalität der Funktionseinheit

|  |  |  |
| --- | --- | --- |
| **Funktionseinheit** | **Kritikalität** | **Begründung** |
| Recheneinheit (Raspberry Pi) | Hoch | Ohne funktionierende Recheneinheit ist keine Systemfunktion möglich. |
| Stromversorgung (Akku) | Hoch | Das System ist ohne Stromversorgung nicht betriebsbereit. |
| Betriebssystem / Root-Zugriff | Hoch | Notwendig für alle weiteren Software-Tests und Anpassungen. |
| Tastatur (Hardware-Eingabe) | Mittel | Grundlegende Eingabe notwendig, jedoch durch Bildschirm ggf. ergänzbar. |
| WLAN | Mittel | Essentiell für viele Anwendungen, aber Systemstart auch offline möglich. |
| Gehäuse (3D-Druck) | Niedrig | Physisch wichtig, aber nicht kritisch für Softwarefunktionen. |

### Testanforderungen

Tests mit Normal-, Grenz- und Fehlerwerten.

Tests unter Ausnahmebedingungen (z. B. Akkuwechsel im Betrieb).

Alle Testergebnisse werden protokolliert.

### Testverfahren

Vorbereitung:

Komponenten anschließen, OS installieren, Stromversorgung sichern.

Durchführung:

Durchführung gemäß Testfalltabellen, manuell.

Auswertung:

Vergleich von Ist- mit Sollverhalten, Bewertung als „Bestanden / Nicht bestanden“.

### Testkriterien

Abdeckungsgrad: Mindestens ein Test pro Anforderung.

Checklisten: Alle Modul- und Systemfunktionen abgedeckt.

Ende-Kriterien: Keine Fehler in hochkritischen Modulen, System vollständig funktionsfähig.

### Testfälle

|  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- |
| **Nr.** | **AFo-Nr.** | **Anwendungsfall (ggf. orientiert an Use Cases)** | **Ausgangs­situation** | **Eingabe­daten** | **erwartetes Ergebnis** | **Bemerkungen, Prüfergebnis** |
| T1 | A5 | Akku ausstecken | Gerät ist ausgeschaltet | Akku entfernen und wieder einsetzen | Gerät startet wie erwartet | Es funktioniert wie erwartet |
| T2 | A6 | Gehäuse prüfen (3D-Druck) | Gehäuseteile vorhanden | Zusammenbauen | Teile passen genau, Gerät sitzt fest |  |
| T3 | A7 | WLAN-Verbindung testen | WLAN verfügbar | SSID + Passwort eingeben | Verbindung bleibt stabil | Wlan lässt sich verbinden und es bleibt verbunden |
| T4 | A2 | Tastatureingabe testen | System betriebsbereit | Text eingeben | Zeichen werden korrekt dargestellt | Tastatur funktioniert |
| T5 | A8 | Konfigurationsdatei ändern | config.yaml geladen | Parameter ändern | Änderung zeigt Auswirkungen im Verhalten | Dies funktioniert |
| T6 | A9 | Budgetprüfung | Komponentenliste vorhanden | Preise eintragen | Gesamtkosten ≤ 250 € |  |
| T7 | A10 | Nachbau mit Doku | Nur Dokumentation vorhanden | Gerät nach Anleitung bauen | Gerät funktioniert wie geplant |  |

## Testprozedur

### Vorbereitung

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

### Durchführung

Initialisierung: System einschalten oder vorbereiten (z. B. Komponenten einsetzen).

Durchführung: Entsprechend des Testfalls Eingaben tätigen, Komponenten prüfen, Funktionen aufrufen oder physikalische Veränderungen vornehmen.

Beobachtung: Reaktion des Systems oder Moduls beobachten.

Vergleich: Ergebnis mit dem erwarteten Resultat aus der Testspezifikation vergleichen.

Dokumentation: Testausgang (Erfolg, Fehler, Besonderheiten) direkt erfassen.

### Nachbearbeitung

Auswertung der Resultate:

Das Ergebnis wird direkt nach jedem Testschritt dokumentiert (z. B. Tabelle oder digitales Protokoll).

Wenn nötig, werden Screenshots, Fotos oder Log-Dateien als Beleg gesichert.

Fehlermeldungen:

Auffälligkeiten (z. B. keine Reaktion, Bootfehler) werden mit Uhrzeit und Beschreibung festgehalten.

Bei Abweichung vom Soll: Testwiederholung und Prüfung der Fehlerquelle.

Protokollierung:

Ergebnisse werden in der Testprotokoll-Tabelle eingetragen (siehe 4.3.2).

Jede Abweichung wird auch im Abschnitt Testauswertung (4.3.3) kommentiert.

## Testprotokoll

### Testobjekt

Testobjekt: Raspberry-Pi-basiertes System mit modularer Bauweise (Version: v1.0)

Testfall: T1 – Akku entfernen und wieder einsetzen

Tester: Nicolas Ammeter

Ort: Innovationlab

Datum: 23.04.2025

Uhrzeit: 14:10 – 14:15 Uhr

### Testresultate

|  |  |  |  |
| --- | --- | --- | --- |
| **Zeitpunkt** | **Handlung** | **Beobachtung** | **Bewertung** |
| 14:10 Uhr | System ist ausgeschaltet | Keine Aktivität sichtbar | Erwartungsgemäß |
| 14:11 Uhr | Akku entnommen | Kein Widerstand, Stecker gut gelöst | Erwartungsgemäß |
| 14:12 Uhr | Akku wieder eingesetzt | Verbindung sitzt fest | Erwartungsgemäß |
| 14:13 Uhr | Gerät eingeschaltet (Power-Button) | LED leuchtet, System startet korrekt | **Bestanden** |

Erwartetes Ergebnis laut Spezifikation: Gerät startet nach Akkueinbau fehlerfrei → erfüllt

Zwischenergebnisse: Keine Zwischenstörungen, keine Verzögerung beim Boot

### Testauswertung

Abweichungen zur Spezifikation: Keine

Einfluss auf Funktionalität: Keine Einschränkung festgestellt. System funktioniert einwandfrei nach Akku-Wiedereinbau.

Mögliche Fehlerursachen: Keine aufgetreten

Trendbeobachtung: Keine Häufung ähnlicher Fehler – Test zeigt, dass die modulare Stromversorgung zuverlässig funktioniert.

# Weiterführung der Projektplanung

## Abgleich von Planung und tatsächlichem Verlauf der Phase Konzept

Wir kamen gut voran, die Teamarbeit funktionierte meist sehr gut und als wir Probleme antrafen, verloren wir nie die Hoffnung und das Telefon ist ein Erfolg geworden.

## Aktualisierung der Risikosituation

Es gab keine Veränderungen an der Risikosituation, die aktuelle Version ist im [Konzeptbericht](https://github.com/PetabyteBrain/BlackberryPi/blob/main/docs/Konzeptbericht.md).

## Planung der nächsten Phase

Unsere nächsten Tage besprechen wir noch die Präsentation und erstellen auch noch den Abschlussbericht.

Dies sollte in etwa so erfolgen:

**Spyros:** Abschlussbericht, Demo Vorbereitung

**Nicolas:** Präsentation, Demo Vorbereitung

**Naomi:** Abschlussbericht

**Aram:** Präsentation