PORTFOLIO — ALEXANDRU HORTOLOMEI
Übergabe an IT / Hosting
================================================================

1. WAS DAS IST
--------------
Eine statische Website. Reines HTML, CSS und JavaScript.
Kein Build-Schritt, keine Abhängigkeiten, keine Datenbank,
kein serverseitiger Code, kein Node, kein PHP.

Der gesamte Ordnerinhalt wird unverändert in das Web-Root
hochgeladen. Danach ist die Seite online.

2. EINSTIEGSPUNKT
-----------------
index.html

Weitere Seiten:
  impressum.html    Impressum
  datenschutz.html  Datenschutzerklärung
  fine-art.html     Platzhalterseite (derzeit nicht verlinkt,
                    nur über direkte Adresse erreichbar)

3. ORDNERSTRUKTUR
-----------------
Im Wurzelverzeichnis liegen nur die HTML-Seiten, favicon.svg,
diese README und vercel.json. Alles Übrige liegt unter assets/:

  assets/fonts/              Urbanist Regular und Medium (TrueType)
                             sowie OFL.txt mit der Lizenz
  assets/img/cases/aquares/  Fallstudie Aquares
  assets/img/cases/houts/    Fallstudie Houts
  assets/img/cases/oya/      Fallstudie Oya
  assets/img/cases/sb/       Fallstudie Schulbuch
  assets/img/cases/eigenzeit/ Fallstudie Eigenzeit
  assets/img/cases/print/    Printarbeiten (Avelura, MPU)
  assets/img/teaser/         Vorschaubilder der Arbeitenübersicht
  assets/img/ui/             Logos, Icons, Illustrationen

Alle Pfade sind relativ. Die Seite läuft damit in jedem
Unterverzeichnis und auch lokal per Doppelklick.

4. UMFANG
---------
101 Dateien, zusammen rund 26 MB, überwiegend JPEG.
Bilder sind bereits für das Web skaliert (1200–1800 px Breite,
progressives JPEG) und werden per loading="lazy" nachgeladen.

5. ANFORDERUNGEN AN DEN SERVER
------------------------------
Keine besonderen. Jeder statische Webspace genügt.

Empfohlen:
  - HTTPS mit Weiterleitung von http auf https
  - Weiterleitung von www auf die Hauptdomain (oder umgekehrt,
    einheitlich)
  - MIME-Typ image/svg+xml für .svg
  - MIME-Typ font/ttf für .ttf
  - Caching: lange Lebensdauer für Bilder, Schriften und SVG,
    kurze für die HTML-Dateien
  - Komprimierung (gzip oder brotli) für HTML, CSS und SVG
  - Fehlerseite 404 auf index.html, falls gewünscht

6. VORGESEHENE DOMAIN UND E-MAIL
--------------------------------
Domain:  alexandruhortolomei.de
E-Mail:  hello@alexandruhortolomei.de

Die Adresse ist im HTML bereits hinterlegt (Footer, Impressum,
Datenschutz). Nach Einrichtung des Postfachs sind keine
Änderungen am HTML nötig.

7. OFFENER PUNKT VOR DEM LIVEGANG
---------------------------------
In datenschutz.html ist der Abschnitt "Hosting und Server-
Logfiles" bewusst unvollständig. Dort stehen die Worte
"Noch zu ergänzen".

Einzutragen sind:
  - Name und Anschrift des Hosting-Anbieters
  - Speicherdauer der Server-Logfiles
  - Hinweis auf den Auftragsverarbeitungsvertrag

Die Seite sollte vor Veröffentlichung einmal rechtlich
geprüft werden.

8. TECHNISCHE HINWEISE
----------------------
Sprache
  Zweisprachig Deutsch und Englisch über data-en-Attribute
  im Markup. Die Umschaltung erfolgt im Browser, es gibt
  keine getrennten Sprachverzeichnisse. Die Auswahl wird in
  localStorage unter dem Schlüssel "site-lang" gespeichert
  und gilt seitenübergreifend.

Schriften
  Urbanist ist lokal eingebunden, es werden keine Schriften
  von Drittanbietern geladen.

Externe Verbindungen
  Keine. Weder Analyse noch Tracking, keine Cookies, keine
  eingebetteten Dienste. Einzige externe Links: LinkedIn
  und safs-beta.de, beide mit target="_blank" und
  rel="noopener".

Formulare
  Keine. Kontakt erfolgt ausschließlich über mailto-Links.

9. FARBEN UND SCHRIFT
---------------------
  #1F2027  Text und dunkle Flächen
  #F9F9F9  Hintergrund
  #5869B6  Akzent
  #D5D9EC  Akzent hell
  #DCDCDC  Linien

  Urbanist Regular 400 und Medium 500.
  Die Schnitte 600 und 700 werden aus Medium abgeleitet.
