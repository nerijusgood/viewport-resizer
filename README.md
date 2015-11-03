# Viewport Resizer

A tiny vanilla javascript module that helps you resize a div or element to your desired viewports. Case use would be resizing viewports to emulate devices on your website or app.

Alpha version.

## Basic Usage

1. Require
```javascript
var viewportResizer = require('viewport-resizer');

```

2.
```javascript
var viewportResizer = require('viewport-resizer');

```

```markup

<div id="fresize-nav">
links will be stored here
</div>

<div id="fresize-content">
	your content
</div>

```


### Options
Pass the following options to fresizer:

```javascript
var options = {
    onconfig: function *(config) {
        // do stuff
    }
};

```
