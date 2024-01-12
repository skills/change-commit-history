<!--
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
  TBD-step-2-notes.
-->

## Step 2: Removing a file from Git history using BFG Repo-Cleaner

_You did TBD-step-1-name! :tada:_

Now that we've deleted the file, people that browse the repository on GitHub.com or anyone looking at just the head commit won't see the file. However, due to Git's nature, the file is still present in the history. In this step, we'll work on removing the file from the repository history.

There are multiple tools available for removing Git history, we'll use BFG Repo-Cleaner in this step. You can find additional documentation on [Using the BFG in GitHub Docs](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository#using-the-bfg).

**What is _TBD-term-2_**: TBD-definition-2

### :keyboard: Activity: Use BFG Repo-Cleaner to remove the `.env` file

1. Install BFG Repo-Cleaner on your machine. You can follow the [instructions on the web site](https://rtyley.github.io/bfg-repo-cleaner/) to do so or you can use a package manager for your operating system.
2. Run each of the following commands to confirm the state of the repository:

   ```shell
   # Confirm .env is removed
   # Expected return: empty
   find . -name ".env"

   # Search for .env in the repository's history
   # Expected return: 2 commits from adding and then removing .env
   git log --stat --all -- .env
   ```

3. Run the following command to delete all references to `.env` that exist in the repository.
   ```shell
   bfg --delete-files .env
   ```
4. The tool will run and make some suggestions about some follow-up commands. Run those to get your local repository cleaned up.
5. Push your changes to GitHub. Note we're using the `--force` argument in this step since we're altering Git history.
   ```shell
   git push --force
   ```
6. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.
