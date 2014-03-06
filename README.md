# tipsy - *Forked and Customized*

Facebook-style tooltip plugin for jQuery

## This Fork of tipsy

This forked version of [tipsy](https://github.com/jaz303/tipsy/tree/master) adds some functionality needed by a friend of mine. Namely:

* Custom show/hide functions
* The ability to add a custom class to individual tooltips based on a data attribute
* The ability to set gravity via a data attribute

For documentation on how to use tipsy, please see [the original repo](https://github.com/jaz303/tipsy/tree/master).

### Data Attributes

* To add a `custom class` via a data attribute, add the class name to an attribute on the element called `data-tooltip-class`
* To set `gravity` via a data attribute, set the value to an attribute on the element called `data-tooltip-gravity`

You can change the names of the data attributes in the options object when calling tipsy (showing defaults):

```javascript
$('a').tipsy({
	dataGravity: 'data-tooltip-gravity',
	dataClass: 'data-tooltip-class'
});
```
