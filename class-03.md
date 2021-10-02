# HTML lists, Control flow with JS, and the CSS box model

## Lists in HTML

HTML contains 3 basic types of lists availiable. Two of them are very similar, while one is slightly different. They are:

* Unordered lists
* Ordered lists
* Definition lists

All lists must be contained in their entirelty within a tag designating which sort of list they are. Those tags ae `<ul>`, `<ol>`, and `<dl>` respectively. Unordered and Ordered lists use the same tag to contain *each one* of their elements: `<li>`. By default, unordered lists will render each `<li>` with a bullet point, and ordered lists will do the same but with ascending numbers, starting at 1.
Definition lists are a bit different. They contain 2 types of list item: `<dt>` for the term to be defined, and `<dd>` for the definition of the preceding term. By default, the definitions will be indented more than the terms.
All lists can be nested within each other, by declaring a new list tag after one of the elements. This can be used to create sublists, for instance, breaking down each step of a task on a list.

## The CSS box model

By default, CSS treats each HTML element as if it has an invisible box around it. When modifying elements individually in CSS, the selector applies not only to the content of the element, but the whole box which represents it. For instance, changing a list element to have a blue background will draw a blue box around the entire list element.
CSS can control the dimensions, shapes, borders, background colors, padding and margins of each of these boxes. The dimensions can be easily defined with the `height` and `width` tags. These can be set to various units, from pixels, to em's/rem's (which are about 17 pixels each), or by percentages, which take into account the current size of the browser window, and change dynamically as the window size changes. You can also limit the dimensions with the `min-width`, `max-width`, `min-height`, and `max-height` tags. For instance, these tags in combination with the height and width tags can allow you to stretch an element as the browser window changes size, but stop stretching as soon as they reach the determined value.
You can change the border around the box with the `border-width` tag, you can change the appearance with the `border-style` tag, and you can change the color with the `border-color` tag. You can add padding (space between the content of an element and the border) with the `padding` or `padding-top`, `padding-left`, `padding-right`, and `padding-bottom` tags. You can add margins (space between the borders and the surrounding elements) with the same tags as padding, but with `padding` replaced with `margin`. You can change where the content sits within its box (for instance, left, right, or center) with the `align` or `text-align` tags, as appropriate.
You can make an element invisible (or specifically visible, for instance if a proceding, more general style has already set it to invisible) with the `visbility` tag by setting it to `hidden` or `visible`. 
You can add shadows with the `box-shadow` tag, by defining 4 lengths (horizontal and vertical offset, blur distance, and spread of shadow, resectively) and then defining a color for the shadow. 
You can make rounded corners with the `border-radius` tag, or select a specific corner to round, for instance `border-top-left-radius` (same for the other corners.) You can define one value for a circular curve, or two values for an eliptical curve (first value for the horizontal length of the curve, and second value for the vertical.)
