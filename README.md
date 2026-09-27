# KinoTom

Privater Prototyp eines kuratierten Filmkatalogs. Die Filme werden auf den
YouTube-Kanälen ihrer jeweiligen Filmschaffenden geöffnet; KinoTom hostet keine
Filmdateien.

## Entwicklung

Die statische Website liegt in `dist/`. Lokal starten:

```sh
python3 -m http.server 8765 --directory dist
```

Die aktuelle private Vorschau wird über Sites gehostet. Der Code kann später
mit GitHub Pages veröffentlicht werden, indem ein GitHub-Actions-Workflow
`dist/` als Pages-Artefakt bereitstellt. GitHub Pages ist für die öffentliche
Freigabe noch nicht aktiviert.

Der Name KinoTom, Rechtstexte sowie Werbung und Analytics sind vor einer
öffentlichen Freigabe zu klären.
