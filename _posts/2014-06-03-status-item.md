---
layout: page
title: "StatusItem"
category: ref
date: 2014-06-03 15:54:56
order: 8
---



Properties | description
---------- | -----------
menu | gets/sets the status items menu


Methods  | Arguments | description
-------- | --------- | ------------
createItem | (*object*) { image: "path/to/image", alternateImage: "path/to/alt/image", onClick: function() { ... } } |

```
//create simple status item
MacGap.StatusItem.create({image:"path/to/image", alternateImage: "path/to/altimage"});
     
//create status item with click callback
MacGap.StatusItem.create({image:"path/to/image", alternateImage: "path/to/altimage", onClick: function() { ... } });

// Create and add a menu to the statusbar. Note that adding a menu to a status item disables any onClick events
// Setting the second 'type' parameter in the create method to 'statusbar' keeps MacGap from automatically adding sub-menus to the menu items you create (this is because the status items don't have a supermenu like the main menu)
var menu  = MacGap.Menu.create('My Menu', 'statusbar'); 

// add items to the menu
menu.addItem('My Menu Item', '', 0, function() { alert('I was clicked!'); });
menu.addItem('Another Menu Item', '', 1, function() { ... });

// Add the menu to the status item.
MacGap.StatusItem.menu = menu;
```




