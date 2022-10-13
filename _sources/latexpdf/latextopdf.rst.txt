================== 
Latex to PDF
==================


Aus der Sphinx Doku eine PDF erstellen
----------------------------------------------------- 

:: 

    make latex 


Installation
--------------------- 

| Auf Windows 
| -PERL installieren
|   https://strawberryperl.com/
| -MikTeX Package Manager installieren
|   https://miktex.org/download
|   -in der GUI unter 'Pakete' latexmk installieren
|   -Im ZIT muss ein Proxy gesetzt werden -> Ändern und Verbindungseinstellungen
::
    
      10.128.9.30:80


latexmk ausführen
-----------------  

latexmk ist ein cmd programm und läuft in der Konsole

Um es im Latex file Ordner auszuführen öffnet man CMD der Befehl ist
:: 
    
    latexmk

Dann werden alle .tex Datein im Ordner berücksichtigt

Wenn man sicher gehen möchte einen .pdf Datei zu bekommen tippt man 

::
    
    latexmk -pdf

Wenn man nur spezifische .tex Datein Konvertieren möchte 

::
    
    latexmk datei.tex

Wenn man dauerhaft seine Änderungen als PDF Konvertiert haben möchte 

::
   
   latexmk -pvc 

Um im Ordner aufzuräumen und alle temporären Datein zu löschen

::
    
    latexmk -c