---
title: "About"
description: "Learn about take-shot, how it works and some of its limitations"
nextUrl: "/getting-started"
nextTitle: "Getting Started"
---

Before you get started with the script, there are a few things that are good to know regarding the
script and some of its limitations.

## Introduction
The script allows you to take "screenshots" of webpages or parts of it, directly on the users browser.
The screenshot is based on the DOM and as such may not be 100% accurate to the real representation
as it does not make an actual screenshot, but builds the screenshot based on the information
available on the page.

## How it works
The script traverses through the DOM of the page it is loaded on. It gathers information on all the elements
there, which it then uses to build a representation of the page. In other words, it does not actually take a
screenshot of the page, but builds a representation of it based on the properties it reads from the DOM.


As a result, it is only able to render correctly properties that it understands, meaning there are many
CSS properties which do not work. For a full list of supported CSS properties, check out the
[supported features](/features/) page.

## Browser compatibility

The library should work fine on the following browsers (with `Promise` polyfill):
 - Firefox 3.5+
 - Google Chrome
 - Opera 12+
 - IE9+
 - Edge
 - Safari 6+
