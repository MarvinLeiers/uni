SR-Latches funktionieren ähnlich wie normale [[Latch|Latches]], erweitern diese jedoch um eine `Reset-Funktionalität`, um den Zustand des Speichers zurückzusetzen. Ein SR-Latch sieht folgender Maßen aus: 
#### SR-Latch mit NOR-Gattern
![[rsbs-sr_latch.png]]

Ein SR-Latch besteht aus zwei Inputs. Einem Reset-Knopf und einem Set-Knopf. Mit dem Set-Knopf kann man den Speicher setzen, während der Reset-Knopf zu zurücksetzen des Speichers dient. 

Auf folgende Weise können die Zustände des SR-Latches manipuliert werden

| $Q^T$ | $Q^{T+1}$ | $R^T$ | $S^T$ |
|:-----:|:---------:|:-----:|:-----:|
|   0   |     0     |   -   |   0   |
|   0   |     1     |   0   |   1   |
|   1   |     0     |   1   |   0   |
|   1   |     1     |   0   |   -   |
- Zeile eins liest man z.B wie folgt: Um den Zustand den Input so anzupassen, dass sich der Zustand Q von `0` nicht verändert, ist es egal, was am Reset-Input anliegt, wichtig ist, das S `0` ist.
- Zeile zwei liest man: Um den Zustand von Q von `0` zu `1` zu verändern, muss Reset `0` sein und Set `1`. 

#### SR-Latch mit NAND-Gattern
NAND-Gatter bieten eine geringere logische Komplexität, weswegen sie gerne benutzt werden. Ein SR-Latch würde mit NAND-Gattern so aussehen:
![[rsbs-sr_latch_nand.png]]
>[!warning] Hinweis
>Beachte, dass die Inputs invertiert sind und die Positionen getauscht haben!

#### Problematische Zustände
Angenommen, S und R sind beide `0`. Dann kommt es zu einer Race-Condition, bei der der Ausgang nicht definiert ist. Da dies unerwünscht ist, kann man folgende Änderungen am Latch vornehmen, um ein enabled D-Latch zu erhalten, das dieses Problem löst:
![[rsbs-enabled_d_latch.png]]
#### Erklärung (enabled) D-Latch:
Der rechte Teil ist äquivalent zum SR-Latch. Der linke Teil ist neu hinzugekommen.

Das Problem beim SR-Latch war, dass die Inputs S und R rein theoretisch den selben Wert annehmen könnten, also beide `0` oder beide `1` und damit ungültige Zustände verursachen. Um dem entgegenzuwirken ersetzt man nun S und R durch einen einzigen Input, nämlich D. Damit für S und R unterschiedliche Inputs kommen, wird D einmal negiert und einmal nicht negiert weitergegeben. Die Signale werden jedoch nur weitergereicht, sofern das Latch enabled ist (Input E = `1`).