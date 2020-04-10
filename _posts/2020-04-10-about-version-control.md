---
layout: post
title: "My Small Guide About VERSION CONTROL"
date: 2020-04-10
---

# What is Version Control?
**'Version Control'** is a term I have come across a lot as a developer(*Not fully one yet :)*). 
I got confused a lot about what it actually meant but as time went by I eventually got a hang of what it is definitely all about. Well *'version control'* is simply a management system that tracks the changes made in a project. These changes can be adding a new file to your project, delecting some content in a file, removing some files, modifying a file or files. Basically, what version control does is anytime you make a change it kind of creates a snapshot of your work. This 'snapshot' is the state of your file at that time which is termed a **'version'**. Version control records the kind of changes being made, the time the changes were made and even who made the change. Pretty cool right? ;)

# How Useful Version Control Is To The Novice And Professional Developers
Whether a novice or a professional developer, having a version control system is extremely handy and worth the time of learning how exactly it works. Here is how useful it is;

1. ## **Team work:** 
  Just imagine developers working individually on same project without knowing what changes were made by their colleagues. A lot of conflicts will emerge when everyone comes together to intergrate their projects which obviously will be time consuming to rectify. But with version control you do not have to worry much about conflicts since it provides developers with a shared workspace to work simultaneously on a given project and notify everyone on who has made what changes. How cool is that? 
  
2. ## **Storage:** 
     Now let's picture a world without version control and you have this cool website to build. You are bound to be saving your work just in case you mess things up. But here's where confusion sets in. Will you save the entire project or save just the changes you made? If you save only the changes you will find it difficult to view the progress you made at a particular time. Meanwhile if you save the entire project at a given time there will be a huge amount of unnecessary and redundant data laying around since you are basically saving thesame thing hence covering up unnecesarry space. 
      It doesn't only end there. You start thinking of how to name these various versions of what you are saving. Let's say you are very organized and able to come up with a very comprehensive naming scheme but as time goes by your project increases and you may lose track of those names. We do not want to worry about whether we saved the last version of our site as 'mycoolwebsite15' or 'mycoolwebsite16'. We should instead worry if the the design of the site is responsive irrespective of the device being used or not. This is where version control comes in to save you all the stress about storage. And trust me it doesn't only store several versions of your project but stores it better than you ten fold. The version control knows there's only one project and all the changes made are recorded in the version control system(VCS).
    
3. ## **Recovery:** 
    Back to your cool site let's say you got busy and hired this to finish building your site. After a few days you came back to see how far the site has gone. Oh no! The site's messed up. The colors are just off and some buttons are not working. Turns out this guy lied on his resume about being a web developer. And the deadline to have the site done is the next day. You just fired him but still you have an unfinished site to build. Without version control it will be quite stressful and time consuming for you to go back and start checking on where he messed things up. It might be such a mess that you'd rather just start over. But with version control, you can easily roll back to previous version of your cool site before he messed things up. Next time just don't hire someone that incompetent! The point is version control provides access to historical versions of your project in case you made a mistake.
  
4. ## **Backup:** 
    Your project files are stored in a central server and every developer has a local copy of all the files present in the central server inside their thier local machine. Any time you start coding, it fetches your project files from the central server and after you are done working it transfers all the files back into the central server therefore at every time you always have a local copy of your project in your local machine. So incase your central server crashes, a backup is always available in your local server. Having version control is a very reliable tool because you always have backup.
  
5. ## **Analyse your project:** 
    When you change a version, version control provides you with proper description of what exactly changed and when it was changed so that you can analyse how your project evolved.

# Examples of Version Control Systems
Some popular version control systems are:

* **Git:**  This is an opensource distributed version control system for tracking changes in source code during software development. 'Distributed' in the sense that everyone working on a project using it has a local copy.

  *Features*
    * Provides strong support for non-linear development.
    * Distributed repository model.
    * Compatible with existing systems and protocols like HTTP, FTP, ssh.
    * Capable of efficiently handling small to large sized projects.
    * Cryptographic authentication of history.
    * Pluggable merge strategies.
    * Toolkit-based design.
    * Periodic explicit object packing.
    * Garbage accumulates until collected.

  * *Pros:*
    * Super-fast and efficient performance.
    * Cross-platform
    * Code changes can be very easily and clearly tracked.
    * Easily maintainable and robust.
    * Offers an amazing command line utility known as git bash.
    * Also offers GIT GUI where you can very quickly re-scan, state change, sign off, commit & push the code quickly with just a few clicks.
  * *Cons:*
    * Complex and bigger history log become difficult to understand.
    * Does not support keyword expansion and timestamp preservation.
    
* **Apache Subversion (SVN):** This is an opensource centralised version control system characterised by reliability as a safe haven.

  *Features*
    * Client-server repository model. However, SVK permits SVN to have distributed branches.
    * Directories are versioned.
    * Copying, deleting, moving and renaming operations are also versioned.
    * Supports atomic commits.
    * Versioned symbolic links.
    * Free-form versioned metadata.
    * Space efficient binary diff storage.
    * Branching is not dependent upon the file size and this is a cheap operation.
    * Other features – merge tracking, full MIME support, path-based authorization, file locking, standalone server operation.

  * *Pros:*
    * Has a benefit of good GUI tools like TortoiseSVN.
    * Supports empty directories.
    * Have better windows support as compared to Git.
    * Easy to set up and administer.
    * Integrates well with Windows, leading IDE and Agile tools.
  * *Cons:*
    * Does not store the modification time of files.
    * Does not deal well with filename normalization.
    * Does not support signed revisions.

* **Mercurial:** This is another open-source distributed version control system like Git. But it was designed for larger projects, mostly outside the scope of designers and independent web developers. The operating systems that it supports are Unix-like, Windows and macOS.

  *Features*
    * High performance and scalability.
    * Advanced branching and merging capabilities.
    * Fully distributed collaborative development.
    * Decentralized
    * Handles both plain text and binary files robustly.
    * Possesses an integrated web interface.

  * *Pros:*
    * Fast and powerful
    * Easy to learn
    * Lightweight and portable.
    * Conceptually simple
  * *Cons:*
    * All the add-ons must be written in Python.
    * Partial checkouts are not allowed.
    * Quite problematic when used with additional extensions..
    
* **CVS:** It is yet another most popular revision control system. CVS has been the tool of choice for a long time.
  
  *Features*
    * Client-server repository model.
    * Multiple developers might work on the same project parallelly.
    * CVS client will keep the working copy of the file up-to-date and requires manual intervention only when an edit conflict occurs
    * Keeps a historical snapshot of the project.
    * Anonymous read access.
    * ‘Update’ command to keep local copies up to date.
    * Can uphold different branches of a project.
    * Excludes symbolic links to avoid a security risk.
    * Uses delta compression technique for efficient storage.
  
  * *Pros:*
    * Excellent cross-platform support.
    * Robust and fully-featured command-line client permits powerful scripting
    * Helpful support from vast CVS community
    * Allows good web browsing of the source code repository
    * It’s a very old, well known & understood tool.
    * Suits the collaborative nature of the open-source world splendidly.
    
  * *Cons:*
    * No integrity checking for source code repository.
    * Does not support atomic check-outs and commits.
    * Poor support for distributed source control.
    * Does not support signed revisions and merge tracking.
    
 *  **Monotone:** Monotone, written in C++, is a tool for distributed revision control. The OS that it supports includes Unix, Linux, BSD, Mac OS X, and Windows.
 
    *Features*
      * Provides good support for internationalization and localization.
      * Focuses on integrity over performance.
      * Intended for distributed operations.
      * Employs cryptographic primitives to track file revisions and authentications.
      * Can import CVS projects.
      * Uses a very efficient and robust custom protocol called netsync.
      
     * *Pros:*
        * Requires very low maintenance
        * Good documentation
        * Easy to learn
        * Portable design
        * Works great with branching and merging
        * Stable GUI
        
     * *Cons:*
        * Performance issues observed for some operations, most visible was an initial pull.
        * Can’t commit or checkout from behind the proxy (this is because of a non-HTTP protocol).

*Other examples include Bazaar, TFS, VSTS.*

I hope you now understand what version control is all about and why it shhould be part and parcel of your life. Hope you find this comprehensive.
Thanks for reading! :)
