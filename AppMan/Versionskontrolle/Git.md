### Inhalte
- [[Git|Grundlagen von Git]]
- [[Git#Grundlegende Befehle von Git|Grundlegende Befehle von Git]]
- [[Dateien ignorieren]]
- [[Branching]]
- [[Git Interna]]
#### Grundlagen von Git

Git ist ein Version Control System und der bekannteste Vertreter der distributed Version Control Systems.

#### Grundlegende Befehle von Git
- `git init` - Erstellt ein neues Git-Repository im aktuellen Ordner. Git Repositories werden durch den unsichtbaren `.git`-Ordner im Root-Verzeichnis des Repositories dargestellt und verwaltet. 
- `git clone <url>`- Klont ein Repository von einem Remote-Server, wie GitHub. Diesen Befehl nutzt man häufig, um ein vorhandenes Repository lokal zugänglich zu machen, wenn man daran arbeiten möchte.
- `git add <datei>` - Damit trackt man eine Datei. Man weist Git also an, diese Datei zu versionieren und Änderungen an dieser Datei zu beobachten.
- `git commit -m <nachricht>` - Man commitet alle Änderungen, die sich in der Staging-Area befinden, in das lokale Repository. Die Änderungen werden mit der in `<nachricht>` eingegebene Nachricht beschrieben. 
- `git status` - Hiermit kann man sich den aktuellen Status der Änderungen im Repository anzeigen. `Untracked`, `Tracked`, `Modified` und `Deleted` sind gültige Zustände, die Dateien in dieser Übersicht annehmen können.
- `git log`- Mit diesem Befehl kann man sich die Historie ansehen, also alle getätigten Commits, inklusive Autor. Mit der Option  `--graph` kann man die Historie als Graphen darstellen.
- `git pull` - Hiermit kann man sich alle Änderungen vom Remote-Repository herunterladen.
- `git push` - Mit diesen Befehl kann man seine lokalen Änderungen in das Remote-Repository überführen.
