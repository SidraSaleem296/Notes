# Week 5

### 🔐 **Access Control Mechanisms** (Chapter 6: Security Mechanism)

***

#### **📚 Learning Objectives**

1. Explore the **importance of access control** in information systems.
2. Understand **authentication factors** and firewall technology.
3. Discuss **remote access**, **content filtering**, and **Virtual Private Networks (VPNs)**.

***

#### **🛡️ Access Control Basics**

**Access Control**: Determines whether and how a user can enter a trusted area within an organization. This includes physical locations, information systems, and even restricted computer rooms.

**Types of Access Control**:

1. **Mandatory Access Control (MAC)**
2. **Non-discretionary Access Control**
3. **Discretionary Access Control (DAC)**

> **Analogy**: Think of access control as the **security checkpoints** at an airport ✈️. Only authorized individuals with valid credentials can pass.

***

#### **1. Mandatory Access Control (MAC)**

* **Definition**: Access is controlled by the **system based on data classification**.
* Users have limited control and are granted access based on **sensitivity levels**.

> **Analogy**: MAC is like a **VIP list** 📝 for data—only those with the right "security clearance" can access certain information.

**Lattice-Based Access Control**:

* Uses a **matrix of authorizations**.
* **Subjects** (users) and **objects** (resources) are assigned levels.
* Two key components:
  * **Access Control List (ACL)**: Defines which users can access a resource.
  * **Capabilities Table**: Shows access rights assigned to each user.

***

#### **2. Non-Discretionary Access Control**

* **Managed by central authority** and often linked to the user’s role or responsibilities.
* **Role-Based Control**: Access tied to the user’s organizational role.
* **Task-Based Control**: Based on specific assignments or duties.

> **Analogy**: This is like having different levels of clearance in an organization—only managers can access certain files 🗄️.

***

#### **3. Discretionary Access Control (DAC)**

* **User-controlled access**; individual users decide who can access information.

> **Example**: A file owner on a shared drive can specify who else can access it.

***

#### **Key Access Control Mechanisms**

1. **Identification** 🆔: Recognizing a user by a unique identifier (e.g., username).
2. **Authentication** 🔑: Verifying the user’s identity using one of three factors:
   * **Something you know** (passwords, PINs)
   * **Something you have** (ID cards, tokens)
   * **Something you are** (fingerprints, iris scans)
3. **Authorization** 📝: Determining what a user is allowed to access.
4. **Accountability** 📜: Ensuring that all actions are traceable to a user (often via logs).

> **Analogy**: This is similar to logging in to a bank account—identification is your **username**, authentication is your **password**, and authorization determines which accounts you can see.

***

#### **🔥 Firewalls**

**Definition**: A firewall is a security mechanism that prevents unauthorized access by controlling the movement of data between trusted and untrusted networks.

**Categories of Firewalls**:

1. **Packet-Filtering Firewalls**
2. **Application Gateways** (Proxy Servers)
3. **Circuit Gateways**
4. **MAC Layer Firewalls**
5. **Hybrid Firewalls**

**Firewall Processing Modes**:

1. **Packet Filtering**: Checks data packet headers to determine if data can pass.
2. **Application Gateways**: Acts as a proxy for specific applications.
3. **Circuit Gateways**: Creates tunnels for specific data.
4. **MAC Layer Firewalls**: Uses NIC addresses to filter traffic.

***

#### **Packet-Filtering Firewalls**

* **Function**: Examines data packet headers to decide whether to allow or deny passage based on IP addresses and port numbers.

> **Analogy**: Packet filtering is like a **bouncer at a club** who checks IDs before allowing entry 🚷.

#### **Application Gateways**

* **Function**: Acts as a **proxy server** by intercepting user requests and forwarding them to the appropriate destination.

> **Example**: A web proxy server that restricts access to certain sites.

***

#### **VPNs (Virtual Private Networks)**

**Definition**: VPNs provide secure connections over an unsecured public network by encrypting data.

**Types of VPNs**:

1. **Trusted VPN**: Uses leased circuits from service providers.
2. **Secure VPN**: Encrypts traffic over public networks.
3. **Hybrid VPN**: Combines both trusted and secure approaches.

**Modes of VPN**:

1. **Transport Mode**: Encrypts data within an IP packet but leaves header information open.
2. **Tunnel Mode**: Encrypts the entire packet, making the destination unknown to outsiders.

> **Analogy**: VPNs are like a **secure tunnel** 🛤️—all data is hidden as it travels across public networks.

***

#### **Content Filtering**

* **Function**: Restricts access to specific content types, websites, or protocols.

> **Example**: A company might use content filtering to block social media access during work hours.

***

### **📝 Exam Questions**

#### **Definition and Explanation**

1. **What is access control, and why is it important?**
2. **Explain the three primary types of access control (MAC, Non-discretionary, DAC).**

#### **Comparison and Differences**

1. **Compare MAC and DAC.** (Highlight the difference in control over access)
2. **Differentiate between Packet Filtering and Application Gateways in firewall categories.**

#### **Application and Scenario-Based**

1. **Describe a situation where a VPN would be necessary for secure communication.**
2. **Which type of firewall would best suit a small business and why?**

#### **Technical Process Questions**

1. **List the four main mechanisms of access control and explain each.**
2. **Explain the three types of VPNs and when each would be most appropriate.**
