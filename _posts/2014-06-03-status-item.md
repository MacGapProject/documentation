---
layout: page
title: "StatusItem"
category: ref
date: 2014-06-03 15:54:56
order: 190
---

Gets/sets the status items menu.

## Methods

### MacGap.StatusItem.create(configObject, callback)

######Arguments

`configObject` is a Javascript object containing the following keys:
    `title`: a `string`
    `titleFontSize`: an `integer`
    `image`: a `string` containing the path to the image to use for the status menu item
    `alternateImage`: a `string` containing the path to the alternate (over/down state) image

######Description

Set up a status bar menu item, or menu.

######Examples:

```js
var item = MacGap.StatusItem.create({
     title: 'Title',
     titleFontSize: 16,
     image:'path/to/image.png', 
     alternateImage: 'path/to/alternateimg.png'
}, function() { 
     alert('Item clicked');
});
```

Putting a custom menu into the status bar:

```js
// Create and add a menu to the statusbar. Note that adding a menu to a status item disables any onClick events
// Setting the second 'type' parameter in the create method to 'statusbar' keeps MacGap from automatically adding sub-menus to the menu items you create (this is because the status items don't have a supermenu like the main menu)
var menu  = MacGap.Menu.create('My Menu', 'statusbar'); 

// add items to the menu
menu.addItem({label: 'My Menu Item', keys: '', index: 0}, function() { alert('I was clicked!'); });
menu.addItem({label: 'Another Menu Item', keys: '', index: 1}, function() { ... });

// Add the menu to the status item.
MacGap.StatusItem.menu = menu;
```
