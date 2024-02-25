#### Zentralisierte Zugriffskontrolle
Bei der zentralisierten Zugriffskontrolle existieren die versionierten Objekte auf einem einzigen Server (Remote-Repository) und sind über das Internet erreichbar. Der Vorteil von solchen zentralisierten ist, dass es erreichbarer als lokale Repositorys ist und aufgrund der oftmals besser ausgestatteten Server, Speicher für größere Dateien ermöglicht. Nachteile sind, dass es einen Single Point of Failure gibt, falls der Server mal nicht wie erwartet funktionieren bzw. erreichbar sein sollte. Beispiele für zentralisierte Zugriffskontrollen sind [SVN](https://subversion.apache.org/)

#### Distributed Version Control Systems
Bei den distributed (verteilten) Version Control Systems hat jeder Client, also jeder Entwickler, eine lokale Kopie des gesamten Repositorys, inklusive der gesamten Historie. Das beseitigt das Problem des Single Point of Failures, den es bei der zentralisierten Zugriffskontrolle gibt. 

Ein berühmtes Beispiel dieser Art von Version Control Systemen ist [[Git]]

#### Vorteile von VCS
Einige Vorteile von VCS sind:
- Änderungen der Dateien werden gespeichert
- Änderungen können nachvollzogen werden (Wer hat sie gemacht?)
- Änderungen können wiederhergestellt werden
- [[Pessimistische Zugriffskontrolle]]
- [[Optimistische Zugriffskontrolle]]
