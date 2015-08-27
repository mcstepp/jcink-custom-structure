# Jcink Custom Structure
A DOM manipulation library specifically designed for the Jcink hosted forum service.

## Major Changes
* Inbuilt support for legacy browsers has been dropped.
* The script has been rewritten to take advantage of prototypal inheritance.
* The majority of the replacement keys have been renamed.
* The behavior of absent values has been changed.
* The Custom Index module no longer relies on `<!-- |input_act| -->`.
* The `target` configuration property is no longer required for any module.
* A module for customizing the appearance of posts in a topic list has been added.

## Basic Usage
1. Host a copy of [cs.min.js](https://github.com/ConnorWiseman/jcink-custom-structure/blob/master/src/cs.min.js) online.
2. Add it to the page header inside the Board Wrappers.
```html
    ...
    <script src="cs.min.js"></script>
</head>
...
```3. Call the desired `initialize` methods at any point in the Board Wrappers *after* the `<% BOARD %>` wrapper tag.
```html
<% BOARD %>
<script>
customIndex.initialize({
    html: 'Testing the spacing here'
});
</script>
```