---
layout: post
title:  "How to Install Maven on macOS using Homebrew"
permalink: /:title
date:   2018-03-12 00:00:00
author: André Maré
images:
  - assets/images/blog-header/homebrew-3-2.png
excerpt:
  This post provides a step-by-step guide with a list of commands on how to install Maven on macOS using Homebrew. Maven is a build automation tool used primarily for Java projects. Maven assist in simple project setup following best practices. It assist in complex dependancy management including automatic updating of artefacts from central repositories into your local repository.

categories: Homebrew
tags: [macOS, homebrew, brew, maven]
---

This post provides a step-by-step guide with a list of commands on how to install Maven on macOS using Homebrew.

##### What is Maven?
Maven is a build automation tool used primarily for Java projects. Maven assist in simple project setup following best practices. It assist in complex dependancy management including automatic updating of artefacts from central repositories into your local repository.

##### What is Homebrew?
Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple’s macOS operating system. It is known as the missing package manager for macOS.

##### Quick Commands
The following is the single command required to install Maven on macOS using Homebrew.
```console
$ brew install maven
```
<br/>

##### Brew Commands
This sections provide a quick set of commands on how to install Maven on macOS using Homebrew. It is assumed that Homebrew is already installed. If not, please follow this [link][1].

<script src="https://gist.github.com/Code2Bits/d057dff8367c906948508438e8aa22ba.js"></script>

##### Tips & Cheatsheet
The Brew Cheatsheet commands can be downloaded from the link below. The PDF document contains a list of the brew commands that are frequently used. This cheatsheet document is not intended as a complete documented list of all commands and for that you should rather visit the official brew documentation page.

[![MarkDown Cheatsheet][2]][3]

> One must learn by doing the thing; for though you think you know it, you have no certainty, until you try. ~ Sophocles

[1]: https://brew.sh/
[2]: {{site.url}}/assets/images/cheatsheets/cheatsheet-homebrew.jpg
[3]: {{site.url}}/assets/cheatsheets/cheatsheet-homebrew.pdf
