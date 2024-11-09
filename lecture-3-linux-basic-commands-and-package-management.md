# 📘 Lecture 3: Linux Basic Commands and Package Management

#### 📌 Topics of Lecture

1. **Linux Basic Commands**: Creating folders, files, listing contents, editing, copying, moving, and deleting.
2. **Package Installation**: Using package managers like `apt`, `yum`, and `apt-get`.

***

#### 💻 Command Line Interface (CLI)

* The **Terminal** allows users to interact with the operating system by entering commands.
* Commands in CLI provide responses from the OS, enabling various tasks on Linux systems.

***

#### 📂 Linux Basic Commands

**🔍 Directory and File Management**

1. **pwd**: Shows the present working directory.
2. **ls**: Lists files/folders in the current directory.
3. **mkdir**: Creates a new directory.
4. **cd**: Changes the current directory.
5. **touch**: Creates a new empty file.
6. **cp**: Copies files/folders to another location.
7. **mv**: Moves files/folders to a new location.
8. **rm**: Deletes files/folders.

**✏️ Editing and Viewing Files**

1. **cat**: Displays the contents of a file.
2. **head**: Outputs the start of a file.
3. **tail**: Outputs the end of a file.
4. **echo**: Displays a line of text and can write it to a file.
5. **vi** and **nano**: Text editors to create/edit files directly in the terminal.

**📄 Other Useful Commands**

1. **whoami**: Prints the current username.
2. **find**: Searches for files in a directory hierarchy.
3. **sleep**: Delays execution for a specified time.
4. **dd**: Copies files with formatting.
5. **ping**: Sends an ICMP ECHO\_REQUEST to network hosts.
6. **wget**: Retrieves files via HTTP or FTP.
7. **hostname**: Gets or sets the system hostname.
8. **man**: Displays manual pages for commands (help).

**💡 Exam Questions:**

1. Describe the function of the `ls`, `cd`, and `mkdir` commands.
2. Explain how to create, move, and delete files in Linux.
3. What is the purpose of the `man` command in Linux?

***

#### 📦 Package Manager and Software Installation

* **Package Managers** automate the process of installing, upgrading, configuring, and removing software.
* Different Linux distributions use specific package managers:
  * **apt**: Advanced Package Tool (for Debian/Ubuntu)
  * **yum**: Yellowdog Updater, Modified (for CentOS/Red Hat)
  * **brew**: Used in macOS for software installation.

**📥 Common apt Commands**

1. **apt update**: Updates package information from all configured sources.
2. **apt upgrade**: Installs available upgrades of packages.
3. **apt install \[package-name]**: Installs a specified package (e.g., `apt install apache2`).
4. **apt remove \[package-name]**: Removes a package but keeps configuration files.
5. **apt purge \[package-name]**: Removes a package along with its configuration files.

**💡 Exam Questions:**

1. Differentiate between `apt` and `apt-get`.
2. What does the `apt update` command do, and why is it necessary before an upgrade?
3. How does `apt purge` differ from `apt remove`?
