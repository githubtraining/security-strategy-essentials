## Removing sensitive information

A contributor opened a pull request to add a new image to the memory game. However, it appears that this contributor also committed a sensitive `.env` file that shouldn't be included. Contributors may commit sensitive information by accident or on purpose without knowing the consequences of these actions.

Before we approve this pull request and merge it in, we need to remove this sensitive `.env` file from the pull request.

## Step 8: Remove sensitive data in a pull request

We can do this by cloning this repository to our computer, and then running a few local Git commands before pushing up a fix on the contributor's branch on GitHub.

1. Clone this repository locally by running `git clone {{ repoUrl }}.git`
1. CD into your newly cloned repository with `cd security-strategy-essentials`
1. Checkout to the contributor's branch with `git checkout add-wolverine-image`
1. Remove the unwanted commit that introduced the `.env` file with a rebase. You can do this with `git rebase -i main` and then remove the entire commit so only the `Add wolverine image to game` commit remains
1. Run `git push -f` to force push your changes to the branch on GitHub

<hr>
<h3 align="center">I'll respond below when you push up a fix to remove the `.env` file.</h3>
