---
title: Signed Numbers
---
Da das [[Binary|Binärsystem]] nur positive Zahlen darstellen kann, hat man sich "Signed" Zahlendarstellungen ausgedacht. Das erste Bit fungiert hier als Vorzeichen, also `+` oder `-`. Steht an der Stelle des MSB eine `0` hat man eine positive Zahl, während eine `1` eine negative Zahl bedeutet.

> [!example] Beispiele
> `1010` -> -2
> `0110` -> +6
> `0000` -> +0
> `1000` -> -0

Diese Schreibweise schränkt jedoch die Anzahl an darstellbaren Zahlen ein, da das MSB für das Vorzeichen reserviert ist. Die Range an verschiedenen Zahlen ist: $-2^{-N}-1$ bis $2^{N-1}-1$, wobei $N$ die Anzahl an Bits ist.

Mathematische Rechnungen mit dieser Schreibweise gehen nicht ganz auf. Deswegen gibt es [[Einerkomplement|Einer-]] und [[Zweierkomplement]], die versuchen dieses Problem zu beheben.