---
title: Addition von Fließkommazahlen
---
Um zwei Fließkommazahlen zu addieren, muss zuerst sichergestellt werden, dass diese über einen gemeinsamen Exponenten verfügen. In der Regel passt man dabei den kleineren Exponenten an den größeren an und verschiebt die Mantisse entsprechend.

>[!tip] Hinweis
>Bei der Verschiebung der Mantisse ist zu beachten, dass diese über eine führende `1` verfügt, die nach Verschiebung nicht vergessen werden darf.

>[!example] Beispiel
>Zu addieren sind in Binärschreibweise die Dezimalzahlen `404,5` und `5,25`
>- `404,5` entspricht der binären `0 10000111 100101001…` mit einem Exponenten von `8`.
>- `5,25` entspricht der binären `0 10000001 0101…` mit einem Exponenten von `2`.
>  
>Jetzt bildet man die Differenz der Exponenten und erhält `6`. Die Mantisse der kleineren Gleitkommazahl (`5,25`) verschiebt man nun um `6` Stellen. Die führende eins darf nicht vergessen werden!
>
>-> `0 10000001 0000010101…`
>
>Diese Zahlen kann man nun einfach addieren und erhält:
>`0.0000010101…` +
>`1.1001010010…`
>-> 
>`1.1001100111…`


