<!-- .slide: data-background="#E6F7FF" -->

# Intro <!-- .element: class="r-fit-text" -->

---

## What is Markdown Slides?

A template project for a Github page

- to quickly create beautiful slides and share them on freely hosted Github pages
- it is based primarily on Markdown &rarr; easy collaboration and version control
- you can host multiple presentations
- to see its full power, just check the [examples](#/03_examples)

It is powered by [reveal.js](https://revealjs.com/), an awesome project by [Hakim El Hattab](https://twitter.com/hakimel) and based on and inspired by [reveal-jekyll](https://github.com/tasmo/reveal-jekyll) by [Thomas Friese](https://twitter.com/_tasmo)

---

## How to add a new presentation?

To add a new presentation called `{my_presentation}`

- create `{my_presentation}.md` in the slides directory
  - by copying `1_example_reveal.md`
  - and adjust the configuration
- create a folder `slides/{my_presentation}/`
- add your markdown files in this folder

---

## How to create slides? (1/3)

- create a markdown file for each section/chapter/ ...
  - you can choose this freely (also all slides in one file is possible)
  - new files are needed for references, i.e. jumping to different sections
- each markdown file should start with any number and is followed by `_name` to make referencing possible
- e.g. `00_Overview.md`, where `Overview` is the file name
  - to refer to the slides in this file link to `#/00_Overview`
- slides are shown in the alphabetical order of their file names

---

## How to create slides? (2/3)

- the content of the slides is written in simple markdown
- slides within a markdown file need to be separated by three `-`
- e.g.

  ```markdown
  ## Slide 1

  Text on slide 1

  -&nbsp;-&nbsp;-

  ## Slide 2

  - List on slide 2
  ```

  - note that you need to remove the space between the `-` to make it work

- the best way is to check these [slides on Github]({{site.githuburl}}/tree/gh-pages/slides/getting_started/_posts)

---

## How to create slides? (3/3)

If you want to use assets, such as images

- create a folder `assets/slides/{my_presentation}`
- use `{&nbsp;{ asset_folder }&nbsp;}` to reference to the file location
  - e.g. if you want to add and image from that folder
  ```html
  <img src="images/latex_marker.JPG" />
  ```
  - note that the spaces are not necessary
