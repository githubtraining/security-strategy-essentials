Removing the previous `.env` file from the branch is great, but it's reactive. We need to ensure future contributions don't include sensitive files by mistake. We can do this by adding a `.gitignore` file to our repository.

## Taking advantage of the `.gitignore` file

From time to time, there are files you don't want Git to check in to GitHub. You may want to ignore files that contain sensitive credentials or information which should not be pushed to your repository. There are a few ways to tell Git which files to ignore.

### Ignoring files

Git uses a file called `.gitignore` to decide which files and directories to ignore when committing.  Keep files containing sensitive data, like configuration or `.env` files, out of your repositories. This is one way to promote security best practices.

The `.gitignore` file can, and should, be committed into your repository.  By sharing this file and making it part of your code, future contributors to the repository will avoid committing sensitive data. There are many examples of `.gitignore` files available for you to use in your own repositories. You can find them in the [gitignore](https://github.com/github/gitignore) repository.

## Step 10: Add a `.gitignore` file

In this pull request, I'm adding a `.gitignore` file. Files ending with `.env` commonly include sensitive data. This helps you keep files with sensitive data secure and private. Let's add those files to the `.gitignore`.

### :keyboard: Activity: Updating the .gitignore file

1. Within this pull request, go to **Files changed**.
1. Click the ellipsis (`...`) in the right upper corner and click **Edit file** to edit the `.gitignore` file.
1. Edit the file by adding `.env` to line 1.
1. Scroll down, and commit your change.

 > _Note: Even after adding a file to the `.gitignore`, the previous commits that have edited that file still exist. If you accidentally committed sensitive data, first change any tokens or passwords. Then, contact GitHub Support for help correcting your history._


<hr>
<h3 align="center">Return to this pull request for my next comment.</h3>

> _Sometimes I respond too fast for the page to update! If you perform an expected action and don't see a response from me, wait a few seconds. Then refresh the page for your next steps._
