---
title: "Hello World"
date: 2017-06-09 09:00:00 +0000
tags: blog jekyll github-pages
---

This is my first blog post and also the initiation of my personal website!

I've wanted to make a site for a while but got serious about a month ago and started to explore options in more detail, including
+ WordPress on a hosting service like Bluehost
+ WordPress on a Digital Ocean droplet (and the ancillary issue of now administrating an Ubuntu server too)
+ Something else like Joomla on a Digital Ocean droplet
+ Bootstrap framework
+ Jekyll on GitHub.

I'm not a developer but an academic physicist with a lot of computational programming experience in fortran, Mathematica, and Matlab. Web technologies were mostly new to me and I spent a lot time learning about the above options and how they work. It was very interesting and I learned much. (Including all the neat things you can do with a Digital Ocean droplet.) I did *many* tutorials along the way.

In the end, I decided on [Github Pages](https://pages.github.com) and [Jekyll](https://jekyllrb.com), for the ease of page and blog post addition using markdown-formatted documents. After deciding on Jekyll, the choice of theme was a whole 'nother problem and initially just went with [minima](https://github.com/jekyll/minima). But after seeing Bruno Coelho's [website](https://4brunu.github.io/), which was similar to what I had in mind for my site, [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) it was. This site was also a good source for more information about using the theme. (We implement the theme differently, however. His use of the Gem-based theme would necessitate using Travis-CI on GitHub, which is beyond my skill set currently! Instead, I forked the theme and will keep it updated by pulls from the upstream repository.)

Thus far, I've modified the theme `head.html` file in `_includes` to invoke MathJax from its CDN. I'm sure I will not be able to write exclusively without invoking an equation at some point! This is a test of that addition... a LaTeX equation of a Lorentz transformation:

\\begin{align}
t &= \gamma (t^\prime + v x^\prime)\\\
x &= \gamma (x^\prime + v t^\prime)
\\end{align}

Works fine, but I can see that the [backslash issue](http://docs.mathjax.org/en/latest/tex.html#tex-and-latex-math-delimiters) will cause no end of Jekyll rebuilds as I'll forget the extra backslash everywhere.
