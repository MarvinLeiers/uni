#### Dateien von Versionierung ausschließen
Manchmal möchte man Dateien von der Versionierung ausschließen. Diese Dateien könnten z.B sensible Daten wie Passwörter enthalten oder es könnte sich um Konfigurations-Dateien handeln, die nicht gepusht werden sollten, um die lokale Konfiguration der anderen Entwickler nicht zu überschreiben. 

Dafür kann man in Git eine spezielle Datei anlegen, die `.gitignore` heißt. In diese Datei kann man alle Dateinamen, Pfade und Datei-Beschreibungen schreiben, die von der Versionierung ausgeschlossen sein sollen. Ein Beispiel für eine `.gitignore`, die einige Dateien und Ordner ausschließt, könnte wie folgt aussehen:

```
# Ignoriere den Ordner .idea und alle sich darin befindlichen Dateien
.idea/  

# Ignoriere alle Ordner namens target und alle sich darin befindlichen Dateien
**/target/  

# Ignoriere alle Dateien mit der Dateiendung .iml
*.iml
```
> Diese `.gitignore` wird üblicherweise für versionierte Projekte in der IDE IntelliJ verwendet

