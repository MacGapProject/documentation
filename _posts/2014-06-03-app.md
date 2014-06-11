---
layout: page
title: "App"
category: ref
date: 2014-06-03 15:54:34
order: 1
---


## App:

Quit application

```js
macgap.app.terminate();
```

Activate application (bring to front)

```js
macgap.app.activate();
```

Hide application

    macgap.app.hide();

Un-hide application

    macgap.app.unhide();

System bell

    macgap.app.beep();

Bounce Dock icon of applications

    macgap.app.bounce();

Open URL in default browser

    macgap.app.open("http://google.com");

Launch application

    macgap.app.launch("TextEdit");

Set a custom user agent string

    macgap.app.setCustomUserAgent('new user agent string');
	
	// Get the system idle time. This example outputs the idle time to the console once per second.
	window.setInterval(function(){
		console.log( macgap.app.systemIdleTime() );
    }, 1000);
