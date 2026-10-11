# Das große Dinosaurier-Popup-Buch

Ein 3D-Popup-Buch im Browser: neun Stationen von der Erduhr über Trias, Jura und Kreide bis zum Einschlag und zum Zeitalter der Säugetiere mit den ersten Vormenschen. Für Klasse 5/6, mit Erzählstimme, Info-Karten und Arbeitsblatt-Export.

- **Online ansehen** (nach dem Einschalten von GitHub Pages, siehe `tools/publish-pages.sh`): https://wilski54.github.io/dinobuch/
- **Eine Datei**: `dist/index.html` (ca. 7,8 MB, alles eingebettet). Doppelklick genügt, auch von der Festplatte (`file://`) und auf dem iPad (Safari).
- **Keine externen Anfragen**: keine Bibliotheken, Schriften, Bilder oder Töne aus dem Netz. Keine Cookies, kein Tracking. Alle Grafiken, Texturen und Klänge entstehen im Code; die Erzählstimme steckt als MP3 in der Datei.
- **Gespeichert wird nur im Browser** (`localStorage`, nur auf diesem Gerät): Lautstärke, Ton an/aus, Ruhiger Modus, Kino-Brüllen, Untertitel, Auto-Vorlesen und welche versteckten Säugetiere du gefunden hast. Alles ist mit Rückfall gebaut; ohne Speicher läuft das Buch trotzdem.

## Bedienung

| Was | Wie |
|---|---|
| Buch öffnen | Auf den Deckel tippen |
| Umblättern | Die Seite irgendwo anfassen und waagerecht zur Buchmitte ziehen (rechte Seite nach links, linke nach rechts, loslassen vor der Hälfte = zurück, schnelles Wischen blättert), oder an der umgeknickten Ecke ziehen, Pfeile unten, die neun Farbpunkte, Tasten ← und → |
| Laschen und Schieber | Bunte Laschen anfassen und ziehen. Manche springen zurück, manche bleiben stehen |
| Tiere | Antippen: das Tier wacht auf, brüllt oder ruft und zeigt eine Info-Karte (mit Größenvergleich zum Menschen). Der Lautsprecher-Knopf liest die Karte vor |
| Umschauen | Auf freier Fläche oder senkrecht über die Seite ziehen: Kamera schwenkt, nach ein paar Sekunden kehrt sie zurück |
| Lesen: heranzoomen und verschieben | Zwei Finger: spreizen zum Zoomen (bis ca. 3x), beide Finger gemeinsam bewegen zum Verschieben. Maus: Mausrad zoomt zum Zeiger, Umschalt + Ziehen oder rechte Taste verschiebt. **Hand-Knopf** (Taste **V**): ein Finger verschiebt statt zu blättern. Die Ansicht bleibt beim Blättern erhalten. **Haus-Knopf** (Taste **0**): Ansicht zurücksetzen |
| Zeitfenster (Erduhr) | Responsiv (rechts vom Buch, sonst links oben: Bild und Text nebeneinander oder untereinander, nur im Notfall Text über dem Bild). Auf der ersten Seite zeigt ein rahmenloses, frei auf dem Tisch schwebendes Bild (weiche Ränder) neben dem Buch zur Uhrzeit des Zeigers passende Szenen (16 Stück: Feuerball Erde, Urozean, erste Bakterien, Sauerstoff, Zellen mit Kern, Schneeball Erde, Ediacara, Kambrium, Tiktaalik, Sumpfwald, großes Sterben, Lucy, Homo habilis, Homo sapiens). Für die Dinosaurier-Zeit zeigt es nur „Jetzt wird geblättert!“, damit das Buch nichts vorweggenommen wird. Pfeile und Punkte im Fenster springen zur nächsten Szene (die letzten Sekunden der Uhr sind sonst kaum zu treffen). Breites Fenster: rechts neben dem Buch, iPad: kompakt links oben, Tipp aufs Bild blendet den Text ein. – Knopf klappt es ein |
| Leseansicht | Auge-Knopf oder Taste **R**: Blick von oben |
| Wetter | Wolken-Knopf oder Taste **W**: Klar → Regen → Sturm → Dunst. Auf der Einschlag-Seite fällt das Wetter aus |
| Ton | Lautsprecher-Knopf oder Taste **M** |
| Vorlesen | „Vorlesen“ neben der Navigation liest die Seiteneinführung. Standardmäßig spricht die Stimme jede Seite kurz von selbst (abschaltbar) |
| Hilfe | Fragezeichen oder Taste **?** / **H**. Dort: Lautstärke, Ruhiger Modus, Kino-Brüllen, Auto-Vorlesen, Untertitel |
| Karte oder Dialog schließen | X, Esc oder neben die Karte tippen |

Adresszusatz `?tier=low`, `?tier=med` oder `?tier=high` erzwingt eine Qualitätsstufe (sonst automatisch: Tablets starten mit „med“ und regeln bei Ruckeln herunter).

## Die Stationen

| # | Station | Zeit | Zum Anfassen |
|---|---|---|---|
| 0 | Deckel, Willkommen, Erduhr | 4,54 Mrd. Jahre | Zeiger drehen, Uhr antippen |
| 1 | Trias | 252–201 Mio. | RENN!-Lasche, Pangaea-Klappe |
| 2 | Jura-Wald | 201–145 Mio. | Halslänge-Regler, SCHWING! |
| 3 | Jura-Lagune (Solnhofen) | ca. 150 Mio. | FLATTER!, „Zeit vergeht“ (Tier wird zum Fossil) |
| 4 | Kreide-Meer | 145–66 Mio. | FLATTER!, STURZ!, Periskop, Wellen antippen |
| 5 | Könige der Kreide | 68–66 Mio. | BEISS!, „Kopf runter!“ |
| 6 | Dino-Babys (Nistkolonie) | 76–74 Mio. | SCHLÜPFE!, „Sonnenuntergang“ |
| 7 | Einschlag | ca. 66 Mio. | METEOR! (glühender Felsbrocken mit Feuerschweif fliegt von links oben quer vor dem Buch ein, dann Blitz, Funkenflug und Vulkanausbruch), Klappe „Spurensuche“ (Iridium) |
| 8 | Säugetiere und Vormenschen | 66–3,7 Mio. | WACHSE!, Zeitsprung-Regler bis Laetoli, LAUF!, Lucy, Familienalbum, „Buch schließen“ |

**Such sie!** Auf fünf Seiten versteckt sich je ein winziges frühes Säugetier (Morganucodon, Castorocauda, Didelphodon, Vielhöckerzähner, Purgatorius). Der Zähler oben rechts zeigt, wie viele gefunden sind; danach öffnet sich das Familienalbum.

## Für den Unterricht

- `texte.json`: alle Seiten- und Kartentexte mit Zeitangaben, Größen, Nahrung, Fundort, Stichworten und **Fragen für Arbeitsblätter** (`fragenFuerArbeitsblatt`), dazu Ideen für Aufgaben (Zeitstrahl, Erduhr rechnen, Größenvergleich, Iridium). Neu erzeugen mit `node tools/export-texte.mjs`.
- `facts.md`: jede wichtige Zahl mit Quelle und Prüfstand („geprüft“, „gerechnet“, „Fachwissen“). Bitte die Punkte mit „Fachwissen“ vor dem Unterricht gegenlesen.
- Sprache: einfache, kurze Sätze, Du-Ansprache; Aussprachehilfen auf den Karten („sprich: …“). Menschen und Dinosaurier werden nie zusammen gezeigt.
- Ruhiger Modus (Hilfe-Dialog, wird auch bei „Bewegung reduzieren“ im Betriebssystem automatisch gewählt): weniger Wackeln, kein Blitz im Sturm, gedämpfter Einschlag.
- Lichtschutz: Jeder Blitz steigt in höchstens 150 ms an. Der Einschlag blitzt nur einmal (kein Flackern, danach weiches Abklingen über ca. 0,7 s), warm getönt und im Ruhigen Modus abgeschwächt. Im Sturm kommt höchstens ein Blitz alle 5 Sekunden (im Ruhigen Modus gar keiner, nur fernes Grollen).

## Technik

- **three.js 0.186** (MIT), **clipper-lib** (Boost-Lizenz, Papierschnitt-Konturen), gebündelt mit **esbuild** zu einer einzigen HTML-Datei. Zur Laufzeit wird nichts nachgeladen.
- **Ton**: Web Audio, komplett synthetisch (Atmosphären, Musikbetten, 38 Tierstimmen, 41 Geräusche, Regen- und Windschicht). Siehe `docs/AUDIO.md`.
- **Erzählstimme**: Neuro-TTS, offline erzeugt mit Piper „de_DE-thorsten-medium“ (Stimme: Thorsten Müller, CC0) über `sherpa-onnx`. 59 Clips (Deckel, 9 Seiten, 49 Karten), zusammen ca. 21 Minuten, 32 kbps Mono, als Base64 eingebettet. Herkunft und Lizenz: `assets/narration/LICENSE.txt`. Ohne passenden Clip fällt das Buch auf die Sprachausgabe des Geräts zurück.
- **Qualitätsstufen** (high/med/low): Auflösung, Schattenkarte, Partikelmenge und Textur-Größen werden automatisch angepasst. Gemessen: ca. 120 MB Texturen im Maximum (nur das aktuelle und die benachbarten Spreads sind gebaut).

### Ordnerstruktur

```
dist/index.html          das fertige Buch (eine Datei)
src/main.js              App: Eingabe, Navigation, UI-Anbindung, Hauptschleife
src/engine/              Buch, Seiten, Pop-ups, Kamera, Licht, Partikel, Wetter, Papierschnitt
src/pages/p0…p8.js       die neun Stationen (+ kit-Dateien mit gemeinsamen Bausteinen)
src/art/                 Tier- und Pflanzen-Silhouetten (alles Code), registry.js
src/audio/               Klangmaschine (Szenen, Stimmen, Musik, Erzählung)
src/ui/ui.js, style.css  Oberfläche (Navigation, Karten, Hilfe)
src/data/                Texte: pages.de.js, animals.de.js, speech.js (Sprechtexte)
assets/narration/        Erzähl-MP3s + Manifest + Satzzeiten + Lizenz
tools/                   Build-, Test- und Export-Skripte
docs/                    AUDIO.md, ART_GUIDE.md, PAGE_GUIDE.md, USER_PROMPT.md
facts.md, texte.json     Faktenbasis und Textexport
```

### Bauen

```bash
npm install                     # three, clipper-lib, esbuild, playwright-core
node build.mjs --main           # dist/index.html (minimiert, mit den Erzähl-MP3s)
node build.mjs --dev            # unminimiert, für die Entwicklung
node build.mjs                  # zusätzlich dist/gallery.html (Tier-Galerie zum Prüfen der Zeichnungen)
node tools/export-texte.mjs     # texte.json neu schreiben
node tools/speech-dump.mjs      # Sprechtexte → assets/narration/_items.json
python3 tools/make-narration.py [--only a,b] [--check] [--asr]   # Erzählstimme neu erzeugen und prüfen
```

`make-narration.py` braucht `pip install sherpa-onnx numpy scipy`, `ffmpeg` mit libmp3lame und das Piper-Modell (siehe Kopf der Datei). Die Clips im Ordner `assets/narration/` sind fertig; nur bei geänderten Texten müssen die betroffenen Clips neu erzeugt werden (`--only card_<id>`).

### Testen

Die Tests laufen mit Chromium und Software-WebGL (SwiftShader), das ist langsam (ca. 3 Bilder pro Sekunde), reicht aber für Screenshots und Logiktests. Der Pfad zu Chromium steht in `tools/harness.mjs`.

```bash
node tools/walk.mjs                  # alle Stationen anfahren, Screenshots nach test-out/
node tools/shot.mjs name 4 1280 720  # eine Station fotografieren (Umgebungsvariable EVAL für eigene Befehle)
node tools/wx-test.mjs               # Wetter-Knopf, Sperre auf Deckel und Einschlag, Tonwerte
node tools/net-check.mjs             # keine externen Anfragen, keine Cookies, keine Konsolenfehler
node tools/touch-test.mjs           # iPad-Format 1024x768 mit Touch: Lasche ziehen, Klappe und Tier antippen, Karte schließen, Navigation, Kamera wischen
node tools/view-test.mjs            # iPad-Format mit Touch: Seite anfassen und blättern, Zwei-Finger-Zoom und -Verschieben, Hand-Knopf, Ansicht zurücksetzen
node tools/zeit-sheet.mjs 2,5.5,9    # Kontaktbögen aller Zeitfenster-Szenen (ohne das Buch zu laden, schnell)
node tools/zeit-live.mjs 2000 650   # Zeitfenster im echten Buch (breit und iPad-Größe)
node tools/zeit-touch.mjs           # Zeitfenster per Touch: Pfeile, Bildtipp, Einklappen
python3 tools/pron-ipa.py Wort ...   # espeak-IPA (mit Betonung) fuer Schreibvarianten
python3 tools/pron-test.py          # Hoerproben-Seite fuer Aussprache-Varianten (tools/pron-spec.json)
node tools/meteor-seq.mjs 1280 720 3.8,5.2,5.8  # Meteor-Ablauf in Bildern zu gegebenen Zeitpunkten (Sekunden nach dem Auslösen)
node tools/mem-check.mjs             # Texturspeicher je Station
node tools/audio-check.mjs           # 158 Klänge offline rendern und messen (Pegel, Klicks, Stille)
```

### Seiten und Tiere ergänzen

- Neues Tier: Silhouette in `src/art/animals/…` (siehe `docs/ART_GUIDE.md`), in `src/art/reg_*.js` eintragen, Karte in `src/data/animals.de.js` anlegen (Felder siehe Kopfkommentar), Stimme in `src/audio/voices.js`. Danach Sprechtext erzeugen (`speech-dump`, `make-narration --only card_<id>`).
- Neue Seite: `src/pages/pN.js` nach `docs/PAGE_GUIDE.md`, Text in `src/data/pages.de.js`, in `src/pages/index.js` eintragen. Anzahl der Blätter: `N_LEAVES` in `src/engine/book.js`.

## Bekannte Grenzen

- **Ton**: Die Klänge sind über Pegelmessung und Spektrogramme abgesichert, aber nicht mit Ohren beurteilt. Bitte einmal auf dem iPad probehören (Tierstimmen, Spieluhr, Einschlag und die Stille danach). iPad-Lautsprecher geben tiefe Töne unter ca. 150 Hz kaum wieder.
- **Tests**: Alle Bildtests liefen mit Software-Rendering (auch das iPad-Format 1024×768 mit simulierter Touch-Eingabe). Die Flüssigkeit auf einem echten iPad ist nicht gemessen; die automatische Qualitätsregelung soll das auffangen. Bitte einmal auf dem iPad in Safari durchblättern.
- **Sprachausgabe-Rückfall** (nur falls ein Clip fehlt): Stimme und Qualität hängen vom Gerät ab.
- **Hosting**: Das Buch ist eine statische Datei und braucht keinen Server. Veröffentlichung über GitHub Pages: `node build.mjs --main && bash tools/publish-pages.sh` schreibt `dist/index.html` auf den Branch `gh-pages`; einmalig auf GitHub unter Settings → Pages → „Deploy from a branch“ → `gh-pages` / root einschalten. Auch die Bibliothek (Repo `Bibliothek`) bindet das Buch über diese Adresse ein.

## Lizenzen

Code und im Code erzeugte Kunst (Figuren, Kulissen, Klänge): **MIT** (`LICENSE`). Texte, Karten und Dokumentation: **CC BY-SA 4.0** (`LICENSE-CONTENT`). Bitte bei Weitergabe nennen: „Das große Dinosaurier-Popup-Buch“ von Stephan Wilski, https://github.com/WIlski54/dinobuch. Einzelheiten und Bestandteile von Dritten (three.js MIT, clipper-lib Boost-Lizenz, esbuild/Playwright nur zum Bauen, Erzählstimme Piper „de_DE-thorsten-medium“ CC0 über sherpa-onnx): `NOTICE.md` und `assets/narration/LICENSE.txt`.
