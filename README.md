flipTimer
=========

[![Build Status](https://codeship.com/projects/4888e750-ea91-0132-e267-628e55ad70cc/status?branch=master)](https://codeship.com/projects/83163)

A jQuery plugin that will count-down to or count-up from a specified date.

## Usage
Link to the required files:
```html
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="css/flipTimer.css">
    <script src="js/jquery-3.1.1.min.js"></script>
    <script src="js/jquery.flipTimer.js"></script>
```
Initialise flipTimer (if no date is set, it will tell the time for today):
```html
<script>
  $(document).ready(function() {
    $('.example').flipTimer({ direction: 'down', date: 'June 17, 2016 23:15:00', callback: function() { alert('times up!'); } });
  });
</script>
```
In the body of your HTML page, choose which digits you want to use:
```html
<div class="example">
  <div class="days"></div>
  <div class="hours"></div>
  <div class="minutes"></div>
  <div class="seconds"></div>
</div>
```

## Tests
To run the test suite, run:
```
npm install
grunt karma:unit
```
This will run the tests and continue to watch for any file changes.

## Demo
There is a <a href="http://andrewjtait.github.io/flipTimer/">demo of flipTimer</a> to view.

## License
Copyright (c) 2013 Andrew James Tait   
Licensed under the MIT, GPL licenses.
