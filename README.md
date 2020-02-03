#SCMENU#

A simple cli program that makes it easier to link Git and Fossil remote
repositories to the local environment.

NOTE: There are some "hardcoded" references. If you download it and use it, make sure you read through it and update those references.

Hardcoded Reference 1: I have my own server running Gitolite so that remote is
origin, GitHub is github and Bitbucket is bbucket, etc.
So after you run the script to link a GitHub repository, if you do a "git branch --all" you will see something like:

```
* develop
  master
  remotes/github/develop
  remotes/github/master
```

Hardcoded Reference 2: I have a file structure like this:

```
$HOME
├── bin
│   └── scmenu -> link to program in scripts directory
├── dev
│   ├── FOSSIL
│   │   └── all the Fossil repositories
│   │   └── fossil-files
│   │       └── ticket-config
│   │   └── fossil-settings
│   │       └── ignore-glob
│   ├── python
│   │   └── Python projects here
│   └── scripts
│       └── Script projects here
```


Hardcoded Reference 3: Depending on the "development workflow", there may only
be the master branch. If a development branch is created, I always call it
develop. If you call it something else, you will have to change it in the
script.

At some time in the future, I may update this to be more "generic" but it will do for now.
