# Git and GitHub: A Guide to Version Control

This guide provides an overview of Git, a version control system, and how it can be used with GitHub.

## Table of Contents

  - [Terminology](#terminology)
    - [What is Git?](#what-is-git?)
    - [What is GitHub?](#what-is-github?)
  - [Version Control with Git](#version-control-with-git)
    - [Initializing a Git Repository](#initializing-a-git-repository)
    - [Cloning a Repository](#cloning-a-repository)
    - [Staging and Committing Changes](#staging-and-committing-changes)
    - [Branching and Merging](#branching-and-merging)
  - [Collaboration with GitHub](#collaboration-with-github)
    - [Forking a Repository](#forking-a-repository)
    - [Pull Requests](#pull-requests)
    - [Git Workflow](#git-workflow)
  - [Best Practices](#best-practices)
    - [Create a README file](#create-a-readme-file)

## Terminology

### What is Git?
Git is a version control system enables multiple team members to collaborate on a project. Key features of Git include:
- Tracking code changes 
- Keeping a record of who made the changes 
- Coding collaboration

### What is GitHub?
GitHub is a cloud platform for storing code and facilitating collaboration.

<p float='left'>
  <img src='/images/git_workflow.png' width='650' />
</p>

Source: [Course Report](https://www.coursereport.com/blog/what-is-github)

## Version Control with Git
<p float='left'>
  <img src='/images/git_basic_commands.png' width='600' />
</p>

Source: [Medium](https://medium.com/frontend-canteen/you-can-master-git-git-commands-with-these-diagrams-40a0b2f5cc42)


### Create a local Git Repository
To begin, open up a terminal (Git Bash) and navigate to where you want to place the project on your local machine using the cd (change directory) command: 
```bash
cd desktop                    # cd command changes directory
mkdir github_projects         # mkdir command creates directories
cd github_projects
```

### Cloning a Repository
To clone a remote repository to your local machine, use the following command:

```bash
git clone <repository_url>
```
Replace <repository_url> with the URL of the repository you want to clone.

### Staging and Committing Changes
Git allows you to stage changes before you commit them. This is useful for grouping related changes into a single commit:

```bash
git add -all                     # Add all modified files for commit
```

To save your changes in Git, you need to commit them:

```bash
git commit -m "Your descriptive commit message"
```
Remember to provide a descriptive commit message for each commit.

### Branching and Merging
Git allows you to create branches for parallel development and later merge them. Here are some essential commands:

<p float='left'>
  <img src='/images/git_branches.png' width='500' />
</p>

```bash
Copy code
git branch                      # List all branches
git branch <branch_name>        # Create a new branch
git checkout <branch_name>      # Switch to a branch
git merge <branch_name>         # Merge changes from a branch
```

## Collaboration with GitHub
### Creating a Repository
[Limiting team members who can create repositories. Empty repositories need to be created using Jenkins].

### Forking a Repository
Forking allows you to create a personal copy of someone else's repository. To fork a repository, follow these steps:
1) Open the repository you want to fork on GitHub.
2) Click the "Fork" button in the top-right corner.
3) Select your account to create a forked copy.


### Pull Requests
Pull requests enable collaboration and contribution to a repository. Here's a typical workflow:
1) Create a new branch for your changes.
2) Make your desired changes to the branch.
3) Commit and push the branch to your forked repository.
4) Open a pull request from your branch to the original repository.
5) Discuss and review the changes with other team members.
Once approved, the changes can be merged into the original repository.

## Best Practices 
### Naming Git Repositories
When naming your repositories, it's important to keep the names consistent, descriptive, and meaningful. To maintain uniformity and improve readability, follow these guidelines:

Use lowercase letters for all words in the repository name.
Separate words with underscores (_) to make the name easier to read.
The name should briefly reflect the repository's purpose or the project it contains. Avoid vague or overly generic names.

### Create a README file
To make it easier for people to understand and navigate your work, we recommend that you create a README file for every repository. You can add a README file to a repository to communicate important information about your project. 

Source: https://docs.github.com/en/repositories/creating-and-managing-repositories/best-practices-for-repositories

## Terminal Commands (ls, cd, mkdir, tab for autocompletion)
