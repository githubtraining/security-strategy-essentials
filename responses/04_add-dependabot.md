## Automated dependency Updates with Dependabot

Manually going through your dependencies for alerts and outdated versions is tedious work. Let's automate this process!

**Welcome to Dependabot**

![download](https://user-images.githubusercontent.com/6351798/67623352-53f86200-f7e1-11e9-957d-47bb009f030f.png)

Dependabot creates pull requests to keep your dependencies secure and up-to-date!

### How does Dependabot work?

1. Dependabot scans your repository and checks for updates or insecure requirements
1. If any dependencies are out-of-date, Dependabot opens a pull request to update each one
1. If tests pass, and the updated version looks good, you simply merge the pull request

### Configuring automated security fixes

You can enable automated security fixes for any repository that uses security alerts and the dependency graph. You can disable automated security fixes for an individual repository or for all repositories owned by your user account or organization. GitHub will automatically enable automated security fixes in every repository that uses security alerts and the dependency graph.

![Screen Shot 2019-10-28 at 1 23 52 PM](https://user-images.githubusercontent.com/6351798/67711794-5c3ed180-f988-11e9-97ba-41451996a2fb.png)

Here, we have a security alert on the **debug** dependency. Clicking on **debug** will show you the pull request created by Dependabot to update the dependency. We just updated to `2.6.9` but Dependabot noticed we are still outdated.

Feel free to [**approve and merge this pull request**]({{ repoUrl }}/pull/4).

<details>
  <summary>How to Install Dependabot if not enabled through automated security fixes</summary>

    - Navigate to Dependabot on the [GitHub Marketplace](https://github.com/marketplace/dependabot-preview)
    - Click the "Install it for free" button
    - Follow on-screen instructions to add Dependabot to your GitHub profile
    - When installing Dependabot, choose `Only select repositories` and choose this repository, {{ repoUrl }}
    - On `app.dependabot.com`, under `repos you want to add`, select {{ repoUrl }} and click the `Add selected` button
    
</details>

#### Important Note!
Dependabot is owned and maintained by GitHub. Dependabot Preview is a public beta for functionality that we are integrating directly into GitHub. These automatic security fixes are in beta and are subject to change.


## Close this issue when done

<hr>
<h3 align="center">I'll respond below when you close the issue.</h3>
