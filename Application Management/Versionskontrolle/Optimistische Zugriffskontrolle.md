Bei der optimistischen Zugriffskontrolle unterscheidet man zwischen dem klassischen Ansatz und dem modernen Ansatz.

#### Klassischer Ansatz:
Beim klassischen Ansatz wird die Ressource nicht für andere Personen gesperrt, sobald jemand einen checkout durchführt. Dies erlaubt das kollaborative Arbeiten an den versionierten Dateien. Aufgrund dieser Besonderheit erfordert der klassische Ansatz (der moderne auch), dass beim Checkout ein Merge durchgeführt wird, falls eine andere Person gleichzeitig Änderungen an der selben Datei vorgenommen hat. Dabei kann es zu sogenannten Merge-Konflikten kommen.

#### Moderner Ansatz:
Der moderne Ansatz der optimistischen Zugriffskontrolle verfügt wie der klassische Ansatz über die Möglichkeit, kollaborativ an den versionierten Objekten zu arbeiten und erfordert ebenfalls einen Merge. Der Unterschied zum klassischen Ansatz ist, dass jede Person zusätzlich zum Remote-Repository ein lokales Repository hat, das erlaubt den Zugriff auf die versionierten Objekte ohne eine Internetverbindung. Außerdem gibt es eine Staging Area, in denen veränderte Objekte zum Commit vorgemerkt werden können. 

Ein anderer Ansatz der Zugriffskontrolle ist die [[Pessimistische Zugriffskontrolle]].