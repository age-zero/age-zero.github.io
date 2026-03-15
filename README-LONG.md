---
cover: /images/mein-bild.jpg
date: 2026-03-20
description: Kurze Beschreibung
dir: rtl
lang: ku-Arab
layout: post
subtitle: Untertitel
subtitle2: optional
title: Titel des Artikels
translations:
  de: /artikel-de/
---

# README-LONG.md

## Age-Zero -- Artikel veröffentlichen

Diese Anleitung beschreibt, wie neue Artikel auf der Age-Zero GitHub
Pages Seite veröffentlicht werden.

------------------------------------------------------------------------

## 1. Neuer Artikel

Alle Artikel liegen im Ordner:

\_posts/

Dateiname:

YYYY-MM-DD-artikelname.md

Beispiel:

2026-03-20-neuer-artikel.md

------------------------------------------------------------------------

## 2. Artikelstruktur

Jeder Artikel beginnt mit einem Front-Matter Block:

Danach folgt der Artikeltext in Markdown.

------------------------------------------------------------------------

## 3. Sprachen

Deutsch:

lang: de

Kurdisch (Sorani):

lang: ku-Arab dir: rtl

Übersetzungen:

translations: de: /artikel-de/

------------------------------------------------------------------------

## 4. Bilder

Bilder werden gespeichert in:

/images/

Einfügen im Artikel:

![Beschreibung](/images/bildname.jpg)

Für Social Media Vorschau:

cover: /images/bildname.jpg

------------------------------------------------------------------------

## 5. Artikel veröffentlichen

git add . git commit -m "add new article" git push

GitHub Pages baut die Seite automatisch neu.

------------------------------------------------------------------------

## 6. Indexseite

Die Startseite listet automatisch alle Artikel mit:

-   Titel
-   Datum
-   Beschreibung
-   Sprachlinks

Du musst dafür nichts manuell ändern.

------------------------------------------------------------------------

## 7. Layout

Artikel werden automatisch über das Post-Layout gerendert:

-   RTL Layout für Sorani
-   LTR Layout für Deutsch
-   Sprachumschalter im Artikel

------------------------------------------------------------------------

## 8. Beispielartikel

\_posts/2026-02-10-strategie-ku.md

Dieser Artikel zeigt die komplette Struktur eines Beitrags.
