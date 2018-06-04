---
layout: post
title:  "How to Install Caffeine on macOS using Homebrew"
permalink: /:title
date:   2018-02-26 00:00:00
author: André Maré
images:
  - assets/images/blog-header/homebrew-3-2.png
excerpt:
  This post provides a step-by-step guide with a list of commands on how to install Caffeine on macOS using Homebrew. Caffeine is a tiny program that puts an icon in the right side of your menu bar. Click it to prevent your Mac from automatically going to sleep, dimming the screen or starting screen savers. Click it again to go back. Right-click (or ⌘-click) the icon to show the menu.

categories: Homebrew
tags: [macOS, homebrew, brew, caffeine]
---

This post provides a step-by-step guide with a list of commands on how to install Caffeine on macOS using Homebrew.

##### What is Caffeine?
"Caffeine is a tiny program that puts an icon in the right side of your menu bar. Click it to prevent your Mac from automatically going to sleep, dimming the screen or starting screen savers. Click it again to go back. Right-click (or ⌘-click) the icon to show the menu." ~ [Caffeine][0]

##### What is Homebrew?
Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple’s macOS operating system. It is known as the missing package manager for macOS.

##### Quick Commands
The following is the single command required to install Caffeine on macOS using Homebrew.
```console
$ brew cask install caffeine
```
<br/>

##### Brew Commands
This sections provide a quick set of commands on how to install Caffeine on macOS using Homebrew. It is assumed that Homebrew is already installed. If not, please follow this [link][1].

<script src="https://gist.github.com/Code2Bits/c8dd8742b3745ab17f8a5bdcaf6208ef.js"></script>

##### Tips & Cheatsheet
The Brew Cheatsheet commands can be downloaded from the link below. The PDF document contains a list of the brew commands that are frequently used. This cheatsheet document is not intended as a complete documented list of all commands and for that you should rather visit the official brew documentation page.

[![MarkDown Cheatsheet][2]][3]

> One must learn by doing the thing; for though you think you know it, you have no certainty, until you try. ~ Sophocles

[0]: http://lightheadsw.com/caffeine/
[1]: https://brew.sh/
[2]: {{site.url}}/assets/images/cheatsheets/cheatsheet-homebrew.jpg
[3]: {{site.url}}/assets/cheatsheets/cheatsheet-homebrew.pdf
