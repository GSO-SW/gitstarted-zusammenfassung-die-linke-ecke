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
- git log
	Der Befehl git Log zeigt die Commit-History des aktuellen Branches. Jeder Eintrag enthält die Commit Nachricht, Hash-Wert, Autor*in und Datum.
- git status
	Bei git status erhält man einen Überblick über das aktuelle Working Directory und den Staging-Bereich. Man sieht welche Changes gestaged sind und welche Dateien nicht.

## Stagen und Arbeiten

## Versionen und Branches

## Sharing und Updaten

- git push
	überträgt Commits vom lokalen Repository in das Remote-Repository. Dadurch werden Änderungen für andere 	verfügbar gemacht.

	- git push --set-upstream origing *branch*
		verknüpft zusätzlich den lokalen Branch mit einem Remote-Branch. Damit merkt sich Git das Ziel für 			zukünftige Push- und Pull-Befehle.

- git fetch
	holt alle Änderungen aus dem Remote-Repository, ohne sie in deinen aktuellen Branch zu übernehmen. Es aktualisiert 	nur die Referenzen zu den entfernten Branches.

- git pull
	holt Änderungen aus dem Remote-Repository und führt sie sofort mit deinem aktuellen lokalen Branch zusammen.
	Es ist eine Kombination aus git fetch und git merge.