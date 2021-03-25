---
author: Malte Bonart
title: Markdown Presentation
subtitle: pandoc + reveal.js + gh pages
date: 2021-03-25
theme: moon # https://revealjs.com/themes/
transition: slide # https://revealjs.com/transitions/
# see all the options here: https://revealjs.com/config/
highlight-style: breezeDark
progress: true
slideNumber: true
hash: true
navigationMode: linear
autoPlayMedia: true
---

# reveal.js


### What can you do with `reveal.js` 

- write your slides in markdown
- include interactive figures, videos, code, math, ...
- use `pandoc` to transform markdown to html
- presentations can be viewed in any webbrowser


### Installation

```
conda install -c conda-forge pandoc 
```

### Usage

```shell
pandoc -t revealjs slides.md -o index.html  \
	--mathjax \
	--standalone \
	--css=styles.css \
	--css=https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css
```

### Tables

#### Test the new headline


| | A | B |
| :---| :---: | :---: |
| <i class="fas fa-clock"></i> | 100 | 400 |
| <i class="fas fa-plus"></i> | 200 | 300n |


### Videos


<iframe data-autoplay width="100%" height="400px" src="https://www.youtube.com/embed/Wfoy_OvNDvw"></iframe>



### Fragments

::: incremental

- Eat spaghetti
- Drink wine
- Do something else

:::


### Plots

<iframe scrolling="no" style="border:none;" seamless="seamless" data-src="static/plotly_example.html" height="450" width="100%"></iframe>


### Math

```
f(x, y) = \frac{\sqrt{x^2+y^2}}{x+y}
```

$$
f(x, y) = \frac{\sqrt{x^2+y^2}}{x+y}
$$

### Code

```python
def fun(a, b):
    print('add numbers')
    return a+b
fun(2, 2)
```


### Images

![](static/coding.jpg){ width=40% }
 
<span class="smallfont">Photo by <a href="https://unsplash.com/@arifriyanto?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Arif Riyanto</a> on <a href="https://unsplash.com/s/photos/coding?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Unsplash</a></span>


### CSS Styling

You can

<p class="smallfont"> change the fontsize </p>

<p class="highlight"> or the color </p>

with a separate stylesheet (`styles.css`)! 



### Links

- [Awesome deep learning projects](https://github.com/NirantK/awesome-project-ideas)
- [Awesome public datasets](https://github.com/awesomedata/awesome-public-datasets)
- [DrivenData DS Competitions](https://www.drivendata.org/)
- [Kaggle DS Competitions](https://www.kaggle.com/competitions)
- [Spiced Project Ideas](http://krspiced.pythonanywhere.com/chapters/final_project/README.html#project-ideas)


### Fontawesome icons

<i class="fas fa-file-code"></i>
<i class="fab fa-github-square"></i>
<i class="fab fa-codepen"></i>
<i class="fab fa-snapchat-ghost"></i>
