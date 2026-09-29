# MoxSync — Downloads & Installation

Distribution des MoxSync-Browser-Add-ons (Tracking der Kartenverfügbarkeit über
mehrere geteilte Moxfield-Collections). Dieses Repository enthält die
installierbaren Builds. Der Quellcode wird separat gepflegt.

**Aktuelle Version: 1.0.9**

---

## Firefox

Firefox erhält Updates automatisch über den self-hosted Update-Mechanismus
(`updates.json` in diesem Repo). Einmal installiert, aktualisiert sich das
Add-on künftig selbst.

### Installation
1. Firefox öffnen und diese Datei aufrufen:
   [`moxsync-firefox-1.0.9.xpi`](https://raw.githubusercontent.com/CMALG/moxsync-dist/main/moxsync-firefox-1.0.9.xpi)
2. Firefox fragt, ob das Add-on installiert werden soll — bestätigen.
3. Fertig. Add-on-ID: `moxsync@extension`

Die `.xpi` ist von Mozilla (AMO) signiert und installiert sich daher auch in
der regulären Firefox-Release-Version.

---

## Chrome / Chromium (Chrome, Edge, Brave, …)

> **Wichtig:** Chromium-Browser unterstützen **kein** automatisches Update für
> Erweiterungen, die außerhalb des Chrome Web Store verteilt werden. Die manuell
> geladene Erweiterung muss bei einer neuen Version **von Hand** aktualisiert
> werden. Ein `updates.json`-Mechanismus wie bei Firefox greift hier nicht.

### Installation (Entwicklermodus)
1. [`moxsync-chrome-1.0.9.zip`](https://raw.githubusercontent.com/CMALG/moxsync-dist/main/moxsync-chrome-1.0.9.zip) herunterladen und in einen
   Ordner entpacken.
2. Im Browser `chrome://extensions` (bzw. `edge://extensions`,
   `brave://extensions`) öffnen.
3. Oben rechts den **Entwicklermodus** aktivieren.
4. **Entpackte Erweiterung laden** klicken und den entpackten Ordner auswählen.

### Aktualisieren
1. Neue `.zip` herunterladen und über den alten Ordner entpacken (oder in einen
   neuen Ordner).
2. Auf `chrome://extensions` bei MoxSync auf **Aktualisieren/Neu laden** klicken
   (bzw. die alte Erweiterung entfernen und die neue laden).

---

## Dateien in diesem Repository

| Datei | Zweck |
| --- | --- |
| `moxsync-firefox-1.0.9.xpi` | Signiertes Firefox-Add-on (mit Auto-Update) |
| `moxsync-chrome-1.0.9.zip` | Chrome/Chromium-Build (manuelle Installation) |
| `updates.json` | Firefox-Update-Manifest (von Firefox automatisch abgerufen) |

_Dieses README wird beim Release automatisch erzeugt._
