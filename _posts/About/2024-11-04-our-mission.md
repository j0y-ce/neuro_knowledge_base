---
layout: post
title: "Our Mission"
date: 2024-11-03 08:44:38 -0400
category: about
author: joyce
short-description: test description
---

-----

The easiest way to change the logo used by Odin is to replace the `logo.png` file in the `assets` folder with your logo. If you change the filename of your logo file, then make sure to update the `brand_logo` variable in `_config.yml`.

After editing your logo file, run `jekyll serve` to see the changes locally. If you're satisfied with your changes, run `jekyll build` and then push your changes to your repo.

<iframe width="560" height="315" src="https://www.youtube.com/embed/YZPmfajMcyw?si=cs5ALcSQfGfY2roO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<style>

bodyX {
  font-family: Arial;
  margin: 0;
}

* {
  box-sizing: border-box;
}

img {
  vertical-align: middle;
}

/* Position the image container (needed to position the left and right arrows) */
.container {
  position: relative;
}

/* Hide the images by default */
.mySlides {
  display: none;
}

/* Add a pointer when hovering over the thumbnail images */
.cursorX {
  cursorX: pointer;
}

/* nextX & prevXious buttons */
.prevX,
.nextX {
  cursorX: pointer;
  position: absolute;
  top: 40%;
  width: auto;
  padding: 16px;
  margin-top: -50px;
  color: white;
  font-weight: bold;
  font-size: 20px;
  border-radius: 0 3px 3px 0;
  user-select: none;
  -webkit-user-select: none;
}

/* Position the "nextX button" to the right */
.nextX {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prevX:hover,
.nextX:hover {
  background-color: rgba(0, 0, 0, 0.8);
}

/* Number text (1/3 etc) */
.numbertextX {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* Container for image text */
.caption-containerX {
  text-align: center;
  background-color: #222;
  padding: 2px 16px;
  color: white;
}

.rowX:after {
  content: "";
  display: table;
  clear: both;
}

/* Six columns side by side */
.columnX {
  float: left;
  width: 16.66%;
}

/* Add a transparency effect for thumnbail images */
.demoX {
  opacity: 0.6;
}

.active,
.demoX:hover {
  opacity: 1;
}
</style>





<div class="container">
  <div class="mySlides">
    <div class="numbertextX">1 / 6</div>
    <img src="{{ site.baseurl }}/assets/img_5terre_wide.jpg" style="width:100%">


  <div class="mySlides">
    <div class="numbertextX">2 / 6</div>
    <img src="{{ site.baseurl }}/assets/img_5terre_wide.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertextX">3 / 6</div>
    <img src="{{ site.baseurl }}/assets/img_mountains_wide.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertextX">4 / 6</div>
    <img src="{{ site.baseurl }}/assets/img_lights_wide.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertextX">5 / 6</div>
    <img src="{{ site.baseurl }}/assets/img_nature_wide.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertextX">6 / 6</div>
    <img src="{{ site.baseurl }}/assets/img_snow_wide.jpg" style="width:100%">
  </div>

  <a class="prevX" onclick="plusSlides(-1)">❮</a>
  <a class="nextX" onclick="plusSlides(1)">❯</a>

  <div class="caption-containerX">
    <p id="caption"></p>
  </div>

  <div class="row">
    <div class="column">
      <img class="demoX cursorX" src="{{ site.baseurl }}/assets/img_woods_wide.jpg" style="width:100%" onclick="currentSlide(1)" alt="The Woods">
    </div>
    <div class="column">
      <img class="demoX cursorX" src="{{ site.baseurl }}/assets/img_5terre_wide.jpg" style="width:100%" onclick="currentSlide(2)" alt="Cinque Terre">
    </div>
    <div class="column">
      <img class="demoX cursorX" src="{{ site.baseurl }}/assets/img_mountains_wide.jpg" style="width:100%" onclick="currentSlide(3)" alt="Mountains and fjords">
    </div>
    <div class="column">
      <img class="demoX cursorX" src="{{ site.baseurl }}/assets/img_lights_wide.jpg" style="width:100%" onclick="currentSlide(4)" alt="Northern Lights">
    </div>
    <div class="column">
      <img class="demoX cursorX" src="{{ site.baseurl }}/assets/img_nature_wide.jpg" style="width:100%" onclick="currentSlide(5)" alt="Nature and sunrise">
    </div>    
    <div class="column">
      <img class="demoX cursorX" src="{{ site.baseurl }}/assets/img_snow_wide.jpg" style="width:100%" onclick="currentSlide(6)" alt="Snowy Mountains">
    </div>
  </div>
</div>

<script>
let slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  let dots = document.getElementsByClassName("demoX");
  let captionText = document.getElementById("caption");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " active";
  captionText.innerHTML = dots[slideIndex-1].alt;
}
</script>
