## Sensitive data elsewhere in the repository contents

Often sensitive data is buried deep in a repository's history. The process for removing these files and commit data is a bit tricker and more involved.

In our repository's history, there is a reference to a `.env` file with sensitive information. We've since added a `.gitignore` to prevent this from happening in the future, but it doesn't modify any previously committed references from the history.

There are a few things we need to think about and take into consideration before we start altering our historical content. But for now, let's start with identifying the commit in question by going through our commit history.

## Step 12: Find historical reference to a previous `.env` file

1. Navigate to the Code tab of the repository and click on the `commits` link directly under the Code tab
1. Scanning through the commit history, locate the commit that added the `.env` file
1. Copy and paste the commit SHA ID as a comment in this issue

<hr>
<h3 align="center">I'll respond below when you add your comment to this issue.</h3>
