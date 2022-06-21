Name des Projekts:	Keras_Projekt

Link zum MyBinder: 	[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/HuseyinBgn/6DeepLearning/HEAD)

Doku:	

Die Beispiele der Übungsaufgabe befinden sich in dem Keras_Projekt.ipynb Datei.
Die erwarteten Ergebnisse sind unterhalb der jeweiligen Befehle dargestellt. 

Hinweis: Um das erwartete Ergebnis nicht zu verlieren wird empfohlen eine Zwischenzeile zw. dem Befehl 
und dem bereits stehendem Ergebnis hinzufügen bevor das Befehl ausgeführt wird!

Zum Ausführen der einzelnen Code-Zeilen "STRG" + "Enter" Tasten drücken.
Beachten Sie keine der Zeilen zu überspringen, denn sonst kann es zu Fehlerhaften Ausführung führen.


1. Libraries installieren & importieren: 
- Hier werden die Librairies für die Datenverarbeitung und -visualisierung installiert und anschließend importiert

2. Die Daten:
- Lending_club_info.csv Datei wird gelesen.
- Lending_club_loan_two.csv Datei wird gelesen.
- Mit der .info() Befehl wird angezeigt, welche Spalten die Tabelle enthält und dessen Datentypen.




3. Explorative Datenanalyse:
- Histogram von "Age" wird erstellt. 
- Ein Jointplot, das den "Area Income" mit "Age" vergleicht.
- Ein Jointplot mit KDE Verteilung, der den "Daily Time Spent on Time" mit "Age" vergleicht.
- Ein weiteres Jointplot mit grüner Farbe, diesmal ein Vergleich zw. "Daily Time Spent on Time" und "Age".
- Pair Plot von "Clicked on Ad".

4. Optional:
- Die Daten werden in Trainings und Testset aufgeteilt.
- Anschließend werden die Trainingsdaten auf dem Künstlich Neuronalen Netz trainiert.

5. Modell erzeugen:
- 

6. Evaluation der Leistung des Modells:
- Nun wird das Künstlich Neuronale Netz mit Testdaten getestet. Es soll die Werte voraussagen.
- Ein Klassifizierungsreport für das Model wird erstellt.