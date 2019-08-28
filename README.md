# jQuery.Rule
CSS Rules manipulation, the jQuery way.

# Usage
These are the methods, the plugin adds to the different namespaces.

## jQuery.fn
- sheet: returns the stylesheets from the matched styles and links.
- cssRules: return all the rules from all the given sheets.
- ownerNode: returns the nodes that belong to the given sheet (opposite to sheets).
- cssText: returns the text of the first matched style/link.

## jQuery.rule
- constructor( $.rule ):
  - 1st argument: nothing, a rule filter, rule literal, css rule or array of rules.
  - 2nd argument: nothing, node filter for link/style, nodes link/style.
- sheets: returns the sheets that match the selector or all of them if none.
- clean: converts a rule literal, to array of rules.
- parent: returns the parent of a rule, neccesary for IE.
- outerText: return the selector with the rules of the given rule.
- text: gets/sets the cssText of the rule.

## jQuery.rule.fn
- append: will add one or more styles in the form of "attr:value; attr:value" to the matched rules.
- css : sets a value to all matched rules.
- outerText: return $.rule.outerText of the first rule.
- text: sets the cssText of the rules, or gets the cssText from the first one.
- appendTo: appends the matched rules to the specified stylesheet(1), can be a selector, dom element, sheet.

All these methods ( from jQuery.rule.fn ) are equal (or very similar) to those in jQuery.fn, but for CSS Rules.
	add, andSelf, animate, appendTo, attr, css, dequeue,
	each, end, eq, fadeIn, fadeOut, fadeTo, filter, get,
	hide, index, is, map, not, pushStack, queue, remove,
	setArray, show, size, slice, stop, toggle.

Some calls to show and hide behave unexpectedly sometimes. Some styles and animations might fail, please report it.

# License
The MIT License. Check 'License'.