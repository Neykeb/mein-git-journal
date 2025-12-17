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


