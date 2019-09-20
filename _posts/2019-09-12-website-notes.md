---
title: "Notes on building this website"
tag:
 - jekyll
 - website
 - admin

excerpt_separator: "<!--more-->"
---

I chose the [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) theme because it was popular and comprehensive and I'd spent too much time faffing around with other solutions.

<!--more-->
It took me an embarrassingly long amount of time to understand that Github pages solution could be used without needing to install Git and other stuff on a desktop. When I finally realised how the jekyll-starter repositories like Minimal Mistakes actually worked I got up and running with something basic quite quickly.

There were some gotchas for a noobie. 

## Layouts 
I was confused as to how to apply layouts, and assumed I had to add
```
layout: post
```
to all posts. But then I understood how the global settings worked [Jekyll - front matter](https://jekyllrb.com/docs/front-matter/)

## tags and categories 
I couldn't understand why the tags or categories on a post didn't work, but that was because to see a summary of tags / categories you need an "archive" page in the "_pages" folder:
[Category page](https://github.com/mmistakes/minimal-mistakes/blob/master/docs/_pages/category-archive.md)

## excerpts

One useful thing for posts is to generate an automatic excerpt by using an excerpt seperator, so you can drop the online code in after the first paragraph of text. 

```
excerpt_separator: "<!--more-->"
```

## extra stuff
While the theme is great, one of the downsides of the greatness is that for a newcomer it's quite overwhelming. Author descriptions and links to social media have to be cleaned up.

