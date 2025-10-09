# Version control and git 


Some material reused and adapted from [Version Control with Git](https://swcarpentry.github.io/git-novice/) by the [Software Carpentry Foundation](https://software-carpentry.org/)

Licensed under [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/)


![Piled Higher and Deeper](https://raw.githubusercontent.com/stevenaeola/progblack_lectures/main/git/phd101212s.png)


 “Piled Higher and Deeper” by Jorge Cham <http://www.phdcomics.com>


## Linear history

![linear development of a document](https://raw.githubusercontent.com/stevenaeola/progblack_lectures/main/git/play-changes.png)


## Multiple authors

![different changes](https://raw.githubusercontent.com/stevenaeola/progblack_lectures/main/git/versions.png)


## Merging changes

![merges](https://raw.githubusercontent.com/stevenaeola/progblack_lectures/main/git/merge.png)


## Version control software


- Revision Control System (RCS)
- Concurrent Versions System (CVS)
- Microsoft Word Track Changes
- Subversion
- git
- mercurial
- darcs



## All about git

- Distributed version control system
- Developed by Linus Torvalds and others to manage the Linux kernel
- Linus named it after himself
- Designed to be fast
- Very widely used in academia and industry ([80.5%](https://survey.stackoverflow.co/2025/technology#most-popular-technologies-office-stack-async-prof))



## The Linux kernel development under git

[Visualised with gource](https://www.youtube.com/watch?v=MkJxlKD2bjk)


## git under the hood

- Different from earlier systems such as RCS, CVS and Subversion: no diffs
- Originally developed under Linux, but available elsewhere
- No central repository, but can synchronise with remotes
- Cloud-hosted repository servers: github; gitlab; bitbucket

Recommend you use github with education: free private repositories


## Key concepts in git


- A __file__ (in a path)
- A __commit__: a snapshot of a collection of files at a particular time
- A __branch__: a linear sequence of commits
- A __repository__: (possibly) many branches of a project
- A __remote__: another place where a repository is stored



## Key commands in git

Working on the command line (like [84% of developers](https://survey.stackoverflow.co/2022/#version-control-vc-interaction))
```
git init
git add
git status
git commit
git push
```


## git init

Creates a directory `.git` where everything is stored

You may also want to do `git config` at this stage

Think about adding a `.gitignore` file


## git add

Puts the current working version of a file into the staging area

Preparing for a commit

Check what will be committed with `git status`


## git commit

Makes a commit based on currently staged files

Will start an editor (see git config)

Consider
```
git commit -m "message"
```
to avoid editor


## git push

Pushes a branch to a remote repository

`git push origin main`

`origin` defined by
```
git remote add origin
```
or
```
git clone
```

The default branch used to be `master` instead of `main`. See [SO article on changing](https://stackoverflow.com/questions/67543278/git-how-to-change-default-branch-for-everything-i-do)


## See also

- [Summary of main commands](https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html)
- [Useful tutorials in particular Getting Started and Collaborating](https://www.atlassian.com/git/tutorials)
- [Git from the bottom up](https://jwiegley.github.io/git-from-the-bottom-up/) an explanation of how git works
