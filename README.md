Name des Projekts:	Deep Learning mit Keras API

Link zum MyBinder: 	[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/HuseyinBgn/6DeepLearning/HEAD)

Doku:	

Die Beispiele der Übungsaufgabe befinden sich in dem Deep_Learning.ipynb Datei.
Die erwarteten Ergebnisse sind unterhalb der jeweiligen Befehle dargestellt. 

Hinweis: Um das erwartete Ergebnis nicht zu verlieren wird empfohlen eine Zwischenzeile zw. dem Befehl 
und dem bereits stehendem Ergebnis hinzufügen bevor das Befehl ausgeführt wird!

Zum Ausführen der einzelnen Code-Zeilen "STRG" + "Enter" Tasten drücken.
Beachten Sie keine der Zeilen zu überspringen, denn sonst kann es zu Fehlerhaften Ausführung führen.

1. Libraries installieren & importieren: 
- Librairies für die Datenverarbeitung und -visualisierung werden installiert und anschließend importiert.

2. Die Daten:
- Lending_club_info.csv Datei wird gelesen.
- Lending_club_loan_two.csv Datei wird gelesen.
- Mit der .info() Befehl wird angezeigt, welche Spalten die Tabelle enthält und dessen Datentypen.

3. Explorative Datenanalyse:
- Countplot von "loan_status". Status der Darlehen, Abgebucht oder vollständig abbezahlt.
- Histogramm von "loan_amnt". Anzahl der Darlehen je nach höhe.
- Korrelationstabelle von der Tabelle Lending_Club_loan_two.
- Heatmap der obigen Tabelle.
- Nutzung der feat_info() Methode um die Beschreibung der "installment" und "loan_amnt" zu bekommen.
- Scatter Plot von "installment" und "loan_amnt".
- Boxplot der "loan_amnt" unterteilt in "loan_status".
- Gruppierung nach "loan_status" und Nutzung der describe() Methode für alle relevanten statistischen Werte.
- Untersuchung der Spalten "Grade" und "Subgrade". 
- Countplot von "Grade", unterteilt nach "loan_status".
- Countplot von "Subgrade".
- Dasselbe Countplot wie oben, diesmal unterteilt nach "loan_status".
- Countplot der "Subgrade" Spalte, gefiltert nach Grade F und G und unterteilt nach "loan_status".
- Hinzufügen neuer Spalte. 1 wenn fully paid, 0 wenn charged off.
- Barplot von "loan_repaid"

4. Fehlende Daten:
- Anzeigen welche Spalten keine Daten enthalten.
- Konvertierung in Prozent
- Anzahl einzigartigen Arbeitsplatzbezeichnungen gesamt.
- Anzahl einzigartigen Arbeitsplatzbezeichnungen einzeln.
- Verwerfen der Spalte "empt_title".
- Countplot der Spalte "emp_length" (Anstellungsdauer) in Jahren.
- Dasselbel Countplot von oben, diesmal nochmal in "loan_status" aufgeteilt.
- Untersuchung auf Zusammenhang zwischen Anstellungsdauer und Rückzahlungen.
- Barplot des Zusammenhangs.
- Verwerfung der Spalte "emp_length".
- Betrachtung nach wiederholende Informationen bei der Spalte "purpose" und "title".
- Verwerfung der Spalte "title".
- Analyse von Spalte "mort_acc". 
- Korrelation der Splate "mort_acc".
- Gruppierung der Spalte "total_acc" und deren Durchschnittswerte.
- Durchschnittlicher Werte von Spalte "total_acc" ist 2.
- Entfernen der Zeilen mit fehlenden Werten mit dropna() Methode.

5. Kategorische Variablen und Dummyvariablen:
- Zeige alle Spalten, die ein Datentyp von "Objekt" sind.
- Spalte "term" wird in Datentyp Integer umgewandelt.
- Spalte "grade" wird verworfen. 
- "Subgrade", "verification_status", "application_type", "initial_list" und "purpose" werden in Dummyvariablen konvertiert.
- Originalspalten werden verworfen.
- Kategorien von Spalte "home_ownership" werden auf 4 reduziert.
- Spalte "address" wird extrahiert und in "zip_code" umgenannt.
- Spalte "zip_code" wird als Dummyvariable umkonvertiert. Originalspalte und "address" Spalte werden verworfen.
- "issue_d" Spalte wird verworfen.
- "earliest_cr_line" Spalte wird extrahiert. und in ein numerisches Feature umgewandelt. Anschließend wird die Originalspalte verworfen.
- Zuletzt erkennt man, dass nur noch Splate "loan_status" ein Typ Objekt ist.
- Auch diese Splate wird verworfen. 

6. Aufteilung in Trainings- und Testdaten:
- 20% der Daten werden als Testdaten getrennt.

7. Daten normalisieren:
- Normalisierung der Daten.

8. Modell erzeugen:
- Ein künstlich neuronales Netz wird erzeugt.
- Input Layer, d.h. die Anzahl der Anfangsknoten sind hier 78.
- 2x Hidden Layer, d.h. die Layer zw. Input und Output. 1. HL hat 39 Knoten, 2. HL hat 19 Knoten. 
- Output Layer mit einem Ergebnis. 
- "Dropouts" geben die Gewichtung/Wichtigkeit der Kanten an.
- "Activation" sind die Funktionen, die verwendet werden. Hier ReLU und Sigmoid Funktionen.
- Anschließend wird das künstlich neuronale Netz mit fit() Methode mit Trainingsdaten trainiert.
- Das Modell wird in einer .h5 Datei gespeichert.

9. Evaluation der Leistung des Modells:
- Visualisierung Verlust der Validierung gegen Verlust des Trainings.
- Durch predict() Methode soll das Modell vorhersagen.
- Klassifikationsreport und Konfusionsmatrix des Modells werden angezeigt.
- Kontrolle ob das Ergebnis tatsächlich gestimmt hat.