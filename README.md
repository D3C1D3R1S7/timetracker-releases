# Time Tracker – Downloads

Zeiterfassung für den Arbeitsalltag: Timer, Wochenkalender, Projekte mit WOT-Kontingenten, Aufgaben,
Outlook-Kalender (Import und Export), Berichte und Übertragung nach ServiceNow.

Es gibt die App in zwei Varianten mit gleichen Funktionen – du brauchst nur eine:

- **Time Tracker** – die Standard-Version (Oberfläche im eingebauten Browser-Fenster).
- **Time Tracker Slint** – native Oberfläche, kleiner und ohne Browser-Komponente.

Jedes Release enthält beide. Die aktuelle Version findest du unter **[Releases](../../releases/latest)**.

> **Lizenz erforderlich:** Installation und Nutzung sind nur mit einem gültigen Lizenzschlüssel erlaubt
> (siehe [LICENSE](LICENSE)). Ohne Schlüssel startet die App nicht.

## Welche Datei?

| System | Time Tracker | Time Tracker Slint |
|---|---|---|
| Windows 10/11 (64 Bit) | `Time-Tracker_<Version>_x64-setup.exe` | `Time-Tracker-Slint_<Version>_x64-setup.exe` |
| Windows ohne Installation | – | `time-tracker-slint.exe` |
| Linux (eine Datei) | `…_amd64.AppImage` | `Time-Tracker-Slint_<Version>_x86_64.AppImage` |
| Linux Debian/Ubuntu | `…_amd64.deb` | `time-tracker-slint_<Version>_amd64.deb` |
| Linux Fedora/openSUSE | `…x86_64.rpm` | `time-tracker-slint_<Version>_linux-x64.tar.gz` (nur die Programmdatei) |
| macOS Apple Silicon (M1–M4) | `…_aarch64.dmg` | `Time-Tracker-Slint_<Version>_macos-aarch64.dmg` |
| macOS Intel | `…_x64.dmg` | `Time-Tracker-Slint_<Version>_macos-x64.dmg` |

Die Dateien `.sig`, `.app.tar.gz`, `latest.json` und `latest-slint.json` sind für die automatische Update-Prüfung –
die brauchst du nicht herunterzuladen.

## Installieren

**Windows:** Setup starten. Meldet Windows „Der Computer wurde durch Windows geschützt“, auf
„Weitere Informationen“ → „Trotzdem ausführen“ klicken. Der Installer zeigt deine **Rechner-ID** und fragt nach dem
Lizenzschlüssel.

**Linux:**
- AppImage: `chmod +x *.AppImage` und starten.
- .deb: `sudo apt install ./<Datei>.deb`
- .rpm: `sudo dnf install ./<Datei>.rpm`
- Benötigt GTK 3 und die AppIndicator-Bibliothek (bei den meisten Desktops vorhanden; die Pakete installieren sie mit).

**macOS:** `.dmg` öffnen und die App in den Ordner „Programme“ ziehen. Die App ist nicht notarisiert: beim ersten
Start per **Rechtsklick → Öffnen** starten (oder im Terminal `xattr -dr com.apple.quarantine "/Applications/<App>.app"`).

## Lizenzschlüssel

1. Beim ersten Start (unter Windows schon im Installer) zeigt die App deine **Rechner-ID** (z. B. `A1B2-C3D4-E5F6-0718`).
2. Schick die Rechner-ID an den Herausgeber. Du bekommst einen Lizenzschlüssel, der mit `TT1-` beginnt.
3. Schlüssel eintragen – fertig. Zusätzliche Funktionen (z. B. Outlook, ServiceNow, Widget) werden mit einem
   Funktions-Schlüssel unter **Einstellungen → Lizenz** freigeschaltet.

Der Schlüssel gilt nur für diesen Rechner und für beide Varianten. Läuft er ab, sperrt sich die App, bis ein neuer
eingetragen ist – deine Daten bleiben dabei erhalten.

## Updates

Unter **Einstellungen → Updates → Update-Adresse** eintragen:

- Time Tracker:
  ```
  https://github.com/D3C1D3R1S7/timetracker-releases/releases/latest/download/latest.json
  ```
- Time Tracker Slint (Windows):
  ```
  https://github.com/D3C1D3R1S7/timetracker-releases/releases/latest/download/latest-slint.json
  ```

Die App meldet dann neue Versionen und installiert sie auf Wunsch selbst. Slint unter Linux und macOS: die neue Datei
von der Release-Seite laden.

## Deine Daten

Alle Zeiteinträge liegen in einer Datenbankdatei auf deinem Rechner (Pfad unter **Einstellungen → Daten**).
Die App legt täglich eine Sicherung an (**Einstellungen → Sicherung**). Es werden keine Daten an den Herausgeber
übertragen.
