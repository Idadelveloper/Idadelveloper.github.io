---
layout: post
title: "GSoC 2021 with RTEMS: Final Report"
date: 2021-08-20
image: /assets/images/rtems.png
category: "Internship"
---


<div class="text-center">
  <img src="/assets/images/rtems.png" class="rounded w-50 mb-10" style="max-width:70%; max-height:70%" alt="Building Code">
</div>


## Project Abstract
The supercore also known as score provides services for all APIs and the core parts of RTEMS, there is no automatic checking of the coding style. Therefore for people new to RTEMS, it can get tricky to get it right when sending patches. This project will improve the situation and work towards automatic style and formatting checking for RTEMS score. By doing so, it will be able to tell if patches need changes before being sent for review.
This project is aimed at creating a tool for automatic style checking of RTEMS. It will be achieved by firstly finding a code checker or "formatter" that matches RTEMS’ coding style, writing a script built into git commit hook that can run over patches before committing or submitting via email, as well as creating a standalone tool in rtems-tools to run over the entire codebase (excluding some parts) checking for any mismatches in the coding style.
The code checker tool to be used will be clang-format since it is the closest whose output matches RTEMS coding style and the goal is to find a combination of clang-format settings combined with changes to the RTEMS style and changes to clang-format such that the output with the right settings matches the RTEMS code style.


### Project Description
There is no automatic checking of the coding style for the core parts of RTEMS. As a result, people new to RTEMS hardly get it right when sending patches. The RTEMS score format is specific to this project and a “formatter” needs to be taught how to handle the format.


### Importance
This project will improve the situation and work towards automatic style and formatting checking for RTEMS score. By doing so, it will be able to tell if patches need changes before being sent for review or applied.


### Mentors
* Dr. Gedare Bloom
* Dr. Kuan-Hsun Chen


## Summary of Work
### First Half
I spent time understanding how RTEMS works and what it is all about. I tried building RTEMS and creating my first hello world application. Immediately after, I started working on the pre-commit hook script which checks for style issues before successfully creating a commit.
#### Code submitted
* Add RTEMS clang-format configuation: [here](https://github.com/Idadelveloper/rtems/commit/cff8ff75b1a4d2f9ee708c0adbf5f215ae0c9e6b)
* Pre-commit hook to check for style differences before commiting: [here](https://github.com/Idadelveloper/rtems/blob/master/hooks/pre-commit)
* Added git diff to rtems-tools/rtemstoolkit/git.py: [here](https://github.com/Idadelveloper/rtems-tools/commit/d20d04deba83aa9ca6778959b7f94eb399de3651)


### Second Half
I started working on the standalone tool in rtems-tools.git that can be used to check for style issues in rtems.git. The pre-commit hook script I initially wrote made things a lot easier for me since I just borrowed some of its functionalities. I tried building LLVM using the RSB but it failed because it was not updated so I ended up building it from source. To see this tool in action, the `rtems-style` command is used. I uses 5 flags:
* `-c`, `--check` : Checks for style issues and prints out a report
* `-r`, `--reformat` : reformate code in a given file or directory
*  `-p`, `--path` : path in which to check or reformat code
*  `-v`, `--verbose` : prints output during style checking but in more detail
*  `-i`, `--ignore` : file(s) to be ignoed when checking for style issues
#### Code submitted
* Tool for style checking and code formatting(rtmes-style): [here](https://github.com/Idadelveloper/rtems-tools/commit/9960110e06559a9881d9a36b2fd0f962b4554ae5)
* Added git diff to rtems-tools/rtemstoolkit/git.py: [here](https://github.com/Idadelveloper/rtems-tools/commit/d20d04deba83aa9ca6778959b7f94eb399de3651)


### TODOS
* Update the rtems-style code.
* Write documentation for rtems-style.
* Update the pre-commit hook script  be compatible with other hosts like Windows and FreeBSD.


### What I learned
* Firstly, I learned about RTEMS and how it is used
* I had no idea what git hooks were. I wrote my first pre-commit hook through this internship.
* It has taught me how to write better and more structured code.
* Had the opportunity to interact with a community spanning multiple timezones.


*All in all, my internship has been amazing. It was made up of ups and downs but that only made me understand things better. I want to use this opportunity and thank the entire RTEMS community for seeing me through the whole internship period.*



