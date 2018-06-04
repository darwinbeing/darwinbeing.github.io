---
layout: post
title:  "How to Install STS on macOS using Homebrew"
permalink: /:title
date:   2018-05-14 00:00:00
author: André Maré
images:
  - assets/images/blog-header/homebrew-3-2.png
excerpt:
  This post provides a step-by-step guide with a list of commands on how to install iTerm2 on macOS using Homebrew. The Spring Tool Suite (STS) is an Eclipse-based development environment that is customised for developing Spring applications.

categories: Homebrew
tags: [macOS, homebrew, brew, sts]
---

This post provides a step-by-step guide with a list of commands on how to install Spring Tool Suite (STS) on macOS using Homebrew.

##### What is STS?
"The Spring Tool Suite (STS) is an Eclipse-based development environment that is customised for developing Spring applications. It provides a ready-to-use environment to implement, debug, run, and deploy your Spring applications, including integrations for Pivotal tc Server, Pivotal Cloud Foundry, Git, Maven, AspectJ, and comes on top of the latest Eclipse releases." ~ [Spring Pivotal][1]

##### What is Homebrew?
Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple’s macOS operating system. It is known as the missing package manager for macOS.

##### Quick Commands
The following is the single command required to install STS on macOS using Homebrew.
```console
$ brew cask install sts
```
<br/>

##### Brew Commands
This section provide a quick set of commands on how to install Spring Tool Suite (STS) on macOS using Homebrew. It is assumed that Homebrew is already installed. If not, please follow this [link][2].

<script src="https://gist.github.com/Code2Bits/a50c96dbdf17f1611dda4bb471d46af5.js"></script>

##### Tips & Cheatsheet
The Brew Cheatsheet commands can be downloaded from the link below. The PDF document contains a list of the brew commands that are frequently used. This cheatsheet document is not intended as a complete documented list of all commands and for that you should rather visit the official brew documentation page.

[![MarkDown Cheatsheet][3]][4]

> One must learn by doing the thing; for though you think you know it, you have no certainty, until you try. ~ Sophocles

[1]: https://spring.io/tools/sts
[2]: https://brew.sh/
[3]: {{site.url}}/assets/images/cheatsheets/cheatsheet-homebrew.jpg
[4]: {{site.url}}/assets/cheatsheets/cheatsheet-homebrew.pdf
