Studie

| Status | In Arbeit / In Prüfung / Abgeschlossen |
| --- | --- |
| Projektname | Blackberry Pi |
| Projektleiter | Spyros Catéchis |
| Auftraggeber | Kurt Järmann |
| Autoren | Aram A. Naomi B. Spyros C. |
| Verteiler | Kurt Järmann |

**Änderungskontrolle, Prüfung, Genehmigung**

| Version | Datum | Beschreibung, Bemerkung | Name oder Rolle |
| --- | --- | --- | --- |
| V 1 | 29.11.24 | Beginn Studie | Aram / Naomi / Spyros |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |

**Definitionen und Abkürzungen**

| Begriff / Abkürzung | Bedeutung |
| --- | --- |
| Pi | Raspberry Pi |
| BlackBerry Pi | Umbauprojekt: BlackBerry mit Raspberry Pi als Herzstück |
| AOSP | Android Open Source Projekt |

**Referenzen**

| Referenz | Titel, Quelle |
| --- | --- |
| [1] | Blackberry Pi Artikel |

**Inhaltsverzeichnis**

[1 Situationsanalyse 3](#_Toc183806603)

[1.1 Ausgangslage 3](#_Toc183806604)

[1.2 Stärken 3](#_Toc183806605)

[1.3 Schwächen 3](#_Toc183806606)

[2 Ziele 4](#_Toc183806607)

[2.1 Rahmenbedingungen 4](#_Toc183806608)

[2.2 Abgrenzung 5](#_Toc183806609)

[3 Liste der Stakeholder 6](#_Toc183806610)

[4 Anforderungen 8](#_Toc183806611)

[5 Lösungsvarianten 8](#_Toc183806612)

[5.1 Variantenübersicht 8](#_Toc183806613)

[5.2 Beschreibung der Varianten 10](#_Toc183806614)

[6 Bewertung der Varianten (Tabelle) 11](#_Toc183806615)

[7 Lösungsbeschreibung 11](#_Toc183806616)

[8 Projektplanung 14](#_Toc183806617)

[9 Empfehlung 14](#_Toc183806618)

[10 Projektfreigabe 14](#_Toc183806619)

**Abbildungsverzeichnis**

Abb. 1 : Gantt-diagramm ; Excel Tabelle, N.B.

# Situationsanalyse

## Ausgangslage

Die Telefone von BlackBerry waren einst die unangefochtenen Marktführer im Smartphone-Bereich und besonders beliebt bei Geschäftskunden, da sie eine physische Tastatur, hohe Sicherheit und effiziente E-Mail-Verwaltung boten. Mit der Einführung des iPhones und der Touchscreen-Revolution durch Apple verschob sich der Fokus der Nutzer jedoch weg von Tastaturen hin zu grossen, interaktiven Displays. BlackBerry verpasste es, sich schnell genug anzupassen, und verlor schliesslich seinen Platz als Marktführer.

Heute ähneln sich die meisten Smartphones in Design und Funktionalität, was die Vielfalt am Markt stark eingeschränkt hat. In dieser homogenen Welt sehen wir eine Chance, BlackBerry neu zu interpretieren und etwas Einzigartiges zu schaffen.

Die bewährte BlackBerry-Architektur und die physische Tastatur bieten weiterhin viele Vorteile, insbesondere für Nutzer, die ein Gerät mit einer "echten" Tasteneingabe bevorzugen. Durch den Einsatz eines Raspberry Pi als Kern können wir die klassische Hardware mit moderner Technik kombinieren und ein Smartphone kreieren, das sowohl funktional als auch innovativ ist. Dieses neue Gerät vereint das Beste aus zwei Welten: Die Retro-Ästhetik und Haptik eines BlackBerry mit der Flexibilität und Leistungsfähigkeit eines Raspberry Pi – und bringt endlich wieder ein „neues Format“ auf den Smartphone-Markt.

## Stärken

*   Da die meisten Handys heutzutage ähnlich aussehen, hätten wir mit der Ästhetik des Blackberrys und der Tastatur einen Vorteil, da es anders als das Produkt der Konkurrenz ist. Dieses aussehen kann einen attraktiven Verkaufspunkt für Blackberry Enthusiasten sein.
*   Dazu haben wir den Vorteil, dass wir unser Produkt Open Source behalten und deswegen jeder Nutzer genau wissen kann, was es beinhaltet und was er eingeht beim Gebrauch unserer Software.
*   Kosteneffiziente Hardware, Beispiel Raspberry Pi. Der Vorteil davon ist, dass die Reparaturen einfach vom Nutzer / einem Dienst gemacht werden können und günstiger wären als andere moderne Handys.
*   Das Blackberry Pi kann auch mit anderen Betriebssystemen laufen, solange es mit den Drivern und Hardware kompatibel ist.
*   Da es Open Source ist, kann es die Möglichkeit geben, Anpassungen am Gerät zu führen, um diese Benutzerspezifisch zu gestalten und zu entwickeln.

## Schwächen

Hohe Abhängigkeit von proprietärer Software (S1):

Viele Nutzer sind auf geschlossene OS (z.B. iOS, Android) angewiesen. Ein offenes, anpassbares System basierend auf Raspberry Pi kann die Abhängigkeit reduzieren.

Hohe Kosten moderner Smartphones (S2):

Premium-Smartphones sind oft sehr teuer. Ein DIY-Handy auf Basis eines Raspberry Pi bietet eine kostengünstige Alternative, insbesondere für technikaffine Nutzer.

Komplizierte Reparierbarkeit (S3):

Viele aktuelle Smartphones sind schwierig zu reparieren (z.B. durch verklebte Komponenten). Unser Projekt kann durch ein modulares Design mit leicht austauschbaren Teilen punkten.

Mangelnde Software-Upgrades bei älteren Geräten (S4):

Hersteller unterstützen ältere Modelle oft nicht mehr mit Updates, was Sicherheitsrisiken birgt. Ein offenes System erlaubt langfristige Pflege und Updates durch die Community.

Eingeschränkte Anpassbarkeit (S5):

Nutzer können Design, Funktionen und Hardware ihrer Smartphones nur begrenzt anpassen. Mit einem Raspberry Pi sind massgeschneiderte Anpassungen möglich.

# Ziele

Freie OS Wahl(Z1):

Mit einer freien resp. unabhängigen OS Wahl ist die Bandbreite des Blackberrys viel besser und man kann.

(referenziert S1)

Kosten & Marken (Z2):

Solange man nicht nur für die Marke bezahlt ist ein Smartphone schon sehr viel billiger, wenn wir dies mit simpler Technologie verknüpfen, bekommen wir ein einfaches Telefon und faires Preis-Leistung Verhältnis.

(referenziert S2)

Simple Technologie(Z3):

Da wir unser Blackberry Pi mit einem Raspberry Pi ausstatten, ein Screen und noch eine Tastatur hinzufügen ist das ganze Telefon sehr simpel und wenn ein Natel simpel ist, ist es auch simpel zum Reparieren. Was vor allem für ein kostengünstiges design ein Schlüsselziel ist.

(referenziert S3)

Sicherstellung langfristiger Software-Upgrades durch ein offenes System (Z4):

Das Projekt BlackBerry Pi zielt darauf ab, ein Smartphone mit einem offenen Betriebssystem zu entwickeln, das von der Community unterstützt werden kann. Dadurch wird es Nutzern ermöglicht, regelmässig Sicherheitsupdates und neue Funktionen zu erhalten, unabhängig von der Herstellerunterstützung. Dies reduziert Sicherheitsrisiken und verlängert die Nutzungsdauer des Geräts erheblich.

(referenziert S4)

Personalisierung(Z5):

Durch die simple Technologie und die freie OS-wahl ist das Natel individualisierbar. Das heisst der Nutzer kann alles personalisieren, eigene teile zum Telefon zusammenstellen. Wenn der Nutzer sehr viel Technik wissen hat, könnte er sogar zuhause sein Handy personalisieren.

(referenziert S5)

## Rahmenbedingungen

1.  **Zeitliche Rahmenbedingungen**

*   Projektzeitraum:

Das Projekt startet in **KW48** und endet in **KW17**. Innerhalb dieses Zeitraums werden alle wichtigen Meilensteine erreicht, darunter die Planung, praktische Umsetzung und abschliessende Präsentation.

*   Regelmässige Termine:

Wöchentliche Arbeitseinheiten finden im Rahmen des Praxistrainings am Freitagmorgen statt. Dieser regelmässige Zeitblock wird genutzt, um Fortschritte im Projekt zu erzielen und spezifische Aufgaben zu bearbeiten.

1.  **Räumliche Rahmenbedingungen**

*   Arbeitsort:

Die praktischen Arbeiten wie Zusammenbau, Tests und andere Projektschritte werden im Gibb Praxistraining durchgeführt. Hier stehen die notwendigen Ressourcen und Werkzeuge für die Umsetzung zur Verfügung.

1.  **Organisatorische Rahmenbedingungen:**

*   Verantwortlichkeiten:

Der Projektverantwortliche ist Michael Peter, der die übergreifende Koordination übernimmt.

Das Praxistraining wird vom Auftragsgeber geführt, der die praktische Umsetzung und Betreuung leitet.

## Abgrenzung

Die Abgrenzung definiert, welche Aspekte und Bereiche das Projekt _BlackBerry Pi_ nicht abdeckt, um den Umfang klar zu definieren und Missverständnisse zu vermeiden. Dies hilft, Fokus und Ressourcen gezielt einzusetzen. Im Folgenden werden einige Ideen und Beispiele aufgeführt:

1.  **Ideen zur Abgrenzung**

*   **Kommerzialisierung und Serienproduktion**
    *   Das Projekt ist rein prototypisch und wird keine grossflächige Serienproduktion oder Vermarktung umfassen.
    *   Beispiel: Es wird keine umfassende Marketingkampagne erstellt oder Logistik für den Verkauf organisiert.
*   **Entwicklung von Drittanbieter-Software**
    *   Das Projekt umfasst die Installation eines Betriebssystems, jedoch keine Entwicklung komplexer Software oder Apps von Grund auf.
    *   Beispiel: Die Anpassung bestehender Apps an das System wird nicht durchgeführt.
*   **Vollständige Kompatibilität mit BlackBerry-Diensten**
    *   Historische BlackBerry-Dienste wie BBM (BlackBerry Messenger) oder BlackBerry-Serverintegration werden nicht reaktiviert oder unterstützt.
    *   Beispiel: Die E-Mail-Push-Funktion von alten BlackBerry-Geräten wird nicht wiederhergestellt.
*   **Hardware-Optimierung auf Industrie-Standard**
    *   Es wird kein auf Effizienz oder Produktionskosten optimiertes Motherboard entwickelt, sondern ein Raspberry Pi genutzt.
    *   Beispiel: Statt einer massgeschneiderten Platine bleibt der Fokus auf der Integration bestehender Komponenten.
*   **Langfristiger Support und Wartung**
    *   Das Projekt wird keine langfristige Pflege des Betriebssystems oder regelmässige Updates garantieren.
    *   Beispiel: Sicherheitsupdates oder neue Features nach der Projektlaufzeit sind nicht vorgesehen.

1.  **Beispiele für typische Ausschlüsse bei einem solchen Projekt**

*   **Mobilfunkzertifizierung**
    *   Das Projekt wird keine umfassende Zertifizierung für den Einsatz in Mobilfunknetzen vornehmen.
    *   Beispiel: Keine Freigabe von Mobilfunkanbietern für LTE/5G.
*   **Multiplattform-Unterstützung**
    *   Es wird nicht darauf abgezielt, das Betriebssystem auf andere Geräte zu portieren.
    *   Beispiel: Der Prototyp bleibt auf das BlackBerry-Gehäuse beschränkt.
*   **Umfassende Benutzeroberfläche**
    *   Es wird keine voll ausgereifte Benutzeroberfläche wie bei kommerziellen Betriebssystemen erstellt.
    *   Beispiel: Minimalistische Funktionalität reicht aus, z. B. für grundlegende Kommunikation oder Terminal-Anwendungen.
*   **Hohe Produktionsqualität**
    *   Da es sich um einen Prototyp handelt, wird keine perfekte Anpassung oder Veredelung der Hardware erfolgen.
    *   Beispiel: Das Gehäuse könnte sichtbare Modifikationen wie Schraublöcher oder zusätzliche Kabel aufweisen.
*   **Komplette Rückwärtskompatibilität**
    *   Das Gerät wird nicht die Fähigkeit haben, alle historischen Funktionen und Anwendungen eines BlackBerry vollständig zu reproduzieren.
    *   Beispiel: Die originale BlackBerry-OS-Funktionalität wird nicht unterstützt.

1.  **Fazit zur Abgrenzung**

Die Abgrenzung soll verhindern, dass das Projekt über seine Kapazitäten hinauswächst. Der Fokus liegt auf einem funktionalen Prototyp, der die Idee eines BlackBerry-Smartphones mit Raspberry-Pi-Kern demonstriert. Bereiche wie Kommerzialisierung, umfangreiche Softwareentwicklung oder langfristiger Support bleiben bewusst ausserhalb des Projektumfangs.

# Liste der Stakeholder

Das Projekt _BlackBerry Pi_ hat verschiedene Stakeholder, die entweder direkt in die Entwicklung und Umsetzung einbezogen sind oder indirekt von den Ergebnissen des Projekts profitieren oder beeinflusst werden. Die Stakeholder lassen sich in folgende Kategorien unterteilen:

1.  **Primäre Stakeholder (direkt betroffen):**

*   **Kunde**
    *   Endnutzer des Geräts, die ein Interesse an einem Smartphone mit physischer Tastatur und modernem Betriebssystem haben.
    *   Erwartungen: Ein hochwertiges, funktionsfähiges und innovatives Gerät, das Retro-Charme mit moderner Technik verbindet.
*   **Entwickler & Projektmanager**
    *   Projektteam, bestehend aus Entwicklern und dem Projektleiter, das für die technische Umsetzung und die Organisation des Projekts verantwortlich ist.
    *   Erwartungen: Klare Anforderungen, Ressourcen, realistische Zeitpläne und Unterstützung durch den Auftraggeber.
*   **Auftraggeber**
    *   Kurt Järmann, der das Projekt ins Leben gerufen hat und als Schnittstelle zwischen Team und Kunde fungiert.
    *   Erwartungen: Ein funktionierender Prototyp, der die Machbarkeit des Konzepts beweist.

1.  **Sekundäre Stakeholder (indirekt betroffen):**

*   **Geldgeber & Investoren**
    *   Personen oder Institutionen, die die finanziellen Mittel bereitstellen, um die Entwicklung zu ermöglichen.
    *   Erwartungen: Transparente Kommunikation, nachvollziehbare Kostenpläne und eine realistische Aussicht auf zukünftige Renditen oder Marktinteresse.
*   **Technikbegeisterte**
    *   Enthusiasten und Maker, die sich für DIY-Technologie und innovative Hardwarelösungen interessieren.
    *   Erwartungen: Detaillierte Dokumentation und eventuell Open-Source-Freigabe der Projektdaten, um Nachbauten zu ermöglichen.
*   **Konkurrenten**
    *   Andere Unternehmen oder Projekte, die sich mit Retro-Technologie oder innovativen Smartphones beschäftigen.
    *   Erwartungen: Aufmerksamkeit auf dem Markt, Interesse an der Strategie und potenzielle Wettbewerbsvorteile durch eigene Innovationen.

1.  **Weitere Stakeholder:**

*   **Geschäftsleitung und betroffene Abteilungen der Stammorganisation**
    *   Interne Gruppen, die über den Fortschritt des Projekts informiert werden müssen, wie z. B. Marketing und Vertrieb, falls das Produkt kommerzialisiert wird.
*   **Ämter und Regulierungsbehörden**
    *   Institutionen, die eventuell für rechtliche Genehmigungen und Zertifizierungen bei einer möglichen Markteinführung des Geräts benötigt werden.
*   **Medien und Öffentlichkeit**
    *   Technologie-Journalisten und Interessierte, die über den Fortschritt und die Ergebnisse des Projekts berichten könnten.

1.  **Kommunikation mit Stakeholdern**

Es ist wichtig, regelmässig und zielgerichtet mit den Stakeholdern zu kommunizieren:

*   **Kunden** erhalten Updates über den Entwicklungsstand.
*   **Entwickler und Projektleiter** führen tägliche Abstimmungen durch.
*   **Geldgeber und Investoren** werden in Meetings über Budget und Fortschritte informiert.
*   **Technikbegeisterte** könnten über Blogs oder Foren eingebunden werden, um Feedback zu erhalten und Interesse zu wecken.
*   **Medien und Öffentlichkeit** werden über fertige Prototypen und Innovationen in einer Pressemitteilung informiert.

# Anforderungen

| Anforderung | Bezeichnung | Beschreibung | Ziel(e) |
| --- | --- | --- | --- |
| Offene Software-Architektur | A1 | Das System muss auf einem offenen Betriebssystem basieren, das langfristige Software-Upgrades und Anpassungen durch die Community ermöglicht. | Z1, Z4 |
| Modulares Hardware-Design | A2 | Das Telefon muss so konstruiert sein, dass Komponenten wie Display, Tastatur oder Akku einfach ausgetauscht oder aktualisiert werden können. | Z3 |
| Freie Betriebssystemwahl | A3 | Es soll möglich sein, verschiedene Betriebssysteme (z. B. Linux-Distributionen) auf dem Gerät zu installieren und zu nutzen. | Z1, Z5 |
| Kosteneffizienz | A4 | Die verwendeten Komponenten müssen günstig sein, sodass das Gerät ein faires Preis-Leistungs-Verhältnis bietet und unter den Kosten gängiger Smartphones bleibt. | Z2 |
| Einfache Reparierbarkeit | A5 | Das Telefon soll mit Standardwerkzeugen leicht zu reparieren sein, um die Lebensdauer zu verlängern und Nachhaltigkeit zu fördern. | Z3 |
| Hohe Anpassbarkeit | A6 | Nutzer sollen das Gerät sowohl in Hardware (z. B. Gehäuse-Design) als auch in Software (z. B. Benutzeroberfläche) individuell anpassen können. | Z5, Z1 |

# Lösungsvarianten

## Variantenübersicht

**1\. Gekauftes Handy von Blackberry**

*   **Beschreibung:  
    Erwerb eines bestehenden Modells, wie z. B. des BlackBerry Key2.**
*   **Vorteile:**
    *   **Fertiges Produkt ohne Entwicklungsaufwand.**
    *   **Sofort einsatzbereit und zuverlässig.**
    *   **Professionelles Design und getestete Hardware.**
*   **Nachteile:**
    *   **Hohe Kosten im Vergleich zum Eigenbau.**
    *   **Einschränkungen bei Anpassungen (Hard- und Software).**
    *   **Abhängigkeit von Hersteller-Updates und proprietären Systemen.**
*   **Link zur Beschreibung:  
    **[**BlackBerry Key2 auf Wikipedia**](https://en.wikipedia.org/wiki/BlackBerry_Key2)

**2\. Eigener Prototyp zusammenbauen**

*   **Beschreibung:  
    Eigenbau eines Blackberry-Pi-Handys durch die Kombination von modularer Hardware und frei verfügbarer Software.**
*   **a. Hardware**
*   **Komponenten:**
    *   **Raspberry Pi: Als Hauptrechner (z. B. Pi Zero 2 W oder Pi 4).**
    *   **Display: Kleines Touchscreen-Display (z. B. 3.5 Zoll LCD).**
    *   **Tastatur: Physische Tastatur (z. B. DIY-Module oder vorgefertigte Lösungen).**
    *   **Gehäuse: Eigenbau, z. B. aus 3D-Druckteilen.**
    *   **Zusatzmodule: Kamera, Akku, Lautsprecher und Mikrofon.**
*   **b. Software**
*   **Betriebssystem: Installation eines freien Betriebssystems wie Raspberry Pi OS, Ubuntu oder LineageOS.**
*   **Vorteile:**
    *   **Maximale Anpassungsfähigkeit und Kosteneffizienz.**
    *   **Open-Source-Software ermöglicht langfristige Updates und Pflege.**
    *   **Lern- und Innovationspotenzial.**
*   **Nachteile:**
    *   **Zeitintensiv und technisch anspruchsvoll.**
    *   **Mögliche Inkompatibilitäten zwischen Komponenten.**

**3\. Modifikation eines bestehenden Smartphones**

*   **Beschreibung:  
    Anpassung eines vorhandenen Smartphones, indem Software ersetzt wird und Hardware soweit möglich modifiziert wird.**
*   **a. Hardware-Anpassungen**
*   **Basisgerät: Nutzung eines alten oder kostengünstigen Smartphones, das bereits eine physische Tastatur besitzt (z. B. ältere Blackberry-Modelle).**
*   **Zusatzmodule: Externe Tastaturen, neue Gehäuse oder Austausch von Komponenten wie Akku.**
*   **b. Software-Anpassungen**
*   **Custom ROMs: Installation eines freien Betriebssystems wie LineageOS, /e/OS oder anderen angepassten Android-Versionen.**
*   **Optimierung: Entfernen von Bloatware und Hinzufügen von sicherheitsorientierten Apps.**
*   **Vorteile:**
    *   **Schneller und weniger zeitaufwendig als ein kompletter Eigenbau.**
    *   **Kosteneinsparung durch die Wiederverwendung bestehender Geräte.**
    *   **Direkter Fokus auf Nachhaltigkeit und Ressourcenschonung.**
*   **Nachteile:**
    *   **Begrenzte Anpassbarkeit der Hardware.**
    *   **Mögliche Inkompatibilitäten bei Softwaremodifikationen.**
    *   **Gerät bleibt abhängig von der ursprünglichen Hardwarequalität.**

**4\. Nutzung eines älteren Smartphones mit angepasstem Open-Source-Betriebssystem**

*   **Beschreibung:  
    Verwendung eines älteren, gebrauchten Smartphones (z. B. ein älteres Android-Gerät) und Installation eines offenen Betriebssystems wie LineageOS oder /e/OS. Dieses Vorgehen ermöglicht es, ein funktionales, kostengünstiges Smartphone zu erstellen, das an die eigenen Bedürfnisse angepasst werden kann, ohne ein Gerät von Grund auf neu zu bauen.**
*   **a. Hardware**
*   **Basisgerät: Ein günstiges, gebrauchtes oder älteres Smartphone (z. B. ein älteres Android-Gerät oder ein gebrauchtes Gerät von Marken wie Fairphone oder Nexus).**
*   **Anpassungen: Gegebenenfalls werden einfache Hardware-Anpassungen vorgenommen, wie der Austausch des Akkus oder das Hinzufügen von Zubehör (z. B. einer physischen Tastatur).**
*   **b. Software**
*   **Betriebssystem: Installation eines offenen, freien Betriebssystems wie LineageOS oder /e/OS. Diese Systeme bieten regelmässige Updates und die Freiheit, die Software an die eigenen Anforderungen anzupassen.**
*   **Optimierung: Entfernen von Bloatware, Anpassung der Benutzeroberfläche und Installation sicherer, funktioneller Apps.**
*   **Vorteile:**
*   **Kostenersparnis: Die Nutzung eines gebrauchten Smartphones ist deutlich günstiger als der Bau eines eigenen Geräts.**
*   **Schnelle Umsetzung: Die Anpassung eines bestehenden Geräts dauert weniger Zeit als der Eigenbau.**
*   **Zukunftssicher: Die Nutzung eines offenen Betriebssystems bedeutet, dass regelmässige Updates und Sicherheits-Patches von der Community bereitgestellt werden.**
*   **Nachhaltigkeit: Wiederverwendung und Recycling von Geräten verringert den Elektronikmüll.**
*   **Nachteile:**
*   **Begrenzte Anpassbarkeit der Hardware: Die Hardware kann nicht vollständig angepasst werden, da sie auf einem bestehenden Gerät basiert.**
*   **Abhängigkeit von der ursprünglichen Hardwarequalität: Das Endprodukt ist immer noch an die Begrenzungen der Originalhardware gebunden.**

## Beschreibung der Varianten

**1\. Eigener Prototyp zusammenbauen**

*   **Beschreibung**:  
    Der erste Schritt besteht darin, ein eigenes Gerät von Grund auf zu bauen, indem man Hardware und Software kombiniert. Der Hauptbaustein ist ein **Raspberry Pi**, auf dem ein offenes Betriebssystem läuft. Dazu kommen ein kleines Touchscreen-Display, eine physische Tastatur und eine individuelle Gehäusekonstruktion, die entweder selbst designt oder durch 3D-Druckteile erstellt wird. Die Komponenten wie Kamera, Lautsprecher und Mikrofon können ebenfalls je nach Bedarf hinzugefügt werden. Diese Variante bietet die grösste Anpassungsfreiheit, da sowohl die Hardware als auch die Software nach den eigenen Anforderungen gestaltet werden können.  
    Das Ziel ist es, ein funktionales Smartphone zu bauen, das langfristig pflegbar ist und mit den neuesten Software-Updates versorgt werden kann. Dies bedeutet jedoch, dass der Entwicklungsaufwand und die technische Komplexität relativ hoch sind.

**2\. Modifikation eines bestehenden Smartphones**

*   **Beschreibung**:  
    Bei dieser Variante wird ein bestehendes Smartphone verwendet, das bereits grundlegende Funktionen erfüllt, aber durch Modifikationen in Hardware und Software den individuellen Anforderungen angepasst wird. Als Basisgerät könnte ein älteres, kostengünstiges Modell gewählt werden. Eine typische Wahl sind Geräte mit physischen Tasten, wie die älteren **Blackberry-Modelle**.  
    In Bezug auf Software wird ein offenes Betriebssystem wie **LineageOS** oder **/e/OS** aufgespielt, um die Kontrolle über Updates und Anpassungen zu behalten. In der Hardware können Komponenten wie der Akku ausgetauscht oder eine externe Tastatur hinzugefügt werden, um die Bedienbarkeit zu verbessern. Diese Variante ist weniger aufwendig als der komplette Eigenbau, erfordert jedoch auch einige technische Fähigkeiten und bietet nicht die gleiche Flexibilität wie der Prototypenbau.

**3\. Nutzung eines älteren Smartphones mit angepasstem Open-Source-Betriebssystem**

*   **Beschreibung**:  
    Bei dieser Lösung wird ein älteres, gebrauchtes Smartphone genutzt, das mit einem Open-Source-Betriebssystem wie **LineageOS** oder **/e/OS** ausgestattet wird. Das Ziel ist es, ein funktionales Smartphone zu schaffen, das an die eigenen Bedürfnisse angepasst ist und von der Community regelmässig mit Updates versorgt wird. Hierbei liegt der Fokus auf der Software und der Minimierung der Bloatware, während die Hardware weitgehend unverändert bleibt.  
    Ein Vorteil dieser Lösung ist die Kosteneffizienz, da gebrauchte Geräte oft zu einem Bruchteil des Preises eines neuen Smartphones erhältlich sind. Es handelt sich um eine schnelle und nachhaltige Lösung, da alte Geräte wiederverwendet und für eine moderne Nutzung optimiert werden. Diese Variante ist besonders für Nutzer geeignet, die Wert auf ein einfaches, funktionales Gerät legen, ohne tief in die Hardware-Entwicklung eingreifen zu müssen.

**4\. Gekauftes Handy von Blackberry**

*   **Beschreibung**:  
    Die einfachste Variante besteht darin, ein bestehendes Modell, wie z. B. das **BlackBerry Key2**, direkt zu kaufen. Dies ist die Lösung mit dem geringsten Aufwand, da das Gerät sofort einsatzbereit ist. Die Blackberry-Geräte bieten eine bewährte Hardware, die für Business-Anwendungen und effiziente Textbearbeitung optimiert ist. Ein Vorteil dieser Option ist die Zuverlässigkeit des Produkts und das professionelle Design, das gut getestet ist.  
    Allerdings gibt es bei dieser Variante Einschränkungen, wenn es um die Anpassung der Software und die Kontrolle über Updates geht. Man ist weiterhin auf den Hersteller angewiesen, was in Bezug auf langfristige Updates und die Freiheit, das Gerät nach eigenen Wünschen zu gestalten, problematisch sein kann. Zudem sind die Kosten im Vergleich zu den anderen Varianten relativ hoch, und man zahlt auch für die Marke.

# Bewertung der Varianten (Tabelle)

| Kriterien | Gewichtung | Eigener Prototyp | Modifikation | Open-Source-Gerät | Blackberry kaufen |
| --- | --- | --- | --- | --- | --- |
| Anpassungsfähigkeit | 25% | 5 | 4 | 3 | 1 |
| Lernpotenzial & Innovation | 20% | 5 | 3 | 2 | 1 |
| Kosten | 20% | 3 | 4 | 5 | 2 |
| Unabhängigkeit | 15% | 5 | 3 | 3 | 1 |
| Komplexität | 15% | 2 | 4 | 5 | 5 |
| Nachhaltigkeit | 5% | 4 | 5 | 5 | 2 |
| Gesamtbewertung | 100% | 4.4 | 3.8 | 3.4 | 2.0 |

**1: Eigener Prototyp zusammenbauen (4.4 Punkte)**  
Diese Variante wird nun als beste Lösung bewertet, da sie maximale Anpassungsfähigkeit, Unabhängigkeit und Lernpotenzial bietet. Sie ist besonders geeignet für Projekte, die auf Innovation und langfristige Kontrolle abzielen.

**2: Modifikation eines bestehenden Smartphones (3.8 Punkte)**  
Eine solide Lösung mit hoher Nachhaltigkeit und moderatem Aufwand. Jedoch begrenzt in der Anpassungsfähigkeit im Vergleich zum Eigenbau.

**3: Nutzung eines älteren Smartphones mit Open-Source-Betriebssystem (3.4 Punkte)**  
Eine pragmatische, kostengünstige Lösung, die jedoch weniger Lernpotenzial und Hardware-Freiheit bietet.

**4: Gekauftes Handy von BlackBerry (2.0 Punkte)**  
Die schlechteste Option in diesem Szenario, da sie weder Anpassungsfähigkeit noch Unabhängigkeit bietet und teuer ist.

# Lösungsbeschreibung

Die gewählte Lösung ist der **Eigenbau eines Smartphones**, das vollständig auf den spezifischen Anforderungen basiert und maximal anpassbar ist. Der Hauptbaustein des Prototyps ist ein **Raspberry Pi**, der als zentrale Recheneinheit fungiert und ein offenes Betriebssystem wie **Raspberry Pi OS, Ubuntu** oder **LineageOS** ausführt. Dieser Ansatz ermöglicht es, sowohl die Hardware als auch die Software an die individuellen Bedürfnisse anzupassen.

1.  **Komponenten der Lösung**

*   **Hardware**
    *   **Raspberry Pi**: Der Hauptprozessor des Geräts, z. B. ein Raspberry Pi 4 oder Pi Zero 2 W, wird als Basis verwendet. Der Raspberry Pi bietet genügend Leistung für den Betrieb eines Smartphones und ermöglicht eine einfache Integration mit anderen Hardware-Komponenten.
    *   **Display**: Ein kleines Touchscreen-Display (z. B. 3,5 Zoll LCD) wird verwendet, um das Benutzerinterface darzustellen. Es wird direkt mit dem Raspberry Pi verbunden und ermöglicht eine einfache Bedienung des Geräts.
    *   **Physische Tastatur**: Um die Benutzerfreundlichkeit zu erhöhen, wird eine physische Tastatur verwendet, entweder als DIY-Modul oder vorgefertigte Lösung, was für die Zielgruppe, die Wert auf physische Tasten legt, von besonderem Vorteil ist.
    *   **Gehäuse**: Das Gehäuse wird entweder selbst designt oder durch 3D-Druckteile gefertigt, um das Gerät individuell anpassbar zu machen.
    *   **Zusatzmodule**: Für grundlegende Funktionen wie Fotoaufnahmen, Audioaufnahmen und Kommunikation werden Module wie **Kamera**, **Lautsprecher**, **Mikrofon** und **Akku** integriert. Diese Komponenten sind ebenfalls modular, sodass sie bei Bedarf einfach ersetzt oder aktualisiert werden können.
*   **Software**
    *   **Betriebssystem**: Das Betriebssystem wird entweder durch ein leicht anpassbares Open-Source-Betriebssystem wie **Raspberry Pi OS** oder eine andere freie Linux-Distribution wie **Ubuntu** oder **LineageOS** installiert. Diese Systeme ermöglichen eine langfristige Unterstützung und Updates durch die Open-Source-Community.
    *   **Anpassbarkeit**: Nutzer können sowohl die Benutzeroberfläche als auch die Systemsoftware individuell anpassen. Dies kann durch den Einsatz von benutzerdefinierten ROMs oder das Entfernen von Bloatware erfolgen, um das System zu optimieren und die Kontrolle über Updates zu behalten.
*   **Vorteile der Lösung**
    *   **Maximale Anpassungsfähigkeit**: Sowohl Hardware als auch Software sind vollständig anpassbar, sodass das Gerät genau nach den Bedürfnissen der Nutzer konzipiert werden kann. Dies umfasst Änderungen am Gehäuse, an der Benutzeroberfläche und an der Funktionalität.
    *   **Lernpotenzial & Innovation**: Der Eigenbau des Geräts bietet umfangreiche Lernmöglichkeiten im Bereich der Hardware- und Software-Integration. Dies fördert das Verständnis und die Kontrolle über die Technologie und ermöglicht kontinuierliche Innovationen.
    *   **Kostenersparnis**: Die Verwendung von Open-Source-Komponenten und kostengünstigen Bauteilen ermöglicht es, das Smartphone zu einem deutlich geringeren Preis zu bauen als der Kauf eines vergleichbaren Geräts auf dem Markt. Die Kosten für Komponenten sind niedriger als die für Marken-Smartphones.
    *   **Unabhängigkeit und Kontrolle**: Durch den Eigenbau behält man die vollständige Kontrolle über das Gerät. Das bedeutet, dass der Nutzer nicht von Herstellerupdates oder proprietären Softwarelösungen abhängig ist.
    *   **Einfache Reparierbarkeit**: Da das Design modular ist, können Komponenten wie Display, Tastatur, Kamera und Akku einfach ausgetauscht oder repariert werden, was die Lebensdauer des Geräts verlängert und zur Nachhaltigkeit beiträgt.
*   **Nachteile der Lösung**
    *   **Komplexität**: Der Eigenbau eines Smartphones ist technisch anspruchsvoll und zeitintensiv. Es erfordert Kenntnisse in der Hardware-Integration, Software-Installation und Problemlösung.
    *   **Mögliche Inkompatibilitäten**: Die Vielzahl von Komponenten und die Notwendigkeit, diese miteinander zu integrieren, können zu Inkompatibilitäten führen, was zusätzliche Anpassungen und Tests erfordert.
    *   **Entwicklungsaufwand**: Der Entwicklungsprozess für einen eigenen Prototypen ist langwierig und erfordert umfassende Planung und technische Fertigkeiten, um ein funktionierendes und robustes Gerät zu erstellen.

1.  **Überprüfung der Anforderungen**

| Anforderung | Beschreibung | Ziel(e) | Erfüllung |
| --- | --- | --- | --- |
| Offene Software-Architektur (A1) | Das System basiert auf einem offenen Betriebssystem, das langfristige Updates ermöglicht. | Z1, Z4 | Vollständig erfüllt |
| Modulares Hardware-Design (A2) | Komponenten wie Display, Tastatur und Akku können leicht ausgetauscht oder aktualisiert werden. | Z3 | Vollständig erfüllt |
| Freie Betriebssystemwahl (A3) | Verschiedene Betriebssysteme wie Linux-Distributionen können installiert werden. | Z1, Z5 | Vollständig erfüllt |
| Kosteneffizienz (A4) | Die verwendeten Komponenten sind günstig und das Gerät bleibt unter den Kosten eines gängigen Smartphones. | Z2 | Vollständig erfüllt |
| Einfache Reparierbarkeit (A5) | Das Gerät kann mit Standardwerkzeugen leicht repariert werden, wodurch es langlebig bleibt. | Z3 | Vollständig erfüllt |
| Hohe Anpassbarkeit (A6) | Nutzer können das Gerät sowohl in Hardware (z. B. Gehäuse) als auch in Software (z. B. UI) anpassen. | Z5, Z1 | Vollständig erfüllt |

1.  **Fazit**

Der Eigenbau eines Smartphones erfüllt alle relevanten Anforderungen, von der offenen Software-Architektur bis zur hohen Anpassbarkeit und Reparierbarkeit. Diese Lösung ist besonders geeignet, um die Ziele der Unabhängigkeit, Kosteneffizienz und Innovation zu erreichen. Trotz der höheren Komplexität bietet der Eigenbau eine langfristige Perspektive, die es ermöglicht, das Gerät kontinuierlich weiterzuentwickeln und an die eigenen Bedürfnisse anzupassen.

# Projektplanung

![A screenshot of a computer
Description automatically generated](data:image/png;base64,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)

Abb. 1 Gantt-diagramm

# Empfehlung

Wir empfehlen, das Projekt zugunsten des **Eigenbaus eines Prototypen** freizugeben. Diese Lösung ermöglicht eine massgeschneiderte, **offene Software-Architektur** und ein **modulares Hardware-Design**, das einfache Wartung und Reparatur sicherstellt. Der Eigenbau bietet maximale **Anpassungsfähigkeit** und **kostengünstige Komponenten**, während er gleichzeitig **Lernpotenzial** und **Innovationsmöglichkeiten** fördert.

Trotz des höheren Aufwands bietet der Eigenbau langfristig mehr Unabhängigkeit, Nachhaltigkeit und Flexibilität als der Kauf eines fertigen Produkts.

**Fazit:** Der Eigenbau stellt die beste Lösung dar, um das Projekt kostengünstig und zukunftssicher umzusetzen.

# Projektfreigabe

Hiermit bestätigt der Auftraggeber die Freigabe des Projekts:

­­­­­­­­­­­­­­­­­­­­­­\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Der Auftraggeber Der Projektleiter

(Ort, Datum, Unterschrift) (Ort, Datum, Unterschrift)