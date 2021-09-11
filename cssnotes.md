# CSS notes

CSS stands for cascading style sheets, and it's a language which allows you to edit the style and appearance of a basic html webpage. Where html is the foundation of a house, CSS is the paint, the furniture, and the interior design. CSS is important for making a webpage look appealing and have a smooth user experience. 

## Basic CSS syntax

The basic syntax of CSS is defining an element, and then defining how you want that element to look. For example, this code would all text in the **paragraph** (p) element font size 14 and blue:
`p \{`
    `font-size: 14px;`
    `color: blue;`
`\}`
A full CSS document will have many of these elements, one after the other, defining how each HTML element should appear. 

## How to inpliment CSS

CSS can be implimented in multiple ways:

* External
* Internal
* Inline

### External

An external stylesheet is a seperate document, stored elsewhere on the server, which is linked to the HTML sheet with the `\<link\>` command in the `\<header\>` tag, for example, `\<link rel="stylesheet" href="mystyle.css"\>`. This stylesheet is saved with the .css extension.

### Internal

An internal stylesheet is defined with the `\<style\>...\</style>` tag (within the `\<header\>` tag) in HTML. It is used for when elements in a page deviate from a standard stylesheet. Within the `\<style\>` tag, normal CSS syntax is used.

### Inline

Inline styles are added to individual elements with the `style` modifier, for example, `\<p style="font-size: 14px;color: blue;"\>...\</p>` would achieve the same result as the example in **basic CSS syntax**. This method makes the HTML messier and less legible, so it should be used very sparingly. Styles added to elements like this will not apply to other elements of the same type, unless also manually specified. 

## Colors

Colors in CSS can be achieved multiple ways; the following three examples will all achieve the same result.

* `color : red;`: Words for basic colors can be used.
* `color : #00ff00;`: Hexidecimal color codes can be used.
* `color : rgb(0,0,255);`: RGB color values can be used.
