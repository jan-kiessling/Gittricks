# Git Cheat-Sheet
​
## Dinge anzeigen lassen
​
- `git status`
- `git branch`: zeigt alle branches an, aktuelle mit \* markiert
- `git log`: zeigt ausführlich alle Änderungen (commits), control+c zum verlassen
- `git log —-graph`: grafische Darstellung von commits & merges
- `glo`: Verkürzte Darstellung der commits, ist ein Alias, kein "normaler" Git Befehl
​
## Befehle für Workflow
​
- `git branch add-html`: Erstellt branch “add-html”
- `git switch add-html`: wechselt von aktueller branch in “add-html” (auch in VScode)
- `git add index.html`: Legt Änderungen der `index.html` Datei auf die Stage
- `git add .`: Alle Dateien auf Stage laden (meistens einfacher wenn nur 1 Datei)
- `git commit -m 'Commit message'`: committe die gemachten Änderungen
- `git push -u origin add-html`: Initiale Pushen von Branches, wenn sie remote (auf Github) noch nicht da sind
- `git push`: Weitere Änderungen zum remote Repository auf Github hinzufügen
- `git pull`: holt Änderungen vom remote Repository zum lokalen Repository
- `git branch -d <branchname>`: Löscht lokalen Branch
​
## Workflow
​
- Vermeiden auf `main` Branch direkt zu committen
- Auf Feature Branch arbeiten, z.B. `add-html`
- Wenn man mit Feature Branch durch ist, auf GitHub einen PullRequest erstellen
- Beim Merge eines PullRequests werden die Änderungen in den `main` Branch gespeichert (bisher nur remote)
- Lokal muss zum `main` Branch gewechselt werden (`git switch main`) und der aktuelle Stand vom remote Repository geladen werden (`git pull`)
- Lokal und remote den Featurebranch löschen
