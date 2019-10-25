We need to remove accidental commit that adds the `.env` file.

run `git clone {{ repoUrl }}.git`
run `git checkout add-wolverine-image`
run `git rebase -i master` and then remove the entire commit so only the `Add wolverine image to game` commit remains
run `git push -f` to force push your changes to the pull pull request
