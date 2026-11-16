# Watschik

Filme und Serien wischen: **gesehen oder nicht?** Bewerten, eine Watchlist führen, Neues entdecken –
und auch mal fünf Minuten Zeit in der Bahn dafür nutzen.

Android-App. **Alle deine Daten bleiben auf deinem Handy.** Kein Konto, keine Werbung,
keine Nutzungsanalyse, kein eigener Server.

> Dieses Repository enthält nur die **fertigen Downloads** (Releases) und Hinweise dazu.
> Der Quellcode wird privat gepflegt.

## Was kann Watschik?

- **Wischen:** rechts gesehen (danach Sterne), links nicht gesehen, oben direkt 5 Sterne,
  unten auf die Watchlist; „Kein Interesse“ per Knopf. Richtung auf Wunsch vertauschbar.
- **Details:** Infos, Besetzung (mit deutschen Synchronsprechern), Trailer in der App
  (deutsch bevorzugt), Streaming-Anbieter mit Direktlink, ähnliche Titel – ohne Spoiler zu späteren Staffeln.
- **Suche & Entdecken:** nach Titel, Schauspiel oder Regie; Vorschläge, die zu deinem Geschmack passen.
- **Roulette:** 1 bis 3 Vorschläge, gefiltert nach deinen Anbietern – mit Entscheidungshilfe,
  auch gemeinsam mit anderen Profilen.
- **Mehrere Profile** mit eigener Bibliothek, optionalem PIN-Schutz und Wechsel per Wisch am Profilbild.
- **Hinweise:** Kinostarts, neue Staffeln, neu bei deinen Anbietern – von deinem Handy erzeugt, ohne Push-Server.
- **Datensicherung:** verschlüsselt (AES-256), per Teilen-Menü aufs nächste Handy; Listen-Export als
  Tabelle oder für Letterboxd.
- **Google-Drive-Sicherung (optional):** automatisch einmal pro Woche, auf dem Handy verschlüsselt, nur im versteckten
  App-Ordner deines Google Drive; Wiederherstellung mit deinem Wiederherstellungscode.
- **Bugs melden / Wünsche:** direkt in der App (Einstellungen → Hilfe & FAQ), optional mit E-Mail oder Discord-Name für Rückfragen.

## Installation

1. Auf der [**Download-Seite**](https://arthurtschik.github.io/Watschik/) die aktuelle Version laden (die Datei heißt immer
   `Watschik.apk`; ältere Versionen findest du unter [Releases](../../releases)).
2. Auf dem Android-Handy öffnen und „Installation aus unbekannten Quellen“ erlauben.
3. Updates einfach über die bisherige Version installieren – die Daten bleiben erhalten.

**Echtheit prüfen:** Alle Versionen auf dieser Seite sind mit diesem Zertifikat signiert
(SHA-256-Fingerabdruck, auch ablesbar mit `apksigner verify --print-certs`):

```
ebf62e653c291be7663da929833bcdefd2179a8ef2d478547702a66ffba41a28
```

Eine APK mit anderem Fingerabdruck stammt nicht von hier.

## Datenschutz

Die vollständige Erklärung steht in der App (Einstellungen → Datenschutz & Rechtliches). Kurz:
Deine Bewertungen und Listen liegen nur auf deinem Handy. Zum Anzeigen von Filmen, Bildern und Trailern
verbindet sich dein Handy direkt mit TMDB, KinoCheck, Wikipedia und – erst beim Ansehen eines Trailers – YouTube.
Der Entwickler erhält davon nichts. „Alle Daten löschen und App zurücksetzen“ steht ganz unten in den Einstellungen.

## Sicherheit

Sicherheitslücken bitte nicht öffentlich melden, sondern nach [SECURITY.md](SECURITY.md).
Releases werden automatisch gebaut und mit einem festen Schlüssel signiert (Fingerabdruck siehe oben).

## Datenquellen und Dank

- **TMDB** – Film- und Seriendaten, Bilder.
  *This product uses the TMDB API but is not endorsed or certified by TMDB.*
- **JustWatch** – Streaming-Anbieter (über TMDB).
- **KinoCheck** – Trailer.
- **Wikipedia / Wikidata** – Synchronsprecher (CC BY-SA 4.0).
- Alle Klänge und das Logo sind selbst erstellt.

## Rechtliches

© Arthurtschik. Die App darf kostenlos genutzt werden; alle Rechte am Quellcode und an Name und Logo
bleiben vorbehalten. Marken und Logos Dritter (z. B. TMDB) gehören ihren jeweiligen Inhabern.

## Kontakt

Arthurtschik · c/o Block Services · Stuttgarter Str. 106 · 70736 Fellbach ·
[arthurtschik.business@gmail.com](mailto:arthurtschik.business@gmail.com)
