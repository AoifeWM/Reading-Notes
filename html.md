# Html notes

## Wireframing

Making a wireframe is an important process in creating an website with a coherent design and aesthetic. A wireframe is basically just a drawing of the website, before any code has been written. It's important to lay out your design elements to make sure that the various elements are obvious, easy to find, and the flow of how the user interacts with the site is intuitive. Wireframe can be done with a pen and paper, or on a free digital tool; some examples are UXPin, InVision, and Wireframe.cc. Making a perfect pretty site isn't the goal, instead you want to just get a good idea of which pieces of information are the most important and highlight them appropriately.

## What is Html?

Html is a language used to create the structure of a website. It contains **elements** which you use to organize and structure the information on your website, such as line breaks, images, titles, headers, footers, and so on. Organizing these properly allows you to easily reference the various sections of your website using CSS, in order to style them.

## Anatomy of an Html document

There are some essential elements of Html which should be included in every page:

* `\<!DOCTYPE html\>`: This tag should be included at the top of every Html page and lets the computer know how to read the page as an html document. It's mostly an artifact of different versions of Html existing, but it's still important to use nowadays.
* `\<html\>...\</html\>`: This is called the root element and should wrap around ALL the Html code in the document.
* `\<head\>...\</head\>`: This is used for all the meta-information about the document, **NOT** the actual content of the page. This element contains the page's title, icon, keywords for search enginges, and things of the sort.
* `\<title\>\[a title\]\</title\>`: This sets the title for the webpage, which will show up at the top of the user's tab. It should be short and informative.
* `\<meta charset="\[charset\]">`: This sets the preferred character set for the webpage to request from the computer to render the page. `\[charset\]` will usually be replaced with `utf-8` as this is the most common characterset.
* `\<body\>...\</body\>`: This tag will contain all the actual information in your document which you want to display to the user.

## Other useful elements

* `\<img src="\[path to image\]" alt="\[title of image\]">`: This will add the desired image.
* `\<h1\>...\</h1\>`,`\<h2\>`,...,`\<h6\>`: These are headers, which will by default make the text bold and large. As the number grows, the header will get smaller and less prominent.
* `\<p\>...\</p\>`: This will designate a paragraph (with line break)
* `\<ul\> \<li\>\[list element\]\</li\> \<li\>\[list element\]\</li\> ...etc \</ul\>`: This will create an unordered list with the given elements.
* `\<ol\> \<li\>\[list element 1\]\</li\> \<li\>\[list element 2\]\</li\> ...etc \</ol\>`: This will create an ordered list with elements 1, 2, etc.
* `\<a href="\[link\]"\>\[link message\]</a>`: This will create a hyperlink with a message.
