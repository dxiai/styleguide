---
hide_hero: true
title: Code Fragments
---

Code fragments appear quite frequemtly on our page. The problem with the site generator is, that we can include dynamic elements on a page. This has the unintended side effect, that we may use code with symbols and sequences that are protected within Jekyll. Even worse, it is possible that we may accidentally include content that is not intended. 

The following example shows this problem. 

```
{% raw %}
# This code should be just shown
{{ page.title }}
{% endraw %}
```

One would not expect to get the following result: 

```
# This code should be just shown
{{ page.title }}
```

In order to get the correct results we need to protect the content of the codeblock. 

```
{% raw %}{% raw %}
# This code should be just shown
{{ page.title }}
{% endraw %}{% endraw %}
```

<p class="alert alert-warning" markdown=1>
The `raw` element introduces 2 extra line breaks. If these are not wanted, one has to start the first line right after the command and end the code right before the end command. 
</p>


```
{% raw %}{% raw %}# This code should be just shown
{{ page.title }}{% endraw %}{% endraw %}
```
