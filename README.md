# commands

## git

`git branch -r | awk -F/ '/\/bugfix/{print $2"/"$3}'` lists all remote branches starting with bugfix

`git branch -r | awk -F/ '/\/bugfix/{print $2"/"$3}' | xargs -I % git push origin -d %` deletes all remote branches starting with bugfix
