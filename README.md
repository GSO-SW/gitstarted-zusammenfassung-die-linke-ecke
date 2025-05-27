# __Git Anleitung__
### - von Anna, Iivo und Edgar -

## Zu Git

## Allgemeine Begriffe

## __Die wichtigsten Git Befehle__
## Setup eines Repositories
- git init
	Mit git init wird ein neues Repository im aktuellen Ordner erstellt. Es wird ein versteckter Ordner mit dem Namen .git erstellt.
- git clone
	Bei git clone wird eine Kopie eines remote Repositorys lokal erstellt. Um es zu *betreten* braucht es noch den git checkout Befehl. 

## Inspizieren

## Stagen und Arbeiten

- git add 
	fügt Änderungen an Dateien zur Staging-Area hinzu, damit sie im nächsten Commit erfasst werden.

- git reset
	fügt Änderungen an Dateien zur Staging-Area hinzu, damit sie im nächsten Commit erfasst werden. Es 	bereitet die Änderungen zum Speichern im Repository vor.

- git commit -m "Nachricht"
	 speichert die in der Staging-Area vorbereiteten Änderungen dauerhaft im lokalen Repository.

- git rm
	entfernt Dateien aus dem Arbeitsverzeichnis und der Staging-Area, sodass sie beim nächsten Commit gelöscht 	werden.

## Versionen und Branches
	fügt Änderungen an Dateien zur Staging-Area hinzu, damit sie im nächsten Commit erfasst werden. 
## Sharing und Updaten

- git push
	überträgt Commits vom lokalen Repository in das Remote-Repository. Dadurch werden Änderungen für andere 	verfügbar gemacht.

	- git push --set-upstream origing *branch*
		verknüpft zusätzlich den lokalen Branch mit einem Remote-Branch. Damit merkt sich Git das Ziel für 			zukünftige Push- und Pull-Befehle.

- git fetch
	holt alle Änderungen aus dem Remote-Repository, ohne sie in deinen aktuellen Branch zu übernehmen. Es 	aktualisiert nur die Referenzen zu den entfernten Branches.

- git pull
	holt Änderungen aus dem Remote-Repository und führt sie sofort mit deinem aktuellen lokalen Branch 	zusammen. Es ist eine Kombination aus git fetch und git merge.