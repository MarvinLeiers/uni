Ein Latch ist ein sehr einfaches Element logischer Schaltungen zur Speicherung von Zuständen. Latches bestehen aus einem Oder-Gatter, das zwei Inputs und zwei Outputs hat. Der erste Input ist die Benutzereingabe. Der erste Output ist der Status, der den Zustand der Speicherung angeben soll. Der zweite Output des Oder-Gatters führt als zweiter Input in das selbe Oder-Gatter: ![[rsbs-latch.png]]
Schaltet man `Input 1` nun auf 0, verändert sich der Output des Oder-Gatters nicht, da `Input 2`  immer noch 1 ist. 

Entscheidener Nachteil dieser Konstruktion ist, dass der Zustand nicht zurückgesetzt werden kann. Ist der Zustand des Latches also einmal auf `1`, kann er nicht wieder auf `0` geändert werden.

>[!info] SR-Latches
>[[SR-Latch|SR-Latches]] lösen dieses Problem, in dem sie ein Setzen (`S`) und zurücksetzen (`R`) des Zustands erlauben.