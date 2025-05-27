# __Git Anleitung__
### - von Anna, Iivo und Edgar -

## Zu Git

## Allgemeine Begriffe

## __Die wichtigsten Git Befehle__
## Setup eines Repositories

## Inspizieren

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