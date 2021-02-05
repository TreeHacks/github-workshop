# Github workshop

## Clone a repository

```git clone https://github.com/TreeHacks/github-workshop.git```

- This will grab the latest code from github and save it to your machine
- Generally, you only need to do this once per project

## Create a new branch

```git checkout -b [branch_name]```

- You can think of branches as "versions" of the codebase
- A common git pattern: create a branch ("feature branch"), make changes, then merge that feature branch back into the main branch

## Make a change

- Create a new file in the "participants" folder named [Your first name]_[Your last name].md
- Add some info about yourself! (eg what school you go to, favorite language, etc.)

## View Status

```git status```

This will show you a list of changes that have been made since the last commit (we'll talk about commits later)

## Add Changes

```git add [path]```

or, to add all changed files:

```git add .```

This adds all of the changes we've made to the "staging area". This doesn't do much in and of itself, but allows us to...

## Commit Changes

```git commit -m "commit message"```

You can think of commits as a set of changes - each is associated with an author, timestamp, etc.

## View Previous Commits

```git log```

With 'git log', we can take a look at the entire history of our branch. At the top, you should see the commit that you just added, followed by commits from other users.

## Push Branch

We now have a change committed locally on our computer, but we want to "push" it up to the github repository so that others can view and modify it. Use:

```git push origin [branch_name]```

To create a new branch on the github repo that matches the one on your local

## Create a pull request

A pull request lets you notify everyone in the repository of your changes and enables those changes to be merged into the main branch. You can do this from the github UI

## Merge pull request

Press the big green merge button on github!

## Pull others' changes

Once other contributors have added their changes, you probably want to get an updated version of the main branch with everyone's work on it.

First checkout the main branch:

```git checkout main```

And pull:

```git pull```