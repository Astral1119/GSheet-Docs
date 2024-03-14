---
title: Contributing
tags: 
dg-publish: true
dg-permalink: contribute
---
# Quickstart
Start by [forking the main repository](https://github.com/Astral1119/GSheet-Docs/fork). Then, [clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) your fork onto your machine. Make sure to run [`git checkout`](https://git-scm.com/docs/git-checkout), like so:

```bash
git checkout -b new-branch-name
```

If you want to use [Obsidian](https://obsidian.md/), download the app onto your machine and open your cloned repository as a vault. You can freely use plugins or themes without modifying anything, as the Obsidian folder is in gitignore. You can then make whatever edits you wish. Please refer to the [[note guidelines]] while making edits.

Every so often, remember to [sync your fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork) and [git pull](https://github.com/git-guides/git-pull) to your machine. When you are done, run the following commands, making sure to replace the commit message and branch name:

```bash
git add .
git commit -m "My commit."
git push origin new-branch-name
```

[`git add`](https://github.com/git-guides/git-add) prepares your files for committing. [`git commit`](https://github.com/git-guides/git-commit) prepares changes to be recorded; you can think of it as taking a snapshot of the files you've added. You can replace the commit message with whatever you want. Finally, [`git push`](https://github.com/git-guides/git-push) sends all changes to your forked repository.

When you `git push`, it will ask for a username and password. Use your GitHub username as requested; however, you will not be able to just use your GitHub password—you will instead have to generate a personal access token. To do this, [create a personal access token](https://github.com/settings/personal-access-tokens/new). Set the name, expiration, and description to whatever you wish; then, set the repository access to `Only select repositories` and select your fork. Finally, under repository permissions, enable the `Contents` permission. This is the only permission you will need. Once you have generated your access token, simply copy/paste it as your password in the command line.

Alternatively, you can use the [git credential manager](https://github.com/git-ecosystem/git-credential-manager).

Once you've used `git push`, go to your fork. You should see an option to `Compare & pull request`. Select this option and follow the steps given. Your request will be reviewed and added if useful.