# 📘 Lecture 7: DevOps and CI/CD Pipeline

#### 📌 Topics of Lecture

1. **DevOps Basics**: Definition, History, and Architecture
2. **DevOps Components**: Key Steps from Planning to Monitoring
3. **CI/CD Concepts**: Continuous Integration, Delivery, and Deployment
4. **Jenkins**: Installation, Configuration, and Pipeline Setup

***

#### 🌐 DevOps Overview

* **DevOps** combines **practices, tools, and a cultural philosophy** to automate and integrate processes between software development and IT teams.
* It fosters collaboration between development, QA, and operations to achieve continuous integration and deployment (CI/CD).

**Key Benefits**:

1. Faster product releases.
2. Enhanced responsiveness to customer needs.
3. Better team collaboration and productivity.

**💡 Exam Questions**:

1. Explain the role of DevOps in modern software development.
2. List three main advantages of adopting DevOps practices.

***

#### 📜 History of DevOps

* **2009**: John Allspaw and Paul Hammond presented "10 Deploys a Day" at Velocity conference.
* **DevOps Days**: First DevOps conference held in Ghent, Belgium.
* **2012**: Alanna Brown published the first **State of DevOps** report at Puppet Labs.

**💡 Exam Questions**:

1. Describe the origin of DevOps and its early influence on software development.
2. What was the significance of the "10 Deploys a Day" presentation?

***

#### 🧩 DevOps Components

1. **Plan**: Using Agile methodology to sync operations and development, ensuring organized workflows.
2. **Code**: Organizes code in files/folders using tools like Git.
3. **Build**: Transforms source code into executable binaries, checking quality before committing.
4. **Test**: QA team uses automation tools to test code, with bug fixes sent back to engineering.
5. **Release**: Manages deployment of new features and fixes efficiently.
6. **Deploy**: Deployment tools (e.g., Docker) retrieve and prepare code for use.
7. **Operate**: Both teams collaborate to configure servers and manage the lifecycle.
8. **Monitor**: Tools like **Splunk** and **Nagios** track system health and detect risks.

**💡 Exam Questions**:

1. List and explain three core components of DevOps.
2. How does the testing phase in DevOps differ from traditional methods?

***

#### 🔄 CI/CD Concepts

1. **Continuous Integration (CI)**: Developers regularly merge code to a central repository with automated builds and tests.
2. **Continuous Delivery (CD)**: Ensures code changes are always ready for production deployment.
3. **Continuous Deployment**: Automates the release of code changes directly to production after successful tests.

**💡 Exam Questions**:

1. Explain the differences between Continuous Integration, Delivery, and Deployment.
2. What is the main benefit of Continuous Deployment in DevOps?

***

#### 🔧 Jenkins: Installation and Configuration

* **Jenkins** is an open-source automation tool for continuous integration and deployment, offering plugins for building, testing, and deploying projects.

**Jenkins Release Types**:

1. **Long Term Support (LTS)**: Stable releases available every 12 weeks.
2. **Weekly Release**: Released weekly with bug fixes, primarily for developers.

**Jenkins Installation** (on Amazon EC2):

1.  Install Java Runtime Environment (JRE).

    ```bash
    bashCopy codesudo apt update
    sudo apt install openjdk-17-jre
    ```
2. Follow Jenkins installation steps on [Jenkins official site](https://www.jenkins.io).

**💡 Exam Questions**:

1. Describe the two types of Jenkins releases.
2. Outline the steps for installing Jenkins on an Amazon EC2 instance.

***

#### 📈 Creating Jobs and Pipelines in Jenkins

1. **Freestyle Project**: Standard Jenkins project, customizable for any build or task.
2. **Pipeline**: Complex workflows with dependencies, ideal for CI/CD processes.

**Basic Pipeline Steps:**

1. **Code**: Integrate with Git for code management.
2. **Build**: Compile source code.
3. **Test**: Automate testing to ensure quality.
4. **Deploy**: Deploy the build on servers or containers.

**Jenkins Integration with GitHub**:

* Use Git Webhooks, Poll SCM, or Scheduled Builds for automatic triggers.

**💡 Exam Questions**:

1. Explain the difference between a Freestyle Project and a Pipeline in Jenkins.
2. Describe two ways to trigger Jenkins builds using GitHub.

***

#### 🧩 Jenkins Pipeline Setup Example

1. Create three jobs in Jenkins (**f1**, **f2**, **f3**) with the following steps:
   * **Job f1**: Link to GitHub, configure SCM poll every minute, add shell command for `python3 f1.py`, and trigger **f2** post-build.
   * **Job f2**: Similar setup with `python3 f2.py` and trigger **f3** post-build.
   * **Job f3**: Executes `python3 f3.py`.
2. **Pipeline View**:
   * Install **Build Pipeline Plugin** to visualize job flow and dependencies.

**💡 Exam Questions**:

1. How do you configure Jenkins to automatically trigger a pipeline job sequence?
2. What is the purpose of using the Build Pipeline Plugin in Jenkins?
