# Introduction to Git
 
Takehome message: **Use git**

## Assignment
Clone https://github.com/beards-lab/Phys520

- Create a initials_your-nick-name.md into the 01_GitTutorial folder
  - E.g. FJ_jez.md
- Write down what you 
  1. like about GitHub
  2. dislike about GitHub
  2. At least one question
- Commit, push, and issue a pull request

## Answers to your questions

### Interfacing
> A question I have is how Git interfaces with editors like VS Code

Various tools has already integrated the basics: commit, pull and push functions, so you don't have to switch the applications. For more complex tasks, there is always possibility to switch to another app. These are just interfaces and the repository could be handled from any tool though.

> I don't like how GitHub has several places to be used. I have only used the web interface before and am only used to using it. 

That is fine for submitting readmes and other text files. But what if (and that is the most common use case) you need to run your source code locally on your computer?

> When I try to create a new text file in a repository, for example a README.md file, the file is still showing as README.md.txt. What can I do differently to get rid of the .txt on those files? 

That is your computer issue - see e.g. https://knowledge.autodesk.com/support/autocad/learn-explore/caas/sfdcarticles/sfdcarticles/How-to-enable-hidden-file-extensions-in-Windows.html

### Security
> It is my understanding that GitHub is not the best tool to use for secure/private data. What other options are available for collaborating and sharing code if working on project with more sensitive data?

Good thinking. You can keep the repository private or private within the team. For added security of really sensitive data, you can use your own git servers or dedicated hosting or gitlab.


### Merging and conflicts
> How does GitHub maintain an accurate copy of a file if multiple people are editing it at the same time?

It is not - all versions are independent and equally important. The issue comes around when *merging* those changes. Any modified or added line is merged automatically, unless two people commited change to the same line iof code. Then the one merging has to make a decision.

> How to avoid merge conflict while working on Git?

Talk to each other :] But do not be afraid of conflicts, they happen and are usually easy to resolve.

> What if when you push the newly edited file and found there is an updated one after your pull request?

This is the task of the repository admin to merge. If there is a conflict, she should decide, which change is better. The pull request is just a merge of two branches, so it always merges the most up to date versions of both. You can continue working on your branch even after issuing a pull request. Always the latest version would be merged. If that is not preferred, you can always start a new branch and issue pull request from this (stale) branch.

> I am confused about the pull requests. Are we supposed to issue a pull request from main-2023 with our username to main-2023 that is within the Beardslab profile? 

Exactly. You have a fork (a copy) of that, which behaves just as any branch. But only the owner can merge that. THat is why you need to suggest merging yours main2023 into "my" main-2023"

### Maintenance
> If a version of your code/document becomes obsolete would it be recommended to get rid of it to clear up some of the version history or would this cause problems along the line as we discussed in class the other day about getting rid of things? It seems eventually with enough edits/commits things would start to get cluttered so how would you maintain clean organization?

You could, but that is not really common. What if you want to return to part of your codes one day? Source code isnot that resource demanding, the repository itself is zipped, so  it takes close to nothing. I wouldnt bother. More important: mark your releases, be clear about what is the MAIN version. 

### Usage
> To what extent will people actually utilize GitHub? (It needs to create a repository first, add a new file, write in the file and then have to commit and push.)

To infinity and beyond. Yes, you have to set up a repository. You do that once for a project. You have to commit often and push from time to time. The rest you do anyway :)

> Does any new repository need a new empty folder? Can I save all the repositories under a collection folder?

You can have a big repository with dozens of folders. Within one folder there is only one repository allowed.

> Is Git really used anywhere outside of coding? I've heard several people mention that it can be used for anything, not just code. Yet I never hear about anybody actually using it for things other than code.

Sure. For example, you can store your LaTex source of your papers. Myself I am maintaining a newsletter https://github.com/modelica/newsletter. More on the topic https://www.reddit.com/r/git/comments/1xymq2/do_people_use_git_for_things_other_than_software/

> Using git on the command line should be a punishhment for murderers. 

They are called Linux people and only some of them are murderers.

### GitHub and HitHub desktop
> If someone modifies code/ a file on Github proper. Do the changes it still have to go through the same committal barriers as they would when committing from a local repository?

Exactly. If you change a file on GitHub.com via the editor, note there is not a "save" but a "commit" button. Same for creating files. So you are commiting without even knowing. Then, if you pull your recent online changes to local it gets merged as in merging two branches.

> Is there a difference between "push" and "publish"? 

Push is to bring your changes (commits) to remote (e.g. github.com). Publish is the same, but here they are referring to creating new branch on remote, making the branch public. Technically it is the same, but might help prevent some unwanted behavior (e.g. this is my testing branch and for some reason I do not want to push (that is publish) that - this is stupid, but can happen).

> How are all the pushed files organized in the remote repository (especially when there are tens of people working on a project)? Are they easy to parse through/does an administrator need to keep up with the remote work space to keep it tidy? C) 

> Does github deskptop have more functionality compared to just using terminal, or are there the same terminal commands that do actions done in github desktop?

In the background the github desktop is just a frontend interface to the commandline comands, but not all of them are included.

> This has nothing to do with what we covered in class, but I know GitHub just came out with GitHub Copilot -- and AI coding assistant. Have any of the instructors tried this out? It seems really freaking cool.   

I have not. There have been some controversions though, as of using the open-source and perhaps also even not open-source repositories to teach the AI.

> I wish there was an easier way to visualize branches and changes

First you can see the Insights / Network diagram for public erpositories. Alternatively, you can grab TortoiseGit (just a moer complex, more powerful git tool) with its ref log https://tortoisegit.org/docs/tortoisegit/tgit-dug-showlog.html

> How would I have created this file in my desktop.. I had troubles finding the folder on my desktop but I can see it fine on the GitHub web interface.

Github desktop can help you with that - just rightclick the file and select show in explorer or edit.

### The class
> Do we have final presentations about our projects?

Honestly, I do not know. But I think you should have :)

> Are we going to be turning in assignments over git all sememster? 

No idea here. But I guess you could? I think Dan prefers sending that on email though.
