# 📘 Lecture 8: Git and Version Control System

#### 📌 Topics of Lecture

1. **Version Control Systems (VCS)**
2. **Git Basics and Terminologies**
3. **Branching and Merging**
4. **Git Commands and Practice**

***

#### 🗂️ Version Control System (VCS)

* **Version Control System (VCS)**: Software that helps developers track and manage changes in source code over time, facilitating collaboration.
* **Types**:
  1. **Centralized Version Control System (CVCS)**:
     * Stores files on a central server, allowing team collaboration.
     * Drawback: If the server fails, collaboration halts.
     * Examples: CVS, Perforce, SVN.
  2. **Distributed Version Control System (DVCS)**:
     * Every client has a full mirror of the repository.
     * Offline operations possible, with syncing only needed for publishing changes.
     * Example: **Git**.

**💡 Exam Questions**:

1. Explain the difference between CVCS and DVCS with examples.
2. What are the limitations of a centralized version control system?

***

#### 🐙 Git: Overview and Terminologies

* **Git**: A free, open-source distributed version control system created by Linus Torvalds in 2005.
* Git tracks changes, enabling collaboration without needing a network or central server.

**Key Git Terminologies**

1. **Local/Remote Repository**:
   * Local repositories reside on a personal machine.
   * Remote repositories are accessible to the entire team.
2. **Working Directory**: The files currently being worked on.
3. **Staging Area**: Temporary area where changes are staged before committing.
4. **Commit**: Captures the project’s state at a specific time.
5. **Branch**: Creates a new line of development to work on features independently.

**💡 Exam Questions**:

1. Define the purpose of a staging area in Git.
2. What is a commit in Git, and why is it important?

***

#### 🖥️ Git Commands

* **Initialize a Repository**: `git init`
* **Add Files to Staging**: `git add <file>`
* **Check Status**: `git status`
* **Commit Changes**: `git commit -m "message"`
* **Push Changes**: `git push`
* **Pull Changes**: `git pull`
* **Clone Repository**: `git clone <repo-url>`

**Additional Commands**

*   **View Commit Log**:

    ```bash
    bashCopy codegit log
    git log --oneline  # Condensed history
    ```

**💡 Exam Questions**:

1. Write the commands for initializing a Git repository and adding a file to the staging area.
2. How can you view a one-line summary of your commit history?

***

#### 🌿 Branching and Merging

* **Branching**: Enables developers to work on copies of the code independently.
  * Master branch: Typically the stable version.
  * Feature branches allow experimentation without affecting the main code.
* **Managing Branches**:
  * View branches: `git branch`
  * Create new branch: `git branch [branch-name]`
  * Switch branch: `git checkout [branch-name]`
  * Delete branch: `git branch -D [branch-name]`
  * Rename branch: `git branch -m [old_name] [new_name]`
* **Merging**:
  * Switch to the main branch, then use `git merge [branch-name]` to integrate changes from another branch.

**💡 Exam Questions**:

1. Explain the purpose of branching in Git.
2. Describe the steps to merge a feature branch into the main branch.

***

#### 🔄 Resetting and Reverting

* **git reset**: Moves the repository back to a previous commit, discarding later changes.
  *   Example:

      ```bash
      bashCopy codegit reset [commit_ID]
      ```
* **git revert**: Adds a new commit that undoes a previous one, keeping the log intact.
  *   Example:

      ```bash
      bashCopy codegit revert [commit_ID]
      ```

**💡 Exam Questions**:

1. What is the difference between `git reset` and `git revert`?
2. When would you use `git revert` instead of `git reset`?

***

#### 🔄 Git Practice

1. **Branch Creation and Merging**:
   * Create a new branch from the master.
   * Commit files to the branch.
   * Merge changes back to the master.
2. **Commit, Reset, and Revert Practice**:
   * Create a series of commits.
   * Perform reset and revert actions to understand their impact on commit history.

**💡 Exam Questions**:

1. How can you check the status of a repository after creating a branch?
2. Describe a scenario where resetting to a previous commit might be necessary.
