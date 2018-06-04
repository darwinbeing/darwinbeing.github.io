---
layout: post
title:  "How to Install Postman on macOS using Homebrew"
permalink: /:title
date:   2018-04-23 00:00:00
author: André Maré
images:
  - assets/images/blog-header/homebrew-3-2.png
excerpt:
  This post provides a step-by-step guide with a list of commands on how to install Postman on macOS using Homebrew. Postman is a REST client application, used to send request messages to an API and get a response message back from the server.

categories: Homebrew
tags: [macOS, homebrew, brew, postman]
---

This post provides a step-by-step guide with a list of commands on how to install Postman on macOS using Homebrew.

##### What is Postman?
Postman is a REST client application, used to send request messages to an API and get a response message back from the server. ~ [Link][1]

##### What is Homebrew?
Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple’s macOS operating system. It is known as the missing package manager for macOS.

##### Quick Commands
The following is the single command required to install Postman on macOS using Homebrew.
```console
$ brew cask install postman
```
<br/>

##### Brew Commands
This section provide a quick set of commands on how to install Postman on macOS using Homebrew. It is assumed that Homebrew is already installed. If not, please follow this [link][2].

<script src="https://gist.github.com/Code2Bits/9df18e8177e932eeb4a7b591bde29439.js"></script>

##### Tips & Cheatsheet
The Brew Cheatsheet commands can be downloaded from the link below. The PDF document contains a list of the brew commands that are frequently used. This cheatsheet document is not intended as a complete documented list of all commands and for that you should rather visit the official brew documentation page.

[![MarkDown Cheatsheet][3]][4]

> One must learn by doing the thing; for though you think you know it, you have no certainty, until you try. ~ Sophocles

[1]: https://www.getpostman.com/
[2]: https://brew.sh/
[3]: {{site.url}}/assets/images/cheatsheets/cheatsheet-homebrew.jpg
[4]: {{site.url}}/assets/cheatsheets/cheatsheet-homebrew.pdf
