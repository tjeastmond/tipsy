# tipsy - *Forked and Customized*

Facebook-style tooltip plugin for jQuery

## This Fork of tipsy

This forked version of [tipsy](https://github.com/jaz303/tipsy/tree/master) adds some functionality needed by a friend of mine. Namely:

* Custom show/hide functions
* The ability to add a custom class to individual tooltips based on a data attribute
* The ability to set gravity via a data attribute

For documentation on how to use tipsy, please see [the original repo](https://github.com/jaz303/tipsy/tree/master).

### Data attributes

* Add a custom class by assigning a value to attribute: `data-tooltip-class`
* Set gravity by assigning a value to attribute: `data-tooltip-gravity`

You can change the names of the data attributes in the options object when calling tipsy (showing defaults):

```javascript
$('a').tipsy({
	dataGravity: 'data-tooltip-gravity',
	dataClass: 'data-tooltip-class'
});
```

### Custom show and hide functions

You can set custom show and hide functions by passing them into the options object:

```javascript
$('a').tipsy({
	show: function($tip, options, tipsy) { ... },
	hide: function($tip, options, tipsy) { ... }
});
```

* `$tip` is a jQuery reference to the tooltip
* `options` is a copy of the options being used
* `tipsy` is the entire instance of the tipsy plugin

