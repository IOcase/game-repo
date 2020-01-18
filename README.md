# eggheadmods
KSP modding folder repo for me and Jay

I have the initial saves we can use to start our project in here. You can clone this repo on your own machine and start making changes. It's best that we coordinate what we work on so that we can add stuff that doesn't interefere with each other. If we can avoid conflicts we can work twice as fast. I'm going to copy and paste a readme I have from earlier.



1. Microsoft Visual Studio student version 2019
https://visualstudio.microsoft.com/free-developer-offers/
This is entirely free software that has plugins for almost anything
I have the initial saves we can use to start our project in here. You can clone this repo on your own machine and start making changes. It's best that we coordinate what we work on so that we can add stuff that doesn't interefere with each other. If we can avoid conflicts we can work twice as fast. I'm going to copy and paste a readme I have from earlier.

2. Github
https://git-scm.com/downloads

3. Unity
https://store.unity.com/download-nuo
Note: Click on "Start here" to download unity

4. Git for unity
https://unity.github.com/

5. Git desktop
https://desktop.github.com/

6. Git Large File System
https://git-lfs.github.com/
NOTE: Git doesn't like storing gigantic files for free so we'll use the GLFS (Git Large File System.) 
The goal of this system is it will only store a reference to the large file in Git and if one of us requests it it'll go and find the file on that machine and transfer it cutting out git as the middle man.
This requires us to coordinate being online at the same time to ensure we can transfer things.

[fixed] -> NOTE: [gitignore fixes this] Make sure that you delete Library from the save file when you save a Unity project. It doesn't have data in it that's useful it's just meant as a cache so you can safely get rid of it since it's fucking huge. (this is actually redundant now. The gitignore fixes this)

7. Microsoft visual studio code
https://code.visualstudio.com/
NOTE: This is different than 1. because it's meant to be a lighter faster version thats easy to open from cmd line prompts. We'll have to become familliar with CMD prompts at some point so this is helpful to have. The git desktop app provides a convenient GUI for us to use instead of cmd all the time
but you just can't avoid using it sometimes. cmd is too powerful compared to the limitations of a GUI.

Introduction:

Provided you've downloaded and installed all of the previous software I'll try to quickly summarise what it is that all of this junk is intended to do. 

Version Control Software (VCS) Git/Github:
The vast majority of creative software on the market will have a plugin that acts as an adaptor for git. That way we can store previous versions of our work and roll back to a working version if we break something. The way git works is the main files are stored in the file directory called MASTER.

MASTER is the game itself pretty much. If you want to add a new feature to the game what you would do is you would open up unity and you would clone the repository from git to your computer. Essentially what this does is it copies a version of the entire game onto your computer. 

The gitignore file thats part of the project basically tells git to only upload the important files that we're actually changing. Unity doesn't actually make a huge amount of important data. Most of it is in the library folder and temporary folders which gitignore tells git to... well... ignore.

The benefit of cloning a repo is that it ensures that people pretty much always have a backup of the whole file system for a project. Although git is really good about backing up on their end to so you shouldn't really have to worry about losing data even on their end. 
Anyways what happens after you clone the repository is you can begin to add edits under your own branch

Branching and Merging:
A branch https://guides.github.com/introduction/flow/ (ctrl + click to open links) is basically a offshoot of the MASTER tree. It's a carbon copy of the master where you can test out new features without affecting the main game itself. 
More than one person can work on a branch at any one time provided 2 people don't edit the same line of code. If they do you'll see it during code review during a commit. A commit is what you'll do once a sub feature has reached completion.

The usual process once you think that your sub feature is ready to be reviewed and added to the branch is you'll make a pull request as part of your commit where people can review what you're adding to make sure that it meets the standard of the repo. Depending on how the repo is organized the 
maintainer (in this case that would be me and you) reviews the code or the change and decides if it's worth adding to the branch or if it'll just fuck things up. Once it passes code review your commit can be PUSHED to the repo. 

What this means is that your code is added to that branch for other people to work on because your feature was deemed complete and worth working on. This process continues until the meta feature (make textures for environment for example) is complete the branch
will initiate a pull request to begin the process of merging the branch with the MASTER. Once the changes have been approved the branch can be MERGED into the MASTER and then that branch gets deleted because that feature is now part of the main project.

It is possible to reverse this process in Git. They make it very easy to roll back changes if they happen so that we don't have to worry about breaking things with experimentation. As long as we make small commits and review the changes we'll have plenty of places to revert back to. This brings me to
my next point:

Comments on Commits:
We have to set a standard for what level of detail we expect when we commit a change to our branch. We need to make sure that the comment makes sense to anyone who reads its so don't write it so you will understand it but so that we will both "added bot" isn't descriptive (I made this mistake)

So putting something like "added second flybot to main stage room" or something like that. "Changed textures for main rooms and church" "Rebalanced blaster damage" .etc

Just try to keep your comments short but informative. I think we should make commits once we have a working version of what it is we want to do. 

Let's worry about doing things quickly so that we make mistakes and learn fast. Then we can move on to making things good once we have an understanding of the system and how it functions. 
I'll walk you through how all of this stuff works don't worry. I want to make this as easy as possible for you because if we learn this together we'll learn faster and have more fun. I can't wait to make games with you Jayden!
