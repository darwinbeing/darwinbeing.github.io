---
layout: post
title:  "How to Install Git on macOS using Homebrew"
permalink: /:title
date:   2018-03-05 00:00:00
author: André Maré
images:
  - assets/images/blog-header/homebrew-3-2.png
excerpt:
  This post provides a step-by-step guide with a list of commands on how to install Git on macOS using Homebrew. Git is a version control system for tracking changes in computer files and coordinating work on those files among multiple people. It is primarily used for source code management in software development, but it can be used to keep track of changes in any set of files. As a distributed revision control system it is aimed at speed, data integrity, and support for distributed, non-linear workflows.

categories: Homebrew
tags: [macOS, homebrew, brew, git]
---

This post provides a step-by-step guide with a list of commands on how to install Git on macOS using Homebrew.

##### What is Git?
"Git is a version control system for tracking changes in computer files and coordinating work on those files among multiple people. It is primarily used for source code management in software development, but it can be used to keep track of changes in any set of files. As a distributed revision control system it is aimed at speed, data integrity, and support for distributed, non-linear workflows." ~ [Wikipedia][0]

##### What is Homebrew?
Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple’s macOS operating system. It is known as the missing package manager for macOS.

##### Quick Commands
The following is the single command required to install git on macOS using Homebrew.
```console
$ brew install git
```
<br/>

##### Brew Commands
This sections provide a quick set of commands on how to install Git on macOS using Homebrew. It is assumed that Homebrew is already installed. If not, please follow this [link][1].

<script src="https://gist.github.com/Code2Bits/0549fc65cab9b52bdd267c0aefd1cd52.js"></script>

##### Tips & Cheatsheet
The Brew Cheatsheet commands can be downloaded from the link below. The PDF document contains a list of the brew commands that are frequently used. This cheatsheet document is not intended as a complete documented list of all commands and for that you should rather visit the official brew documentation page.

[![MarkDown Cheatsheet][2]][3]

> One must learn by doing the thing; for though you think you know it, you have no certainty, until you try. ~ Sophocles

[0]: https://en.wikipedia.org/wiki/Git
[1]: https://brew.sh/
[2]: {{site.url}}/assets/images/cheatsheets/cheatsheet-homebrew.jpg
[3]: {{site.url}}/assets/cheatsheets/cheatsheet-homebrew.pdf
