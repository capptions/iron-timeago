# < sc-timeago >

Polymer 1.0 element that shows a date/time as 'some time ago' using moment.js

`sc-timeago` is an element that displays a date/time in the past/future as a human readable string.

The element has the following public properties:

| Attribute | Purpose | Default |
|----------------|-------------|-------------|
| timeago | This is where moment stores the human readable time | `nul` |
| datetime | This is the user input for the from date (YYYY-MM-DD) | `nul` |
| timeout | This is how often they want the time to update (it's 1 minute as default) | 60000 |

Usage:

```html
  <sc-timeago date="2015-01-01"></sc-timeago>
```

Contributions welcome, please create issues!
