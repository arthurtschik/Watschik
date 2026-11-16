# Sicherheit

## Sicherheitslücke melden

Bitte **keine öffentlichen Issues** für Sicherheitslücken. Schreib stattdessen eine E-Mail an
**arthurtschik.business@gmail.com** (Betreff „Watschik Sicherheit“) oder nutze – falls aktiviert –
auf GitHub unter *Security → Report a vulnerability* die private Meldung.

Hilfreich sind: betroffene Version, Schritte zum Nachstellen und die erwartete Auswirkung.
Ich antworte so schnell ich kann und melde mich, sobald es eine korrigierte Version gibt.

## Unterstützte Versionen

Gepflegt wird jeweils die **neueste Version** (siehe Releases). Ältere Versionen bekommen keine Korrekturen.

## Was Watschik schützt – und was nicht

- Es gibt **keinen Server und kein Konto**; Bewertungen und Listen liegen nur auf dem Gerät.
- **Sicherungen** sind mit AES-256-GCM verschlüsselt (Schlüssel per PBKDF2-SHA256, 600.000 Runden, Passwort ab 8 Zeichen).
  Beim Einlesen wird jede Sicherung streng geprüft; sie kann weder Einstellungen verändern noch eine PIN setzen.
- Die optionale **Google-Drive-Sicherung** verschlüsselt auf dem Handy (AES-256-GCM) mit einem zufälligen Wiederherstellungscode, der
  nur im Android Keystore liegt. Watschik nutzt ausschließlich den versteckten App-Ordner (`drive.appdata`), keinen anderen Drive-Inhalt;
  ohne den Code kann weder Google noch der Entwickler die Sicherung lesen. Der Zugriff lässt sich jederzeit im Google-Konto widerrufen.
- **Bugs melden / Wünsche** wird erst beim Antippen von „Senden“ über den Formulardienst Web3Forms an den Entwickler geschickt
  (Text, freiwillige Kontaktangabe, App- und Android-Version). Die App begrenzt Länge und Häufigkeit; es gibt keinen eigenen Server.
- Die **PIN** eines Profils ist ein **Sichtschutz** gegen neugierige Blicke (mit Wartezeit nach Fehlversuchen),
  **keine Verschlüsselung** der Daten auf dem Gerät. Wer das entsperrte Handy oder dessen Speicher in der Hand hat,
  kann die Daten lesen.
- Der **TMDB-Schlüssel** steckt – verschleiert – in der APK und lässt sich von jedem auslesen, der die App
  gezielt zerlegt. Er ist kostenlos und mit keinen Nutzerdaten verbunden; im Missbrauchsfall wird er gesperrt und ersetzt.
- **Updates aus der App:** Watschik fragt bei GitHub das neueste Release ab, lädt die `Watschik.apk` und prüft sie
  gegen die SHA-256-Prüfsumme der Release-Abfrage. Vor der Installation kontrolliert die App Paketname, Signatur und
  Versionsnummer (nur neuere Versionen mit demselben Signaturschlüssel). Installiert wird erst nach deiner Bestätigung
  im Android-Dialog. Die Funktion ist in den Einstellungen abschaltbar.
- Releases werden ausschließlich automatisch gebaut und mit einem Schlüssel signiert, der nur als geheimer
  Wert in der Bau-Umgebung existiert. Den Fingerabdruck des Zertifikats findest du in der README.
