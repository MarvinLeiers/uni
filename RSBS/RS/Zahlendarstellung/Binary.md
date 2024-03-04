---
title: Binärsystem
---
Zahlen im Binärsystem bestehen aus den Ziffern "0" und "1". Eine Ziffer innerhalb einer Zahl wird als Bit bezeichnet. Das Bit ganz links wird als Most-Significant-Bit (MSB) bezeichnet, während das Bit ganz rechts als Least-Significant-Bit (LSB) bezeichnet wird. 

#### Umwandlung ins Dezimalsystem

> [!info]
> Häufig ist es sinnvoll, die Zahl zuerst in das Dezimalsystem umzuwandeln, bevor man sie in das Zielsystem umwandelt.

Um eine Binärzahl in eine Dezimalzahl umzuwandeln, weist man den jeweiligen Bits eine Wertigkeit zu. Dabei fängt man bei der Wertung mit dem LSB an und arbeitet sich von rechts nach links zum MSB vor. Die Wertung der Bits geschieht in Zweierpotenzen, also 1, 2, 4, 8, 16, 32… 

Nun addiert man die zugeordneten Wertigkeiten der Bits, multipliziert mit dem Wert des Bits zu einer Summe. Diese Summe ist die Repräsentation der Binärzahl im Dezimalsystem.

> [!example] Beispiel
> Die Binärzahl `0101` soll in das Dezimalsystem überführt werden.
> 
> 1. Weise den Bits ihre Wertigkeit zu (von rechts nach links): 1 -> 1, 0 -> 2, 1 -> 4, 0 -> 8
> 2. Bilde die Summe: $1*1 + 0*2 + 1*4 + 0*8 = 5$
> 
> Damit ist die Dezimaldarstellung von `0101` gleich 5.








