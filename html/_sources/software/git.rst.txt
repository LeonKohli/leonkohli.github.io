Versionsverwaltung mit GIT
========================== 

Neues Repository anlegen
------------------------ 
Einmalig für den Projektstart
::
   
   cd <mein/zielordner>
   git init --bare
   # Initialized empty Git repository in
   # //BEFS-00188-043.sz.zitbb.lvnbb.de/sz-daten$/Raum8/repos/name/


Kopie eines Repos
------------------  
Einmalig auf lokalem Laufwerk
::
   
   git clone O:\Raum8\repos\janneck
   git config --global user.name Janneck
   git config --global user.email janneck.lehmann@zit-bb.brandenburg.de
   

Jeden Tag, wenn neue Inhalte entstehen
-------------------------------------- 
::
   
   git status # was hat sich geändert
   git add .  # alles neue hinzufügen zum "Stash" 
   git reset  # wenn die Liste nicht korrekt ist
              # meist unerwünschte Dateien und Ordner
   git commit -m "ein einzeilieger Kommentar"
   git pull
   git push

Clone im ZIT nur mit Proxy
-------------------------- 
.. index:: Proxy
	   
::
   
   set http_proxy=10.128.9.30:80
   set https_proxy=10.128.9.30:80
