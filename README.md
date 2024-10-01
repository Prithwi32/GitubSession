# Contributing to Open Source Projects using Git

Welcome to our project! We're excited that you're considering contributing to open-source development. This guide will walk you through the essential Git commands and best practices to make your contribution easy and successful.

## Table of Contents
1. [Forking the Repository](#forking-the-repository)
2. [Cloning the Repository](#cloning-the-repository)
3. [Creating a Branch](#creating-a-branch)
4. [Making Changes](#making-changes)
5. [Committing Changes](#committing-changes)
6. [Pushing Changes](#pushing-changes)
7. [Creating a Pull Request](#creating-a-pull-request)
8. [Syncing Your Fork](#syncing-your-fork)
9. [Tips for Writing Good Commit Messages](#tips-for-writing-good-commit-messages)

---

## 1. Forking the Repository

Before you start contributing, you need to fork the repository. Forking creates a copy of the repository under your own GitHub account.

Steps:
1. Navigate to the repository page.
2. Click the "Fork" button at the top-right corner.
3. You'll now have a copy of the repository in your GitHub account.

---

## 2. Cloning the Repository

After forking the repository, you need to clone it to your local machine so you can work on it.

```bash
git clone https://github.com/your-username/repository-name.git
```

---

## 3. Creating a Branch
After cloning the repository, create a new branch to work on your changes. Always work in a separate branch to avoid conflicts with the main branch:

```bash
git checkout -b feature/your-branch-name
```

---


## 4. Making Changes
Now that you're in your branch, make the necessary changes to the code, documentation, or other parts of the project. Be sure to test everything before moving on to the next step.


---

## 5. Committing Changes
Once your changes are complete, it's time to commit them. Follow these steps:

1. Add the changes to the staging area:

```bash
git add .
```
2. Commit the changes with a clear and descriptive message:

```bash

git commit -m "Your descriptive message here"
 ```

3. Make sure your commit message clearly explains the changes you made.

## 6. Pushing Changes
After committing your changes locally, push the branch to your GitHub repository.

```bash

git push origin feature/your-branch-name
```
This will upload your branch to your forked repository on GitHub.

## 7. Creating a Pull Request
With your changes pushed to GitHub, you're ready to submit a pull request (PR) so the maintainers can review your work.

* Navigate to your forked repository on GitHub.<br>
* Click the "Compare & pull request" button.<br>
* Provide a title and a detailed description of your changes.<br>
* Submit the pull request.<br>
* After reviewing, the maintainers will either merge your PR or provide feedback for revisions.<br>

## 8. Syncing Your Fork
If the original repository is updated while you're working, you might want to sync your fork to keep it up-to-date. Here's how:

1. Add the upstream repository as a remote:

```bash
git remote add upstream https://github.com/original-owner/repository-name.git
```
2. Fetch the latest changes from the upstream repository:

```bash
git fetch upstream
```
3. Merge the upstream changes into your local main branch:

```bash
git checkout main
git merge upstream/main
```
4. Push the updated main branch to your fork:

```bash
git push origin main
```

## 9. Tips for Writing Good Commit Messages
* Keep it concise: Aim for a commit message that's under 50 characters.<br>
* Use the imperative mood: For example, write "Fix bug" instead of "Fixed bug."<br>
* Provide context: Include the issue number or describe the purpose of the change. <br>Example: Fix #42 - Resolve bug in user authentication.




