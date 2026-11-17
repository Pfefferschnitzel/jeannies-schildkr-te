# 🐢 Jeannies Schildkröten 🌼

Ein kleines Garten-Verteidigungsspiel: Die bösen Schildkröten wollen Jeannies Blumen fressen!
Als Spielerin baust du mit Steinen Wege um, ohne die Schildkröten zu töten, und leitest sie
zur Kleeblattwiese am rechten Rand, wo sie sich satt fressen und glücklich weiterziehen.

## Spielen

Einfach "index.html" im Browser öffnen (oder GitHub Pages aktivieren).

## Spielprinzip

- 🪨 **Steine bauen:** Klick auf eine Wiese baut einen Stein, Klick auf einen Stein baut ihn zurück.
- 🧠 **Umleiten statt töten:** Die Schildkröten suchen sich per Wegfindung (BFS) immer den kürzesten
  Weg zur nächsten Blume. Wird der Weg blockiert, werden sie kurz **krummelig** (😤) und suchen eine
  neue Route.
- 🍀 **Kleeblattwiese:** Sind die Blumen unerreichbar, wandern die Schildkröten zur Kleeblattwiese,
  fressen Klee und werden als 💚 gezählt.
- 🌊 **Wellen:** Jede Welle bringt mehr und schnellere Schildkröten. Pro geschaffter Welle gibt es
  +2 Steine, alle 3 gerettete Schildkröten +1 Stein.
- 🥀 **Niederlage:** Frisst eine Schildkröte alle Blumen auf, ist das Spiel vorbei.

## Technik

Reines HTML/CSS/JavaScript in einer Datei, keine Abhängigkeiten. Rendering über die Canvas 2D API,
Wegfindung über Multi-Source-BFS-Distanzfelder, die bei jeder Stein-Änderung neu berechnet werden.
