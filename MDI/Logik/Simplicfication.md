---
title: Vereinfachen von logischen Ausdrücken
---
Das Ziel bei der Vereinfachung von logischen ist die Reduktion der Anzahl von atomaren Ausdrücken. Oft kann man Zusammensetzungen verschiedener Ausdrücke innerhalb der Formel zusammenfassen bzw. ganz rauskürzen. Einige Regeln, die man dazu anwenden kann sind hier dargstellt:

- Oder-Regeln: 
	- `A+w` ist immer wahr.
	- `A+f` ist immer gleich dem Wert von A.
- Und-Regeln:
	- `Aw` ist immer gleich dem Wert von A.
	- `Af` ist immer falsch.
- Kommutativ-Gesetz (Vertauschgesetz):
	- `A+B = B+A` 
	- `AB = BA` 
- Assoziativ-Gestz (Klammergesetz):
	- `(A+B)+C = A+(B+C)`
	- `(AB)C = A(BC)`
- Distributiv-Gestz (Ausklammern):
	- `A(B+C) = AB+AC`
	- `A+(BC) = (A+B)(AC)`
- Komplementär-Gestz:
	- `A+¬A = w`
	- `A¬A = f`
- Absorbtions-Gesetz:
	- `A+(AB) = A`
	- `A+(¬AB) = A+B`
	- `A(A+B) = A`
	- `A(¬A+B) = AB`