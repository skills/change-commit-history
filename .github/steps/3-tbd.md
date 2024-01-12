<!--
  <<< Author notes: Step 3 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
  TBD-step-3-notes.
-->

## Step 3: Avoiding future commits with `.env`

_Nice work finishing TBD-step-2-name :sparkles:_

In a real-life scenario, you'd ask anyone with a copy of the repository to delete it and clone the repository fresh. In a real scenario, you'd also take [additional steps](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository#fully-removing-the-data-from-github) to ensure no sensitive data is cached on GitHub.com.

For our next step, we'll configure Git so it ignores a future addition of the `.env` file. If someone should add it to the local copy of their repository, it will remain only on the contributor's machine and won't be pushed to GitHub.

**What is _TBD-term-3_**: TBD-definition-3

### :keyboard: Activity: TBD-step-3-name

1. Locate the file we added to the repository titled `.gitignore`.
2. Add `.env` to the file.
3. Stage, commit, and push the file to GitHub:
   ```shell
   git add .gitignore
   git commit -m "ignore .env files"
   git push
   ```
4. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.
