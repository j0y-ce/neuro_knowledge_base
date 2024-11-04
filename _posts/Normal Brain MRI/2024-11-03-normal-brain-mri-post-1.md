---
layout: post
title: "Test Post Normal Brain MRI"
date: 2024-11-03 08:44:38 -0400
category: subcategory-content-3
author: joyce
short-description: test description
---

-----

The easiest way to change the logo used by Odin is to replace the `logo.png` file in the `assets` folder with your logo. If you change the filename of your logo file, then make sure to update the `brand_logo` variable in `_config.yml`.

After editing your logo file, run `jekyll serve` to see the changes locally. If you're satisfied with your changes, run `jekyll build` and then push your changes to your repo.

Image test 1.

![Image]({{ site.baseurl }}/assets/whitelab_logo.jpg){: width="500" }

Image test 2

![Image]({{ site.baseurl }}/assets/whitelab_logo.jpg){: width="100%" }

Image test 3

![Image]({{ site.baseurl }}/assets/whitelab_logo.jpg){: height="auto" }


<a href="{{ site.baseurl }}/about">Link to document inside this website</a>



<a href="{{ site.baseurl }}/content">Link to document inside this website</a>


<a href="{{ site.baseurl }}/subcategory-content-1">Link to document inside this website</a>


<a href="{{ site.baseurl }}/subcategory-content-1/first-content-post">Link to document inside this website</a>


<a href="https://en.namu.wiki/w/Find%20Love%20or%20Die%20Trying">Link to webpage outside this website</a>

<!-- need to double enter to start new lines -->
<!-- need to use the site baseurl in the curly brackets to make internal links work seamlessly -->
