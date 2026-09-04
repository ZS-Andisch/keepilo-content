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

**cookbooks-en (Release-Asset):** *The Fireless Cook Book* (Mitchell,
1909, [Project Gutenberg #60598](https://www.gutenberg.org/ebooks/60598))
als Markdown mit einem Abschnitt je Rezept — Kochen mit Restwärme in der
Kochkiste. Gemeinfrei; Gutenberg-Kopf und -Lizenz sind entfernt, die
Herkunft steht als erste Zeile im Dokument und in der `meta.json`. v1
enthielt zwei weitere Gutenberg-Bücher (Goudiss 1918, Hiller 1910), v2
nicht mehr. Gebaut mit `tools/gutenberg_cookbooks.py` und
`tools/build_content_pack.dart --src`.

**Moderne Notfall-Kochbücher** (Houston Health Department, Erie County
Emergency Eats, Good and Cheap) stehen nur als Verweis im `manifest.json`
und werden direkt vom jeweiligen Anbieter geladen — hier liegt nichts davon.

**manifest.json:** verweist außerdem auf Modelle (HuggingFace) und den
BBK-Ratgeber Notfallvorsorge — beide werden direkt von ihren Anbietern
geladen, hier liegt nur der Verweis.

Gebaut wird das Paket mit `tools/build_content_pack.dart` aus dem
SurvivalApp-Repo.
