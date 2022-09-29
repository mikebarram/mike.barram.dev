---
title: "What could go wrong with a simple jQuery value selector?"
date: "2014-11-07"
tags: ['uom','uom-js']
draft: false
---

In this case the value selector is used like this:
```js:
$(“.pPlacement select option\[value='” + PlacementId + “‘\]”).attr(‘selected’, true);
```
When PlacementId changes from a number to text and that text then contains an apostrophe, then it breaks!

To explain the code above, thee’s a dropdown list of placements and from somewhere we have the value of the one that we want to have as the selected option. The selector picks the option with the value equal to PlacementId and selects it.

The problem with this is similar to a SQL injection attack – we’re executing code that contains a variable. To get around this, we only use the variable as a parameter, like this:
```js:
$(“.pPlacement select option”).each(function() {  
  if(this.value == PlacementId) $(this).attr(‘selected’, true);  
});
```