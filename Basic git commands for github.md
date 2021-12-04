# 1. Checkout a remote branch

When working in your local repository, you may want to checkout and work on branch code rather than the main code line. Just as with the main code line, when you push branch code to Bitbucket Cloud, it tracks that branch for you. To see which branches you or others on your workspace pushed, see the Branches list in your repository.

#### Using Git to checkout a branch on the command line:
For the purposes of these steps, <feature_branch> will refer to the name of your branch.

On your local system, make sure you have a local repository cloned from the remote repository. Then, do the following:

    Change to the root of the local repository.

    $ cd <repo_name>      

    List all your branches:

    $ git branch -a      

    You should see something similar to the following:

    * main   <feature_branch>
      remotes/origin/<feature_branch>
      remotes/origin/main     

    Notice that it lists both the branches that are local and the remote branches on Bitbucket. Using the list as reference, choose the branch you want to checkout.  In this example, the feature branch is the branch.

    Checkout the branch you want to use.

    $ git checkout <feature_branch>      

    Confirm you are now working on that branch:

    $ git branch      

    You should see something similar to the following:

    $ git branch 
    * <feature_branch>
      main     

Going forward, all your Git commands apply to the branch.  When you push the changes to your remote Bitbucket repository, those changes apply to the repository's branch.

