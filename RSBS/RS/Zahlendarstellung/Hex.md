---
title: Hexadezimalsystem
---
Zahlen im Hexadezimalsystem bestehen aus den Ziffern 0-9 und A-F, wobei A-F den Ziffern 10, 11, 12, 13, 14 und 15 entsprechen. Da die Folge von 1 und 0 (`10`) nicht von einer Zehn unterschieden werden kann, hat man die Buchstaben A-F als Ergänzung eingeführt. ^80dc02

#### Umwandlung ins Dezimalsystem

> [!info]
> Häufig ist es sinnvoll, eine hexadezimale Zahl zuerst in das Binärsystem umzuwandeln, bevor man sie in das Zielsystem umwandelt.

Um eine Zahl des Hexadezimalsystems in eine binäre Zahl umzuwandeln, geht man wie folgt vor: Man betrachtet die hexadezimalen Ziffern einzeln und wandelt diese dann gesondert in das Binärsystem um. Eine hexadezimale Ziffer entspricht genau 4 Bit. Den Ziffern weist man Wertigkeiten zu. Die Wertigkeiten bei Zahlen-Ziffern entspricht genau der Ziffer selbst. Bei Buchstaben-Ziffern entspricht die Wertigkeit der Ziffer, wie im [[Hex#^80dc02|ersten Paragraphen]] angegeben. Diese Wertigkeiten der einzelnen Ziffern wandelt man dann in Binärzahlen um und die Binärzahlen wie [[Binary|hier]] beschrieben in das Dezimalsystem. 

> [!example] Beispiel
> Die hexadezimale Zahl `FC` soll in eine Dezimalzahl umgewandelt werden. Dafür konvertieren wir die Zahl zunächst in das Binärsystem und vom Binärsystem in das Dezimalsystem
> 
> `F`  hat die Wertigkeit 15 (in Binär `1111`)
> `C` hat die Wertigkeit 12 (in Binär `1100`)
> 
> Demnach ist die binäre Darstellung von FC `1111 1100`, was 252 im Dezimalsystem entspricht.

