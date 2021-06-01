---
hide_hero: true
# callouts: callouts
---

## Normale Seiten

Eine normale Seite enthält "statische" bzw. generische Informationen. Oft sind es Landeseiten für spezielle Inhalte oder Projekte. Normale Seiten **müssen** von anderen Seiten oder über [Menus](https://www.dxi.ai/styleguide/#nicht-fertig) **explizit** verlinkt werden.

## Andere Inhalte

Neben den Normalenseiten gibt es noch zwei zusätzliche Inhaltstypen: 

- Blog-Posts 
- Datenseiten

## Blog-Posts 

Ein Blog-Post ein ein kleiner in sich geschlossener Artikel. Das können Neuigkeiten, Reflexionen oder Ankündigungen sein. Neue Videos sollten auch als Blog-Beiträge angekündigt werden. Die drei neusten Blog-Posts landen auf der [dxi.ai Homepage](https://www.dxi.ai/) und sind über die [Blogs-Kategorie](https://www.dxi.ai/blog/) erreichbar.

Jeder Blog-Beitrag muss im Ordner `_posts` abgelegt werden. Der Dateiname hat das Format: `YYYY-MM-DD-autorenname.md`. Dabei muss darauf geachtet werden, dass die Dateiendung zwingend `.md` sein muss! Ohne diese Endung ignoriert die Webseite diesen Inhalt einfach. Das Datum im Dateinamen ist idealerweise das Veröffentlichungsdatum.

Falls ein Autor mehr als einen Beitrag an einem Tag erstellt, dann wird für jeden zusätzlichen Beitrag ein Zähler hinzugefügt. Beispiel:

- Erster Beitrag: `2021-06-01-glahn.md`
- Zweiter Beitrag: `2021-06-01-glahn-1.md`
- Dritter Beitrag: `2021-06-01-glahn-2.md`
- usw.

Jeder Blog-Beitrag muss die folgende einführende Struktur haben.

```
---
layout: post
title:  Title of the blog
author: Autorennamen
date: YYYY-MM-DD
tags: 
- development
- test
---
```

**Achtung:** Die Tags müssen als YAML-Liste erfasst werden, selbst wenn es sich nur um ein einzelnes Tag handelt. Sind die Tags keine Liste, dann bricht das Layout.

## Datenseiten

Datenseiten sind speziell. Diese Seiten beinhalten eine YAML-Datenstruktur, aus der der eigentliche Seiteninhalt erzeugt wird. 

[<i class="fa fa-home"/> &nbsp; Back to Home](https://www.dxi.ai/styleguide/){: .btn.btn-success}
