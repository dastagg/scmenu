#SCMENU#

A simple cli program that makes it easier to link Git and Fossil remote
repositories to the local environment.

NOTE: There are some "hardcoded" references. If you download it and use it, make sure you read through it and update those references.

For example: I have my own server running Gitolite so that remote is origin, GitHub is github and Bitbucket is bbucket.
So after you run the script to link a GitHub repository, if you do a "git branch all" you will see something like:

```* develop
  master
  remotes/github/develop
  remotes/github/master
```


At some time in the future, I may update this to be more "generic" but it will do for now.
