hmtbrandeis
===========
Here are the basic instructions for:

1. Getting started with git, from the very beginning

2. The normal commands for pulling and pushing

3. Specific instructions for submitting a pull request

4. Oxygen download instructions

----

GETTING STARTED

download git-->git-scm.com/downloads
create github account on github.com

at this point on your computer you should have Git Bash. This is akin to the hg command prompt.

visit https://github.com/jscontras/hmtbrandeis.git
click FORK (upper right corner)

open Git Bash--clone

  $ git clone https://github.com/[your username]/hmtbrandeis

configure remotes--keep track of original

  $ cd hmtbrandeis
  
  $ git remote add upstream https://github.com/jscontras/hmtbrandeis.git
  
  $ git fetch upstream

find your local files folder on your computer. I found mine in users/jenny/hmtbrandeis
if you want, create a shortcut of your folder to your desktop

----

NORMAL FUNCTION

check status of your local files (to see if anything changed) -->
 
$ git status

pulling files

  $ git fetch upstream
  
  $ git merge upstream/master
  
[[make all of your changes, save locally]]

commit and push

  $ git add [FILE NAME YOU CHANGED]
  
  $ git commit
  
  $ git push origin master

So the feature of git is that whenever you commit and push, you only do it to your branch.
If you want changes saved to the master file you need to send a pull request to the master owner

----

SUBMITTING A PULL REQUEST

this is for when you want to make changes to the master copy, it's basically like merging the branches on hg but without all of the annoying problems (hopefully)

go to the hmtbrandeis repository page
click on change view to "my-branch"
click compare/review (box with two arrows pointing at each other in a loop, it's green)

set base fork : jscontras/hmtbrandeis

set base : master

set head : [your username]/hmtbrandeis

set compare : my-branch

click on "start a discussion about this..."
enter title and description
click "send pull request"

DONE!

----

DOWNLOADING OXYGEN

go to the Brandeis LTS software page

download the installer, if you haven't already

download the software for Oxygen XML editor

click on "License and support information"

download a one year license--make sure to copy it!

  ***when prompted upon installation, paste the license key into the box
  
MAKE SURE TO SPECIFY THAT YOU WANT TO OPEN XML FILES
