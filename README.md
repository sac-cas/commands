# commands

## git

git branch -r | awk -F/ '/\/bugfix/{print $2"/"$3}' | xargs -I % git push origin -d %
