---
cover: /images/bild.jpg
date: 2026-03-20
description: Kurzbeschreibung
dir: rtl
lang: ku-Arab
layout: post
subtitle: Untertitel
title: Titel
---

# README.md

## Artikel veröffentlichen (Kurzfassung)

1.  Neuer Artikel im Ordner erstellen:

\_posts/YYYY-MM-DD-artikelname.md

Beispiel:

\_posts/2026-03-20-neuer-artikel.md

2.  Artikel beginnt mit Front-Matter:

```{=html}
<!-- -->
```
3.  Danach folgt der Artikeltext in **Markdown**.

4.  Bilder liegen in:

/images/

5.  Veröffentlichen:

git add . git commit -m "add article" git push

GitHub Pages baut die Seite automatisch neu.
