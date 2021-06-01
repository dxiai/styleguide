---
title: Alerts and Buttons
hide_hero: true
---

# Alerts

- Alerts are used to highlight sections of contents. There are four types of colors used throughout our documents: 

  - `primary` stands for definitions, 
  - `info` indicates general highlights,
  - `warning` shows potential causes of errors, 
  - `danger` points to misuse, and 
  - `success` stands for best practices.

- Buttons are used for linking resources. 
  - `success`refers to other pages, 
  - `primary` means data. 

<p class="alert alert-warning">hello warning</p>


<p class="alert alert-info" markdown=1> 

a quote as a warning. This would be awesome. This is not really working for us :( This quote *should* be handled correctly. this is achieved by the `markdown=1` attribute, which surprisingly also works in moodle!

</p>

Moodle folks support `markdown=1` but not `markdown="1"`. Moodle will then start rendering a Page or text field in a way that it is no longer useful. Jupyter Notebooks don't support mixing HTML and inline markdown at all. GitHub has its own way of mixing markdown inside HTML tags. However, this approach is **only** supported by GH, but not even on github pages. On the other hand, github markdown no longer supports bootstrap css classes. 

# Buttons

We use buttons to highlight important links, such as pointers to subchapters. For buttons and alerts we have a smal compatibility layer for bulma so we can use bootstrap classes. This makes it easier to load the same markdown in moodle.

Moodle uses fontawesome 4 and we should use these icons. 

<p class="btn btn-primary"><i class="fa fa-file-o"></i> This is a button</p>

The initial theme uses fontawesome 5, but we switched it back to 4 to be as compatible to our moodle theme as possible.

<p class="button is-primary"><i class="fa fa-file"></i> This is another button</p>

We can have special Buttons directly in markdown as shown below. It is important to remember that **Moodle** does not allow such trickery. Thus, we can use only the above strategy for course material. The following example will only work on dxi.ai webpages.

```markdown
[<i class="fa fa-home"/> Back to Home](https://www.dxi.ai/styleguide/){: .btn.btn-success}
```

Note that css attribute work only with links. However, we should not use them, because moodle markdown does not render them, just like github markdown. having such links is only useful for resources that are confied to a page. 

The result is the following link: 

[<i class="fa fa-home"/> Back to Home](https://www.dxi.ai/styleguide/){: .btn.btn-success}