# DevOps Project

## Build a Version-Controlled DevOps Project with Git

# DevOps Project

## Project Overview
This project is a hands-on implementation of a version-controlled DevOps workflow using Git and GitHub. It demonstrates best practices for repository management, branching strategies, pull requests, tagging, and documentation. 

The project serves as a foundational exercise for managing DevOps projects with version control.

---

## Table of Contents
1. [Project Objectives](#project-objectives)
2. [Technologies Used](#technologies-used)
3. [Repository Structure](#repository-structure)
4. [Branching Strategy](#branching-strategy)
5. [Implementation Steps](#implementation-steps)
6. [Key Features](#key-features)
7. [Usage Guide](#usage-guide)
8. [Task Documentation](#task-documentation)
9. [Versioning](#versioning)
10. [Contributing](#contributing)

---

## Project Objectives
- Manage a DevOps project using Git best practices.
- Implement branching strategies for efficient collaboration.
- Use pull requests for code reviews and merging.
- Document all tasks and processes in Markdown.
- Demonstrate versioning with Git tags.

---

## Technologies Used
- **Version Control**: Git
- **Remote Repository Hosting**: GitHub
- **Documentation**: Markdown


---

## Branching Strategy
- **main**: The production-ready branch. Contains stable code.
- **dev**: The development branch. Integrates all feature branches before merging into `main`.
- **feature/<feature-name>**: Branches for individual features or tasks.

---

## Implementation Steps

1. **Initialize the Repository**:
   - Create a local repository:
     ```bash
     mkdir devops-project
     cd devops-project
     git init
     ```
   - Create a `.gitignore` file and commit it:
     ```bash
     echo "node_modules/" >> .gitignore
     git add .gitignore
     git commit -m "Add .gitignore"
     ```

2. **Push to GitHub**:
   - Link the repository to GitHub:
     ```bash
     git remote add origin https://github.com/lokesh-matha/devops-project.git
     git branch -M main
     git push -u origin main
     ```

3. **Create Branches**:
   - Development branch:
     ```bash
     git checkout -b dev
     git push -u origin dev
     ```
   - Feature branches:
     ```bash
     git checkout -b feature/initial-setup
     git push -u origin feature/initial-setup
     ```

4. **Make Changes and Commit**:
   - Work on a feature branch and commit changes:
     ```bash
     echo "print('Hello, DevOps!')" > app.py
     git add app.py
     git commit -m "Add app.py with a basic script"
     ```

5. **Merge with Pull Requests**:
   - Open a pull request on GitHub to merge `feature/<feature-name>` into `dev`.
   - After approval, merge the branch and delete it.

6. **Tagging for Versioning**:
   - Add a version tag:
     ```bash
     git tag -a v1.0 -m "Initial version"
     git push origin v1.0
     ```

7. **Merge `dev` into `main`**:
   - Merge changes from `dev` to `main` after testing:
     ```bash
     git checkout main
     git merge dev
     git push
     ```

---

## Key Features
- **Branch Management**: Organized workflow with `main`, `dev`, and feature branches.
- **Pull Requests**: Ensure code reviews before merging.
- **Versioning**: Git tags for tracking releases.
- **Task Documentation**: Detailed progress tracking using Markdown.

---

## Usage Guide

### Clone the Repository
```bash
git clone https://github.com/lokesh-matha/devops-project.git
cd devops-project


## Work on a Feature

### Create a new branch
     ```bash
    git checkout -b feature/initial-setup

     ```
### Make changes to the code

     ```bash
    echo "print('Hello, DevOps!')" > app.py


     ```
### Add and commit changes
     ```bash
    git add .
    git commit -m "Implement initial-setup"

     ```
### Push the branch
     ```bash
  git push -u origin feature/<feature-name>


     ```
## Merge Changes

### Open a pull request
On GitHub, open a pull request to merge feature/<feature-name> into dev.

###Review and Test
Review the code and resolve any issues.
Merge the pull request into dev

###Merge dev into main
```bash
    git checkout main
    git merge dev
    git push
  ```
##Task Documentation
All tasks and progress are documented in docs/tasks.md. Example tasks include:

 Initialize the repository

 Create branching strategy

 Implement features

 Tag releases

##Versioning
Versioning is managed using Git tags to track stable releases:

v1.0: Initial setup with branching and basic configuration.

###To create a new version
  ```bash
      git tag -a v1.1 -m "Description of changes"
      git push origin v1.1
    ```
##Authors
Naga Lokesh Mathaa


