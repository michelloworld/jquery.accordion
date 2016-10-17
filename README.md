# jquery.accordion
================

A simple, lightweight, responsive jQuery Accordion

### Install
```html
<script type="text/javascript" src="jquery.js"></script>
<script type="text/javascript" src="jquery.accordion.js"></script>
```

### Sample Structure
```html
HTML attributes:
[data-acc-link] => Set a name that match with the content
[data-acc-content] => Set a name that match with the link

<div class="example1">
	<div class="panel">
	  <div class="panel-heading" data-acc-link="demo1">Demo1</div>
	  <div class="panel-body acc-open" data-acc-content="demo1">
	    Content here
	  </div>
	</div>
</div>
```

### Usage
```javascript
$(function() {
	$('.example1').accordion({
		duration: 400 // default is 200,
		multiOpen: false //default is true
	});
});
```

### Options
```
duration: 400,
// animation speed of the open / close item 
multiOpen: true/false,
// default is "true". Set to "false" if you want to open one by one
```