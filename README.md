# 2020-08-17: VT SWC Git lesson

Additional resources:

- git + rstudio: https://happygitwithr.com/
- dan's reference guide for git (but uses branches): https://chendaniely.github.io/training_ds_r/help-faq.html
- swc git lesson: https://swcarpentry.github.io/git-novice/
- if you want to know more about branches and forks: https://www.youtube.com/watch?v=uvWhSYBkZJ0
- Setting up ssh links: https://bi-sdal.github.io/training/ssh-keys.html

## Local

- `git init`: create git repository in current folder
- `git config --global user.name "Daniel Chen"
- `git config --global user.email "chendaniely@gmail.com"

- `git status`: tells you what is going on in your repository
- `git add <FILE>`: places <FILE> into the staging area
    - `git add README.md`
- `git commit`: commits files in the staging area
    - if you opened this in VI(M): <ESC> `:q!`
    - `git config --global core.editor "nano -w"`
- `git commit -m "MESSAGE"`: allows you to type a one line commit message in 1 step

- `git log`: shows you your history
    - `git log --oneline`: shows you your 1-line version of history

- `HEAD`: tells you where you are looking at in history

- `git diff`: shows you current state with last known state differences
    - `git diff --staged`: shows difference from staging area with last known
    - you can use `git log --oneline` to specify different versions in history

## Remotes

- `git remote add origin <URL>`: adds <URL> with the name origin
- `git push origin master`: pushes the master branch to the origin remote
- `git pull origin master`: pulls the master branch from origin to local computer

- You can make changes to different parts of a file and it will be combined automatically
- in a merge conflict, look for the `>>>` `===` `<<<` and fix those lines to what you want

- `git clone <URL>`: to download a git repo on to your local computer