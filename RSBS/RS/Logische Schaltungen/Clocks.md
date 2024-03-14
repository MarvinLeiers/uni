Clocks sind Bauelemente logischer Schaltungen, die als Taktgeber fungieren. Sie generieren einen gleichmäßigen Rhythmus von elektrisch steigenden und sinkenden Kanten:![[rsbs-clock.png]]
Man benötigt Clocks um einen einheitlichen Puls / Takt vorzugeben, anhand dessen verschiedene Elemente synchronisiert werden können. 

#### Pulsgenerator
Durch geschicktes Kombinieren von Bauteilen, lässt sich ein Pulsgenerator bauen, der gebraucht werden kann, um kurze Impulse in regelmäßigen Abständen zu erzeugen. Folgendermaßen kann ein Pulsgenerator realisiert werden:
![[rsbs-pulse_generator.png]]
Aufgrund der Verzögerung des Negationsbauteiles sind bei Umschalten der Clock kurzzeitig beide Eingänge des Und-Gatters wahr, was dazu führt, dass der Ausgang kurz aktiviert ist.