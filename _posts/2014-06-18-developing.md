---
layout: page
title: "Developing your app"
category: doc
date: 2014-06-03 15:55:26
order: 2
---

### Enable Developer Tools for debugging

You can enable Webkit's developer tools within your MacGap application, by entering the following command into your Terminal.

```
defaults write com.MG developer 1
```

After the above has been done, you will be able to right-click anywhere in your app window and select 'Inspect Element' as you usually can in Safari.

MG is the default app name in Xcode. Be sure to replace this if you have changed your app's name.
