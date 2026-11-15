# TAS – Releases

Hier liegen nur die fertigen Installations- und Update-Dateien von TAS für macOS.
Der Quellcode ist privat.

## Installation

Beim [neuesten Release](https://github.com/nikg819/TAS-Releases/releases/latest) das passende Paket laden:

| Mac | Datei |
|---|---|
| Apple-Prozessor (M1, M2, M3, …) | `TAS-osx-Setup.pkg` |
| Intel-Prozessor | `TAS-osx-x64-Setup.pkg` |

Welcher Prozessor? Apple-Menü  → „Über diesen Mac“: steht dort „Chip Apple M…“ → Apple, steht dort „Prozessor Intel…“ → Intel.

### „Apple konnte nicht überprüfen …“

TAS ist nicht über ein kostenpflichtiges Apple-Entwicklerkonto signiert. macOS blockiert das Paket
deshalb beim ersten Öffnen. So gibst du es frei:

1. Im Hinweis auf **„Fertig“** klicken (nicht „In den Papierkorb“).
2. **Systemeinstellungen → Datenschutz & Sicherheit** öffnen und ganz nach unten scrollen.
3. Bei „TAS-…-Setup.pkg wurde blockiert“ auf **„Dennoch öffnen“** klicken und mit dem Mac-Passwort bestätigen.
4. Installation durchlaufen lassen – TAS liegt danach unter **Programme** und startet automatisch.

Alternativ im Terminal (danach per Doppelklick öffnen):

```bash
xattr -d com.apple.quarantine ~/Downloads/TAS-osx-Setup.pkg
```

## Updates

TAS prüft beim Start selbst, ob hier ein neues Release liegt, und bietet links unten
„Jetzt aktualisieren“ an. Vorher wird automatisch ein Backup erstellt. Updates brauchen keine erneute Freigabe.
