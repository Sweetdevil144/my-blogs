---
title: "Automate Your Git Workflow with this Simple Bash Script"
datePublished: Thu Aug 17 2023 16:31:12 GMT+0000 (Coordinated Universal Time)
cuid: cllfdp2w2000509mt9wdvbssb
slug: automate-your-git-workflow-with-this-simple-bash-script
canonical: https://dev.to/sweetdevil144/automate-your-git-workflow-with-this-simple-bash-script-5cm5
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1692289778674/7772d948-ece1-4689-b2b7-5f4c02434ccc.jpeg
tags: productivity, programming-blogs, bash, git, beginners

---

The github repository for this script -> [Script](https://github.com/Sweetdevil144/git-automation.git)

Hey there fellow coders! 🚀

Ever found yourself doing the same repetitive git commands every time you want to push some changes? I know, it can be a bit annoying. But guess what? Bash scripts to the rescue! I know how you feel if you are remembering the repetative push and commits while reading these lines. Simply put, we have all been there. So, I decided that why not make a script of our own. From then on, I whipped up a neat little script that does the heavy lifting for you. Let's dive right in!

## What Does This Script Do? 🤔

This script aims to automate three core git actions:
1. Switching to the branch you specify.
2. Checking if there are any changes to commit.
3. Committing those changes with a message you provide and pushing to the specified branch.

Sounds fun, right?

## Breaking Down The Code 🛠

```bash
#!/bin/bash
```
The shebang! This tells the system that our script should run with the Bash shell.

Now, the script first checks if you've given it the required inputs: a branch name and a commit message.
```bash
if [ "$#" -ne 2 ]; then
  echo "Usage: $0 <branch_name> <commit_message>"
  exit 1
fi
```

The magic `$#` gives us the count of arguments you've passed in. If it's not two, the script will remind you how to use it.

```bash
branch_name="$1"
commit_message="$2"
```
Here we're just storing the arguments in nicely named variables to make things clearer later.

Now, let’s define our helper functions:

**1. `check_changes()`**: This checks if there are any changes to commit. If there aren't, it'll let you know and end the script.

```bash
check_changes() {
  if [ -z "$(git status --porcelain)" ]; then
    echo "No changes to commit."
    exit 0
  fi
}
```

**2. `commit_and_push()`**: It does exactly what the name says. First, it stages all changes. Then, it commits with the message you provided. Lastly, it pushes to the branch.

```bash
commit_and_push() {
  git add .
  git commit -m "$commit_message"
  git push origin "$branch_name"
}
```

Alrighty, the main show! 🎪

The script first checks if you're inside a Git repository.
```bash
if ! git rev-parse --is-inside-work-tree >/dev/null 2>&1; then
  echo "Error: Current directory is not a Git repository."
  exit 1
fi
```

If you are, it switches to the branch you mentioned:
```bash
git checkout "$branch_name"
```

Then, our good friend `check_changes` checks if there are any... well, changes.

And finally, `commit_and_push` comes into play and, well, commits and pushes the changes.

## How Do I Use This Script? 🚀

Clone the given Github repository and navigate into the script directory. To use it:

1. Make it executable: `chmod +x git-auto.sh`
2. Run the script: `./git_commit_and_push.sh <your-branch-name> "Your commit message over here"`

Voila! Less hassle, more coding! 🎉

## Wrapping Up

This script is a neat way to save some keystrokes and automate repetitive git actions. Feel free to expand upon it or tailor it to better fit your workflow. Happy coding, and may the force of automation be with you! 🤓

*P.S. Always remember to have backups and test new scripts in a safe environment before using them on critical projects!*