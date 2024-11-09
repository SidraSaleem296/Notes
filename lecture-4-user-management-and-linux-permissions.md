# 📘 Lecture 4: User Management and Linux Permissions

#### 📌 Topics of Lecture

1. **User Management**: Creating, modifying, and deleting user accounts and groups.
2. **Linux File System Access Permissions**: Types, chmod, chown, and a case study on permissions.

***

#### 👤 User Management

**➕ Creating Users and Groups**

1. **Add User**:
   * `adduser`: Friendly utility for adding users.
   * `useradd`: Low-level utility for adding users.
   *   **Syntax**:

       ```bash
       bashCopy codesudo adduser [options] username
       sudo useradd [options] username
       ```
2. **Add Group**:
   * `addgroup`: Friendly utility for adding groups.
   * `groupadd`: Low-level utility for adding groups.
   *   **Syntax**:

       ```bash
       bashCopy codesudo addgroup [options] groupname
       sudo groupadd [options] groupname
       ```

**➖ Deleting Users and Groups**

1. **Delete User**:
   * `deluser`: Removes a user from the system.
   * `userdel`: Low-level command for user deletion.
   *   **Syntax**:

       ```bash
       bashCopy codesudo deluser [options] username
       sudo userdel [options] username
       ```
2. **Delete Group**:
   * `delgroup`: Removes a group from the system.
   * `groupdel`: Low-level command for group deletion.
   *   **Syntax**:

       ```bash
       bashCopy codesudo delgroup [options] groupname
       sudo groupdel [options] groupname
       ```

**✏️ Modifying Users and Groups**

* **Modify User** (`usermod`): Adjusts settings like username, password, home directory, and default shell.
  *   **Syntax**:

      ```bash
      bashCopy codesudo usermod [options] username
      ```
* **Add/Remove User from Group**:
  *   Add to group:

      ```bash
      bashCopy codesudo usermod -a -G groupname username
      ```
  *   Remove from group:

      ```bash
      bashCopy codesudo gpasswd -d username groupname
      ```

**🔄 Switching Users**

* **su** (Switch User): Allows switching to another user with their password.
  *   **Syntax**:

      ```bash
      bashCopy codesu [options] username
      ```

**💡 Exam Questions:**

1. Describe the purpose and syntax of the `useradd` and `groupadd` commands.
2. Explain how to add a user to a group and remove a user from a group.
3. What is the `su` command, and when would you use it?

***

#### 🔒 Linux File System Access Permissions

**🗝️ Types of Permissions**

1. **User (u)**: Owner of the file or directory.
2. **Group (g)**: Group of users with shared permissions.
3. **Others (o)**: All other users.

**🔓 Permission Levels**

1. **Read (r)**:
   * **Files**: Allows reading content.
   * **Directories**: Allows listing files within.
2. **Write (w)**:
   * **Files**: Allows modifying content.
   * **Directories**: Allows adding or deleting files.
3. **Execute (x)**:
   * **Files**: Allows running a program.
   * **Directories**: Allows entering the directory.

**📜 Linux Permission String**

* Permission string format: **10 characters**
  * 1st character: File type
  * Next 9 characters: Permissions (user, group, others)

**🔄 Changing Permissions (chmod)**

* **chmod**: Alters permissions for files or directories.
  *   **Syntax**:

      ```bash
      bashCopy codechmod [permissions] filename
      chmod -R [permissions] directoryname
      ```

**👤 Changing Ownership (chown)**

* **chown**: Modifies file ownership or group association.
  *   **Syntax**:

      ```bash
      bashCopy codechown [user:group] filename
      chown -R [user:group] directoryname
      ```

**💡 Exam Questions:**

1. Explain the three types of users in Linux permissions and their access levels.
2. What is the purpose of the `chmod` command? Provide an example.
3. How does the `chown` command differ from `chmod`?

***

#### 📝 Case Study: User Management and Linux Permissions

**Scenario**: Suppose a software project team has four roles:

* **Team Lead (1)**: Read/execute permissions only.
* **Developers (2)**: Group-readable/writeable/executable permissions.
* **Code Reviewers (2)**: Read/execute permissions only.
* **Code Testers (2)**: Read/execute permissions only.

**Required Permissions**:

* Team Lead: Limited to read and execute.
* Developers: Full group permissions.
* Reviewers and Testers: Limited to read and execute.

**💡 Exam Questions:**

1. How would you set up permissions for a team with varying roles on a Linux project?
2. Describe how you would configure permissions to ensure only developers can write files.
