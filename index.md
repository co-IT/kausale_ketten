# Kausale Kette 1

**What**: Unverständlicher "Spaghetti Code"

**How**: Niedrige Kohäsion und hohe Kopplung

**Why**: Tell, don't ask verletzt

**Beispiel:** Der Zweck des Codes ist nur schwer verständlich und die Wartbarkeit ist schlecht, was daran liegt, dass Logik, die eigentlich zusammengehört, um den Use Case bzw. die Intension verstehen zu können, über mehrere Klassen und Methoden verteilt ist. Dabei wird häufig abhängig von dem Zustand eines anderen Objekts unterschiedliche Logik ausgeführt. Das wiederum erhöht die Kopplung des einen Objekts an das andere. Das zu Grunde liegende Probleme ist, dass der Status in der einen Klasse gehalten wird, während die passende Logik dazu in einer anderen steht, statt gemäß OOP-Prinzipien beides zusammenzuhalten.


# Kausale Kette 2

**What**: Unzufriedene Kunden

**How**: Missverständnisse mit der FA

**Why**: Keine gemeinsame Sprache

**Beispiel:** Der Kunde ist mit den Ergebnissen unzufrieden, weil er der Meinung ist, dass es anders besprochen wurde. Hintergrund sind Missverständnisse zw. der Fachabteilung und den Entwicklern, weil Begriffe unterschiedlich interpretiert wurden. Das zu Grunde liegende Problem ist eine fehlende gemeinsame Sprache.

# Kausalte Kette 3

**What**: Viele Bugs

**How**: Falsche Nutzung möglich

**Why**: Implementation First Ansatz verwendet

**Beispiel:** Die Applikation gibt regelmäßig Fehler aus bzw. die meiste Zeit der Entwickler geht für Bugfixing drauf. Hintergrund sind ungültige Aufrufe und Objektzustände, die der konsumierenden Code produziert. Das zu Grunde liegende Problem besteht darin, dass der verwendete Code geschrieben wurde ohne Rücksicht auf den Kontext, in dem Fall den Konsumenten, zu nehmen. Häufig damit einher gehen nachträgliche Anpassungen an der Implementation selbst, um doch noch irgendwie die Nutzung für den Konsumenten zu ermöglichen.

# Kausalte Kette 4

**What**: Lange Entwicklungszeiten für neue Anforderungen

**How**: Geschäftslogik (Domäne, Businesslogik) nicht erweiterbar

**Why**: Vermischung von Aspekten bzw. Separation of Concerns nicht eingehalten

**Beispiel:** Die Geschwindigkeit der Weiterentwicklung nimmt von Sprint zu Sprint ab bzw. vermeintlich weniger komplizierte Adaptionen bestehender Funktionalität dauern länger als erwartet. Hintergrund ist, dass die bisherige Geschäftslogik nur schlecht erweiterbar ist. Das zu Grunde liegende Problem ist die Vermischung von Aspekten, z.B. Domänenlogik und Infrastruktur. Letzteres blutet in die Domänenlogik rein, sodass bei Neuerungen um die Infrastruktur herum gebaut werden muss und eine Erweiterbarkeit viel schwieriger zu gewährleisten ist.