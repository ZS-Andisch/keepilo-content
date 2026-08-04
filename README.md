# SurvivalApp — Inhalte

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

**manifest.json:** verweist außerdem auf Modelle (HuggingFace) und den
BBK-Ratgeber Notfallvorsorge — beide werden direkt von ihren Anbietern
geladen, hier liegt nur der Verweis.

Gebaut wird das Paket mit `tools/build_content_pack.dart` aus dem
SurvivalApp-Repo.
