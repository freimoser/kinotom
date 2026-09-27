# KinoTom

Prototyp eines kuratierten Filmkatalogs. Die Filme werden auf den
YouTube-Kanälen ihrer jeweiligen Filmschaffenden geöffnet; KinoTom hostet keine
Filmdateien.

## Entwicklung

Die statische Website liegt in `dist/`. Lokal starten:

```sh
python3 -m http.server 8765 --directory dist
```

Die Seite wird bei jedem Push auf `main` per GitHub Actions aus `dist/` auf
GitHub Pages veröffentlicht. Die bisherige Sites-Vorschau ist davon getrennt
und wird durch GitHub-Pushes nicht automatisch aktualisiert.

Die Pages-Version ist eine öffentliche Vorschau mit `noindex`. Der Name
KinoTom, Rechtstexte sowie Werbung und Analytics sind vor dem offiziellen
Launch zu klären.

## Google Search Console

- URL-Präfix-Property: `https://freimoser.github.io/kinotom/`
- Sitemap: `https://freimoser.github.io/kinotom/sitemap.xml`
- Für die Eigentumsbestätigung kann die von Google bereitgestellte HTML-Datei
  unverändert in `dist/` abgelegt und auf `main` veröffentlicht werden.
- `noindex` in `dist/index.html` erst entfernen, wenn Impressum und Datenschutz
  mit den echten Betreiberangaben veröffentlicht und geprüft wurden. Solange
  `noindex` aktiv ist, zeigt GSC die Seite als nicht indexierbar an.
- Bei Umzug auf eine eigene Domain Canonical-URL, Sitemap und GSC-Property
  entsprechend aktualisieren.
