# Keepilo — Inhalte

Inhaltspakete und Download-Manifest für die SurvivalApp. Die App lädt von
hier nur über die Release-Assets und `manifest.json` — dieses Repo ist kein
Ort zum Stöbern, die Inhalte gehören in die App.

## Quellen und Lizenzen

**survival-basics-en (Release-Asset):** 33 Kapitel des
[SurvivalManual-Wikis](https://github.com/ligi/SurvivalManual/wiki),
Stand siehe `meta.json` im Paket (Commit-Hash). Grundlage ist das
gemeinfreie US Army Survival Manual FM 21-76; die Kuratierung und
Erweiterungen des [SurvivalManual-Projekts](https://github.com/ligi/SurvivalManual)
stehen unter GPLv3. Dieses Paket gibt beides unverändert weiter —
Quelle und Lizenz stehen je Kapitel in der `meta.json` und werden in
der App am Dokument angezeigt.

**cookbooks-en (Release-Asset):** drei gemeinfreie Kochbücher von
[Project Gutenberg](https://www.gutenberg.org/), als Markdown mit einem
Abschnitt je Rezept: *The Fireless Cook Book* (Mitchell, 1909, #60598 —
Kochen mit Restwärme in der Kochkiste), *Foods That Will Win the War and
How to Cook Them* (Goudiss, 1918, #15464 — Sparen und Ersetzen von
Weizen, Fleisch, Fett, Zucker) und *Left-Over Foods and How to Use Them*
(Hiller, 1910, #72831 — Resteküche). Gutenberg-Kopf und -Lizenz sind
entfernt; die Herkunft steht als erste Zeile in jedem Dokument und je
Dokument in der `meta.json`. Gebaut mit `tools/gutenberg_cookbooks.py`
und `tools/build_content_pack.dart --src`.

**manifest.json:** verweist außerdem auf Modelle (HuggingFace) und den
BBK-Ratgeber Notfallvorsorge — beide werden direkt von ihren Anbietern
geladen, hier liegt nur der Verweis.

Gebaut wird das Paket mit `tools/build_content_pack.dart` aus dem
SurvivalApp-Repo.
