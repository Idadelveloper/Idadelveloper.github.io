---
layout: post
title: "Halfway Through Outreachy"
date: 2021-01-20
---

![Yocto Project Logo](/assets/images/yocto.png "Yocto's Pic"){: .center-image }


Welcome once more to my blog! Once again, I’m interning for the Yocto Project and my project is “Enhancing the Yocto Project’s license tracing”. If you just heard about the Yocto Project and are a little curious, you can read about it [here](https://idadelveloper.github.io/blog/2021/01/11/my-audience). This is my 8th week of this internship and honestly, it’s been 8 weeks of learning and frustration.


As we all know, the Yocto Project build system is typically used to build customized Linux images from source for embedded applications. Along with the image, a manifest of packages and their corresponding licenses is prepared, however, the accuracy of the license information in the manifest is dependent on the accuracy of the metadata we have for each package (what is in the recipe file). As part of the build, we have an internal mapping from output files to source files which are currently used to prepare source packages to aid in debugging, however with the increasing presence of [SPDX](https://spdx.dev/) headers in source files it could also be used to allow tracing the license of sources used in building a package/image to help improve our metadata and future license manifests. [SPDX](https://en.wikipedia.org/wiki/Software_Package_Data_Exchange) stands for Software Package Data Exchange which is a file format used to document information on the software licenses under which a given piece of computer software is distributed. SPDX is authored by the SPDX Working Group, which represents more than twenty different organizations, under the auspices of the Linux Foundation.


My internship project is split into 3 main tasks:
1. Take the [proof-of-concept implementation](http://git.yoctoproject.org/cgit/cgit.cgi/poky-contrib/log/?h=rpurdie/license-experiments-osls) of linking sources with SPDX headers to output files and get it to a state where it can be merged into the repository.
2. Use the functionality to examine the accuracy of our license tagging (LICENSE fields in recipes); look for errors/noise in the comparison, and produce a simple report with the results.
3. Run a check over sources in a "world" build looking for percentage coverage of SPDX headers, and run it for several past releases to see if there is a noticeable change over time.


The first two weeks were just me getting familiar with the code base, reaching out to my mentors, and setting up my system. Going through the code written by someone else and trying to understand what’s going on is something I never did in my life and it was quite difficult. I think at a certain point in time I had up to 100 Firefox tabs open most leading to YP docs due to googling stuff back and forth. I came across lots of new variables, libraries, methods but the more I kept googling about them, the more I encountered something new leading me to google once more. It was like I was stuck in an endless loop of googling. All that paid off but I wish I took things a little slower. I was trying to force myself to understand as much as I could in little time of which it didn’t work out. 


I started doing actual work during the third week. Earlier around the first week, my mentor and I chatted about what task 1 comprised of and how I’ll accomplish it. The goal of the task has been to take the proof of concept (for linking sources with SPDX license headers and structuring in output files - which has already been put together) to a state where it can be merged. The plan to achieve this task was by improving both performance and the codebase.
 
 
I began by working on implementing a feature that enables customized configurations for warning logs during a build process. This was achieved by creating a new configuration parameter in the config file of the build. The first feedback from these features was from my mentor who provided more insights on how to improve and measure the efficiency of this new feature. He tasked me with measuring the build time and made a comparative analysis with the build time before the feature was implemented. 
 
 
Further on improving the proof-of-concept, we realized during the build processes we get warning messages which should not be warning messages (false positives). My mentor tasked me with investigating why the false-positives exist and develop a working solution to fix them. My approach was to reach out to the community members and inquire what they could tell me about the false-positives. This opened up some conversations which I am currently compiling and reviewing. Currently, I am working on several possibilities as to why the false-positives and hope to have this task accomplished and submit my first patch to the mailing list (after reviewing with my mentor).
 
 
Looking back at my project timeline, I am few weeks behind. I underestimated the magnitude of this first task. Regardless, I am having a good time. The beginning was quite challenging. The imposter syndrome hit me so hard I felt like giving up but I kept pushing and now I’m proud of how far I’ve gone and can’t wait to get all my tasks done and dusted!
