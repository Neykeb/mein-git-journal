# Mein Git Lernjournal

## Grundlagen

Frage: Ein Commit speichert drei Dinge. Was sind sie? (Hinweis: Wer, Was, Warum).

1.  **Was** wurde geändert? (z.B. Zeile 5 im Dokument X wurde gelöscht, zwei neue Absätze in Dokument Y wurden hinzugefügt).
2.  **Wer** hat es geändert? (Der Benutzername der Person).
3.  **Warum** wurde es geändert? (Der Entwickler schreibt eine kurze Nachricht, z.B. "Rechtschreibfehler im Vorwort korrigiert").


Frage: Was ist der "Stamm" (trunk) des Baumes in der Terminologie der Versionskontrolle?

Stell dir die Geschichte deines Projekts wie den Stamm eines Baumes vor. Jeder Commit ist ein kleiner Ring im Stamm, der das Wachstum dokumentiert. Was aber, wenn du etwas Neues ausprobieren möchtest, ohne die stabile Hauptversion (den "Stamm") zu gefährden? Zum Beispiel möchtest du ein neues Kapitel für dein Buch experimentell schreiben.

Dafür erstellst du einen **"Branch"** (einen Ast). Dieser Ast ist eine exakte Kopie deines Projekts zu einem bestimmten Zeitpunkt. Auf diesem Ast kannst du nun ungestört arbeiten, neue Commits machen und alles ausprobieren, was du möchtest. Der Hauptstamm bleibt davon völlig unberührt.

Wenn du mit deiner Arbeit auf dem Ast fertig und zufrieden bist, kannst du ihn wieder mit dem Hauptstamm **"mergen"** (zusammenführen). Das System versucht dabei, deine Änderungen intelligent in die Hauptversion zu integrieren.

Dieses Prinzip ist unglaublich mächtig, weil mehrere Personen gleichzeitig an verschiedenen "Ästen" (Features, Bugfixes) arbeiten können, ohne sich gegenseitig in die Quere zu kommen.

## Architektur

Frage: Was ist in einem zentralisierten System (wie einer Bibliothek) der "Single Point of Failure"?

Stell dir eine Bibliothek vor. In der Mitte des Raumes steht ein riesiges Regal – das ist der **zentrale Server**. In diesem Regal befindet sich das *einzige* Originalexemplar der gesamten Projekthistorie.

Wenn du an etwas arbeiten möchtest, gehst du zu diesem Regal und leihst dir eine Kopie der neuesten Version einer Datei aus (ein "Checkout"). Du arbeitest an deiner Kopie an deinem Schreibtisch. Wenn du fertig bist, bringst du die Datei zurück und gibst deine Änderungen ab (ein "Commit"). Deine Änderungen werden direkt auf dem zentralen Server gespeichert.


Frage: Wo wird in einem verteilten System (wie Git) die vollständige Projekthistorie gespeichert?

Jetzt stell dir ein anderes System vor. Anstatt einer zentralen Bibliothek gibt es einen Hauptserver, aber jeder Entwickler bekommt bei der ersten Ausleihe nicht nur die neueste Version, sondern eine **vollständige 1:1-Kopie der gesamten Bibliothek** für seinen eigenen Schreibtisch. Jeder Entwickler hat also die komplette Projekthistorie lokal auf seinem eigenen Computer.

Du arbeitest an deinem Projekt und machst Commits. Diese Commits werden in deiner *lokalen* Kopie des Repositories gespeichert. Du kannst Branches erstellen, die History ansehen, Versionen vergleichen – alles blitzschnell und ohne eine Internetverbindung.

Erst wenn du deine Arbeit mit anderen teilen möchtest, stellst du eine Verbindung zum zentralen Server her und schiebst deine Änderungen dorthin ("Push"). Um die Änderungen der anderen zu erhalten, holst du sie dir vom Server ab ("Pull").

