---
title: "Package Management on Linux"
date: 2022-05-06T14:16:39+02:00
draft: false
tags: ["tech", "linux"]
image: "cover.png"
---
Yesterday I wrote about [package managers on Windows](https://darkshark9k.ml/p/package-management-on-windows/), and I've felt like this post needed a Linux counterpart.

You might think the package manager situation on Linux is easy - and you are right.
There is apt, dnf, pacman, zypper.

Every distribution that isn't closely based on another, ships with a different package manager. 

This article could end here, but it doesn't, because that's not the whole story.

In the original article I said that scoop only ships open source apps in it's repositories.
I briefly mentioned Chocolatey, which has a larger collection of apps - some of them also commercial.

## The scary story about FLOSSing
The distribution specific package managers mostly only ship open source apps - they are like scoop.
The Chocolatey equivalent would be Snap.

### Snapd
Snap - or Snapd, or Snappy or Snapcraft - is a distribution independent package manager.
It provides a base layer on which packages are built, each package contains every libary that it needs to run.

The significant service Snap offers is the Snapstore. It is a central place where companies can distribute their software for linux.

And then, there is also Flatpak.

### Flatpak
Flatpak is more like Winget or Scoop.

Like Snapd it is also a distribution independent package manager - it provides a base layer on which every app is built, and every app contains everything it needs to run.

The significant difference is, Flatpak is a package format - nothing more. There is no cental store, where apps are distributed.

*Ok, technically there is: Flathub. But Flathub isn't hard coded, you can change the repository at any time and provide your own.*

## Wrapping Up
As I've said: It doesn't matter which package format you use.
Use what works for you.