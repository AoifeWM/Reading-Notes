# Problem domain, objects, and the DOM

## The Problem Domain

The problem domain means the scope and individual pieces of a problem you are trying to solve with coding. This can be the most difficult part of figuring out how to accomplish a project. When the problem domain is clear, it's straightforward to plug in the appropriate pieces and make the code run once you're familiar with the language you're using. However, most real life problems are messy and their bounds are blurry and uncertain. It can be difficult to start doing productive work before you've figured out the problem domain, so this should always be done before starting.

## Objects

### Primitive values and object references

There are two types of values in JS, primitive values and object references. The primitive values are :

* Boolean
* Null
* Undefined
* Number
* BigInt
* String
* Symbol

Every other datatype (ie arrays, functions, and dates) are actually just special objects. Primitive values are stored in the location they're created in memory, whereas object references are simply references to another location where the object and its data are stored. Primitive values are immutable (meaning if they are changed, they are overwritten completly) whereas object references are mutable (meaning their individual values can be changed without creating a whole new object). However you must be careful because object references can both point to the same object, and if they are doing so, then altering one will also alter the other. Also, two seperate objects, even with identical contents will fail a strict equality check (`===`) because they are at different memory addresses. Duplicate references to the same object will still return true under strict equality checks. To compare objects properly with strict equality checks, you must either iterate through all their values and check each against eachother, or convert the whole object into a primitive value (for instance with the `JSON.stringify()` function or the `.getTime()` function).

### Objects in general and object literals

Objections are, in their most basic form, ollections of values and functions. However, in objects, these are known as properties and methods respectively. The easiest way to define an object is literal notation, where it is declared as a variable and its properties and methods are defined within squigly brackets. Its properties and methods are accessed by referring to the name of the object, followed by a peroid, and then a reference to the chosen property/method (ie `myCar.model` or `myCar.refillGas(5)`).

### Document Object Model

Documents are just a type of object. Within javascript, you can manipulate the HTML document using references to the document object, for instance `document.write()` is a method call of the document object. There are 4 types of "nodes" within the document object: The document itself, element nodes (ie. `header` or `div`), attribute nodes (attached to element nodes), and text nodes (the contents of the element nodes.)
