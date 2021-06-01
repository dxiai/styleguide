---
hide_hero: false
title: Code Fragments
---

Code fragments appear quite frequemtly on our page. The problem with the site generator is, that we can include dynamic elements on a page. This has the unintended side effect, that we may use code with symbols and sequences that are protected within Jekyll. Even worse, it is possible that we may accidentally include content that is not intended. 

Code fragments are enclosed by three grave accents (<code>```</code>) around a code fragment. The quotes are ***not*** part of the code fragment and **must** remain in sperate lines. 

### Syntax highlighting

Markdown can render syntax highlighting for code fragments. It is strongly encouraged to use syntax highlighting whenever possible.

To activate syntax highlighting one has to add a language marker immidiatly after the starting grave accents. For example <code>```R</code> activates the syntax highlighing for the R language. The following example illustrates this: 

This markdown code 

<pre>
```R
library(tidyverse)

data %>% 
    mutate(vector = as.numeric(vector)) -> 
        numData
```
</pre>

generates the code fragment below:

```R
library(tidyverse)

data %>% 
    mutate(vector = as.numeric(vector)) -> 
        numData
```


The preamble <code>```javascript</code> activates syntax highlighting for javascript. 

<p class="alert alert-warning" markdown=1>Moodle does not support syntax highlighting for code fragments. Any additional language marker is simply ignored. Therefore, the language marker should be present in case that Moodle supports syntax highlighting in the future.</p>


## Technical terms

Technical terms refer to keywords of our programming language, function names, operators, library names etc. These terms often appear in our documentation. To highlight the special role of these terms, we enclose the term with single grave accents (<code>`</code>). 

For example, when we discuss any `tidyverse` modules, we would write <code>`tidyverse`</code> to highlight the technical meaning of the term. 

### Functions

If we refer to programming functions in our documentation, we treat it as a technical term. In order to emphasize that the term refers to a function, we add round brackets directly after the function name. 

For example, instead of writing "The `tibble` function" we use the function notation and write "The `tibble()` function". 

## Common problems with code-fragments in Jekyll

Jekyll uses the `liquid` transformation language, which is very similar to Moodle's `mustache` syntax for rendering data to HTML. The major difference to Moodle is that `liquid` knows no end and analyses the markdown of the content for `liquid`-commands. For content management this can be helpful at times, but there are some edge cases where this behaviour gets into the way. 

`liquid` has to types of markup syntaxes: the command and the output syntax. The command syntax is used for describing functional areas. Such commands are enclosed by `{% raw %}{% command %}{% endraw%}`. Normally a command comes with an `end`-command, which encloses a logic block. The output syntax encloses some "variable" with double curly brackets such as `{% raw %}{{ variable | data_processing }}{% endraw %}`. As double curly brackets is the variable quotation operator of the `tidyverse` in `R`, we need to be extra careful with this code on the web-page.

<p class="alert alert-warning" markdown=1>Moodle has no such feature. Therefore, code fragments that are intended for Moodle **must not** include the `raw`-command. </p>

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

In order to get the correct results we need to protect the content of the codeblock using the `raw` and `endraw` commands. 

<p class="alert alert-danger" markdown=1>It is not possible to show code examples that contain the `raw` and the `endraw` commands!</p>

<p class="alert alert-warning" markdown=1>
In pretty formatting, the `raw` command introduces 2 extra line breaks. While this is the recommended format, it is sometimes unwanted. In order to omit the extra lines in the output, one has to start the first line right after the command and end the code right before the end command. 
</p>


The following example shows the `raw`-command in pretty format. 

```
{% raw %}
# This code should be just shown
{{ page.title }}
{% endraw %}
```

The same code in the compressed format.  


```
{% raw %}# This code should be just shown
{{ page.title }}{% endraw %}
```
[<i class="fa fa-home"/> Back to Home](https://www.dxi.ai/styleguide/){: .btn.btn-success}
