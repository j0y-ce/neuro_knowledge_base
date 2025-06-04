# Neuro Knowledge Base

Neuro Knowledge Base is a customized fork of the Odin knowledge base.


# Creating Categories
At the time of this writing, the main page has 3 categories - About, Content, and Concept Maps.

If you want to create a new category:
1. Open _data/category_list.yml
2. Add the following under existing category configuration, replacing with the title you want. Ensure you use the same capitalization.

```
new-category:
  name: New Category Name
  description: New Category Description
```

3. duplicate either about.html, concept-maps.html, or content.html into new-category.html
4. Update category property to new-category, with first letter uncapitalized
5. Update title property to new-category, with first letter capitalized
6. Push the change to Github, wait for build to finish
7. Load the main page twice to see changes reflected

You should now see a new category, and you can start creating new posts within the category.
You should create folders in the _posts folders that match the title of this new category for ease of organization.


# Creating Posts
When you create a post, you have 3 options:
1. Creating a post directly under a category, e.g. "Our Mission" under Category "About"
2. Creating a subcategory with multiple posts under a category, e.g. "Basics of MRI" under Category "Content"
3. Creating a post in a subcategory, e.g. "MRI Sequences - T1" in "Basics of MRI" under Category "Content".


# Creating Posts directly under a Category

1. Duplicate the _posts/About/"2024-11-04-our-mission.md" file in the _posts/About folder, and put it in the corresponding category folder in the _posts folder.
2. Change the category field of the copied file to whatever category (lower-case) you've moved it into.
3. Update the date in both the doc properties and filename. Make sure you don't change the date format of the title.
4. Change the title property in the copied doc to whatever you want visitors to see when they visit the page.
5. Update the short-description property to whatever description you want visitors to see when they visit the page.
6. Ensure the author property matches who you want to be seen as the doc author.
7. Push the change to Github, wait for build to finish
8. Load the corresponding category page twice to see changes reflected

```
---
layout: post
title: "Contact Us"
date: 2024-11-03 08:44:38 -0400
category: about
author: joyce
short-description: test description
---
```



# Creating Subcategories in a Category
1. Create a Subcategory by opening up _data/subcategory_list.yml and adding something resembling the lines under the existing lines. Ensure the title is in the same format as all the other subcategories, but just increment the number. Update the parent-category and parent-category-name fields to match the category you want to create them in. Add whatever text you want for the name and description.

```
subcategory-content-5:
   name: New SubCategory Name
   parent-category: content
   parent-category-name: Content
   description: This is a new subcategory for content
```

2. Create a folder in _posts that matches the name of the Subcategory for ease of organization.
3. Push the change to Github, wait for build to finish
4. Reload the category page till it shows up.


# Creating Posts in Subcategories
It's similar to creating posts directly under a category, but with slight modifications:
1. Duplicate the _posts/Basics of MRI/"2024-11-03-mri-basics-post-1.md" file and copy it into the _posts folder corresponding to this Subcategory. If that folder doesn't exist, create one in _posts.
2. Update the category field to match the subcategory ID in the _data/subcategory_list.yml file, e.g. subcategory-content-5
3. Update the date in both the doc properties and filename. Make sure you don't change the date format of the title.
4. Change the title property in the copied doc to whatever you want visitors to see when they visit the page.
5. Update the short-description property to whatever description you want visitors to see when they visit the page.
6. Ensure the author property matches who you want to be seen as the doc author.
7. Push the change to Github, wait for build to finish
8. Load the corresponding subcategory page twice to see changes reflected

# Adding Text to a Post

Every post will have some lines that look like the following, that separate document properties from the text:
```
---

-----
```
Just type in free text as if it was Microsoft Word under it to render the text.
Don't forget to push changes to github and reload the corresponding doc twice to see changes reflected.


# Adding Images to a Post
1. Create the image file in assets folder, suppose it's image.filetype
2. In a post, add the following line based on desired behaviour:

```
Example 1 - Fixed Width
![Image]({{ site.baseurl }}/assets/whitelab_logo.jpg){: width="500" }

Example 2 - Auto Width
![Image]({{ site.baseurl }}/assets/whitelab_logo.jpg){: width="100%" }

Example 3 - Auto Height
![Image]({{ site.baseurl }}/assets/whitelab_logo.jpg){: height="auto" }
```


# Adding Links to a Post
Examples:
```
<a href="{{ site.baseurl }}/about">Link to About Category inside this website</a>

<a href="{{ site.baseurl }}/content">Link to Content Category inside this website</a>

<a href="{{ site.baseurl }}/subcategory-content-1">Link to user-created Subcategory inside this website</a>

<a href="{{ site.baseurl }}/subcategory-content-1/first-content-post">Link to Post in user-created Subcategory inside this website</a>

<a href="https://en.namu.wiki/w/Find%20Love%20or%20Die%20Trying">Link to webpage outside this website</a>
```

# Test

# Adding Videos to a Post
1. Go to YouTube or whatever video hosting site you want to link from
2. Click Share Button
3. Copy the Embed Video Code that it gives you
4. Stick the Embed Video Code Straight into a Post
5. Push the change to Github, wait for build to finish
6. Load the corresponding page twice to see changes reflected

# Adding New Authors
Copy paste existing structure in _data/authors.yml like so:

```
new-author:
  name: New Author
  image: whitelab_logo.jpg
```

# Updating Email Links, Website Name, Logos, URLs, Top Level Properties, etc.
1. Navigate to _config.yml and identify properties corresponding to the property you want to change.
2. Push the change to Github, wait for build to finish
3. Load the corresponding page twice to see changes reflected


# Formatting Text to be Bold or Italic
```
Multiple Ways:

<b>Bold Text Example</b>
**Bold Text Example**

<i>Italic Text Example</i>
*Italic Text Example*

***Bold and Italic Text Example***
```


# Rendering Tables
```
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

<table style="border: 1px solid #990000; border-collapse: collapse">
<colgroup>
<col width="30%" />
<col width="70%" />
</colgroup>
<thead>
<tr class="header" style="border: 1px solid #990000; border-collapse: collapse">
<th style="border: 1px solid #990000; border-collapse: collapse">Field</th>
<th style="border: 1px solid #990000; border-collapse: collapse">Description</th>
</tr>
</thead>
<tbody>
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

```

# Rendering Point-Form Format
```
Multiple Ways:


Example Summary
- Point 1
- Point 2
- Point 3
    * Subpoint 1
    * Subpoint 2
    * Subpoint 3

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
```


NOTE - If you're changing the URL, reach out to me for help - it is more complex.
In general, if there's any changes here that you'd be uncomfortable with, reach out to me.


ACW Software
