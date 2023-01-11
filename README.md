# EGA-handlings
These files a used to process EGA csv files. e.g., to put them in a structure to use them in other applications.

Hier die ERläutereungen: leider geht die Tabellenformatierung verloren ❗ 

Erstellen eines Excelsheets aus dem Grid-Export für die VB10:
Aufgabe	Details	Kommentare / Hinweise
Daten aus csv-Datei auslesen mit final:	→ Bevor die Daten aus der CSV-Datei ordentlich ausgelesen werden können, muss die ursprüngliche csv-Datei mit Excel geöffnet und Text in Spalten convertiert werden.	
ConvertEGA-CSVIntoExcel.ipynb 	→ Dann kann sie wieder als CSV gespeichert werden.
	→ Diese muss dann in muss dann in das Google-Drive Verzeichnis EGA-handlings übertragen werden.
in G:\Meine Ablage\EGA-handlings	  
Generierung neuer Spalten und umformatieren der Spalteninhalte	die angegebene ConvertEGA-CSVIntoExcel.ipynb liest die csv-Datei aus.	
	        - Die Spalten werden neu angeordnet
	        - Hazard Type leer wird Chapter eingefügt.
	        - Aus 'Hierarchy #' wird: 'Section', 'Chapter', 'Function', 'Hazard', 'Cause', 'Measure',
	        - Headline & Requirement wird in H & R gekürzt
	        - Wird eine erste Exce-Datei und csv-Datei erstellt.
Headline der Excel-Datei formatieren und Spalten gruppieren & Abspeichern in "Resultdata"	→ Liste mit Spalten, die gruppiert werden sollen.	
	✅>>> ToDo: Liste mit der üblichen VB10 Gruppierung final festlegen.
	→ Excel-Datei mit den gruppierten Spalten wird erneut abgespeichert.
	ACHTUNG: es dauert einen Moment, bis die Excel-Datei nach dem Speichern verfügbar ist.
	        
Öffnen der generierten Excel-Datei
Format: Req-Grid VB10 EGA v03 --- Datum - Uhrzeit.xlsx	Beim Öffnen dieser Datei muss in Daten > Gliederung > Richtung > 'Hauptzeilen unter Detaildaten' & 'Hauptspalten rechts von Detaildaten' weggeklickt/deaktiviert werden.
Das ist zwar auch im Python-Code gemacht. Dennoch funktioniert dies beim ersten Öffnen der Excel-Datei nicht.	
	Nach dem Speichern ist die Datei dann final für den Einsatz  im Projekt.
	Dort können noch weiere Formatierungen vorgenommen werden.
Sicherungskopien	Es gibt verschiedene Sicherungskopien (in G:\Meine Ablage\Colab Notebooks) mit ähnlichem Namen, bei denen unterschiedlicher Code verwendet wurde.	
	Hier kann eventuell für die Zukunft Code übernommen werden.
	Die finale Version ist auf das absolute Minimum reduziert.
	
Daten in GitHub sichern	✅>>> ToDo: Sicherung der Daten in GitHub	
