# GameShelf – Download

**Version 1.6.0** · Erstellt von 1nf3ct10n

GameShelf ist eine kleine Windows-App, die alle auf deinem PC installierten Spiele an einem Ort zeigt – mit Covern, kurzen Gameplay-Clips, Favoriten und einem „Spielen“-Knopf. Alles bleibt lokal auf deinem Rechner: Es gibt kein Konto, GameShelf lädt keine Cover herunter und sendet keine Daten an einen Server.

---

## Was die App kann

- **Spiele automatisch finden** – beim Start (und über „↻ Neu suchen“ bzw. **F5**) liest GameShelf deine Bibliothek ein:
  Steam, Epic Games, GOG, Ubisoft, Xbox-Spiele, FiveM/RedM sowie Spiele, die sich in Windows registriert haben (z. B. von EA, Rockstar, Battle.net, Riot).
- **Eigene Spiele und Ordner hinzufügen** – über „+ Spiel hinzufügen“ (eine `.exe` oder Verknüpfung auswählen) oder über „Ordner“ für weitere Bibliotheksordner.
- **Spielen** – startet Steam-, Epic- und Ubisoft-Spiele über ihren Launcher, andere direkt. Wenn ein Spiel nicht richtig startet, kannst du über „•••“ → „Startdatei zuweisen …“ selbst festlegen, was gestartet wird (in den Spieldetails auch mit Startoptionen).
- **Suchen, Filtern, Sortieren** – Suchfeld (**Strg+F**, **Esc** leert die Suche), Filter nach Plattform, „Alle Spiele“ / „Favoriten“, „Tools anzeigen“ und Sortierung (Name A–Z, Z–A oder Spielzeit).
- **Favoriten** – Stern auf der Karte anklicken.
- **Zuletzt gestartet** – eigene Reihe mit den Spielen, die du zuletzt gestartet hast.
- **Ausblenden** – Einträge, die du nicht sehen willst, über „•••“ → „Aus Bibliothek ausblenden“. Unter „Ausgeblendete Einträge“ holst du sie zurück.
- **Eigene Cover** – „•••“ → „Cover ändern …“ (JPG/PNG). In den Spieldetails kannst du zum Original-Cover zurück.
- **Gameplay-Clips als animiertes Cover** – „•••“ → „Gameplay-Clip …“ bzw. „Gameplay-Clip ersetzen …“. Erlaubt sind GIF sowie Videos (MP4, WMV, MOV) bis 80 MB. Videos laufen stumm in einer Schleife von ca. 25 Sekunden.
- **Clip-Optimierung (automatisch)** – Videos werden im Hintergrund einmalig in eine leichte Kopie umgewandelt (H.264, max. 960 Pixel breit, max. 30 Bilder/s, ohne Ton, max. 25 Sekunden). Die Kopie läuft flüssiger und spart Leistung. Das Original bleibt unverändert. Solange die Umwandlung läuft, wird das Original abgespielt.
- **Update-Hinweis** – GameShelf schaut beim Start (höchstens einmal am Tag, im Hintergrund) nach, ob es eine neue Version gibt. Wenn ja, erscheint oben ein kleiner Hinweis mit „Zur Download-Seite“ und „Später“. Es wird nichts automatisch heruntergeladen oder installiert. Unter „App & Updates“ kannst du auch selbst „Nach Updates suchen“ oder die automatische Prüfung abschalten.
- **Spielzeit** – Startest du ein Spiel über GameShelf, misst die App, wie lange es läuft (auch bei Spielen, die über Steam, Epic oder die Xbox-App starten: GameShelf erkennt das Spiel an seinem Installationsordner). Die Zeit wird regelmäßig gespeichert, bei einem Absturz geht höchstens etwa eine Minute verloren. Bei Steam-Spielen liest GameShelf zusätzlich Steams eigene Spielzeit (nur lesend). Angezeigt wird der größere der beiden Werte – so wird nichts doppelt gezählt. Du siehst die Spielzeit auf der Karte und in den Spieldetails (mit Anzahl der Sitzungen) und kannst nach Spielzeit sortieren. Gemessen wird nur, solange GameShelf geöffnet ist.
- **Discord-Status** – Läuft ein Spiel, das du **über GameShelf gestartet** hast, zeigt Discord bei deinem Profil „Spielt GameShelf“ mit dem Spielnamen, der Spieldauer und einem Knopf „GameShelf holen“. Wenn das Spiel endet, verschwindet die Anzeige. Ist Discord nicht geöffnet, passiert einfach nichts. Abschalten kannst du das unter „App & Updates“ → „In Discord anzeigen, was ich gerade über GameShelf spiele“.
- **Spieldetails** – Klick auf ein Spiel zeigt Plattform, Größe, letzten Start, Installationsordner und alle Aktionen.

## Voraussetzungen

- **Windows 10 oder Windows 11** (64 Bit)
- **.NET Framework 4.8** – ist in Windows 10 (ab Version 1903) und Windows 11 bereits enthalten.
- **Nur für AV1-Videos:** Die kostenlose „AV1 Video Extension“ aus dem Microsoft Store. Normale MP4-Videos (H.264) und GIFs brauchen nichts extra.

## Installation

1. Unter **[Releases](https://github.com/1nf3ct10nn/GameShelf-Download/releases/latest)** die ZIP-Datei (z. B. `GameShelf-1.6.0.zip`) herunterladen und **entpacken** (Rechtsklick → „Alle extrahieren …“).
2. `GameShelf.exe` doppelklicken.
3. Windows zeigt eventuell „Der Computer wurde durch Windows geschützt“ (SmartScreen), weil die App nicht digital signiert ist. Dann auf **„Weitere Informationen“** und danach **„Trotzdem ausführen“** klicken.
4. Optional, aber empfohlen: In der App **„App & Updates“ → „Desktop einrichten / Verknüpfung reparieren“** wählen. Dann wird GameShelf fest nach `%LOCALAPPDATA%\Programs\GameShelf` kopiert und eine Desktop-Verknüpfung angelegt.

## Aktualisieren

1. Die neue ZIP-Datei unter **[Releases](https://github.com/1nf3ct10nn/GameShelf-Download/releases/latest)** herunterladen und entpacken.
2. Im laufenden GameShelf **„App & Updates“ → „Neue Version installieren …“** wählen und die neue `GameShelf.exe` aus dem entpackten Ordner auswählen.
3. GameShelf schließt sich, installiert die neue Version und behält alle deine Daten (Favoriten, Cover, Clips, Verlauf). Vor der Installation wird automatisch eine Sicherung angelegt.

Es gibt **kein automatisches Update** – GameShelf weist dich nur auf neue Versionen hin, du entscheidest selbst, wann du aktualisierst.

## Wo liegen meine Daten?

Alles liegt unter `%LOCALAPPDATA%\GameShelf` (in die Adresszeile des Explorers eintippen):

| Ordner / Datei | Inhalt |
|---|---|
| `library.json` | Deine Einstellungen: Favoriten, ausgeblendete Spiele, eigene Spiele, Cover- und Clip-Zuordnung, Verlauf, Spielzeit, Startoptionen |
| `library.json.bak` | Vorige Version der Einstellungen (automatische Sicherung) |
| `Covers\` | Deine eigenen Cover-Bilder |
| `Clips\` | Deine Gameplay-Clips (Originale) |
| `ClipCache\` | Die optimierten H.264-Kopien der Clips (kann gelöscht werden, wird neu erzeugt) |
| `Backups\` | Sicherungen, die beim Einrichten/Aktualisieren angelegt werden |
| `video.log` | Protokoll zur Video-Wiedergabe – hilfreich bei Problemen |

Das Programm selbst liegt nach dem Einrichten unter `%LOCALAPPDATA%\Programs\GameShelf`.

## Probleme lösen

- **Ein Spiel fehlt:** „↻ Neu suchen“ (F5). Hilft das nicht, über „+ Spiel hinzufügen“ die `.exe` auswählen oder den Bibliotheksordner über „Ordner“ hinzufügen. „Scan-Details“ zeigt, was gefunden wurde.
- **Ein Spiel startet nicht:** „•••“ → „Startdatei zuweisen …“ und die richtige `.exe` wählen.
- **Ein Video-Cover bleibt leer oder ruckelt:**
  - Kurz warten – beim ersten Mal wird der Clip im Hintergrund optimiert.
  - Bei AV1-Videos die „AV1 Video Extension“ aus dem Microsoft Store installieren.
  - Den Ordner `ClipCache` löschen und GameShelf neu starten – die Kopien werden neu erstellt.
  - Die Datei `video.log` an 1nf3ct10n schicken; dort steht, was beim Abspielen passiert ist.
- **„Einstellungen konnten nicht gelesen werden“:** Die Datei `library.json` ist beschädigt. GameShelf überschreibt sie dann bewusst nicht. Du kannst `library.json.bak` in `library.json` umbenennen, um die vorige Version zurückzuholen.
- **Desktop-Symbol fehlt oder zeigt ins Leere:** „App & Updates“ → „Desktop einrichten / Verknüpfung reparieren“.

## Selbsttest

Für Fehlersuche gibt es einen eingebauten Selbsttest. Er schreibt nur in den angegebenen Ordner und ändert nichts an deinen Daten:

```powershell
GameShelf.exe --self-test C:\Temp\gameshelf-test.txt
# optional mit einem eigenen Clip:
GameShelf.exe --self-test C:\Temp\gameshelf-test.txt C:\Pfad\zu\clip.mp4
```

Geprüft werden u. a. Versionsangaben, Speichern/Laden der Bibliothek, der Clip-Cache und die Video-Optimierung. Das Ergebnis steht in der Textdatei.
