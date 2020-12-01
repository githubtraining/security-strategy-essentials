Nice, your log output is no longer showing reference to those previous commits. So, what exactly just happened?

### Our commit history has been modified

You probably noticed that when you ran the `git filter-branch` command, Git did some rewriting to some commits in the repository's history. Since we needed to alter the commits that referenced the `.env` file, it altered the commit ID, and all proceeding commits that point back to those commits.

This is why you need to consider local work and branches that are based on this previous history. This is okay to run, as long as everyone contributing in the repository is aware of the situation and can plan accordingly.

### Is the sensitive information gone?

Those commits no longer show in the file contents in your repository history. You can see this by navigating to your <a href="{{ repoUrl }}/commits/main">repository's commit history</a> and clicking on the "Add .env file" commit. Notice that there are now no referenced files or content recorded.

However, we can still access the cached commit if we know the old commit ID: {{ repoUrl }}/commit/848cd8c2043f6161a4f0043bffee212777281494

### Removing the old cached commits

This is where we'll need to contact the amazing GitHub Support team for assistance.

Even though we removed these commits, the historical reference to them can still be found if you know the commit ID. In a real world situation, you'll need to contact **GitHub Support** to perform the following:

- Run garbage collection on the repository to remove these unreferenced commit(s)
- Invalidate the Git cache to permanently remove any cached references

For our situation, we can skip contacting GitHub Support for this example! :smile:

<hr>
<h3 align="center">Find your final issue <a href="{{ url }}">here</a> now.</h3>
