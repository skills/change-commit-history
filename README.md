<header>

<!--
  <<< Author notes: Course header >>>
  Read <https://skills.github.com/quickstart> for more information about how to build courses using this template.
  Include a 1280×640 image, course name in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Next to "About", add description & tags; disable releases, packages, & environments.
  Add your open source license, GitHub uses the MIT license.
-->

# Remove commit history

Accidental commits can be tricky to remove with Git. In this GitHub Skills course, you'll use BFG Repo-Cleaner to change the history of a Git repository. You can apply what you learn in this course to fully remove sensitive material from your own repository.

</header>

<!--
  <<< Author notes: Course start >>>
  Include start button, a note about Actions minutes,
  and tell the learner why they should take the course.
-->

## Welcome

A trustworthy commit history is the backbone of version control with Git. As a result, altering commit history is difficult by design. Sometimes, the history needs to be altered to remove credentials or other sensitive data that is mistakenly checked in. In this course, we'll learn how to remove content from repository's complete history and apply best practices for preventing accidental commits in the future.

- **Who is this for**: Intermediate users of Git, organizations
- **What you'll learn**: How to remove a file from Git's entire history
- **What you'll build**: You'll manipulate the history of a Git repository
- **Prerequisites**: We recommend you clone this repository to your machine and use the command line to follow along. You'll also need to install BFG Repo-Cleaner, but the steps will be covered in the course.
- **How long**: This course takes less than 1 hour to complete.

In this course, you will:

1. Remove content from the root directory of a repository
2. Use BFG Repo-Cleaner to remove content from repository history
3. Avoid future accidental commits by adding a pattern to `.gitignore`

### How to start this course

<!-- For start course, run in JavaScript:
'https://github.com/new?' + new URLSearchParams({
  template_owner: 'skills',
  template_name: 'change-commit-history',
  owner: '@me',
  name: 'skills-change-commit-history',
  description: 'My copy of the skills course on changing commit history',
  visibility: 'public',
}).toString()
-->

[![start-course](https://user-images.githubusercontent.com/1221423/235727646-4a590299-ffe5-480d-8cd5-8194ea184546.svg)](https://github.com/new?template_owner=skills&template_name=change-commit-history&owner=%40me&name=skills-change-commit-history&description=My+copy+of+the+skills+course+on+changing+commit+history&visibility=public)

1. Right-click **Start course** and open the link in a new tab.
2. In the new tab, most of the prompts will automatically fill in for you.
   - For owner, choose your personal account or an organization to host the repository.
   - We recommend creating a public repository, as private repositories will [use Actions minutes](https://docs.github.com/en/billing/managing-billing-for-github-actions/about-billing-for-github-actions).
   - Scroll down and click the **Create repository** button at the bottom of the form.
3. After your new repository is created, wait about 20 seconds, then refresh the page. Follow the step-by-step instructions in the new repository's README.

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Post in our discussion board](https://github.com/orgs/skills/discussions/categories/change-commit-history) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2024 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

</footer>
