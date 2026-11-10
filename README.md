# optimus-prime-deck

**Hand-coded HTML slide decks at 1920×1080, built to be imported into Canva.**

Each deck is a single HTML file where every slide is a fixed 1920×1080 block. The decks are hosted on GitHub Pages so Canva can import them by URL, then they are edited and presented from Canva.

Live: https://melvernmogens.github.io/optimus-prime-deck/

## Decks

| File | Deck | Slides |
|---|---|---|
| `index.html` | *OPTIMUS PRIME — The Prime Directive* (cinematic, v1) | 5 |
| `optimus-prime-deck-v2.html` | Optimus Prime v2 – Canva-compatible fills and gradients | 5 |
| `optimus-prime-deck-v3.html` | Optimus Prime v3 – split fracture around the text band, twin radial halos | 5 |
| `prasmul-deck-v1.html` … `-v3.html` | *Universitas Prasetiya Mulya — Sebuah Pengantar* (Indonesian) | 10 |
| `prasmul-v2/index.html`, `prasmul-v3/index.html` | Prasmul deck, editorial keynote rebuild (same deck at folder paths) | 10 |
| `prasmul-positioning-harga/index.html` | *Membaca Positioning dari Daftar Harga* – Prasmul positioning read from its published S1 fee structure | 8 |

## Canva import notes

These came out of getting the decks to survive Canva's HTML import:

- Use solid fills for headline text, not gradient text.
- Bake blur into gradients instead of using CSS `filter: blur` or blend modes.
- Avoid `transform: translateY(...)` and rotation on key elements; Canva crops to the box before the transform.
- When Canva caches an old version, publish the new deck at a new path.

## View / edit

Open any file in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

To import into Canva, use the GitHub Pages URL of the deck, e.g. `https://melvernmogens.github.io/optimus-prime-deck/optimus-prime-deck-v3.html`.

Fonts load from Google Fonts (Anton, Barlow Condensed, Inter, Instrument Serif, IBM Plex Mono, Archivo, JetBrains Mono).

Built by [Melvern Mogens](https://github.com/MelvernMogens).
