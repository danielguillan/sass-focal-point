# Focal Point

A Sass port of Adam Bradley's [Focal Point](https://github.com/adamdbradley/focal-point) Pure HTML/CSS Adaptive Images Framework.

This mixin allows you to take full control over the set of generated CSS classnames, the media query breakpoint and the inner element type.

First, learn more about the original Focal Point https://github.com/adamdbradley/focal-point and then come back for the mixin.

## Installation

1. Copy `_focal-point.scss` in your Sass folder
 
2. Import focal-point into your Sass stylesheet

	`@import "focal-point";`

3. Include the mixin
	
	`@include focal-point;`
	
## Custom CSS output
	
With the focal-point mixin you get full control over the CSS output. Pass the arguments you'd like to customize. You decide how many classes you need, landscape and/or portrait, your own media query breakpoint, …

	@include focal-point($grid: 12, $portrait: true, $breakpoint: 768px, $inner-element: div);


### Grid
12 cells and 6 classes for each position are too much for you? Just create a smaller grid. _Defaults to true_

	$grid: 6 (only use even numbers)

### Landscape classes
Don't need landscape classes? _Defaults to true_

	$landscape: false

### Portrait classes
Don't need portrait classes? _Defaults to true_

	$portrait: false

### Breakpoint
Set your own breakpoint. _Defaults to 767px_

	$breakpoint: 31em		

### Inner element
Need to use an inner figure or prefer using a class instead of the default div? _Defaults to div_

	$inner-element: .inner-point
