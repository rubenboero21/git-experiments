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
  - https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging
- Modify a file (liam.txt) on new branch
- Push changes to branch:
  - git add liam.md
  - git commit -m "commit message"
  - git push --set-upstream origin "branch name"
- Created pull request via GitHub website
  - https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request?tool=webui

Ruben:
- On GitHub website:
  - Reviewed and accepted pull request
  - Merged branch into main
  - https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/approving-a-pull-request-with-required-reviews

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
  - This failed partially through because of the conflict
  - https://stackoverflow.com/questions/13106179/error-fatal-not-possible-to-fast-forward-aborting
- Opened the conflicting file with VSCode to get a nice graphical view of the conflicting lines 
- Fixed the merge conflict by removing the change Ruben made from the file
- Used "git rebase --continue"
- Merge conflict resolved
