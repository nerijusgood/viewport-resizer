# Viewport Resizer

A tiny vanilla javascript module that helps you resize a div or element to your desired viewports. Case use would be resizing viewports to emulate devices on your website or app.

Alpha version.

<p align="center">
  <img src="http://i.imgur.com/xIcLhNq.gifv" width="500">
</p>

## Install

```shell
npm install --save viewport-resizer
```

## Usage

Require:
```javascript
var viewpresize = require('viewport-resizer');

```

The function:
```javascript
viewpresize.viewpr(options);

```

Add markup:
```markup

<div id="viewpr-list">
	Viewport size links
</div>

<div id="viewpr-content">
	Content that will be resized
</div>

```

## Options

**Add custom viewports**

Example shows default settings:
```javascript
var options = {
	viewports : [
		{
			size: '320',
			name:  'Mobile'
		},
		{
			size: '768',
			name:  'Tablet'
		},
		{
			size: '1024',
			name: 'Horizontal Tablet'
		},
		{
			size: '1280',
			name: 'Desktop'
		}
	]
};
```

**Available options**

```javascript
showName: boolean
```
If set to `true` shows the name of the viewport, else size number.

```javascript
svg: boolean
```
If set to `true` adds svg `use` to markup to allow svg sprite icons (demo).

```javascript
reset: string
```
Set custom name to reset button (dafault `reset`)

```javascript
wrapper: string
```
Change the id name of wrapper of content (dafault `viewpr-content`)

```javascript
links: string
```
Change the id name of link wrapper (dafault `viewpr-list`)

```javascript
animation: string
```
Change inlined css on wrapper item (default `-webkit-transition:width .3s ease-in-out; -moz-transition: width .3s ease-in-out; -ms-transition: width .3s ease-in-out; -o-transition: width .3s ease-in-out; transition: width .3s ease-in-out;`)


**Example**

```javascript
var options = {
	viewports : [
		{
			size: '320',
			name:  'Mobile'
		},
		{
			size: '480',
			name: 'Mobile Horizontal'
		},
		{
			size: '1280',
			name: 'Monitor'
		}
	],
	showName: true,
	reset: 'Original',
	animation: ''
};
```

This example will create only 3 viewports with custom reset button name and no animation.
