Hey! We're going to work through a git flow exercise, that will show you both how git and github work together to improve developer speed and workflow. You'll be adding your name to the file `namelist`.

### Step 1

First, you'll want to `fork` my repository. A fork is a copy of a repository, so forking allows you to freely experiment with changes without affecting the original project.  Forks act as a sort of bridge between the original repository and your personal copy, and you can submit `pull requests` to help make other people’s projects better by offering your changes up to the original project. To do this, you need to find the `fork` button on the top right of the page:

![fork](img/fork.png?raw=true)

Click `fork`, and wait while the :sparkles: magic :sparkles: happens!

### Step 2

In order to add your name to `namelist.md`, you first have to somehow get a copy of it onto your local computer so that you can make a change. We'll do this with `clone`, which, as you might expect, clones the repo onto your computer. Navigate to the folder of your choice in the command line. I would recommend `Documents`, or something similar. Once you're there, you're ready to clone the repo into that folder.

`$ git clone https://github.com/YOURNAME/intro-to-git`

You should see some text in your terminal. Now that you've cloned it, you're ready to begin making a change. The primary branch is called `master`.

## Step 4

Ok, now that we have our own copy of the repo, we can make the change. Open `namelist.md` with a text editor of your choice and add your name to the list. Once you've done this, go back to your terminal.

## Step 5

In your terminal, type `git status`. You should see `namelist.md` listed in the results, as you just made a change to that file. `git status` is used to tell you about the current status of your branch (which is `master`), in terms of things you might have added, deleted, or changed. Now, type:

`$ git add namelist.md`.

This queues up your change, so that you can commit it to your branch.

## Step 6

Now that you've added your change, it's ready to be committed. To commit, you'll type:

`$ git commit -m "added my name to the list of names"`

You should now be ready to push up the branch!

## Step 7

To push up your branch, type:

`$ git push origin master`

Here, you're `push`ing the branch you edited with your change up to GitHub, where the `origin` is the location of repo you forked from me.

## Step 8

Time to open a pull request! If you hop back onto GitHub, and open https://github.com/YOURNAME/intro-to-git, you should see:

![fork](img/pr.png?raw=true)

Click `pull request`, and you should be taken to a new screen, which will look like this:

![fork](img/compare.png?raw=true)

Click the green `Pull Request` button, and see the resulting prompt!

Title it, hit `Create Pull Request`, and you're all set!
