# Time Tracker – Downloads

Zeiterfassung für den Arbeitsalltag: Timer, Wochenkalender, Projekte mit WOT-Kontingenten, Aufgaben,
Outlook-Kalender (Import und Export), Berichte und Übertragung nach ServiceNow.

Hier liegen nur die fertigen Installationspakete. Die aktuelle Version findest du unter
**[Releases](../../releases/latest)**.

> **Lizenz erforderlich:** Installation und Nutzung sind nur mit einem gültigen Lizenzschlüssel erlaubt
> (siehe [LICENSE](LICENSE)). Ohne Schlüssel startet die App nicht.

## Welche Datei?

| System | Datei | Hinweis |
|---|---|---|
| Windows 10/11 (64 Bit) | `Time-Tracker_<Version>_x64-setup.exe` | Installer, empfohlen |
| Linux (64 Bit) | `…_amd64.AppImage` | eine Datei, läuft ohne Installation |
| Linux Debian/Ubuntu | `…_amd64.deb` | Paket mit Startmenü-Eintrag |
| Linux Fedora/openSUSE | `…x86_64.rpm` | Paket mit Startmenü-Eintrag |
| macOS Apple Silicon (M1–M4) | `…_aarch64.dmg` | |
| macOS Intel | `…_x64.dmg` | |

Die Dateien `.sig`, `.app.tar.gz` und `latest.json` sind für die automatische Update-Prüfung – die brauchst du
nicht herunterzuladen.

## Installieren

**Windows:** Setup starten. Meldet Windows „Der Computer wurde durch Windows geschützt“, auf
„Weitere Informationen“ → „Trotzdem ausführen“ klicken. Der Installer zeigt deine **Rechner-ID** und fragt nach dem
Lizenzschlüssel.

**Linux:**
- AppImage: `chmod +x Time-Tracker_*.AppImage` und starten.
- .deb: `sudo apt install ./Time-Tracker_*_amd64.deb`
- .rpm: `sudo dnf install ./Time-Tracker-*.x86_64.rpm`

**macOS:** `.dmg` öffnen und „Time Tracker“ in den Ordner „Programme“ ziehen. Die App ist nicht notarisiert:
beim ersten Start per **Rechtsklick → Öffnen** starten (oder im Terminal
`xattr -dr com.apple.quarantine "/Applications/Time Tracker.app"`).

## Lizenzschlüssel

1. Beim ersten Start (unter Windows schon im Installer) zeigt die App deine **Rechner-ID** (z. B. `A1B2-C3D4-E5F6-0718`).
2. Schick die Rechner-ID an den Herausgeber. Du bekommst einen Lizenzschlüssel, der mit `TT1-` beginnt.
3. Schlüssel eintragen – fertig. Zusätzliche Funktionen (z. B. Outlook, ServiceNow, Widget) werden mit einem
   Funktions-Schlüssel unter **Einstellungen → Lizenz** freigeschaltet.

Der Schlüssel gilt nur für diesen Rechner. Läuft er ab, sperrt sich die App, bis ein neuer eingetragen ist –
deine Daten bleiben dabei erhalten.

## Updates

Unter **Einstellungen → Updates → Update-Adresse** eintragen:

```
https://github.com/D3C1D3R1S7/timetracker-releases/releases/latest/download/latest.json
```

Die App meldet dann neue Versionen und installiert sie auf Wunsch selbst.

## Deine Daten

Alle Zeiteinträge liegen in einer Datenbankdatei auf deinem Rechner (Pfad unter **Einstellungen → Daten**).
Die App legt täglich eine Sicherung an (**Einstellungen → Sicherung**). Es werden keine Daten an den Herausgeber
übertragen.
