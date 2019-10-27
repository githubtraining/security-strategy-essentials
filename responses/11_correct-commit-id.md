Nice, that's the commit that added the `.env` file. We'll need to remove the contents of this commit, as well as the commit that removed it from the history.

## Step 13: Remove historical reference to a previous `.env` file

We can do this with the following commands:

1. Since we cloned the repository earlier, let's run `git checkout master` to put us back on the master branch
1. Run `git pull` to update our local repository with the changes we merged from the contributor's pull request
1. Run `git filter-branch --index-filter "git rm -rf --cached --ignore-unmatch .env" HEAD` to remove the historical reference to the `.env` file

  **Note:** There is a lot going on with this command. We won't be diving into everything this command is doing, but it's filtering through the master branch and removing any cached reference to a `.env` file.

1. Next, let's run `git push -f` to force push this change to the master branch
1. Let's now run `git log --oneline` to get a list of our modified commit hisotry
1. Paste your log output into this issue as a comment

<details>
  <summary>Here is an example of a log output using `git log --oneline`:</summary>
  <hr>

```
d27dde6 (HEAD -> master, origin/master, origin/HEAD) Merge pull request #8 from {{ user.username }}/add-gitignore
65c1b71 Update .gitignore
a9b1b74 Merge add-wolverine-image into master
e2262cd Add wolverine image to game
9414843 Merge pull request #6 from {{ user.username }}/a-a-ron-patch-1
16d5372 Create SECURITY.md
28b3625 Merge pull request #1 from {{ user.username }}/update-dependency
3f7b819 Update package.json
e9ae69a Change package.json file to highlight where dependency update should go
831b1d1 Add empty .gitignore file
78cfef0 Remove .env file
8f08f15 Add .env file
e6e2377 Update README.md and Octocat game
528248c Initial commit
```
  <hr>
</details>

<hr>
<h3 align="center">I'll respond below when I see your comment</h3>
