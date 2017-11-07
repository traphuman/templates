# templates

In sites/default/files/humantesting/templates/git:

git init
git remote add origin https://github.com/traphuman/templates.git

# Execute by cron this script

#!/bin/bash
cd sites/default/files/humantesting/templates/git
git fetch origin master
git pull origin master

#each 12 hours

0 */12 * * * /script
