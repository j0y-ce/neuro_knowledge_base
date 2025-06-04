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

Example Summary
- Point 1
- Point 2
- Point 3
    * Subpoint 1
    * Subpoint 2
    * Subpoint 3

<b>Bold Text Example</b>
*Bold Text Example*

<i>Italic Text Example</i>
**Italic Text Example**

***Bold and Italic Example***

<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ol>

<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ul>

Table Example


| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |


<table style="border: 1px solid #990000; border-collapse: collapse">
<colgroup>
<col width="30%" />
<col width="70%" />
</colgroup>
<thead class="header" style="border: 1px solid #990000; border-collapse: collapse">
<tr class="header" style="border: 1px solid #990000; border-collapse: collapse">
<th style="border: 1px solid #990000; border-collapse: collapse">Field</th>
<th style="border: 1px solid #990000; border-collapse: collapse">Description</th>
</tr>
</thead>
<tbody class="header" style="border: 1px solid #990000; border-collapse: collapse">
<tr>
<td markdown="span">First column **fields**</td>
<td markdown="span">Some descriptive text. This is a markdown link to [Google](http://google.com). Or see [some link][mydoc_tags].</td>
</tr>
<tr>
<td markdown="span">Second column **fields**</td>
<td markdown="span">Some more descriptive text.
</td>
</tr>
</tbody>
</table>


<iframe width="560" height="315" src="https://www.youtube.com/embed/YZPmfajMcyw?si=cs5ALcSQfGfY2roO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<style>


/* Position the image container (needed to position the left and right arrows) */
.container {
  position: relative;
}

/* Add a pointer when hovering over the thumbnail images */
.cursor {
  cursor: pointer;
}

/* Next & previous buttons */
.prev,
.next {
  cursor: pointer;
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

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover,
.next:hover {
  background-color: rgba(0, 0, 0, 0.8);
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* Container for image text */
.caption-container {
  text-align: center;
  background-color: #222;
  padding: 2px 16px;
  color: white;
}

.row:after {
  content: "";
  display: table;
  clear: both;
}


.active,
.demo:hover {
  opacity: 1;
}

div.scroll-container {
  background-color: #333;
  overflow: auto;
  white-space: nowrap;
  padding: 10px;
}

div.scroll-container img {
  padding: 10px;
}


</style>

<div class="container">
  <div class="mySlides">
    <div class="numbertext">1 / 6</div>
    <img src="{{ site.baseurl }}/assets/img_5terre_wide.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">2 / 6</div>
    <img src="{{ site.baseurl }}/assets/img_mountains_wide.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">3 / 6</div>
    <img src="{{ site.baseurl }}/assets/img_lights_wide.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">4 / 6</div>
    <img src="{{ site.baseurl }}/assets/img_nature_wide.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">5 / 6</div>
    <img src="{{ site.baseurl }}/assets/img_mountains_wide.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">6 / 6</div>
    <img src="{{ site.baseurl }}/assets/img_snow_wide.jpg" style="width:100%">
  </div>

  <a class="prev" onclick="plusSlides(-1)">❮</a>
  <a class="next" onclick="plusSlides(1)">❯</a>

<!--
  <div class="caption-container">
    <p id="caption"></p>
  </div>

  <div class="row">
    <div class="column">
      <img class="demo cursor" style="width:100%" onclick="currentSlide(1)" >
    </div>
    <div class="column">
      <img class="demo cursor" style="width:100%" onclick="currentSlide(2)">
    </div>
    <div class="column">
      <img class="demo cursor" style="width:100%" onclick="currentSlide(3)">
    </div>
    <div class="column">
      <img class="demo cursor" style="width:100%" onclick="currentSlide(4)" >
    </div>
    <div class="column">
      <img class="demo cursor" style="width:100%" onclick="currentSlide(5)" >
    </div>    
    <div class="column">
      <img class="demo cursor" style="width:100%" onclick="currentSlide(6)" >
    </div>
  </div>
</div>-->


<div class="scroll-container">
  <img src="{{ site.baseurl }}/assets/img_5terre_wide.jpg" alt="Cinque Terre">
  <img src="{{ site.baseurl }}/assets/img_woods_wide.jpg" alt="Forest">
  <img src="{{ site.baseurl }}/assets/img_lights_wide.jpg" alt="Northern Lights">
  <img src="{{ site.baseurl }}/assets/img_nature_wide.jpg" alt="Mountains">
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
  let dots = document.getElementsByClassName("demo");
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
