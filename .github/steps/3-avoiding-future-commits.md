<!--
  <<< Author notes: Step 3 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 3: Avoiding future commits with `.env`

_Nice work removing the file from entire history of the repository! :sparkles:_

The steps we've taken so far ensure that any _new_ clones of the repository don't contain the sensitive data. But what about collaborators that may already have a copy of the repository? You should ask anyone with a copy of the repository to delete it and clone the repository fresh. In a real-life scenario, you'd also take [additional steps](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository#fully-removing-the-data-from-github) to ensure no sensitive data is cached on GitHub.com.

Now that we've mitigated the risk of exposing sensitive content, we'll be proactive and prevent its addition.

We'll now configure Git so it ignores a future addition of sensitive content by adding `.env` to `.gitignore`. If someone should that file to the local copy of their repository, it will remain only on the contributor's machine and won't be pushed to GitHub.

**What is `.gitignore`?** This special file allows us to tell Git naming patterns to ignore. You can read more about it in [Ignoring files on GitHub Docs](https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files).

### :keyboard: Activity: Add `.env` to `.gitignore`

1. Update the local copy of your repository to ensure you have the most recent version of the course files.
   ```shell
   git pull
   ```
2. Locate the file we added to the repository titled `.gitignore`.
3. Add `.env` to the file.
4. Stage, commit the file:
   ```shell
   git add .gitignore
   git commit -m "ignore .env files"
   ```
5. Push the file to GitHub.com
   ```shell
   git push
   ```
6. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.
