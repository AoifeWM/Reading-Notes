# Transitions, Transforms, and Animations in CSS

## Transforms

Transforms are a new way to size, position, and change elements. The browser support of this is fairly limited but more browsers are becoming compatible as time passes. Transforms can be 2d or 3d. The transform property can be initiated with  `transform:` in CSS. Here are some example properties: 

* `rotate:([value in degs])`: used to rotate an element (accepts degrees).
* `scale:([value])`: used to change visible size of an element (without changing its box size. Can also specify `scaleX` or `scaleY`)
* `translate`: used to shift an element visibly (but not by border box, also works with `translateX` and `translateY`. Takes pixel or percent values)
* `skew`: distorts elements. (same as above with X/Y. accepts degrees)

These transformations can be combined to produce interesting effects. By default the origin for all these transformations is the dead center of the element but this can be changed with the `transform-origin` argument.

3d transformations can be achieved by using the `perspective` and `perspective-origin` arguments.

## Transitions and animations

Transitions (for instance, an element slowly changing color) can be achieved with the `transition-property`, `transition-duration` and `transition-timing-function` properties. A property (ie background color, font size, etc.) is selected, the time the transition will take place is selected, and the timing function can be used to determine how smoothly the transition goes (for instance, `linear` will go the same speed the whole time, whereas `ease-in` will start slow and then go faster.)
