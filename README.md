# __Git Anleitung__
### - von Anna, Iivo und Edgar -

## Zu Git

VCS (Version Control Systems) sind Systeme die für die Erfassung und Aufzeichnungen von Veränderungen (meißtens von Dateien) verantwortlich sind. Git ist ein VCS, welches schnelle und einfacher Verzweigung (Branching) und Zusammenführung dieser Zweige (Merging) erlaubt.

## Allgemeine Begriffe

* __Repositories__

    Ein Git Repository ist ein Speicherort, an dem der Quellcode eines Projekts sowie alle Änderungen und deren Historie gespeichert werden. Es dient als Werkzeug zur Versionskontrolle, mit dem Entwickler Änderungen am Code verfolgen, verwalten und gemeinsam bearbeiten können.
   
* __Branches__

    Ein Branch ist eine Art Abzweigung für Commits. Es können mehrere Branches erstellt werden für unterschiedliche Teile der Entwicklung. Auf diese Branches wird dann commited. Die Änderungen existieren dann getrennt von einander, bis sie zusammengefügt werden. (Merging)

* __Working Directory__

    Die Working Directory ist der Speicherort der aktuellen Versionen, deiner Dateien. Dein lokales Repository.

* __Staging Area__

    Die Staging Area ist ein Bereich von Git wo drin gespeichert wird welche Dateien beim nächsten commit mit einbezogen werden.

* __Historie__

    Die Historie ist die vollständige Aufzeichnung aller Änderungen der Dateien der jewailigen Branches.

## __Die wichtigsten Git Befehle__
## Setup eines Repositories
- __git init__

	Mit git init wird ein neues Repository im aktuellen Ordner erstellt. Es wird ein versteckter Ordner mit dem Namen .git erstellt.

- __git clone__

	Bei git clone wird eine Kopie eines remote Repositorys lokal erstellt. Um es zu *betreten* braucht es noch den git checkout Befehl. 

## Inspizieren
- __git log__

	Der Befehl git Log zeigt die Commit-History des aktuellen Branches. Jeder Eintrag enthält die Commit Nachricht, Hash-Wert, Autor*in und Datum.

- __git status__

	Bei git status erhält man einen Überblick über das aktuelle Working Directory und den Staging-Bereich. Man sieht welche Changes gestaged sind und welche Dateien nicht.

## Stagen und Arbeiten
- __git add__

	fügt Änderungen an Dateien zur Staging-Area hinzu, damit sie im nächsten Commit erfasst werden.

- __git reset__

	fügt Änderungen an Dateien zur Staging-Area hinzu, damit sie im nächsten Commit erfasst werden. Es bereitet die Änderungen zum Speichern im Repository vor.

- __git commit -m "Nachricht"__

	 speichert die in der Staging-Area vorbereiteten Änderungen dauerhaft im lokalen Repository.

- __git rm__

	entfernt Dateien aus dem Arbeitsverzeichnis und der Staging-Area, sodass sie beim nächsten Commit gelöscht 	werden.

## Versionen und Branches
- __git branch (Name)__

	Mit git branch (Name) wird ein neuer Branch mit dem angegebenen Namen erstellt. Dabei bleibt man im aktuellen Branch. Um zum neuen Branch zu wechseln muss man separat git checkout benutzen.

- __git checkout__

	Wechselt zu einem anderen Branch oder bestimmten Commit. Man muss entweder den Hash oder einen Branchnamen angeben.

- __git merge__

	Bei git merge (branch) wird ein Merge des angegebenen Branches in den aktuellen Branch durchgeführt. 

- __git rebase__

	integriert Änderungen eines Branches, indem es dessen Commits auf einen neuen Ausgangspunkt umsetzt. Dadurch wird die Projektgeschichte geglättet und übersichtlicher, ohne einen Merge-Commit zu erzeugen.

- __git cherry-pick__

	übernimmt einen bestimmten Commit aus einem anderen Branch und fügt ihn in den aktuellen Branch ein. Dabei wird nur dieser eine Commit angewendet, ohne den ganzen Branch zu mergen.

## Sharing und Updaten

- __git push__

	überträgt Commits vom lokalen Repository in das Remote-Repository. Dadurch werden Änderungen für andere 	verfügbar gemacht.

	- git push --set-upstream origing *branch*
		verknüpft zusätzlich den lokalen Branch mit einem Remote-Branch. Damit merkt sich Git das Ziel für 			zukünftige Push- und Pull-Befehle.

- __git fetch__

	holt alle Änderungen aus dem Remote-Repository, ohne sie in deinen aktuellen Branch zu übernehmen. Es 	aktualisiert nur die Referenzen zu den entfernten Branches.

- __git pull__
	
	holt Änderungen aus dem Remote-Repository und führt sie sofort mit deinem aktuellen lokalen Branch 	zusammen. Es ist eine Kombination aus git fetch und git merge.