####How to check out a specific branch from github

```
Fri, 2009-09-11 10:57 | by Samuel Lampa
I ran into troubles trying to check out a specific branch from github.

I asked about it at #git on FreeNode IRC channel. I'll summarize how to do it:

First run:
git clone git://github.com/...[path to your project]...git

Then go:
git branch -a
...to see what branches you have. One of the lines you see might be:
remotes/origin/[NameOfYourBranch]

In order to start a local branch, based on that remote branch, and switch to it, go:
git checkout -t -b [NameOfYourBranch] remotes/origin/[NameOfYourBranch]

It will give you a message:
Branch [NameOfYourBranch] set up to track remote branch [NameOfYourBranch] from origin.
Switched to a new branch '[NameOfYourBranch]'
```
