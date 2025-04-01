# git-experiments
## Part 1 
Ruben:
- Created repo on GitHub
- On command line:
  - cd into desired location
  - git clone https://github.com/rubenboero21/git-experiments.git
  - cd into cloned repo
  - vi ruben.txt, added text to the document
  - git status to see the file to add
  - git add ruben.txt
  - git commit -m "commit message"
  - git push

Liam:
- On command line:
  - git clone https://github.com/rubenboero21/git-experiments.git
  - git pull
  - cat ruben.txt
- Emotional support

## Part 2
- git log (as per instructions)
Liam:
- Created branch on command line:
  - git branch "branch name"
  - git checkout "branch name"
- Modify a file (liam.txt) on new branch
- Push changes to branch:
  - git add liam.md
  - git commit -m "commit message"
  - git push --set-upstream origin "branch name"
- Created pull request via GitHub website

Ruben:
- On GitHub website:
  - Reviewed and accepted pull request
  - Merged branch into main

- git log (as per instructions)

## Part 3
Ruben:
- Modified ruben.txt to have multiple lines (to have a more meaningful conflict)
- Pushed changes

Liam:
- Pulled changes
- Modified a line in ruben.txt
- Pushed changes

Ruben:
- Did not pull changes
- Also modified the same line as Liam did above
- Tried to git pull, got merge conflict error
- Used "git pull --rebase" command. 
  - This failed as well because of the conflict
- Opened VSCode to get a nice graphical view of the conflicting lines 
- Fixed the merge conflict by removing the change Ruben made from the file
- Used "git rebase --continue"
- Merge conflict resolved
