# hd-intersection-observer

Is an abstract layer built on top of the IntersectionObserver Api, it would make it easier to use and more efficient to instantiate multiple observers.

## Installation

`npm install hd-intersection-observer`

## How to use

```
// will start observing the element if its on the view port
const observer = observeFunc(
document.body,
(isInView, entry) => {
// do something
},
// document or any HTML element of choice
{ root: document }
);

// When called it will unobserve the element (for cleanup).
observer();
```
