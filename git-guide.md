# Command line git

1. status
  Shows status of the local repository. This status includes:
  number of local commits that have not been synced with remote (GitHub)
  list of files in local folder than are NOT being tracked by git
  list of files in local folder that have changes that need to be committed
  git status

2. clone
    Copies the contents of a remote repository into a local repository 
    Command: ```git clone```

3. add
    In the local repository adds files for tracking 
    Command: ```git add```

4. rm
    Remove file from tracking. However, this does not erase the history of the file being tracked 
    Command: ```git rm```

5. commit
    Takes a snapshot of the files for tracking before pushing to the remote repository

6. push
    Sends the track local repository files up to the remote repository
    command: ```git push```

7. fetch
  Downloads objects from a different repository
  command: ```git fetch```

8. merge
    Merge changes from a branch into a single branch
    command: ```git merge ```

9. pull
    Pulls and updates the local repository againsts changes to the rmote repository.
    command: ```git pull``

10. branch
    Creates a branch of the current respositry
    command: ```git branch```

11. checkout
    Switches the current branch being wokred on
    command: ``` git checkout```
    
# Git files & folders

1. .git folder - makes the commandline aware of a git repository. stores data about the repo
2. .gitignore file - file containing files which should not be tracked within git.


# GitHub
1. Pull requests - Tells other collaborators changes made to brances 
2. SSH authentication to repositories - Allows passowrdless access to remote repos based on SSH Public keys
