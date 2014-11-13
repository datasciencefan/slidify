---
title       : Course Project
subtitle    : State of the Union Word Cloud
author      : datasciencefan
job         : Data Analyst
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [quiz, bootstrap]#{mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Summary of Project

This project creates a **word cloud** out of the select text. Options for the text are **State of the Union speeches** (a speech made every year by the U.S. president). Other options include a **Minimum Frequency** (the minimum number of times a word appears in the speech for it to appear in the word cloud) and a **Maximum Number of Words** (which limits the number of words in the word cloud)

https://datasciencefan.shinyapps.io/WordCloud/

---

## Steps to Use the Project

1. Select a speech in the "State of the Union" dropdown menu
2. Click the "Change" button - the word cloud updates
3. Moving the sliders automatically updates the word cloud!

--- &radio

## Question

What is the course project?

1. A digital puppy runs around on screen
2. _A **word cloud**_
3. An algorithm for calculating the earth's size
4. The number 43

*** .hint 
I couldn't figure out how to do the digital puppy, so it's not that one!

*** .explanation 
The project is a word cloud!!

---

## Embedded R Code Calculation

Based on the options (number of speeches, and ranges of the slider variables), let's calculate **the number of different word clouds** we can make with the app!


```r
s = 10  #speechs
f = 16  #"minimum frequency" values
w = 150 #"Maximum Number of Words" values

combos = s * f * w
combos
```

```
## [1] 24000
```
**Thank you!**
