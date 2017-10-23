Hey! We're going to work through a git flow exercise, that will show you both how git and github work together to improve developer speed and workflow. You'll be adding your name to the file `namelist`.

### Step 1

In order to add your name to `namelist.md`, you first have to somehow get a copy of it onto your local computer so that you can make a change. We'll do this with `clone`, which, as you might expect, clones the repo onto your computer. Navigate to the folder of your choice in the command line. I would recommend `Documents`, or something similar. Once you're there, you're ready to clone the repo into that folder.

`$ git clone https://github.com/codebytere/intro-to-git`

You should see some text in your terminal. Now that you've cloned it, you're ready to begin making a change. The primary branch is called `master`.

## STEP 2

In keeping with the GitHub Flow™, you'll first need to make a branch so that you can add
your name to `namelist.md`. This is done with:

`$ git checkout -branch MYNAME_branch`

Replace `MYNAME` in the above with your own name. `git checkout` is the command used for switching branches. To add a new branch, we use the `-branch` flag.

## Step 3

Ok, now that we have our own branch, we can make the change. Open `namelist.md` with a text editor of your choice and add your name to the list. Once you've done this, go back to your terminal.

## Step 4

In your terminal, type `git status`. You should see `namelist.md` listed in the results, as you just made a change to that file. `git status` is used to tell you about the current status of your branch, in terms of things you might have added, deleted, or changed. Now, type:

`$ git add namelist.md`.

This queues up your change, so that you can commit it to your branch.

## Step 5

Now that you've added your change, it's ready to be committed. To commit, you'll type:

`$ git commit -m "added my name to the list of names"`

You should now be ready to push up the branch!

## Step 6

To push up your branch, type:

`$ git push origin MYNAME_branch`

`MYNAME_branch` is the branch that you created earlier and replaced with your name. Here, you're `push`ing the branch yu created with your change up to GitHub, where the `origin` is the location of repo you originally cloned from me.

## Step 7

Time to open a pull request! If you hop back onto github, and open https://github.com/codebytere/intro-to-git, you should see a little yellow bar that says `you recently pushed branches` and askes if you want to open a pull request. Click it, and see the resulting prompt. 