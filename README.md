# Dot Sphere Generator

Generator animirane, "halftone" tackaste sfere u browseru — canvas 2D, bez build koraka, jedan `index.html` fajl.

## Pokretanje

Samo otvori `index.html` u browseru (Chrome/Edge preporuceno zbog WebM exporta). Nema instalacije, nema build-a.

Ili preko GitHub Pages: Settings → Pages → Deploy from branch → `main` / `/ (root)`.

## Funkcionalnosti

- **Grid** — broj prstenova/segmenata, velicina i boja tacaka, providnost zadnje (nevidljive) strane sfere
- **Pozadina** — providna (za export sa alfa kanalom) ili puna boja
- **Swirl (Twist)** — spiralno uvijanje grid-a od pola do pola, plus nezavisan "swirl drift"
- **Twirl** — 2D distorzija (kao Photoshop Twirl filter), vise izrazena na ivici nego u centru
- **Rotacija celog objekta** — staticna pocetna orijentacija (X/Y/Z) + animirana brzina rotacije po sve tri ose
- **Kretanje tacaka (wobble)** — per-dot "disanje" nezavisno od rotacije
- **Keyframes & Bezier animacija** — kljucni kadrovi za 8 parametara (rotacije, twist, twirl, wobble amplituda, velicina tacke, providnost zadnje strane), sa custom bezier easing krivama po segmentu (drag & drop graf editor, kao Graph Editor u After Effects)
- **Loop alati** — automatski izracunava trajanje za savrsen loop (jedan pun obrtaj)
- **Export**
  - PNG sekvenca (ZIP, sa alfa kanalom) — najpouzdanije za After Effects
  - WebM (transparent) — radi pouzdano samo u Chrome/Edge desktop

## Napomene

- Sve racunanje se desava lokalno u browseru, nema servera ni mreznih poziva (osim JSZip biblioteke sa cdnjs.cloudflare.com).
- Za savrsen loop drzi animirane "drift" i "swirl/twirl animacija" parametre na 0, ili rucno podesi trajanje loop-a da odgovara njihovom periodu.

## Licenca

MIT — slobodno koristi, menjaj i deli.
