# Git and GitHub: A Guide to Version Control

This guide provides an overview of Git, a version control system, and how it can be used with GitHub.

## Table of Contents

  - [Terminology](#terminology)
    - [What is Git?](#what-is-git?)
    - [What is GitHub?](#what-is-github?)
  - [Version Control with Git](#version-control-with-git)
    - [Initializing a Git Repository](#initializing-a-git-repository)
    - [Cloning a Repository](#cloning-a-repository)
    - [Committing Changes](#committing-changes)
    - [Branching and Merging](#branching-and-merging)
  - [Collaboration with GitHub](#collaboration-with-github)
    - [Creating a Repository](#creating-a-repository)
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
GitHub is a cloud platform that not only stores code but also for collaboration. 

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
To begin, open up a terminal (Git Bash) and move to where you want to place the project on your local machine using the cd (change directory) command

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

### Staging Changes
Git allows you to stage changes before you commit them. This is useful for grouping related changes into a single commit:

```bash
git add -all                     # Add all modified files for commit
```

### Committing Changes
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

### Git Workflow

To ensure a smooth and efficient collaborative development process, it's important to follow best practices when working with Git. Here are some suggested guidelines:

- **Branching Strategy**: Adopt a branching strategy that suits your project and team. Common strategies include the Gitflow workflow, feature branches, or trunk-based development. Choose a strategy that promotes isolation, parallel development, and easy collaboration.

- **Commit Message Conventions**: Write clear and descriptive commit messages to provide meaningful context about the changes made. Consider using a consistent format, such as the [Conventional Commits](https://www.conventionalcommits.org/) format, which helps standardize commit messages and facilitates automated changelog generation.

- **Conflict Resolution**: When multiple team members are working on the same codebase, conflicts may arise during merges or pull requests. Encourage regular communication and coordination to minimize conflicts. In case of conflicts, use Git's built-in merge tools or popular third-party tools like KDiff3 or Beyond Compare to resolve conflicts efficiently.

- **Code Reviews**: Emphasize the importance of code reviews as part of the development process. Encourage team members to review each other's code, provide constructive feedback, and ensure adherence to coding standards and best practices. Code reviews help improve code quality, identify potential issues, and promote knowledge sharing among team members.

Remember, these are general best practices, and you can tailor them to your specific project and team requirements.

## Best Practices 
### Create a README file
To make it easier for people to understand and navigate your work, we recommend that you create a README file for every repository. You can add a README file to a repository to communicate important information about your project. 

Source: https://docs.github.com/en/repositories/creating-and-managing-repositories/best-practices-for-repositories
