# double-calender-1

Weinkeller Inventar – eine Single-Page-App (`index.html`) zum Verwalten deiner Weinsammlung: Flaschen mit Kategorie, Rebsorte, Region, Jahrgang, Kaufdatum, Preis, Trinkfenster und Bewertung erfassen, Bestand per "Flasche öffnen" pflegen und Statistiken zu Kellerwert, Kategorien und Trinkreife einsehen. Daten werden lokal im Browser gespeichert (localStorage) und lassen sich als JSON exportieren/importieren.

Flaschen lassen sich zusätzlich per Barcode (EAN) erfassen: Kamera-Scan (über [html5-qrcode](https://github.com/mebjas/html5-qrcode)) oder manuelle Eingabe, dazu ein automatischer Datenabgleich mit [Open Food Facts](https://world.openfoodfacts.org) (Name, Region, Kategorie-Hinweis – Jahrgang, Preis und Bewertung müssen weiterhin manuell ergänzt werden, da sie nicht Teil des Barcodes sind). Wird ein bereits erfasster Barcode erneut gescannt, bietet die App an, den Bestand statt einen Duplikat-Eintrag zu erhöhen. Der Kamera-Scan benötigt eine HTTPS-Seite (z.B. GitHub Pages) – bei einer lokal geöffneten Datei funktioniert nur die manuelle Eingabe.

Zu jedem Wein lässt sich außerdem ein Foto aufnehmen (wird vor dem Speichern automatisch verkleinert, um den begrenzten Browser-Speicherplatz zu schonen) und erscheint als Miniaturbild links in der Kellerliste sowie größer in der Detailansicht.

Design: natives iOS-Look-and-Feel – Systemschrift (San Francisco via `-apple-system`), iOS-Systemfarben (Blau als Akzent, Grün/Rot/Orange/Gelb/Teal als Statusfarben), gruppierte Listen ohne Rahmen, ein Segmented Control für die Filter und ein echter iOS-Schalter für das Geschenk-Flag.
