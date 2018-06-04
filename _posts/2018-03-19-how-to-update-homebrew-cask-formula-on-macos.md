---
layout: post
title:  "How To Update Homebrew Cask Formula on macOS"
permalink: /:title
date:   2018-03-19 00:00:00
author: André Maré
images:
  - assets/images/blog-header/homebrew-3-2.png
excerpt:
  Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple's macOS operating system. It is known as the missing package manager for macOS. After you installed a number of applications on your macOS making use of Homebrew Cask, it is only a matter of time before newer versions of those applications are available and you need to upgrade those apps. Homebrew Cask offers a very simple way to upgrade your applications. By running the <em>brew update</em> & <em>brew cask upgrade</em> commands, all of your installed applications will be updated, but you may want to update only specific applications. This post will list the commands required to update and upgrade specific applications on your Mac.

categories: Homebrew
tags: [macOS, homebrew, brew, cask, update]
---

This post provides a step-by-step guide with a list of commands on how to update homebrew cask formula on macOS using Homebrew Commands.

##### What is Homebrew?
Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple’s macOS operating system. It is known as the missing package manager for macOS.

##### Why Update Formula?
After you installed a number of applications on your macOS making use of Homebrew Cask, it is only a matter of time before newer versions of those applications are available and you need to upgrade those apps. Homebrew Cask offers a very simple way to upgrade your applications. By running the <em>brew update</em> & <em>brew cask upgrade</em> commands, all of your installed applications will be updated, but you may want to update only specific applications. This post will list the commands required to update and upgrade specific applications on your Mac.

##### Brew Commands
This section provide a quick set of commands on how to update homebrew cask formula on macOS using Homebrew. It is assumed that Homebrew is already installed. If not, please follow this [link][2].

<script src="https://gist.github.com/Code2Bits/79fad2a699e5d33f3afbd62d65740dc0.js"></script>

##### Tips & Cheatsheet
The Brew Cheatsheet commands can be downloaded from the link below. The PDF document contains a list of the brew commands that are frequently used. This cheatsheet document is not intended as a complete documented list of all commands and for that you should rather visit the official brew documentation page.

[![MarkDown Cheatsheet][3]][4]

> One must learn by doing the thing; for though you think you know it, you have no certainty, until you try. ~ Sophocles


[2]: https://brew.sh/
[3]: {{site.url}}/assets/images/cheatsheets/cheatsheet-homebrew.jpg
[4]: {{site.url}}/assets/cheatsheets/cheatsheet-homebrew.pdf
