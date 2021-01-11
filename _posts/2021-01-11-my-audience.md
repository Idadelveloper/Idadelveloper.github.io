---
layout: post
title: "Enhancing the Yocto Project's License Tracing and Making Contributions"
date: 2021-01-11
---

![Yocto Project Logo](/assets/images/yocto.png "Yocto's Pic"){: .center-image }

The (Yocto Project)[https://www.yoctoproject.org/] is an open-source collaboration project that helps developers create custom Linux-based systems for embedded products, regardless of the hardware architecture. It provides a flexible set of tools and space where embedded developers worldwide can share technologies, software stacks, configurations, and best practices to create tailored Linux images for embedded and Internet of Things (IoT) devices. Ok, I know this sounds a little complicated. Let me simplify it.
It is a build system for Linux distributions, primarily for the embedded market. That means it is being used to compile for example the software package that is being run in a fancy coffee maker. Now everything is published under a certain license. The YP already has some means of tracing the licenses, to make sure only the intended things go into the released software package. To come back to the coffee maker example, this means the manufacturer has to provide license texts for parts of it but probably doesn't want to hand out the internals of the actual company software, as it might contain intellectual property about the electronics being used, or outstanding knowledge about brewing.

As a result, a lot of open-source developers have agreed upon using so-called SPDX headers which denote what license their software is under. And this is where this particular Outreachy project comes into play. It is about automatically checking the license information inside the source packages, relaying that information to the build system, and producing reliable reports. As a result, I have to work deep in the core technology of how a Linux system as a whole is being built from source as well as read, understand, and write quite advanced Python code as this is what the build system is written in.

If you want to make contributions to this amazing project, you will find their repository at (https://git.yoctoproject.org/git/poky)[https://git.yoctoproject.org/git/poky]. Before making any contributions, be sure to check the README in the repository you're making changes to for additional contribution instructions. Also, make sure you subscribe to the mailing list-(lists.yoctoproject.org)[https://lists.yoctoproject.org/g/yocto]. You make contributions to this project by submitting patches via email. Read more about patch submission (here)[https://www.openembedded.org/wiki/How_to_submit_a_patch_to_OpenEmbedded]. Feel free to ask your questions on the mailing list or the IRC public chat on (freenode)[http://freenode.net/] and go to #yocto. It’s made up of hundreds of amazing developers more than willing to help.

Hope you understood what the Yocto Project is all about and I’m looking forward to having you join the community :)
