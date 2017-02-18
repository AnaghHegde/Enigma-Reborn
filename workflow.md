# Development Workflow

## Fixing issues


### Step 1: Pick an issue to fix
 
 After selecting the issue
 
  1.Comment on the issue saying you are working on the issue.

  2.We except you to discuuss the approach either by commenting or in the gitter.
  
  3.Updates or progress on the issue would be nice.

### Step 2: Branch policy<br>

  Start off from your `development` branch and make sure it is up-to-date with the latest version of the committer repo's
 `development` branch. Make sure you are working in development branch only.<br>
 `git pull upstream development`
    
 If you have not added upstream follow the steps given [here](https://help.github.com/articles/configuring-a-remote-for-a-fork/).

### Step 3: Coding Policy

### Step 4: Submitting a PR

 Once a PR is opened, try and complete it within 2 weeks, or at least stay actively working on it.
 Inactivity for a long period may necessitate a closure of the PR. As mentioned earlier updates would be nice.

### Step 5: Code Review
 Your code will be reviewed, in this sequence, by:

 * Travis CI: by building and running tests.<br>
   If there are failed tests, the build will be marked as a failure.
   You can consult the CI log to find which tests.<br>
   Ensure that all tests pass before triggering another build.
 * The CI log will also contain the command that will enable running the failed tests locally.<br>
 * Reviewer: A core team member will be assigned to the PR as its reviewer, who will approve your PR or he will suggest changes.

 Squash your commits. If you don't know what does squashing of commits is read from [here](http://stackoverflow.com/a/35704829/6181189). Then follow the steps given below.

 1. Run this command : <br>
   `git rebase -i HEAD~numberofcommits` numberofcommits is how many commits you wan't to squash.
 
 2. Then a pop-up would appear with your default text editor.
 
 3. In that file replace all of the pick with squash excluding the first one.Save the editor.
 
 4. Run this command `git push -f origin yourbranch`
 
    Usually origin is your remote if it is not so replace origin with the remote.
