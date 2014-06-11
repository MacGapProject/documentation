---
layout: default
title: "Jekyll Docs Template"
---

#MacGap

The MacGap project provides HTML/JS/CSS developers an Xcode project for developing Native OSX Apps.

The project exposes a JavaScript API for OS X integration, such as displaying native OS X 10.9 notifications. The MacGap project is extremely lightweight and nimble; a blank application is about 380KB.

### Features:
* tiny compiled app sizes
* Mac App Store compatible
* access to many Mac OS X-specific features

## Pre-requisites

MacGap 2 works on OSX 10.9 and later. MacGap 1 works on OSX 10.6 and later.

Generate apps with the [macgap generator](http://github.com/maccman/macgap-rb), no compile necessary.

    gem install macgap

    macgap new myapp
    macgap build myapp

##API

MacGap exposes an object called `MacGap` inside JavaScript.
##Attributes

MacGap was forked/ported from Phonegap-mac. It's under the same license (MIT).

##Custom Build

To build, make sure you have installed the latest Mac OSX Core Library. Download at [http://developer.apple.com/](http://developer.apple.com/).

Just clone the repository and build in Xcode. The file `public/index.html` is loaded on startup.
