# Trainingsplan aufs iPhone — Schritt für Schritt

Zwei Teile. **Teil A** dauert 2 Minuten und du hast den Plan sofort im Kalender.
**Teil B** dauert ~10 Minuten und gibt dir die App mit Icon, Offline-Betrieb, Fortschritt
und Claude-Anbindung. Mach A jetzt, B wenn du 10 Minuten hast.

---

## TEIL A — Kalender aufs Handy (2 Minuten, jetzt)

1. Öffne die **Claude-App auf dem iPhone** und geh in diese Unterhaltung.
2. Scroll zur Datei **`hyrox-block1.ics`** und tippe sie an.
3. iOS öffnet den Kalender und fragt, was passieren soll → **Alle hinzufügen**
   (falls die Auswahl kommt: einen eigenen Kalender „Hyrox" wählen, dann kannst du ihn
   später mit einem Schalter aus- und einblenden).
4. Fertig. 32 Termine bis zum Renntag, jeweils mit Erinnerung 30 min vorher und der
   kompletten Einheit in den Notizen. Dazu täglich 21:30 die Rückenroutine.

Uhrzeiten passen nicht? Einzelne Termine im Kalender einfach verschieben — beim Import
(anders als beim Abo in Teil B) sind sie beschreibbar.

---

## TEIL B — Die App aufs Handy (~10 Minuten)

Ergebnis: eigenes Icon auf dem Homescreen, Vollbild, offline im Gym-Keller nutzbar,
Häkchen und Zahlen bleiben gespeichert, und pro Trainingstag ein Knopf, der Claude mit
dem vollen Kontext öffnet.

### B1 — Hosten (am Rechner, ~5 min)

GitHub Pages, kostenlos, kein Server.

1. **Konto:** [github.com](https://github.com) → *Sign up*.
   Nimm ein **privates** Konto, keines das an die Arbeit gebunden ist.
2. **Repository:** oben rechts **+** → *New repository*
   - *Repository name:* `hyrox`
   - **Public** wählen (Hinweis dazu unten)
   - *Create repository*
3. **Dateien hochladen:** auf der leeren Repo-Seite auf **uploading an existing file**.
   Diese **8 Dateien** aus dem entpackten Ordner reinziehen:
   ```
   index.html
   sw.js
   manifest.webmanifest
   icon-180.png
   icon-512.png
   icon-maskable.png
   hyrox-block1.ics
   hyrox-tracker.xlsx
   ```
   → unten **Commit changes**.
   *Wichtig: die Dateien selbst hochladen, nicht den Ordner — sonst liegt `index.html` eine
   Ebene zu tief und die Seite bleibt leer.*
4. **Pages einschalten:** Reiter **Settings** → links **Pages**
   - *Source:* `Deploy from a branch`
   - *Branch:* `main` und `/ (root)` → **Save**
5. **1–2 Minuten warten**, Seite neu laden. Oben steht deine Adresse:
   ```
   https://DEIN-NAME.github.io/hyrox/
   ```
   Im Browser öffnen und prüfen, dass der Plan da ist.

**Zu „Public":** Der Inhalt ist damit für jeden erreichbar, der die URL kennt. Drin steht
nur der Trainingsplan — keine persönlichen Daten. Deine eingetragenen Zahlen liegen
ausschließlich auf deinem Handy, nie auf GitHub. Pages aus privaten Repos braucht ein
Pro-Konto.

### B2 — Adresse aufs iPhone

Schick dir die URL selbst: WhatsApp an dich, private E-Mail, Notiz. Nur dieser eine
Textlink muss vom Rechner aufs Handy — keine Dateien.

### B3 — Zum Homescreen (30 Sekunden)

1. URL in **Safari** öffnen. *(Muss Safari sein — nur Safari kann auf iOS zum Homescreen
   hinzufügen.)*
2. **Teilen-Symbol** unten (Quadrat mit Pfeil nach oben).
3. Runterscrollen → **Zum Home-Bildschirm**.
4. Name `Hyrox` bestätigen → **Hinzufügen**.
5. Icon antippen. Läuft im Vollbild.

> **Der eine Fehler, der weh tut:** iOS behandelt Safari und die Homescreen-App als zwei
> getrennte Speicher. Also **erst zum Homescreen hinzufügen, dann anfangen zu loggen** — und
> ab dann immer über das Icon öffnen. Was du vorher in Safari eingetragen hast, ist in der
> App nicht sichtbar.

### B4 — Kalender abonnieren (optional, statt Teil A)

In der App unten auf **Referenz**, oben die Karte *„Auf dieses Gerät holen"* →
**Kalender abonnieren**. Der Kalender aktualisiert sich dann automatisch, wenn ich Monat 2
nachliefere. Nachteil: abonnierte Kalender sind schreibgeschützt, Termine lassen sich nicht
verschieben.

Beides parallel ist unnötig — entweder Import (Teil A, beschreibbar) oder Abo (hier,
selbstaktualisierend).

---

## Mit Claude an einer Einheit arbeiten

Auf **jeder** Trainingseinheit — im Tab *Heute* und in jedem Tag, den du im Tab *Plan*
antippst — sitzt unten ein oranger Knopf:

**„Diese Einheit mit Claude anpassen"**

Der öffnet einen neuen Claude-Chat, in dem schon alles drinsteht:

- dein komplettes Profil (Rennen, Zielzeit, Maße, aktuelle 5-km-Zeit, Rückenthema,
  Equipment inklusive defekter Klimmzugstange und fehlender Carry-Möglichkeit, Gym ab 01.09.,
  Zeitfenster, Wochenstruktur, alle Paces)
- die geplante Einheit dieses Tages mit allen Vorgaben
- dein Log dazu, falls du schon etwas eingetragen hast (km, Anstrengung, Rücken, Notiz)

Du musst also **nichts erklären**. Einfach dahinter schreiben, was los ist:

> „Habe nur 30 Minuten"
> „Rücken zieht heute, was mache ich stattdessen"
> „Bin im Hotel, nur Körpergewicht"
> „Fühlt sich zu leicht an, kann ich mehr?"
> „Wie lange halte ich die Hantel beim Farmers Hold, wenn 20 kg zu leicht wird?"

Wenn der Chat nicht automatisch mit dem Text aufgeht, nimm den zweiten Knopf
**„Nur den Prompt kopieren"** und füge ihn in Claude ein — gleiches Ergebnis.

**Für den ganzen Block:** Tab *Fortschritt* → **„Block mit Claude auswerten"**. Da hängt
dein komplettes Log dran (alle Wochen, Ist/Soll-km, RPE, Rücken-Scores, Notizen, Benchmark-
Splits). Das ist der Knopf für den **06.09.**, wenn Monat 2 geplant wird.

Damit gilt: die App ist das Nachschlagewerk und das Logbuch, Claude ist das Coaching
obendrauf — und die Brücke dazwischen sind zwei Knöpfe, statt jedes Mal den Kontext neu zu
tippen.

---

## Der Tracker

Excel auf dem iPhone ist keine Freude — `hyrox-tracker.xlsx` ist für den Rechner gedacht.
Über `…/hyrox-tracker.xlsx` von überall ladbar. Wenn du die App nutzt, kannst du ihn auch
komplett ignorieren: sie erfasst dieselben Zahlen.

## Später aktualisieren

Wenn Monat 2 dazukommt: im Repo `index.html` per Upload ersetzen → *Commit changes*. Die App
holt sich die neue Version beim nächsten Öffnen mit Internet automatisch. **Deine
eingetragenen Zahlen bleiben erhalten**, die liegen getrennt vom Programmcode.

## Daten und Sicherheit

Häkchen, km, RPE, Rücken-Scores und Notizen liegen nur im Speicher deines Geräts. Kein Konto,
kein Server, keine Übertragung. Kehrseite: bei „Website-Daten löschen" oder Löschen der App
sind sie weg. Vor Aufräumaktionen einmal *Fortschritt → Zusammenfassung teilen* an dich selbst
schicken.
