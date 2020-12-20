---
title: Alerts and Buttons
hide_hero: true
---

A teaser text can be included at the top. 

# Alerts

This page should have a header but no hero information

I wonder if a force deployment is possible. This pages is supposed to be almost empty. ventually we should have some information by now. I wonder what the problem is. and why this deployment takes so long.

This page should get immediately updated. More or less at least

It seems that some information has been restricted from a sass bug. Stupidly pg paged did not report such error. 

The following chunk checks the different types of links and information that we have in our Moodle content, so we can move it into github as soon as we can. 

- Alerts are used to highlight sections of contents, where primary stands for definitions, info general highlights, warning potential elements of errors, danger points to misuse. Success stands for best practices. 

- Buttons are used for linking resources. Success means other pages, primary means data. The file icon indicates an internal link, the download icon is used with data, and the link, or export icon is used with external links.

<p class="alert alert-warning">hello warning</p>


<p class="alert alert-info" markdown=1> 

a quote as a warning. This would be awesome. This is not really working for us :( This quote *should* be handled correctly. this is achieved by the `markdown=1` attribute, which surprisingly also works in moodle!

</p>

Moodle folks support `markdown=1` but not `markdown="1"`. Moodle will then start rendering a Page or text field in a way that it is no longer useful. Jupyter Notebooks don't support mixing HTML and inline markdown at all. GitHub has its own way of mixing markdown inside HTML tags. However, this approach is **only** supported by GH, but not even on github pages. On the other hand, github markdown no longer supports bootstrap css classes. 

# Buttons

We use buttons to highlight important links, such as pointers to subchapters.

Moodle uses fontawesome 4.

<p class="btn btn-primary"><i class="fa fa-lg fa-file-o"></i> This should be a button</p>

Out theme uses fontawesome 5 or 6.

<p class="button is-primary"><i class="fa fa-lg fa-file"></i> This should be a button</p>

We can have special Buttons directly in markdown as shown below. It is important to remember that **Moodle** does not allow such trickery. Thus, we can use only the above strategy for course material.

[<i class="fas fa-home"/> Back to Home](https://www.dxi.ai/tmppages/){: .btn.btn-success}
