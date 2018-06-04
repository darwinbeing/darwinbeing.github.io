---
layout: post
title:  "How to Install Eclipse on macOS using Homebrew"
permalink: /:title
date:   2018-04-09 00:00:00
author: André Maré
images:
  - assets/images/blog-header/homebrew-3-2.png
excerpt:
  This post provides a step-by-step guide with a list of commands on how to install Eclipse IDE on macOS using Homebrew. Eclipse is an integrated development environment (IDE) used in computer programming, and is the most widely used Java IDE. It contains a base workspace and an extensible plug-in system for customizing the environment. Eclipse is written mostly in Java and its primary use is for developing Java applications, but it may also be used to develop applications in other programming languages via plug-ins.

categories: Homebrew
tags: [macOS, homebrew, brew, eclipse]
---

This post provides a step-by-step guide with a list of commands on how to install Eclipse IDE on macOS using Homebrew.

##### What is Eclipse?
Eclipse is an integrated development environment (IDE) used in computer programming, and is the most widely used Java IDE. It contains a base workspace and an extensible plug-in system for customizing the environment. Eclipse is written mostly in Java and its primary use is for developing Java applications, but it may also be used to develop applications in other programming languages via plug-ins. ~ [Link][1]

##### What is Homebrew?
Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple’s macOS operating system. It is known as the missing package manager for macOS.

##### Quick Commands
The following is the single command required to install Eclipse IDE on macOS using Homebrew.
```console
$ brew cask install eclipse-jee
```
<br/>

##### Brew Commands
This section provide a quick set of commands on how to install Eclipse on macOS using Homebrew. It is assumed that Homebrew is already installed. If not, please follow this [link][2].

<script src="https://gist.github.com/Code2Bits/069dfb2d3f2973585310d2853672b407.js"></script>

##### Tips & Cheatsheet
The Brew Cheatsheet commands can be downloaded from the link below. The PDF document contains a list of the brew commands that are frequently used. This cheatsheet document is not intended as a complete documented list of all commands and for that you should rather visit the official brew documentation page.

[![MarkDown Cheatsheet][3]][4]

> One must learn by doing the thing; for though you think you know it, you have no certainty, until you try. ~ Sophocles

[1]: https://www.eclipse.org/ide/
[2]: https://brew.sh/
[3]: {{site.url}}/assets/images/cheatsheets/cheatsheet-homebrew.jpg
[4]: {{site.url}}/assets/cheatsheets/cheatsheet-homebrew.pdf
