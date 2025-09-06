<!-- .slide: data-background="#E6F7FF" -->

# Examples <!-- .element: class="r-fit-text" -->

What can this stuff do? <!-- .element: class="r-fit-text" -->

---

The following examples are mostly based on the [revealjs](https://revealjs.com/) examples on [Github](https://github.com/hakimel/reveal.js/tree/master/examples) and adjusted to use mainly Markdown only.

---

## Control Features

- press `f` for full screen mode
- press `b` to pause the presentation
- press `s` for speaker view
- press `o` to see a slide overview (not working)
- use `alt` + `mouse click` to zoom in and out

---

<!-- .slide: data-background="#00ffff" -->

## Colored background

---

<!-- .slide: data-background-transition="slide" data-background="https://a-nau.github.io/assets/img/sidebar-bg.jpg" -->

## Background images

---

<!-- .slide: data-background-video="https://s3.amazonaws.com/static.slid.es/site/homepage/v1/homepage-video-editor.mp4,https://s3.amazonaws.com/static.slid.es/site/homepage/v1/homepage-video-editor.webm" -->

## Video background

---

<!-- .slide: data-background-iframe="https://slides.com/news/make-better-presentations/embed?style=hidden&autoSlide=4000" -->

## Iframe background

---

<!-- .slide: data-background-iframe="https://www.youtube.com/embed/h1_nyI3z8gI" data-background-interactive-->

## data-background-iframe

---

## Video on slide

<iframe width="560" height="315" src="https://www.youtube.com/embed/V0otZkH4VuM?si=0WM7OEDfIfUevdxz" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen>
<span class="media-title-hidden">Youtube Video: PAGANINI: 24 Caprices (complete) Antal Zalai, violin 🎵 classical music</span>
</iframe>

---

## Image on slide

<figure aria-labelledby="blackboard">
<img src="1_example_reveal/images/blackboard.jpg" data-autoplay alt="a photo of a blackboard (a black rectangle with chalk marks on it)">
<figcaption class="media-title-hidden" id="blackboard">A photo of a blackboard</figcaption>
</figure>

From [Stux](https://pixabay.com/users/stux-12364/) on [Pixabay](https://pixabay.com/photos/black-board-chalk-traces-school-1072366/), but image is stored locally.

---

<!-- .slide: data-background-video="http://clips.vorwaerts-gmbh.de/big_buck_bunny.mp4"-->

## data-background-video

---

## Math: An Identity of Ramanujan

<figure>
$$ \frac{1}{\Bigl(\sqrt{\phi \sqrt{5}}-\phi\Bigr) e^{\frac25 \pi}} =
  1+\frac{e^{-2\pi}} {1+\frac{e^{-4\pi}} {1+\frac{e^{-6\pi}}
  {1+\frac{e^{-8\pi}} {1+\ldots} } } }$$
</figure>

---

## Coding

<figure aria-labelledby="code1">

```python[1-2]
import dataclasses
import yaml2pyclass

class Config(yaml2pyclass.CodeGenerator):
    @dataclasses.dataclass
    class ClusterConfigClass:
        eps: float
        min_num_samples: int

    image_size: list
    cluster_config: ClusterConfigClass
    path_output: str
```

<figcaption id="code1">Example code listing</figcaption>
</figure>

First do `import`s

---

## Coding

<figure aria-labelledby="code2">

```python[4-12]
import dataclasses
import yaml2pyclass

class Config(yaml2pyclass.CodeGenerator):
    @dataclasses.dataclass
    class ClusterConfigClass:
        eps: float
        min_num_samples: int

    image_size: list
    cluster_config: ClusterConfigClass
    path_output: str
```

<figcaption id="code2">Another example code listing</figcaption>
</figure>

Then follows the rest

---

## Coding large

<figure aria-labelledby="scrollcode">

```html[3-5|18-20]
<table>
  <tr>
    <td>Apples</td>
    <td>$1</td>
    <td>7</td>
  </tr>
  <tr>
    <td>Oranges</td>
    <td>$2</td>
    <td>18</td>
  </tr>
  <tr>
    <td>Kiwi</td>
    <td>$3</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Banana</td>
    <td>$2</td>
    <td>2</td>
  </tr>
</table>

```

<figcaption id="scrollcode">Scrollable code listing</figcaption>
</figure>


---
## Fragments using markdown

- Appears last <!-- .element: class="fragment" data-fragment-index="3" -->
- Appears first <!-- .element: class="fragment" data-fragment-index="1" -->
- Appears second <!-- .element: class="fragment" data-fragment-index="2" -->

---

## Stacking on top

<div class="r-stack">
<figure role="group" aria-labelledby="stack">
  <img crossorigin="anonymous" src="https://placecats.com/450/300" width="450" height="300" class="fragment fade-in-then-out">
  <img src="https://placecats.com/300/450" width="300" height="450" class="fragment fade-in-then-out">
  <img src="https://placecats.com/400/400" width="400" height="400" class="fragment fade-in-then-out">
<figcaption id="stack">Overlapping Images</figcaption>
</figure>
</div>
---

## Horizontal stacking

<figure role="group" aria-labelledby="hstack">
<div class="r-hstack">
  <img src="https://placecats.com/450/300" width="450" height="300" class="fragment fade-in-then-out">
  <img src="https://placecats.com/300/450" width="300" height="450" class="fragment fade-in-then-out">
  <img src="https://placecats.com/400/400" width="400" height="400" class="fragment fade-in-then-out">
<figcaption id="hstack">Horizontal Overlapping Images</figcaption>
</figure>
</div>
---

## Vertical stacking

<figure role="group" aria-labelledby="vstack">
<div class="r-vstack">
  <img src="https://placecats.com/450/300" width="450" height="300" class="fragment fade-in-then-out">
  <img src="https://placecats.com/300/450" width="300" height="450" class="fragment fade-in-then-out">
</div>
<figcaption id="vstack">Vertical Overlapping Images</figcaption>
</figure>

---

<!-- .slide: data-transition="zoom"-->

## data-transition: zoom

---

<!-- .slide: data-transition="zoom-in fade-out"-->

## data-transition: zoom-in fade-out

---

## Default

---

<!-- .slide: data-transition="convex"-->

## data-transition: convex

---

<!-- .slide: data-transition="convex-in concave-out"-->

## data-transition: convex-in concave-out
