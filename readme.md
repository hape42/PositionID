# PositionID – Die Grundidee

## Motivation
Schon seit langer Zeit wollte ich mir interessante Backgammon-Stellungen merken, um sie später mit GNU Backgammon oder BGBlitz zu analysieren. Besonders dann, wenn ich eine andere Zugwahl getroffen hätte oder eine Take/Pass-Entscheidung anders bewertet hätte.

Früher hatte ich immer einen Block mit einem vorgezeichneten Board dabei. Doch während eines Spiels bleibt kaum Zeit, eine Stellung sauber zu notieren – die Mitspieler warten schließlich nicht. Später musste ich die Positionen dann mühsam in GNU BG eingeben, um endlich eine Analyse durchzuführen und zu verstehen, warum der Spieler eine andere Entscheidung getroffen hat als ich.

Viele Jahre später bieten moderne Technologien eine wesentlich komfortablere Lösung für dieses Problem. Und genau hier setzt **PositionID** an.

## Die Lösung
Anstatt hektisch zu schreiben, mache ich einfach ein Foto oder einen Screenshot des Boards.

Ein Tool analysiert dieses Bild und erkennt die Backgammon-Stellung. Falls wichtige Informationen fehlen oder unklar sind, werden sie interaktiv abgefragt, z. B.:
- **Match- oder Moneygame?**
- **Aktueller Matchstand?**
- **Cube-Position und -Wert?**
- **Homeboard links oder rechts?**
- **Fehlende Steine: auf der Bar oder bereits ausgespielt?**

Sobald alle Daten vorliegen, wandelt das Tool die Position in eine **XGID** oder **GNU ID** um. Diese ID kann dann direkt in **BGBlitz**, **GNU Backgammon** oder **XG Gammon** zur Analyse genutzt werden.

## Technischer Überblick
- **Plattformunabhängig**: Das Tool soll auf **Mac, Windows, Linux, iOS und Android** laufen – lokal, ohne Serverabhängigkeit.
- **Bilderkennung**: In der ersten Phase wird **OpenCV** zur Bilderkennung verwendet. Später könnte eine eigene, speziell trainierte KI diese Aufgabe übernehmen.
- **Frontend**: Noch offen – möglicherweise eine plattformunabhängige Web-App.
- **Erste Schritte**: Da ich in diesen Bereichen noch keine Erfahrung habe, starte ich mit einem **Python-Kurs**, um die Grundlagen zu erlernen.

## Projektorganisation
- Alle Dokumente – auch temporäre Zwischenschritte – werden auf **GitHub** gespeichert und versioniert.
- Ein **Projekttagebuch** soll Fortschritte, Rückschläge und Herausforderungen dokumentieren.

