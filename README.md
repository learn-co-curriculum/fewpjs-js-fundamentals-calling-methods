# JavaScript Fundamentals: Calling Methods

## Learning Goals

1. What are JavaScript methods

## Introduction

In the previous lesson, we did a very important thing in the JavaScript
language, we _called a method_. We glossed some of the detail about what
was happening at the technical level here. Let's put some technical
vocabulary around what we did.

## What are JavaScript Methods

We _called_ the _method_ `querySelector` *on* the _object_ held in the
_document_ variable. _Calling_ is the same as _running_. We did that when
we wrote:

```js
document.querySelector();
```

The _object_ assigned to the `document` variable provides a method called
`querySelector` that looks through all of the data it was initialized with
for HTML elements that "match" the _argument_ that the method takes.

_Objects_ are helpers that manage _state_ and associatqed _behavior_ as one
thing. _Objects_ are usually "brought into existence" with some initial data
or _state_. Programmers call that _initializing_. Objects usually furnish
_methods_ which allow programmers to update, search, delete, etc. the data
the objects were initialized with.

When we _called_ `document.querySelector()`, we provided it an _argument_, a
bit of text, a `String` of text that goes inside the `()`.

In its argument, `document.querySelector()` expects us to provide a CSS
identifier that will help us find the node we want.

If the `document` object finds an HTMLElement that it knows about, it _returns_
it. Otherwise it returns `null`.

(tools console screenshot of found / not found)

The thing `document.querySelector()` returns is _also_ an object. It, too, has
both information and methods, state and behavior, properties and methods (they
all mean the same thing). This HTMLElement _instance_ provides methods like `remove()`.

## Conclusion

JavaScript methods are actions that can be performed on objects. Objects have
many useful methods that help us modify and iterate through them, for example.
The DOM selection method `document.querySelector()` is a powerful tool for finding
elements needed to make updates and changes to the DOM using methods like `remove()`.

## Resources

[JavaScript Object Methods](https://www.w3schools.com/js/js_object_methods.asp)