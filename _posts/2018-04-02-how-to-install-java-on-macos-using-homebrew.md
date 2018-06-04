---
layout: post
title:  "How to Install Java on macOS using Homebrew"
permalink: /:title
date:   2018-04-02 00:00:00
author: André Maré
images:
  - assets/images/blog-header/homebrew-3-2.png
excerpt:
  This post provides a step-by-step guide with a list of commands on how to install Java on macOS using Homebrew. This approach will always install the latest version of Java and I will explain in another post how to install specific versions of Java.

categories: Homebrew
tags: [macOS, homebrew, brew, java]
---

This post provides a step-by-step guide with a list of commands on how to install Java on macOS using Homebrew.

##### What is Java?
Java is a general-purpose computer-programming language that is concurrent, class-based, object-oriented, and specifically designed to have as few implementation dependencies as possible. Java applications are typically compiled to bytecode that can run on any Java virtual machine (JVM) regardless of computer architecture. [Link][1]

##### What is Homebrew?
Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple’s macOS operating system. It is known as the missing package manager for macOS.

##### Quick Commands
The following is the single command required to install Java on macOS using Homebrew.
```console
$ brew cask install java
```
<br/>

##### Brew Commands
This section provide a quick set of commands on how to install Java on macOS using Homebrew. It is assumed that Homebrew is already installed. If not, please follow this [link][2].

<script src="https://gist.github.com/Code2Bits/860cbfdbef188b017103626790012b15.js"></script>

##### Tips & Cheatsheet
The Brew Cheatsheet commands can be downloaded from the link below. The PDF document contains a list of the brew commands that are frequently used. This cheatsheet document is not intended as a complete documented list of all commands and for that you should rather visit the official brew documentation page.

[![MarkDown Cheatsheet][3]][4]

> One must learn by doing the thing; for though you think you know it, you have no certainty, until you try. ~ Sophocles

[1]: https://www.oracle.com/java/index.html
[2]: https://brew.sh/
[3]: {{site.url}}/assets/images/cheatsheets/cheatsheet-homebrew.jpg
[4]: {{site.url}}/assets/cheatsheets/cheatsheet-homebrew.pdf
