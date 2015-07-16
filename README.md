sc-timeago
============

Polymer 1.0 element that shows a date/time as 'some time ago' using moment.js

`<sc-timeago>` is an element that displays a date/time in the past/future as a human readable string.

## Getting started

### Install with bower

First you need bower, [see their site](http://bower.io/) for details 

```
bower install --save sc-timeago
```

### Attributes

| Attribute Name | Functionality  | Default |
|----------------|-------------|-------------|
| timeago | This is where moment stores the human readable time | `nul` |
| datetime | This is the user input for the from date (YYYY-MM-DD) | '0000-00-00T00:00:00.000Z' |
| timeout | This is how often they want the time to update (it's 1 minute as default) | 60000 |

### How to use

```html
  <sc-timeago datetime="2015-01-01T00:00:00.000Z"></sc-timeago>
```

Contributions welcome, please create issues!
