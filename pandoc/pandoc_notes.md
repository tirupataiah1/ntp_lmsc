---
title: "Pandoc Miscellaneous Notes"
date: "04 August 2024"
---

# Pandoc

## Slide Shows

### Speaker Notes

* Speaker notes for both .pptx and reveal.js are of the following format / syntax:

```
::: notes

Some notes here

Even more notes

Notes can be paragraphs, lists (obtained by starting with a dash), etc.

:::
```

* See the [pandoc manual](https://pandoc.org/chunkedhtml-demo/10.5-speaker-notes.html) for additional details

### Columns

* Putting stuff in side-by-side columns is a little bit more involved:

```
:::::::::::::: {.columns}
::: {.column width="40%"}
contents...
:::
::: {.column width="60%"}
contents...
:::
::::::::::::::
```

* Essentially you have to 1st make a super container (with about 5 colons) with the class `.columns`
* Within this you put your the columns that you need to display side-by-side
    * These columns are standard blocks like the speaker notes above
    * These columns should belong to the class `.column` and should have a `width` attribute
* For additional details consult the [Pandoc User Manual](https://pandoc.org/chunkedhtml-demo/10.6-columns.html)

# Not Exactly Pandoc, but Related (Markdown)

## Emojis in Markdown

* There are a few emojis that you can add in .md files that is supported by GFM. Note that Pandoc supports GFM.
* The emoji markup `:white_check_mark:` (which produces :white_check_mark:) and `:x:` (which produces :x:) are very useful taks management
* These were taken from from the excellent [GitHub Gist](https://gist.github.com/rxaviers/7360908) which contains many other useful emoji markups as well. This gist itself was obtained from the [Unicode / emojis in Github markdown](https://stackoverflow.com/questions/34538879/unicode-emojis-in-github-markdown) discussion thread.
* In this context this [html entity code](https://stackoverflow.com/questions/4041720/html-code-for-text-checkbox) discussion thread is also very useful (along with the links and other references therein)



