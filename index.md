---
title: DxI Temporary Pages
hero_height: is-large
hide_navigation: true
hero_darken: true
---

## Introduction

This should be a bulma style page... not sure why it does not show.

You can use the [editor on GitHub](https://github.com/dxiai/tmppages.github.io/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

[link other page](other_index.md){: .btn.btn-primary}

Note that css attribute work only with links. However, we should not use them, because moodle markdown does not render them, just like github markdown. having such links is only useful for resources that are confied to a page. 

This page is a markdown tutorial, because we need it for testing. It happens that sometimes a deployment runs too fast after a theme release.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

> A simple quote, which does not work in moodle. 

<p class="alert alert-warning" markdown=1> 

a quote as a warning. This would be awesome. This is not really working for us :( This quote *should* be handled correctly. this is achieved by the `markdown=1` attribute, which surprisingly also works in moodle!

</p>

Moodle folks support `markdown=1` but not `markdown="1"`. Moodle will then start rendering a Page or text field in a way that it is no longer useful. Jupyter Notebooks don't support mixing HTML and inline markdown at all. GitHub has its own way of mixing markdown inside HTML tags. However, this approach is **only** supported by GH, but not even on github pages. On the other hand, github markdown no longer supports bootstrap css classes. 

Do we support mathjax on dxi.ai?

$$

\sum_{i=1}^{n}{foo_n}

$$

No mathjax support in our theme. This needs fixing the theme to include the mathjax cdn. while mathJax is supported, it needs some fixing to get the layout correct. right now the css seems to interfere with lowered indeces and markup. 

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/dxiai/tmppages.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
