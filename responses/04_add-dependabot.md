## Automated dependency updates with Dependabot

Manually going through your dependencies for alerts and outdated versions is tedious work. Let's automate this process!

**Meet Dependabot**

![download](https://user-images.githubusercontent.com/6351798/67623352-53f86200-f7e1-11e9-957d-47bb009f030f.png)

Dependabot creates pull requests to keep your dependencies secure and up-to-date!

### How does Dependabot work?

Dependabot is the actor for GitHub's [automated security updates](https://help.github.com/en/github/managing-security-vulnerabilities/configuring-automated-security-updates). 

1. GitHub uses the dependency graph and security alerts to scan your repository and notify you of potential dependency updates
1. If any dependencies are out-of-date, Dependabot opens a pull request to update each one
1. If tests pass, and the updated version looks good, you simply merge the pull request

### Configuring automated security updates

You can enable automated security updates for any repository that uses security alerts and the dependency graph. You can disable automated security updates for an individual repository or for all repositories owned by your user account or organization. GitHub will automatically enable automated security updates in every repository that uses security alerts and the dependency graph.

![Screen Shot 2019-10-28 at 1 23 52 PM](https://user-images.githubusercontent.com/6351798/67711794-5c3ed180-f988-11e9-97ba-41451996a2fb.png)

Here, we have a security alert on the **debug** dependency. Clicking on **debug** will show you the pull request created by Dependabot to update the dependency. We just updated to `2.6.9` but Dependabot noticed we are still outdated.

If you navigate to your [pull requests]({{ repoUrl }}/pulls), you'll notice Dependabot has done its job and is trying to bump, or update, the version of `debug`. Feel free to **approve and merge the pull request**.

## Close this issue when done

<hr>
<h3 align="center">I'll respond below when you close the issue.</h3>
