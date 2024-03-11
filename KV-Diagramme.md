KV-Diagramme sind eine Art, Schaltungen bzw. logische Formeln zu vereinfachen. Um eine Vereinfachung durchzuführen, ist es ratsam, eine logische Formeln zunächst in die DNF zu bringen und anschließend die Min-Terme abzulesen. 

> [!warning] 
> Bei der Wahrheitstabelle ist wichtig, dass man die einzelnen Variablen rückwärts notiert. Die erste Zeile sieht also nicht so aus `A | B | C | Z`, sondern so `C | B | A | Z`

Nun bildet man eine KV-Map und nummeriert die einzelnen Felder nach der in der Vorlesung bekannten Methode durch. Werte für `Z` in der Wahrheitstabelle, die wahr sind, werden durch eine `1` im entsprechenden Feld der KV-Map repräsentiert, falsche Werte entsprechend mit `0` 

%%
TODO: Tabelle erstellen
%%

#### Vereinfachte Gleichung ablesen
Um aus einer vorliegenden KV-Map eine vereinfachte Form einer Gleichung abzulesen, bildet man lediglich die Primimplikanten, weist ihnen die jeweilige Variablen-Belegung zu, und-verknüpft diese neuen Min-Terme und bildet daraus in DNF-Form eine neue logische Gleichung