# Git Focused

This is a demo-repository showcasing how Git works.

## Commands

- git init
  - creates a new git repo (empty)
- git add
  - stage files to be committed
- git commit
  - create the commit
- git status
  - shows the status of the working directory
- git log
  - shows a history of past commits
- git remote
  - identifies other git repos to push/pull
- git push
  - send new commits to another git repo
- git pull
  - retrieve new commits from another git repo
- git clone
  - creates a local copy of a remote repository for you on your computer
- git branch
  - if given a name, creates a new branch with that name
  - if not given a name, it will list branches and indicate the current branch
- git checkout
  - switch to another branch
  - ... and does like fifty other things (we'll get to those in time)
- git merge
  - merges changes from another branch into the current branch

## Working Directory

- Untracked Files - new to the repository
- Modified Files - known files that have been changed
- Staged Files - ready to be committed

## Sync

> The repository you are pushing/pulling with is referred to as the _remote_
> repository. This is often times on GitHub, but it is not the only option.

Synchronization occurs between two repositories. When you
push or pull, the history of the two repositories are compared.

When pushing, you need to be up to date and have new commits to contribute.

> Up-to-date is defined as having all of the commits that are in the remote
> repository on the branch that you are trying to push to.
>
> To test this, you can write `git pull`. If it says `Already up to date.`
> then you're ready to push. If not, sort that out!

When pulling, the remote needs to have new commits to pull down.

In order for changes to be propagated, they need to be contained within a commit.

## Branching

Each branch represents a different "stream" of work. This can be anything
ranging from having a "stable" stream to a "I'm-working-on-this-feature" stream
to a "experimental" stream.

To make a new branch, type `git branch $BRANCH_NAME_HERE`. For instance, to
create a `develop` branch, you can type `git branch develop`.

To switch to a branch, type `git checkout $BRANCH_NAME_HERE`. For instance, to
switch to the `develop` branch, you can type `git checkout develop`.

To merge work from another branch, type `git merge $BRANCH_NAME_HERE`. For
instance, to merge work from the `feat-unittesting` branch, type
`git merge feat-unittesting`.

### Common Conventions

Here are some common branches you can expect to run into. Each team has its
own conventions that you should adhere to.

> Try to avoid using capitlized letters in your branch names -- there are
> platform-differences that you will run into if you don't.

- master
  - the default, the stable, the ready-to-ship
- develop
  - the experimental -- work is shared here
- feat-xxx
  - focused on a single feature

## License

MIT License - Copyright (c) 2020 Academy of Interactive Entertainment
