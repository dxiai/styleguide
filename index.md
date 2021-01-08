---
title: DxI Styleguide
hero_height: is-large
hide_navigation: false
---

## Einleitung

Zur Bearbeitung und Verwaltung der Inhalte können wir den [Editor von GitHub](https://github.com/dxiai/tmppages.github.io/edit/gh-pages/index.md) verwenden. Dazu verwenden wir sowohl für die Website als auch unsere Kursmaterialien sog. Markdown Dateien. Dabei müssen wir berücksichtigen, dass weder diese Webseite noch Moodle den GitHub dialekt von Markdown verstehen. Die hier verwendeten Varianten haben ein paar Eigenheiten, die in diesem Styleguide beschrieben werden. In den meisten Fällen wird das kein Problem darstellen, weil es sich um Abweichungen im Detail handelt. Die in diesem Styleguide beschriebenen Techniken zeigen die Vorgehen zur Erstellung von Inhalten für die dxi.ai Web-seite und für unsere Moodle Kurse. 

<p class="alert alert-warning" markdown=1>**Status dieses Dokuments** - Dieser Styleguide wurde ursprünglich auf Englisch geschrieben. Der Rest der Webseite ist auf Deutsch. Wir arbeiten noch an der Übersetzung der einzelnen Seiten.</p>

## Warum Markdown

Markdown ist viel einfacher als HTML, vor allem wenn ein WYSIWYG Editor das ganze aufbereitet. Ausserdem ist die Versionierung von Markdown sehr viel einfacher und wir können Regeln für die Formatierung und den Stil leichter umsetzen, weil wir nur sehr einfacher Formatierungsregeln haben. 

Markdown wird dann von einem Prozessor in HTML umgewandelt. Bei Moodle kann man zum Beispiel "unformatierten Text" als Markdown interpretieren lassen. Unsere Webseite wird bei jeder Ergänzung im [Inhaltsrepository](https://github.com/dxiai/dxiai.github.io) durch GitHub Pages mit [Jekyll](https://jekyllrb.com/) neu gebaut und anschliessend automatisch veröffentlicht. 

## Zielsetzung 

Dieser Styleguide gibt einen Überblick zu den Eigenheiten der verschiedenen Markdown Dialekte, die wir in unserem Team verwenden. Dazu gehören:

- [GitHub flavoured markdown](https://github.github.com/gfm/)
- [dxi.ai "Jekyll" Markdown (karmadown)](https://kramdown.gettalong.org/syntax.html)
- Moodle Markdown 
- Jupyter Markdown

### Markdown

Dieser Abschnitt beinhaltet ein einfaches Markdown Tutorial.

Es zeigt die Grundprinzipien dieser Formatierungssyntax. Markdown ist eine leichtgewichtige und einfach zu verwendente Formatierungssyntax für Textblöcke. Es beinhaltet verschiedene Konventionen, z.B. für **fetten Text** oder *kursiven Text*.  

> Einrückungen für Zitate zentraler Bestandteil von Markdown, die leider nicht von Moodle unterstützt werden. 


```markdown
Dieser Codeblock hat eine Syntaxhervorhebung.

# Überschrift 1
## Überschrift 2
### Überschrift 3

- Punkte
- Liste

1. Nummerierte
2. Liste

**Fett** und _Kursiv_ sowie `Code` Text.

Ein [Link](url) und ein ![Bild](src)
```

Mehr Details zum [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Weitere Themen

Webseiten sind komplexer als die Dokumentation auf Github festhält. Das gilt vor Allem für Lernmaterialien, die verschiedene Hervorhebungen haben. Dazu zählen die folgenden Gestaltungselemente. 

[Warnungen und Buttons](alerts.md){: .btn.btn-primary}

[Code Fragmente](code.md){: .btn.btn-primary}

[Formeln](mathjax.md){: .btn.btn-primary}

[Blogs und Seiten](blogs.md){: .btn.btn-primary}

[Automatisierung](automation.md){: .btn.btn-primary}


### Jekyll Themes

Diese Webseite verwendet für das Layout und Formatirungen ein angepasstes [Jekyll Theme](https://github.com/dxiai/dxiai-theme). Dieses Theme sollte für alle Projekte verwendet werden. Änderungsvorschläge am Theme sollten per [Issue](https://github.com/dxiai/dxiai-theme/issues) angefordert werden.

