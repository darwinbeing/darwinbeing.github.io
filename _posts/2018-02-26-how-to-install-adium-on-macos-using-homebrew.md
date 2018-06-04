---
layout: post
title:  "How to Install Adium on macOS using Homebrew"
permalink: /:title
date:   2018-02-26 00:00:00
author: André Maré
images:
  - assets/images/blog-header/homebrew-3-2.png
excerpt:
  This post provides a step-by-step guide with a list of commands on how to install Adium on macOS using Homebrew. Adium is a free instant messaging application for Mac OS X that can connect to AIM, XMPP (Jabber), ICQ, IRC and more. Adium can connect you to any number of messaging accounts on any combination of supported messaging services and then chat with other people using those services.

categories: Homebrew
tags: [macOS, homebrew, brew, adium]
---

This post provides a step-by-step guide with a list of commands on how to install Adium on macOS using Homebrew.

##### What is Adium?
"Adium is a free instant messaging application for Mac OS X that can connect to AIM, XMPP (Jabber), ICQ, IRC and more. Adium can connect you to any number of messaging accounts on any combination of supported messaging services and then chat with other people using those services." ~ [Adium][0]

##### What is Homebrew?
Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple’s macOS operating system. It is known as the missing package manager for macOS.

##### Quick Commands
The following is the single command required to install Adium on macOS using Homebrew.
```console
$ brew cask install adium
```
<br/>

##### Brew Commands
This sections provide a quick set of commands on how to install Adium on macOS using Homebrew. It is assumed that Homebrew is already installed. If not, please follow this [link][1].

<script src="https://gist.github.com/Code2Bits/b9d5325d260ab6c72cc3b408750cbd32.js"></script>

##### Tips & Cheatsheet
The Brew Cheatsheet commands can be downloaded from the link below. The PDF document contains a list of the brew commands that are frequently used. This cheatsheet document is not intended as a complete documented list of all commands and for that you should rather visit the official brew documentation page.

[![MarkDown Cheatsheet][2]][3]

> One must learn by doing the thing; for though you think you know it, you have no certainty, until you try. ~ Sophocles

[0]: https://www.adium.im/
[1]: https://brew.sh/
[2]: {{site.url}}/assets/images/cheatsheets/cheatsheet-homebrew.jpg
[3]: {{site.url}}/assets/cheatsheets/cheatsheet-homebrew.pdf
