# Fresizer

A tiny javascript module that helps you resize a specific element to your desired sizes. Case use would be resizing viewports to emulate devices on your website or app.

UNSTABLE. Please wait till 1.0.0 version for production use.

## Basic Usage

```javascript
var fresizer = require('fresizer');


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
