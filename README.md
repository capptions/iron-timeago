sc-timeago
============

Polymer 1.0 element that shows a date/time as 'some time ago' using moment.js

`sc-timeago` is an element that displays a date/time in the past/future as a human readable string.

The element has the following public properties:

- `timeago`: the output string, this is the only property rendered in the element template
- `datetime`: the date string for which the output should be rendered
- `timeout`: milliseconds before which the string should be refreshed (`60000`), set to 0 to prevent automatic refresh 

Usage:

```html
  <sc-timeago date="2015-01-01T14:00:00.000Z"></sc-timeago>
```

Contributions welcome, please create issues!