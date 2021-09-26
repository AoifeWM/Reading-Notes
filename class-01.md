# Introductory HTML, CSS, and Javascript

Html, css, and javascript work together to create websites. To put it simply, HTML provides the basic structure and the bulk of the informational content, CSS provides the style and appearance of the site, and JavaScript provides all the extra bells and whistles, like text forms, buttons, interactive content, and pretty much anything more complicated than links and static content.

## HTML

HTML is a type of text document, which is rendered into a webpage when it's read by a computer. HTML uses special containers to sort the content on the page, called *elements*, which are designated with *tags*. These tags don't show up to the user who views the web page, they just tell the computer how to interpret each piece of content it is given. The basic format for a tag is `<[tag]>...</[tag]>`. There are a few tags that are essential and every webpage uses them:

* `<!DOCTYPE html>`: this should be at the top of every HTML document, and it lets the computer know to prepare to read an HTML document.
* `<html>`: this tag wraps around the whole document and lets the computer know that everything contained should be read as HTML.
* `<head>`: this tag wraps around important information *about* the page, which will typically not be displayed directly on the webpage, for instance, keywords for search engines, the title of the tab to be displayed by the browser, and the icon next to the title.
* `<body>`: this tag wraps around all the substantial content in the document, which will be displayed to the user, including the header, footer, main text, etc.

Tags also have attributes. These designate various values for the tag to read, for instance, the `<img>` tag will almost always be written as `<img src="mypicture.jpg" alt="this is my picture!">`. The two attributes here are the image source (`src="mypicture.jpg"`) and the alt text which shows up when hovering over the image (`alt="this is my picture!"`).

### Other HTML syntax

Here are some more useful pieces of syntax in html:

* `<!-- Comments -->`: this tag will allow you to comment anything inside of it. Commented text isn't acted upon by the computer. You can use it to temporarily delete or disable sections of code during testing, to remind yourself and other developers what a certain piece of code does, or to store a piece of code that another developer might want to try using later by uncommenting it.
* ID and class attributes (`id="example"`, `class="example2"`): these are arbirtary attributes which you can use to label certain elements, primarily so they can be identified and acted upon seperately by CSS or javascript. They can be named whatever you like, but their names should probably relate to their purpose.
* Escape characters (typically `\`): These allow you to use characters that html would otherwise start reading as internal syntax; for instance, say you want to display the characters `<` or `>`; the computer might try to generate a tag out of these and get confused. If you type `\<` the computer will know to display `<` as a character rather than trying to start a tag. You can also use specific codes for each character; for instance, `&copy;` will display a copyright symbol, `&lt` will display as `<`, and more. These can be looked up in reference tables on the internet.
* `<div>` and `<span>` tags: these tags don't inherently tell html to treat the contained content in a certain way, except starting a new line in the case of `<div>` (but not `<span>`); rather, they allow you to designate sections of code for new arbitrary behavior or styling. They're often used with *id* or *class* attributes.
* `<iframe>`: The iframe tag allows you to put another website in a smaller frame within your own page. It's often used to embed things such as google maps. It must be used with the attributes `src` to define the page to display, and `height` and `width` to define the size of the frame.
* `<meta>`: This tag allows you to set meta-information about your webpage, for instance, keywords for search engines, a description to display when the page shows up as a search result, a characterset to preferrentially use (often UTF-8), and more.

## Before you start coding

Before you actually start typing out code, it's a good idea to have so idea of what your website will look like first. A very useful tool to start this process is called a wireframe. It may sound fancy, but really it's only a pen and paper mockup of what you want your site to look like. You should plan out the general space and size of important elements, like the name/logo at the top, the navigation bar with links to other parts of your site, how the bulk of the text on your page will be presented, where and how large you will place images, etc. You should try to keep in mind which elements are the most important, and where you can place them to make them easy to find for the end user. For instance, it's very standard for a site logo with a link to the home page to be at the top left, and a navigation bar with links to other parts of the site be along the top as well, or along the left side, so placing these elements in their standard places will help users intuitively find them and make your site a more pleasant experience for them to use.
A wireframe is just supposed to be a rough sketch, so you shouldn't worry about making it perfect, as it will be easy to modify later. It helps you organize your code and keep a consistent visual aesthetic throughout your site to have these things planned first.

## Basics of JavaScript

JavaScript can add a lot of functionality to a website. Pieces of JavaScript are called scripts, and their basic purpose is to tell the computer to run a process which is outside the bounds of HTML and CSS at certain points in your website. An important factor in creating effective scripts which are functional and not buggy is to break down your goal into many different individual steps and make sure each one runs smoothly on its own. Scripts can handle packets of information called objects. Objects can be set up to have any number of internal values which vary from object to object, they can handle events happening to them (for instance by changing their internal values) and they can run their own processes, called methods. Objects let your code procedurally handle many complex pieces of information; for instance, a library reference program might store each book as an object, each containing internal values such as ISBN code, author, genre, page length, an image of the cover, whether or not the book is checked out currently, who it is checked out to, etc. In such a system, adding a new book would be as simple as creating a new object to track it and plugging in all the apropriate values. 
Objects are so powerful that they're used almost ubiquitously in modern programming. For instance, an HTML document is handled as an object by the computer; each individual element is an internal value of the object. JavaScript adds new methods to the document object in order to let it do new, fancy things.

### Adding JavaScript to an HTML page

Although javascript can be directly written into an HTML page, best practice is usually to create a seperate file ending with the `.js` extension. You identify this file to the HTML page by using the `<script src="[filename].js">[...]</script>` tag in the HTML document. From there, you can call various parts of your new javascript element directly from the HTML page. You can use this to add alerts, prompt the user for information, edit the HTML of the webpage on the fly, and much much more.
