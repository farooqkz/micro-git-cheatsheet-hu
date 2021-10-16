# micro-git-cheatsheet-hu

### What is this?

Micro Git cheatsheet containing only so necessary commands. For Hormozgan University Git workshop

### What is a VCS?

Version control systems are software that help track changes make in code over time. As a developer edits code, the version control system takes a snapshot of the files. It then saves that snapshot permanently so it can be recalled later if needed.

Benefits of VCSs:
 - You'll always have history of your code.
 - They are great for team/group work.
 - You will be able to automate tasks. Thus saving your team's time.

Source: [Microsoft DevOps Docs](https://docs.microsoft.com/en-us/devops/develop/git/what-is-version-control)

### What is Git?

Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

Source: [Git SCM](https://git-scm.com/)

### The actual cheatsheet

#### Initialize/Create a Git repository locally

To create a Git repository on your computer, locally:

```
git init
```

And voila! You have a Git repository.

#### Commit changes 

```
git add myfile1.py myfile2.py
git commit -m "meaningful commit message"
```

#### Commit a single file

```
git commit -m "meaningful commit message" myfile.py
```

#### Push changes to remote repository

```
git push
```

#### Pull change from remote repository

```
git pull
```

#### Fetch from upstream(Rebase)

`upstream` is just a name which of course, you can change it.

```
git remote add upstream https://repository_address # for the first time
git fetch upstream # for each time
git checkout master # or main if master is not your branch
git rebase upstream/master # well done
```
