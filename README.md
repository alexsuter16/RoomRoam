# RoomRoam
Guidelines zur Projektarbeit im Modul
«Anwendungsentwicklung mit Python»
1. Allgemeines
Dieses Modul beinhaltet projektbasiertes Lernen der Konzepte der Programmierung mit der
Programmiersprache Python. Die Konzepte werden anhand des Anwendungsszenarios eines
Hotelreservierungssystems eingeführt.
Die Projektarbeit im Modul ist eine Gruppenarbeit, die in mehreren Iterationen durchgeführt
wird (siehe Semesterplan). In jeder Iteration werden Programmierkonzepte eingeführt,
beginnend mit grundlegenden Konzepten bis hin zu fortgeschritteneren Konzepten, die
benötigt werden, um die Anforderungen des Anwendungsszenarios auf agile Weise zu
erfüllen. Die Anforderungen für die Projektarbeit wurden in Form einer Reihe von vordefinierten
User Stories (siehe unten) bereitgestellt. Die Lektionen sind unterteilt in 2 Stunden interaktive
Programmierung, gefolgt von 2 Stunden Anwendung auf die Projektarbeit oder das Üben der
Konzepte (mit Coaching durch den Dozenten).
Die Modulbenotung für jeden Studierenden am Semesterende errechnet sich aus zwei Teilen:
• Abgabe der Projektarbeit - Die Projektarbeit wird mit einer Note zwischen 1 und 6 bewertet
und fliesst zu 70% in die Gesamtnote des Moduls ein. Diese Projektarbeit führt zu einer
Gruppennote. Falls sich die Beteiligung einer Person erheblich vom Gruppenbeitrag
unterscheidet, können die Bewerter/innen eine gesonderte Bewertung vornehmen. (das
Bewertungsraster ist unten im Appendix einsehbar).
• Individuelle schriftliche Prüfung: Die schriftliche Einzelprüfung findet während der
offiziellen Prüfungszeit statt und muss über die MooPad-Prüfungsinfrastruktur der
Hochschule für Wirtschaft FHNW abgelegt werden. Die MooPad-Prüfung wird mit einer
Note zwischen 1 und 6 bewertet und geht zu 30% in die Modulgesamtnote ein. Die
Enthält iPad-kompatible Fragen über die Anwendung der Programmierkonzepte.
Die Studierenden müssen beide Teile mit einer Note von mindestens 4,0 bestehen.
2. Inhalt und Projektphasen
Einfache User Stories aus einem «Mediastore» dienen als Grundlage für die Lektionen. In der
Projektarbeit werden die Studierenden das Hotelreservierungssystem durch die Umsetzung
der gegebenen User Stories weiter ausbauen. Je nach Interesse der Gruppenmitglieder kann
eine Gruppe nach Absprache mit einem Dozenten die User Stories anpassen oder erweitern.
Die Endabgabe der Gruppe umfasst den funktionalen Code und die entsprechende
Dokumentation (siehe «Deliverables» unten). Die Abgabe der Projektarbeit wird im
Semesterplan als "Abgabe" gekennzeichnet.
2
3. Deliverables
Der Abgabetermin für die Projektarbeit ist auf Moodle angegeben. Dabei gibt jedes Team
Folgendes an:
- Source Code und Artefakte
o Link zum Deepnote-Projekt mit allen ausführbaren Notebooks, Dateien und der
endgültigen Datenbank,
o Link zum GitHub-Repository,
o Link zu einer Projekt Board
- Dokumentation/Bericht (Link zu GitHub Markdown-Datei(en))
- Link zum Präsentationsvideo (das auf Microsoft Stream, SWITCHtube oder YouTube
gehostet wird; eingeschränkter/ungelisteter Zugang möglich und empfohlen). Es wird
empfohlen, dass jedes Teammitglied an der Videopräsentation beiträgt.
Bereitstellung des erforderlichen Zugangs für alle Dozenten/Coaches.
4. Verwendete Software
Im Unterricht werden u.a. folgende Tools verwendet (siehe Abschnitt «Tools» auf Moodle):
• Modellierung: Visual Paradigm v.17.2: Damit wird das Class-diagramm erstellt. Zur
Nutzung gibt es eine akademische Lizenz.
• Datenbank: SQLite (https://sqliteonline.com/)
• Deepnote: Als Cloud-basierte Projekt mit “Computational Notebooks”
, Zusammenarbeit,
Ergebnisse und entsprechende Dokumentation (Notebooks). Zur Nutzung gibt es eine
akademische Lizenz.
• GitHub: Versionskontrolle, Zusammenarbeit, und Gesamtdokumentation (READ.me).
5. User Stories «Hotelreservierungssystem»
Dieser Abschnitt enthält eine Liste von minimalen und optionalen User Stories, die im
Rahmen dieser Projektarbeit implementiert werden sollten.
Minimale User Stories
Die folgenden User Stories decken die grundlegenden Anforderungen für dieses Projekt
ab und können mit der mitgelieferten «hotel_reservation_sample.db» umgesetzt werden.
1. Als Gast möchte ich die verfügbaren Hotels durchsuchen, damit
ich dasjenige auswählen kann, welches meinen Wünschen
entspricht. Wünsche sind:
1.1. Ich möchte alle Hotels in einer Stadt durchsuchen,
damit ich das Hotel nach meinem bevorzugten Standort
(Stadt) auswählen kann.
1.2. Ich möchte alle Hotels in einer Stadt nach der
Anzahl der Sterne (z.B. mindestens 4 Sterne) durchsuchen.
1.3. Ich möchte alle Hotels in einer Stadt durchsuchen,
die Zimmer haben, die meiner Gästezahl entsprechen (nur 1
Zimmer pro Buchung).
3
1.4. Ich möchte alle Hotels in einer Stadt durchsuchen,
die während meines Aufenthaltes ("von" (check_in_date)
und "bis" (check_out_date)) Zimmer zur Verfügung haben,
damit ich nur relevante Ergebnisse sehe.
1.5. Ich möchte Wünsche kombinieren können, z.B. die
verfügbaren Zimmer zusammen mit meiner Gästezahl und der
mindest Anzahl Sterne.
1.6. Ich möchte die folgenden Informationen pro Hotel
sehen: Name, Adresse, Anzahl der Sterne.
2. Als Gast möchte ich Details zu verschiedenen Zimmertypen
(Single, Double, Suite usw.), die in einem Hotel verfügbar
sind, sehen, einschliesslich der maximalen Anzahl von Gästen
für dieses Zimmer, Beschreibung, Preis und Ausstattung, um eine
fundierte Entscheidung zu treffen.
2.1. Ich möchte die folgenden Informationen pro Zimmer
sehen: Zimmertyp, max. Anzahl der Gäste, Beschreibung,
Ausstattung, Preis pro Nacht und Gesamtpreis.
2.2. Ich möchte nur die verfügbaren Zimmer sehen, sofern
ich meinen Aufenthalt (von – bis) spezifiziert habe.
3. Als Admin des Buchungssystems möchte ich die Möglichkeit haben,
Hotelinformationen zu pflegen, um aktuelle Informationen im
System zu haben.
3.1. Ich möchte neue Hotels zum System hinzufügen
3.2. Ich möchte Hotels aus dem System entfernen
3.3. Ich möchte die Informationen bestimmter Hotels
aktualisieren, z. B. den Namen, die Sterne usw.
4. Als Gast möchte ich ein Zimmer in einem bestimmten Hotel
buchen, um meinen Urlaub zu planen.
5. Als Gast möchte ich nach meinem Aufenthalt eine Rechnung
erhalten, damit ich einen Zahlungsnachweis habe.
Hint: Fügt einen Eintrag in der «Invoice» Tabelle hinzu.
6. Als Gast möchte ich meine Buchung stornieren, damit ich nicht
belastet werde, wenn ich das Zimmer nicht mehr benötige.
Hint: Sorgt für die entsprechende Invoice.
7. Als Gast möchte ich eine dynamische Preisgestaltung auf der
Grundlage der Nachfrage sehen, damit ich ein Zimmer zum besten
Preis buchen kann.
Hint: Wendet in der Hochsaison höhere und in der Nebensaison
niedrigere Tarife an.
8. Als Admin des Buchungssystems möchte ich alle Buchungen aller
Hotels sehen können, um eine Übersicht zu erhalten.
9. Als Admin möchte ich eine Liste der Zimmer mit ihrer
Ausstattung sehen, damit ich sie besser bewerben kann.
10. Als Admin möchte ich in der Lage sein, Stammdaten zu verwalten,
z.B. Zimmertypen, Einrichtungen, und Preise in Echtzeit zu
aktualisieren, damit das Backend-System aktuelle Informationen
hat.
4
Hint: Stammdaten sind alle Daten, die nicht von anderen Daten
abhängen.
User Stories mit DB-Schemaänderung
Die folgenden User Stories erfordern eine Änderung des Datenbankschemas, z.B. das
Hinzufügen neuer Tabellen, die Definition neuer Beziehungen und die Generierung
neuer Daten. Implementiert mindestens zwei der folgenden User Stories oder fügt
eure eigenen User Stories hinzu, so dass ihr mindestens eine neue Tabelle, eine
entsprechende Beziehung und Daten hinzufügen müsst.
1. Als Admin möchte ich alle Buchungen bearbeiten können, um
fehlende Informationen zu ergänzen (z.B. Telefonnummer).
2. Als Gast möchte ich auf meine Buchungshistorie zuzugreifen
("lesen"), damit ich meine kommenden Reservierungen verwalten
kann.
2.1. Die Anwendungsfälle für meine Buchungen sind
"neu/erstellen", "ändern/aktualisieren",
"stornieren/löschen".
3. Als Gast möchte ich nach meinem Aufenthalt eine Bewertung für
ein Hotel abgeben, damit ich meine Erfahrungen teilen kann.
4. Als Gast möchte ich vor der Buchung Hotelbewertungen lesen,
damit ich das beste Hotel auswählen kann.
5. Als Gast möchte ich für jeden Aufenthalt Treuepunkte sammeln,
die ich dann für Ermässigungen einlösen kann.
Hint: Nur häufige Gäste sollten Treuepunkte erhalten.
Definieren Sie eine Regel, um häufige Gäste zu identifizieren.
6. Als Gast möchte ich meine Buchung mit der von mir bevorzugten
Zahlungsmethode bezahlen, damit ich meine Reservierung
abschliessen kann.
User Stories mit Datenvisualisierung
In den folgenden User Stories geht es um die Visualisierung von Daten mit dem
Deepnote-Block «Charts» (https://deepnote.com/docs/chart-blocks). Man muss die
Ergebnisse einer SQL-Abfrage in einem «Dataframe» speichern und eine geeignete
Visualisierung auswählen. Wählt eine der folgenden User Stories oder definiert eine
eigene User Story, in der ihr Daten mit dem «Charts»-Block visualisieren könnt. Ihr
könnt euch an einer einfachen Anleitung orientieren, um die passende Visualisierung zu
wählen, z.B. https://www.atlassian.com/data/charts/how-to-choose-pie-chart-vs-bar-
chart .
1. Als Admin möchte ich die Belegungsraten für jeden Zimmertyp in
meinem Hotel sehen, damit ich weiss, welche Zimmer am
beliebtesten sind und ich meine Buchungsstrategien optimieren
kann.
Hint: Wählt ein geeignetes Diagramm, um die Auslastung nach
Zimmertyp darzustellen (z. B. wie oft jeder Zimmertyp gebucht
wird).
5
2. Als Admin möchte ich eine Aufschlüsselung der demografischen
Merkmale meiner Gäste sehen, damit ich gezieltes Marketing
planen kann.
Hint: Wählt ein geeignetes Diagramm, um die Verteilung der
Gäste nach verschiedenen Merkmalen darzustellen (z. B.
Altersspanne, Nationalität, wiederkehrende Gäste).
Möglicherweise müssen Sie der Tabelle „Gäste“ einige Spalten
hinzufügen.
Optionale User Stories
Die Umsetzung der folgenden User Stories erfordert zusätzliche Untersuchungen oder
Selbststudium, z. B. Dateiverarbeitung, Bibliotheksintegration oder andere
fortgeschrittene Konzepte. Wenn Ihr Euch selbst herausfordern wollt, wählt aus diesen
User Stories, aber erst nachdem Ihr die minimalen User Stories implementiert habt!
1. Als Admin möchte ich die Gesamteinnahmen meines Hotels sehen,
damit ich die finanzielle Leistung des Hotels analysieren kann.
1.1. Zeigt die Gesamteinnahmen (Revenue) an, die sich aus
allen Buchungen für einen bestimmten Zeitraum ergeben.
1.2. Eine zeitliche Aufschlüsselung (z. B. Umsatz nach
Monat, Quartal, Jahr) bereitstellen.
Hint: Füge eine Trendlinie ein, um zu veranschaulichen,
wie sich die Einnahmen im Laufe der Zeit verändern.
2. Als Gastnutzer möchte ich die Details meiner Reservierung in
einer lesbaren Form erhalten (z.B. die Reservierung in einer
dauerhaften Datei speichern), damit ich meine Buchung später
überprüfen kann.
Hint: Erzeugt eine «booking.txt»-Datei oder verwendet die
Python-Bibliothek «fpdf» oder eine ähnliche Library, um eine
PDF-Version zu erzeugen.
3. Als Gastnutzer möchte ich eine Karte mit Zoom- und
Filterfunktion sehen können, welche Sehenswürdigkeiten oder
Restaurants in der Nähe meines gebuchten Hotels liegen, um
meine Aufenthaltsplanung zu erleichtern.
Hint: Verwende die Python-Bibliothek «geopandas» oder eine
ähnliche.
4. Als Gastnutzer möchte ich ein Zimmer buchen und eine
Buchungsbestätigung mit allen Details per E-Mail erhalten, um
einen verbindlichen Nachweis meiner Reservierung zu haben.
Hint: Verwende die Python-Bibliothek «smtplib» oder eine
ähnliche.
6. Verwendung von generativen Tools wie ChatGPT
In diesem Modul geht es auch darum, etwas zu lernen. Daher empfehlen wir, generative Tools
mit Bedacht einzusetzen. Wir sind der Meinung, dass diese Tools zur Unterstützung genutzt
werden sollten, um Unklarheiten zu beseitigen und euch auf die Coaching-Session
vorzubereiten. Betrachtet die generativen Tools als eine Art «Stützräder» und nicht als Ersatz,
6
der die Arbeit für euch erledigt. Während der Coaching-Session werden wir gezielt darauf
achten, ob ihr den Inhalt der Unterrichtseinheiten verstanden habt und euer Vorgehen im
Projektverlauf kontinuierlich hinterfragen. Auf diese Weise müsst ihr auch während der
Coaching-Session mit Wissen glänzen.
Wenn ihr diese Tools aus irgendeinem Grund verwendet haben, geben Sie bitte eine
angemessene Begründung und die entsprechenden Aufforderungen in Ihrer
Projektdokumentation an. Stellen wir fest, dass der Einsatz von Tools sich negativ auf das
Lernen der Gruppe oder eines Einzelnen auswirkt,
