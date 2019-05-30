--- 
title: "Yet another study guide for 'R for Data Science'"
author: "Bryan Shalloway"
date: "2019-05-29"
site: bookdown::bookdown_site
url: https\://brshallo.github.io/R4DS_Solutions/
github-repo: https\://github.com/brshallo/R4DS_Solutions
documentclass: book
bibliography: [book.bib, packages.bib]
biblio-style: apalike
link-citations: yes
description: "My notes and solutions to 'R for Data Science' by Garrett Grolemund and Hadley Wickham"
output:
  bookdown::gitbook:
    css: style.css
    includes:
      after_body: disqus.html
    split_by: "rmd"
    number_sections: FALSE
    config:
      sharing:
        twitter: yes
        linkedin: yes
        facebook: no
        weibo: no
        instapaper: no
        google: no
      toc:
        before: |
          <li><a href="./">Chapter contents</a></li>
        after: |
          <li><a href="https://github.com/rstudio/bookdown" target="blank">Published with bookdown</a></li>
---


# Purpose of book

This book contains my solutions and notes to Garrett Grolemund and Hadley Wickham's, (R for Data Science)[https://r4ds.had.co.nz/]. *R for Data Science* (R4DS) is my go-to recommendation for getting started in R programming, "data science", or the "tidyverse".

First and foremost, this book was set-up as a resource and refresher for myself^[And as a chance to experiment with using (bookdown)[https://bookdown.org/].]. To check your work as you go through R4DS, I would recommend using the solutions located (here)[https://jrnold.github.io/r4ds-exercise-solutions/]. Jeffrey Arnold, the creator and mantainer of this site, has done an excellent job of getting community feedback^[See more about his project (here)[https://resources.rstudio.com/rstudio-conf-2019/solving-r-for-data-science].] and well vetted solutions. Though feel free to use this book as another point of reference^[I worked through the problems independently, so for open-ended questions you'll likely see slightly different solutions.].

## Organization and features of book

*Most chapters contain the following:*

* A list of functions (and sometimes notes) from the chapter^[When functions show up in multiple locations I typically only note them the first time they appear.]
* A list of "Key exercises" I deemed good for discussion in a study group
* Solutions to exercises 
    * Exercise subsections are arranged in the same chapter --> section --> subsection as the original book. Chapters, sections, and subsections without exercises are usually not included.
    * The beginning of sections may occassionally contain additional notes, e.g. [3.8: Position Adjustment]
* The "Appendix" sections in chapters typically containg alternative solutions to problems or additional notes/thoughts pertaining to the chapter more generally
    * I use the numbering scheme {chapter}.{section}.{subsection}.{problem number} to refer to exercise solutions in "Appendix" sections
* There are a few minor cautions with using this book[^1]

[^1]: 
    * For the most part, I did not substantially update the solutions from my first time going through the book. Therefore, some of the solutions and syntax may be different from how I would approach the problem now (with more coding experience).
    * Occassionally I use related, but slightly different (or newer), methods than are shared in the book (e.g. using `mutate_at()`, `mutate_if()`, `mutate_all()` and not just `mutate()`)
    * some methods in functions may be (or may become) deprecated, e.g. using `fun()` within `mutate_at()` rather than `~`
    * The chapter and exercise numbers are hard-coded, so if R4DS exercise order changes, the exercise solutions will no longer correspond perfectly with the R4DS source
    * Formatting is not always consistent between chapters, e.g. 
        * the first 14 chapters italicize or bold questions, whereas later chapters do not
        * Notes containing functions are usually highlighted solely with backticks, e.g. `foo`, though occassionally also have parentheses, e.g. `foo()`
        * More differences can be seen if inspecting the specific .Rmd files for each chapter...

## Origin of this book

I first read and completed the exercises to R4DS in early 2017 on the tail-end of completing a Master's in Analytics program. My second time going through R4DS came in early 2018 when myself and a colleague, Stephen Kimel, organized an internal "R for Data Science" study group within NetApp^[(Here)[https://youtu.be/eeCELJNWEuw] is part of an internal talk I gave plugging "tidy" data science -- and implicitly, the R4DS study group.].  Roughly a year later, I got around to publishing these solutions and notes into this book.

## Acknowledgements

*Thank you:*

* (Garrett Grolemund)[https://twitter.com/StatGarrett] and (Hadely Wickham)[https://twitter.com/hadleywickham] for their amazing book!
* The various (tidyverse)[https://www.tidyverse.org/] and (RStudio)[https://www.rstudio.com/] developers for producing outstanding packages, products, as well as resources for learning
* (R for Data Science Online Learning Community)[https://www.rfordatasci.com/] and (#rstats)[https://twitter.com/hashtag/rstats?src=hash&lang=en] communities for creating such inspiring, safe, places to post ideas, ask questions, and grow your R skills
* Stephen Kimel, and my colleagues in the "data science" study group at NetApp