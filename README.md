# ZukunftsAG Szenariobewertung

Bewertungsmatrix für fünf Modelle (Bestehendes Modell, Autonomie-Kombi-Modell, Autonomie-Modell (groß), Minimal-Modell +, Minimal-Modell) anhand von sieben Kriterien. Jede Zelle enthält Argumente als Text und eine manuell gewählte Ampel. Unter jeder Spalte steht eine Gesamteinschätzung mit Kommentar und Ampel.

## Dateien

| Datei | Zweck |
|---|---|
| `index.html` | Oberfläche und Logik. Wird nur bei Funktionsänderungen angepasst. |
| `data.js` | Alle Inhalte (Argumente, Ampeln, Modell- und Kriteriennamen). Diese Datei wird gemeinsam bearbeitet. |

## Arbeitsablauf in der Gruppe

1. Repository klonen oder aktuellen Stand pullen.
2. `index.html` im Browser öffnen (Doppelklick genügt, ein Server wird nicht benötigt).
3. Argumente eintragen und Ampeln setzen. Änderungen werden automatisch als lokaler Entwurf im Browser gesichert.
4. Über **data.js exportieren** die Datei herunterladen und im Repository ersetzen.
5. Committen, pushen und bei Bedarf einen Pull Request öffnen.

Der Export schreibt die Felder immer in gleicher Reihenfolge und mit Zeilenumbrüchen pro Wert. Dadurch zeigt Git nur tatsächlich geänderte Zellen als Unterschied an, und Konflikte lassen sich zeilenweise lösen.

Wurde `data.js` nach einem Pull verändert, meldet die Seite, dass der lokale Entwurf auf einem älteren Stand beruht, und bietet an, ihn zu verwerfen.

## Modelle oder Kriterien ändern

In `data.js` lassen sich Namen ändern sowie Einträge unter `modelle` und `kriterien` ergänzen oder entfernen. Fehlende Zellen werden beim Laden automatisch angelegt. Die Spaltenbreite ist in `index.html` über `--spalte` einstellbar.

## Veröffentlichung

Über GitHub Pages (Settings, Pages, Branch `main`, Ordner `/root`) steht die Matrix als Webseite zur Verfügung. Bearbeitet wird weiterhin über das Repository.

## Ampelbedeutung

Grün ist günstig für das Modell, Rot ungünstig, Gelb gemischt oder offen. Beim Kriterium Risiko/Nachteil steht Grün für ein geringes Risiko.
