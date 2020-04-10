---
layout: post
title: "My Small Guide About VERSION CONTROL"
date: 2020-04-10
---

## What is version control?
'Version Control' is a term I have come across a lot as a developer(*Not fully one yet :)*). 
I got confused a lot about what it actually meant but as time went by I eventually got a hang of what it is definitely all about. Well 'version control' is simply a management system that tracks the changes made in a project. These changes can be adding a new file to your project, delecting some content in a file, removing some files, modifying a file or files. Basically, what version control does is anytime you make a change it kind of creates a snapshot of your work. This 'snapshot' is the state of your file at that time which is termed a 'version'. Version control records the kind of changes being made, the time the changes were made and even who made the change. Pretty cool right? ;)

## How Useful Version Control Is To The Novice And Professional Developers
Whether a novice or a professional developer, having a version control system is extremely and worth the time of learning how exactly it works. Here is how useful it is;
1. **Team work:** 
  Just imagine developers working individually on same project without knowing what changes were made by their colleagues. A lot of conflicts will emerge when everyone comes together to review the work which obviously will consume time to finally rectify. But with version control you do not have to worry much about conflicts since it provides developers with a shared workspace to work simultaneously on a given project and notify everyone on who has made what changes. How cool is that? 
2. **Storage:** 
  Now let's picture a world without version control and you have this cool website to build. You are bound to be saving your work just in case you mess things up. But here's were confusion sets in. Will you save the entire project or save just the changes you made? If you save only the changes you will find it difficult to view the progress you made at a particular time. Meanwhile if you save the entire project at a given time there will be a huge amount of unnecessary and redundant data laying around since you are basically saving thesame thing hence covering up unnecesarry space. It doesn't only end there. You start thinking of how to name these various versions of what you are saving. Let's say you are very organized and able to come up with a very comprehensive naming scheme but as time goes by your project increases and you may lose track of those names. We do not want to worry about whether we saved the last version of our site as 'mycoolwebsite15' or 'mycoolwebsite16'. We should instead worry if the the design of the site is responsive irrespective of the device being used. This is where version control comes in to save you all the stress about storage. And trust me it doesn't only store several versions of your project but stores it better than you ten fold. The version control knows there's only one project and all the changes made are recorded in the version control system(VCS).
3. **Recovery:** 
  Back to your cool site let's say you got busy and hired someone to finish building your site. After a few days you came back to see how far the site has gone. Oh no! The site's messed up. The colors are just off and some buttons are not working. Turns out this guy lied on his resume about being a web developer. And the deadline to have the site done is the next day. You just fired him but still you have an unfinished site to build. Without version control it will be quite stressful and time consuming for you to go back and start checking on where he messed things up. It might be such a mess that you'd rather just start over. But with version control, you can easily roll back to previous version of your cool site before he messed things up. Next time just don't hire someone that incompetent! The point is version control provides access to historical versions of your project in case you made a mistake.
4. **Backup:** 
  Your project files are stored in a central server and every developer has a local copy of all the files present in the central server inside their thier local machine. Any time you start coding, it fetches your project files from the central server and after you are done working it transfers all the files back into the central server therefore at every time you always have a local copy of your project in your local machine. So incase your central server crashes, a backup is always available in your local server. Having version control is a very reliable tool because you always have backup.
5. **Analyse your project:** 
  When you change a version, version control provides you with proper description of whatexactly changed and when it was changed so that you can analyse how your project evolved.

##Examples of Version Control Systems
Some popular version control systems are:
* **Git:**  This is an opensource distributed version control system for tracking changes in source code during software development. 'Distributed' in the sense that everyone working on a project using it has a local copy.
  * *Pros:*
    * Branches are easy to merge.
    * Addons can be written in many languages.
    * Offline use.
  * *Cons:*
    * Does not support 'commits' across multiple branches or tags.
* **Apache Subversion (SVN):** This is an opensource centralised version control system characterised by reliability as a safe haven.
  * *Pros:*
    * Easy to use.
  * *Cons:*
    * Must work online

* **Mercurial:** This is another opensource distributes version control system like Git. But it was designed for larger projects, mostly outside the scope of designers and independent web developers.
  * *Pros:*
    * Easy to learn.
    * Web server built in.
  * *Cons:*
    * Addons must be written in Python.

*Other examples include Bazaar, Monotone.*

I hope you now understand what version control is all about and why it shhould be part and parcel of your life. Hope you find this comprehensive.
Thanks for reading! :)
