# 🐢 Jeannies Schildkröten 🎱

Ein Garten-Verteidigungsspiel im Billard-Stil: Die bösen Schildkröten wollen Jeannies Blumen
fressen! Als Spielerin setzt du Steine in ihren Weg, sodass sie wie Billardbälle abprallen,
und lenkst sie so zur Kleeblattwiese am rechten Rand. Töten ist verboten, sie werden nur kurz
krummelig.

## Spielen

Einfach "index.html" im Browser öffnen (oder GitHub Pages aktivieren).

## Spielprinzip

- 🐢 Schildkröten kriechen **geradlinig** auf die nächste Blume zu. Eine gestrichelte Linie zeigt ihr Ziel.
- 🪨 **Klick auf eine Wiese** setzt einen Stein, Klick auf einen Stein hebt ihn wieder auf.
- 😤 Prallt eine Schildkröte an einem Stein ab, wird sie kurz **krummelig** und dann **benommen**:
  sie kriechet geradeaus weiter wie ein Billardball und wird dabei etwas langsamer.
- 🍀 Nur im benommenen Zustand erreichen sie die **Kleeblattwiese** am rechten Rand, fressen Klee
  und werden als 💚 gezählt. Kettenstöße über mehrere Steine lösen einen 🎱-Bonus-Banner aus.
- 🪃 Am Zaun drehen benommene Schildkröten um und nehmen wieder Kurs auf die nächste Blume.
- 🌊 **Wellen:** Jede Welle bringt mehr und schnellere Schildkröten. Pro geschaffter Welle gibt es
  +1 Stein und eine neue Blume wächst nach (max. 10), alle 3 gerettete Schildkröten +1 Stein.
- 🥀 **Niederlage:** Frisst eine Schildkröte alle Blumen auf, ist das Spiel vorbei.

## Technik

Reines HTML/CSS/JavaScript in einer Datei, keine Abhängigkeiten. Rendering über die Canvas 2D API.
Die Schildkröten bewegen sich physikalisch (geradlinig mit Reflexion an Steinen und Zaun,
Winkel-Jitter gegen Endlosschleifen).
