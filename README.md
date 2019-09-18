# JavaScript Fundamentals: Calling Methods

## Learning Goals

* Define a JavaScript method

## Introduction

In the previous lessons, we did a very important thing in the JavaScript
language, we _called a method_. We glossed over some of the detail about 
what was happening at the technical level at that time. Let's put some new
vocabulary around what we did.

## Define a JavaScript Method

Let's consider the `document.querySelector` method.

This code _calls_ the _method_ `querySelector`. The
method is said to be "defined in" the object `document`.

_Calling_ is the same as _running_. We do that when
we write:

```js
document.querySelector(); // Notice the addition of ()
```

When we _call_ `document.querySelector()`, we provide it an _[argument](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/arguments)_, a
bit of text, a `String` of text that goes inside the `()`.

The method `document.querySelector()` expects us to provide a CSS
identifier that will help us find the node we want as an _argument_.

If the `document` object finds an `HTMLElement` in its representation of the page, it _returns_
it. Otherwise the method returns `null`.

<img src="https://curriculum-content.s3.amazonaws.com/fewpjs/fewpjs-js-fundamentals-calling-methods/console.png">

The thing `document.querySelector()` returns is _also_ an object. It, too, has
both information and methods, state and behavior, properties and methods (they
all mean the same thing). This `HTMLElement` _[instance](https://developer.mozilla.org/en-US/docs/Glossary/Instance)_ has methods like `remove()`.

## Conclusion

JavaScript methods are actions that can be performed on objects. Objects have
many useful methods that help us modify and iterate through them, for example.
The DOM selection method `document.querySelector()` is a powerful tool for finding
elements needed to make updates and changes to the DOM using methods like `remove()`.

## Resources

[JavaScript Object Methods](https://www.w3schools.com/js/js_object_methods.asp)
