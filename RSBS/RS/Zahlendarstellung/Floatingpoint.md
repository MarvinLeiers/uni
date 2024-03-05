---
title: Gleitkommazahlen
---
Wir haben gelernt, wie man mithilfe des [[Zweierkomplement|Zweierkomplements]] negative Zahlen in binärer Schreibweise darstellt, mit denen man mathematisch korrekte Berechnungen durchführen kann. In diesem Kapitel werden die Charakteristiken der Gleitkommadarstellung im Binärsystem näher gebracht, um Kommazahlen darstellen zu können. 

Fließkommazahlen sind in dem Standard [IEEE754](https://en.wikipedia.org/wiki/IEEE_754) definiert.

Um eine dezimal-dargestellte Kommazahl in eine binäre Schreibweise zu überführen, geht man wie folgt vor.

1. Wandle Zahl vor dem Komma und Zahl nach dem Komma in Binär um.
2. Bilde den Exponenten, indem das Komma vor der ersten Ziffer steht.
3. Mantisse ablesen (Zahl hinter dem Komma).
4. Addiere den Bias (in der Vorlesung 127) auf den Exponenten und wandle in Binär um
5. Füge die Zahl zusammen. Nicht vergessen, die fehlenden Nullen zu ergänzen, um eine 32 Bit Zahl zu erhalten

Eine Fließkommazahl besteht aus einem Sign Bit an erster Stelle, also einem Bit, das anzeigt, ob die Fließkommazahl positiv oder negativ ist, dem Exponenten und der Mantisse.

> [!example] Beispiel anhand der Zahl 5,25
> 1. 5 -> `0101`. 0,25 -> `0100`
> 	 -> als Fixed Point Number -> `0101.0100`
> 2. Verschiebe das Komma um `2` Stellen -> `1.010100` * $2^2$
> 3. Mantisse -> `010100`
> 4. $2+127=129$ -> `10000001`
> 5. `0 10000001 010100000000000000000`
