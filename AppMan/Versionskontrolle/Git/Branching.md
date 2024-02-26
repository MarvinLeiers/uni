 Die meisten der VCS unterstützen Branches. Mit Branches kann man von der Hauptlinie eines Repositories abzweigen und kann seine Arbeit fortsetzen, ohne die Hauptline (Master-Branch) zu beeinflussen. Dies kann besonders hilfreich sein, wenn man neue Features austesten möchte oder um die Arbeit zwischen Entwicklern zu unterteilen, sodass sie sich nicht gegenseitig beeinflussen. 

#### Wichtige Befehle bezüglich Branching
- `git branch <name>` - Erzeugt einen neuen Branch mit dem angegebene Namen. Dieser Branch ist zu Beginn eine Kopie des Branches, auf dem man den Befehl ausgeführt hat.
- `git checkout <name>` - Mit diesem Befehl wechselt man zu einem existieren Branch, mit der Option `-b` erstellt man einen neuen Branch und wechselt gleichzeitig zu diesen Branch.
- `git merge <name>` - Dieser Befehl wird benutzt, um einen Branch in einen anderen zu mergen. Der Branch `<name>` wird in den Branch, auf dem man diesen Befehl ausführt, integriert. 
- `git branch -d <name>` - Mit diesem Befehl kann löscht man einen Branch.

#### Merge Konflikte
Nicht immer ist ein Merge erfolgreich. Werden von zwei unterschiedlichen Entwicklung an der gleichen Datei widersprüchliche Änderungen vorgenommen, weiß git nicht, welche Änderungen bei einem Merge übernommen werden sollen. In solchen Szenarien müssen die Merge Konflikte manuell von einem Entwickler behoben werden. Dabei wird entschieden, welche Änderungen in die finale Datei übernommen und welche Änderungen verworfen werden sollen.