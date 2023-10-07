# Chapter 2

_**Chapter 2: Software Quality Factors (Attributes) 📊**_

_**Section 1:**_

**2.1 Complaints from the City Computer Club members – an introductory mini case** 🏢🖥️

The City Computer Club, established by municipal corporations and public services’ IT department managers, discussed the implementation experiences of its members in their organizations. Below is a transcription of part of the meeting, highlighting software quality issues:

🛒 **Sales Information System Fails:**

* "Our new sales information system seems okay. The invoices and inventory records are correct, the discounts granted to our clients follow our very complicated discount policy precisely, but our new sales information system frequently fails.
* Recently, it has been failing at least twice a day, and each time for at least twenty minutes. Yesterday, it took an hour and a half for us to get back to work.
* Softbest, the software house that developed our computerized sales system, does not accept responsibility."

📡 **RD-1 Firmware Challenges:**

* "Just a year ago, we launched our successful new product – RD-1, a police radar detector. The RD-1 firmware embedded in the product seemed to be the reason for its success.
* But, when we began planning the development of the European version of the product, RD-E1, we found out that the RD-1 firmware had only been partially documented, and the code, mostly written with no adherence to the company’s work instructions.
* Consequently, the development department had to develop a new firmware, as almost no parts of the RD-1 design and programming could be reused."

🏫 **Issues with "Blackboard" Software:**

* "Our software package for schoolteachers 'Blackboard', launched just three months ago, is already installed in 187 schools.
* The development team just returned from a week in Hawaii - their vacation bonus. But we have suddenly started to receive daily complaints from the 'Blackboard' maintenance team.
* They claim that the lack of failure detection features in the software, in addition to the poor programmer’s manual, have caused them to invest more time to deal with bugs and minor software changes than that agreed upon in the purchasing contracts with clients."

📜 **Loan Contract Software Training Challenges:**

* "The new version of our loan contract software is really accurate. We have already processed 1,200 customer requests, and checked each of the output contracts - no errors were found.
* But we did face a severe unexpected problem – training a new staff member to use this software takes about three weeks. This is a real problem in customer departments suffering from high employee turnover.
* The project team claims that as they were not required to include software user training as a requirement to be considered during the software development period, an additional two to three months of work will be required to solve the problem."

🔍 There are a number of characteristics common to all these "buts":

* 📈 The software projects satisfactorily fulfilled the basic requirements to perform the correct calculations (correct inventory figures, correct average class scores, correct loan interests, etc.). Apparently, the software packages successfully fulfilled the correctness requirements.
* 🛠️ The software projects suffered from poor performance in important areas such as software maintenance, software reliability, software reuse, and user training. Apparently, the software packages fail to fulfill the maintainability, training usability, reliability, and reusability requirements.
* 📝 The common cause for poor performance of the software projects developed in these areas was a lack in essential parts of the project requirements. These parts should have been designated to cover important aspects of software functionality.

These issues illustrate the critical importance of considering factors beyond correctness in software development to ensure overall software quality. 🚀





_**Section 2:**_

**2.2 The Need for Comprehensive Software Quality Requirements**

🧠 **Key Takeaways**:

* Comprehensive software quality requirements are essential to avoid issues faced by users, developers, and maintenance staff.
* Such requirements cover all aspects of software use throughout its life cycle.
* Fulfilling comprehensive requirements leads to increased user satisfaction and better efficiency for development and maintenance teams.
* Software quality requirements have multidimensional nature.
* Software quality factors are groups of attributes/characteristics defined in requirement documents.
* The emphasis on various quality factors may vary between software projects.
* This chapter will review a wide range of software quality factors.
* Various software quality models have been proposed over the years.
* These models include criteria/subfactors that should be measurable and support testing and quality measurement.

❓ **Questions and Confusions**:

**1. How do we ensure that all relevant quality factors are included in the requirements?**

* **Tip:** Conduct thorough stakeholder interviews and engage domain experts to gather insights into potential quality factors.
* Create a comprehensive checklist of common quality factors to ensure none are overlooked.
* Use established software quality models as references (e.g., ISO/IEC 25010, McCall's model) to guide your requirements gathering process.

**2. Can you provide an example of a real-world situation where missing requirements caused issues?**

* **Example:** Consider a banking application that lacks a requirement for proper error handling. If a user enters incorrect information during a funds transfer, and the system doesn't provide clear error messages or fail gracefully, it can result in user frustration, financial errors, and a poor user experience.

**3. What are some common software quality factors that are often overlooked?**

* **Commonly Overlooked Factors:** Usability, scalability, compatibility with different devices/browsers, security, and performance under load are often overlooked but crucial quality factors.

**4. Are there any practical tips for creating comprehensive software quality requirements?**

* **Practical Tips:**
  * Involve stakeholders early and continuously gather feedback to ensure requirements are aligned with their needs.
  * Use user stories or use cases to capture real-world scenarios and context for quality requirements.
  * Prioritize requirements based on their impact and importance to the project.
  * Collaborate with developers and QA teams to ensure that requirements are feasible and testable.
  * Document requirements clearly, using a standardized format, and include acceptance criteria.
  * Consider both functional and non-functional (performance, security, usability) requirements.
  * Keep requirements up-to-date throughout the project's lifecycle as changes occur.
  * Conduct regular reviews and validations of requirements with the project team and stakeholders.



_**Section 3:**_

**2.3 McCall’s classic model for software quality factors**

Several models of software quality factors and their classification to factor categories have been suggested over the years. The classic model of software quality factors, suggested by McCall, consists of 11 factors (McCall et al. 1977). The McCall factor model, despite decades of “maturation,” continues to provide a practical, up-to-date method for classifying software quality requirements. Subsequent alternative models and factors, additional to McCall’s factors, will be discussed later in this chapter.

**McCall’s factor model classifies all software requirements into 11 software quality factors.** The 11 factors are grouped into three categories: product operation, product revision, and product transition. McCall’s software quality model is presented below:

🌟 **McCall’s software quality factors model**

_Product operation factors_:

* ✅ **Correctness**
* 🔄 **Reliability**
* ⚡ **Efficiency**
* 🔒 **Integrity**
* 🎯 **Usability**

_Product revision factors_:

* 🧰 **Maintainability**
* 🧩 **Flexibility**
* 🔍 **Testability**

_Product transition factors_:

* 🌐 **Portability**
* 🔄 **Reusability**
* 🤝 **Interoperability**

McCall’s model and its categories are illustrated in McCall’s model of software quality factors tree:

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

![McCall’s software quality factor model tree](https://chat.openai.com/c/Image\_Link\_Here)

The next three sections are dedicated to a detailed description of the software quality factors included in each of McCall’s categories.

**2.3.1 McCall’s product operation software quality factors**

According to McCall’s model, five software quality factors are included in the product operation category, all of which deal with requirements that directly affect the daily operation of the software. 🚀

✅ **Correctness** Correctness requirements are related to the outputs of software systems, such as a query display of a customer’s balance in the sales accounting information system or the air supply as a function of temperature specified by the firmware of an industrial control unit. A specification is required for each output (system function). This output specification is usually multidimensional; some common dimensions are:

* The required accuracy of the output.
* The required completeness of the output information.
* The required up-to-datedness of information.
* The required response time.
* The standards for coding and documenting the software system.

🔄 **Reliability** Reliability requirements deal with failures to provide service. They determine the maximum allowed software system failure rate, the maximum allowed percentage of a software system’s downtime, and the maximum allowed recovery times. The requirements can refer to the entire system or to one or more of its separate functions.

_Examples_:

1. The failure frequency of a heart-monitoring unit operating in a hospital’s intensive care ward is required to be less than one in 20 years.
2. One requirement of the new software system to be installed in the main branch of the Independence Bank, which operates 120 branches, is that on average, it will not fail more than 1 time per 12 months during the bank’s office hours.

⚡ **Efficiency** Efficiency requirements deal with the hardware resources needed to perform all the functions of the software system in conformance with all other requirements. The main hardware resources to be considered are the computer’s processing capabilities (measured in Million Instructions Per Second (MIPS), megahertz – million cycles per second, etc.), its data storage capability in terms of memory and disk capacity (measured in gigabytes (GBs), terabytes (TBs), etc.), and the data communication capability of the communication lines (usually measured in megabits per second (MBPSs), and gigabits per second (GBPSs)).

_Examples_:

1. A chain of stores is considering two alternative bids for a software system. Bid B is more efficient than Bid A because fewer hardware resources are required.
2. An outdoor meteorological unit. The system performs measurements once per hour, logs the results, and transmits the results once a day to the meteorological center by means of wireless communication. The unit is equipped with a 1,000 milliampere hour cell, which is capable of supplying the power requirements of the unit for at least 30 days. An alternative meteorological unit of higher efficiency is able to cope with all the requirements with a 500 milliampere unit.

🔒 **Integrity** Integrity requirements deal with the software system security, that is, requirements to prevent unauthorized access, to distinguish between the majority of personnel only allowed to see the information (read-only permit), and a limited group who will be allowed to add and change data (write permit), and so forth. Integrity requirements are defined to cope with risks of “nonfriendly” unauthorized attempts to damage the software system and its performance.

_Example_: The Engineering Department of a local municipality operates a geographic information system (GIS). The department is planning to allow citizens access to its GIS files through the Internet. The software requirements include "read-only" access and limited access to certain maps.

🎯 **Usability** Usability requirements deal with the scope of staff resources needed to train a new employee and to operate the software system. The usability requirements relate to the (a) operation usability, the productivity of the user, that is, the average number of transactions performed per hour, and (b) training usability, the average time spent training a new employee.

_Example_: The software usability requirements for the new help desk system initiated by a home appliance manufacturing company specify that a staff member should be able to handle at least 60 service calls a day, and training a new employee will take no more than 2 days (16 training hours). At the end of training, the trainee will be able to handle 45 service calls a day. 📚



**2.3.2 Product Revision Software Quality Factors**

According to the McCall model of software quality factors, three quality factors comprise the product revision category. These factors deal with requirements that affect various software maintenance activities:

🔧 **Maintainability** Maintainability requirements determine the efforts needed by users and maintenance personnel to identify the reasons for a software failure, correct the failure, and verify the success of the correction. These requirements pertain to various aspects, including the modular structure of software, internal program documentation, and the programmer's manual, among other items.

_Example_: Typical maintainability requirements: (a) The size of a software module will not exceed 30 statements. (b) The programming will adhere to the company's coding standards and guidelines. 🛠️

🔄 **Flexibility** The flexibility factor deals with the capabilities and efforts required to support adaptive maintenance activities. It includes the resources (in man-days) needed to adapt a software package to different customers, varying extents of activities, and a different range of products within the same trade. Flexibility requirements also support perfective maintenance activities, such as changes and additions to the software to improve its service and adapt it to changes in the firm's technical or commercial environment.

_Example_: Teacher Support Software (TSS) is a software product designed for documentation of student achievements, calculation of final grades, printing of term grade statements, and automatic printing of warning letters to parents of failing pupils. Flexibility requirements for TSS include being suitable for teachers of all subjects and school levels (elementary, middle, and high school) and enabling nonprofessionals to create new types of reports according to schoolmaster's requirements or demands of the city's department of education. 📚

🧪 **Testability** Testability requirements deal with the testing process of a software system and its operation. Testability requirements for ease of testing may include special features in the programs that help testers, such as providing predefined intermediate results and log files. Testability requirements related to software operation involve automatic diagnostics performed by the software system before operating to check if all components are in working order and to obtain a report on detected faults. Another type of requirement deals with automatic diagnostic checks performed by maintenance technicians to detect the causes of software failures.

_Example_: An industrial computerized control unit is programmed to calculate production status measures, report machinery performance, and operate a warning signal in predefined situations. One testability requirement is to develop a set of standard test data, including the expected correct reactions of the system in each case. These standard test data are run every morning before production begins to verify that the computerized unit responds properly. 🧪



**2.3.3 Product Transition Software Quality Factors**

According to McCall, three quality factors are included in the product transition category, which pertains to the adaptation of software to other environments and its interaction with other software systems:

🌐 **Portability** Portability requirements are related to adapting a software system to different environments, including varying hardware and operating systems. These requirements enable the software product to be used in diverse situations and environments, widening its market and applicability.

_Example_: A software package initially designed for the Windows 2007 environment is required to allow for easy and cost-effective migration to Linux environments, ensuring compatibility across different platforms. 🖥️

🔄 **Reusability** Reusability requirements involve the two-directional use of software components. In one direction, it's about utilizing a software module or an entire application from an existing software product in a new software project under development. This can include software developed internally, open-source software, or purchased software. In the other direction, it pertains to developing software modules or entire projects in a way that enables their reuse in future projects. Reusable software is expected to be well-tested, with corrections made based on previous user experiences, resulting in resource and time savings and higher-quality software.

_Example_: A software development unit decides to design and program certain modules for a hotel swimming pool project in a way that allows their reuse in a future spa software system planned for development next year. This proactive reusability requirement includes modules for entrance checks, club member visit recording, restaurant billing, and membership renewal payments. ♻️

🔌 **Interoperability** Interoperability requirements focus on creating interfaces between a software system and other software systems or equipment firmware. These requirements specify how the software should interact with other systems or equipment, sometimes naming the specific software or firmware it needs to interface with. They may also dictate accepted standard output structures in specific industries or application areas.

_Example_: The firmware of medical laboratory equipment must process its results according to a standard data structure, allowing the output to be compatible with various medical laboratory information systems. Additionally, the laboratory information system is required to interface seamlessly with a medical clinic information system, automating the transmission of patients' test results to physicians' clinics. 🏥



_**Section 4:**_

**2.4 The ISO/IEC 25010 Model and Other Alternative Models**

📊 _Models of Software Quality Factors_

* Several quality factor models developed over decades:
  * Boehm's model (Boehm et al., 1978)
  * FURPS model (Grady and Caswell, 1987)
  * Evans and Marciniak's model (1987)
  * Deutsch and Willis's model (1988)
  * Dromey's model (1995)
  * GEOQUAMO model (Georgiadou, 2003)
  * ISO/IEC 25010:2011 (ISO/IEC, 2011)
  * AOSQUAMO model (Kumar, 2012)

🌐 _The ISO/IEC 25010 Model_

* Developed by ISO/IEC international professional team.
* Composed of 8 factors:
  1. 🌟 **Functional Suitability** - Accurate and complete results.
  2. 🚀 **Performance Efficiency** - Efficient resource usage.
  3. ♻️ **Compatibility** - Exchange and perform functions with other systems.
  4. 👤 **Usability** - User-friendliness.
  5. ⚙️ **Reliability** - Protection from unauthorized access.
  6. 🔒 **Security** - Data and system protection.
  7. 🧰 **Maintainability** - Easy modifications.
  8. 🌍 **Portability** - Adaptability to different environments.

🔄 _ISO/IEC 25010 vs. McCall's Model_

* ISO/IEC 25010 shares similarities with McCall's model, including correctness, integrity, and interoperability.

📈 _Standard Evolution_

* ISO/IEC 25010:2011 replaced ISO/IEC IS 9126-1:2001.
* Basis for software metrics in various domains.

📊 _Additional Software Quality Models_

* Alternative models propose 14 additional factors:
  1. ✔️ **Effectiveness**
  2. 🔄 **Evolvability**
  3. 📈 **Expandability**
  4. 🧩 **Extensibility**
  5. 🤖 **Human Engineering**
  6. 🧰 **Manageability**
  7. 🔨 **Modifiability**
  8. ⚡ **Productivity**
  9. ⚠️ **Safety**
  10. 😊 **Satisfaction**
  11. 🤝 **Supportability**
  12. 🛡️ **Survivability**
  13. 🤔 **Understandability**
  14. 🔍 **Verifiability**

🔍 _Additional Factors Explained_

* **Effectiveness**: Successful task completion.
* **Evolvability**: Adapting to future requirements.
* **Expandability**: Preparing for larger populations or applications.
* **Extensibility**: Meeting new requirements.
* **Human Engineering**: User interface and ease of use.
* **Manageability**: Administrative tools for software modifications.
* **Modifiability**: Efforts needed for customer-specific changes.
* **Productivity**: Task performance rate.
* **Safety**: Eliminating hazardous conditions.
* **Satisfaction**: User perception vs. requirements.
* **Supportability**: Ease of installation and maintenance.
* **Survivability**: Service continuity and recovery.
* **Understandability**: User capability and documentation.
* **Verifiability**: Efficient design verification.



_**Section 5:**_

**2.5 Understanding Software Compliance**

* Quality models require evaluating software development and maintenance processes and products.
* Goal: Assess how well these processes comply with quality factor requirements.
* Challenges: Gap between general attributes and explicit review questions, requiring quantitative measurement.

**🌉 Bridging the Gap: Explanatory Criteria**

* Solution: Add explanatory criteria (subfactors) for each quality factor.
* Criteria make each quality factor measurable and actionable.
* Combining quantitative and qualitative criteria.

**📊 Importance of Measurable Criteria**

* Criteria help:
  * Define software requirements.
  * Formulate review questions.
  * Prepare test plans.
  * Develop software metrics.
* Quantitative criteria assess software project compliance.
* Various authors propose criteria (e.g., Evans and Marciniak, Sharma et al., Al-Qutaish, Kumar).

**📋 Criteria Examples for McCall's Factors**

Table 2.1 McCall’s model factors and criteria (subfactors)

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

* Correctness
  * Accuracy
  * Completeness
  * Up-to-datedness
  * Availability (response time)
* Reliability
  * System and application reliability
  * Failure recovery
  * Hardware failure recovery
* Efficiency
  * Efficiency of processing
  * Efficiency of storage
  * Efficiency of communication
  * Efficiency of power usage (for portable units)
* Integrity
  * Access control
  * Access audit
* Usability
  * Operability
  * Learning and training ability
* Maintainability
  * Simplicity
  * Modularity
  * Self-descriptiveness
  * Coding and documentation guidelines compliance (consistency)
* Flexibility
  * Modularity
  * Generality
  * Simplicity
  * Self-descriptiveness
* Testability
  * Simplicity
  * Failure maintenance testability
  * Traceability
* Portability
  * Software system independence
  * Reusability
  * Coding and documentation guidelines compliance (consistency)
* Interoperability
  * Commonality
  * System compatibility
  * Software system independence
  * Modularity

**🌐 ISO/IEC 25010 Criteria**

Table 2.2 ISO/IEC 25010 product quality model factors and criteria (subfactors)

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

* Functional suitability
* Performance efficiency
* Compatibility
* Usability
* Reliability
* Availability
* Fault tolerance
* Recoverability
* Security
* Confidentiality
* Integrity
* Nonrepudiation
* Performance efficiency
* Time behavior
* Resource utilization
* Capacity
* Maintainability
* Modularity
* Coexistence
* Reusability
* Analyzability
* Usability
* Appropriateness recognizability
* Learnability
* User error protection
* User interface aesthetics
* Accessibility

**🌐 Criteria for Alternative Quality Models**

Table 2.3 Factors and criteria of Alternative quality models (For factors not included in McCall/s and ISO/IEC 25010 quality models)

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

🔗 Criteria often overlap and contribute to successful compliance across multiple factors, highlighting the interconnected nature of software quality factors.



_**Summary**_

1. 📜 **Comprehensive Requirements Documents**
   * Many cases of low customer satisfaction result from software projects meeting basic correctness requirements but lacking in areas like maintenance, reliability, software reuse, or training.
   * Lack of defined requirements in these aspects leads to lapses in software functionality.
   * Comprehensive requirement specifications covering all software use aspects throughout the lifecycle are essential.
   * Software quality models define various quality factors; requirement definitions should incorporate these factors.
2. 📊 **Structure of McCall’s Classic Factor Model**
   * McCall’s factor model categorizes all software requirements into 11 quality factors.
   * These factors are grouped into three categories: Product Operation, Product Revision, and Product Transition.
   * Product Operation Factors:
     * Correctness
     * Reliability
     * Efficiency
     * Integrity
     * Usability
   * Product Revision Factors:
     * Maintainability
     * Flexibility
     * Testability
   * Product Transition Factors:
     * Portability
     * Reusability
     * Interoperability
3. 🌐 **Quality Factors of ISO/IEC 25010:2011 Model**
   * Developed by a joint ISO/IEC international team, the ISO/IEC 25010:2011 model includes eight significant factors.
   * Four of these factors were also present in McCall's model:
     * Functional Suitability
     * Performance Efficiency
     * Compatibility
     * Usability
     * Reliability
     * Security
     * Maintainability
     * Portability
4. 🔄 **Additional Factors from Alternative Models**
   * Various alternative software quality models have been proposed, introducing 14 additional quality factors.
   * These factors often overlap with each other and McCall's factors.
5. 📋 **Software Compliance with Quality Factors**
   * The gap between general software quality factors and explicit specification requirements can be challenging.
   * Explanatory criteria for each factor bridge this gap.
   * Criteria help specify quality requirements, define review questions, prepare test plans, and develop software quality metrics.
   * They assess the degree of compliance with software quality factors in software projects.

🔍 Understanding and implementing software quality factors is essential for delivering high-quality software and ensuring customer satisfaction.



_**Review Questions**_

Sure, I'll incorporate emojis into the notes for each question and provide answers as well.

**2.1 Review Questions**

a. 🤔 **What are the three factor categories belonging to McCall’s factor model?**

* Answer: McCall's factor model consists of three factor categories: Product Operation, Product Revision, and Product Transition.

b. 📋 **Which factors are included in each of the categories?**

* Answer: Factors in each category are as follows:
  * Product Operation Factors:
    * Correctness
    * Reliability
    * Efficiency
    * Integrity
    * Usability
  * Product Revision Factors:
    * Maintainability
    * Flexibility
    * Testability
  * Product Transition Factors:
    * Portability
    * Reusability
    * Interoperability

**2.2 Software Requirement Specification**

For each section, fill in the name of the McCall’s factor that best fits the requirement.

1. 🚀 **The probability that the “Super-lab” software system will be \_\_\_\_\_\_ found in a state of failure during peak hours (9 am to 4 pm) is required to be below 0.5%.**
   * Factor: Reliability
2. 🔄 **The “Super-lab” software system will enable the direct \_\_\_\_\_\_ transfer of laboratory results to those files of hospitalized patients managed by the “MD-File” software package.**
   * Factor: Interoperability
3. ⏲️ **The “Super-lab” software system will include a module that \_\_\_\_\_\_ prepares a detailed report of the patient’s laboratory test results during the current hospitalization. The time required to obtain this printed report will be less than 60 seconds.**
   * Factor: Efficiency
4. 🔄 **The “Super-lab” software to be developed for hospital \_\_\_\_\_\_ laboratory use may be adapted later for private laboratory use.**
   * Factor: Reusability
5. 📚 **The training of a laboratory technician, requiring no more \_\_\_\_\_\_ than 3 days, will enable the technician to reach level C of “Super-lab” operator. This means that the trainee will be able to manage the reception of 20 patients per hour.**
   * Factor: Usability
6. 🕵️ **The “Super-lab” software system will record details of users \_\_\_\_\_\_ logging in. In addition, the system will report attempts by unauthorized persons to obtain medical information from the laboratory test results database. Reports will include detailed information about unauthorized attempts to access the database of “Super lab”.**
   * Factor: Security
7. 💰 **The “Super-lab” subsystem that deals with billing patients \_\_\_\_\_\_ for their tests may eventually be used as a subsystem in the “Physiotherapy Centre” software package.**
   * Factor: Reusability
8. 📊 **The “Super-lab” software system will process the monthly \_\_\_\_\_\_ reports of the hospital departments’ management, the hospital management, and the hospital controller, in accordance with Appendix D of the development contract (not attached).**
   * Factor: Correctness
9. ⚙️ **The software system should be able to serve 12 workstations \_\_\_\_\_\_ and 8 automatic testing machines with a single model AS20 server; and a CS25 communication server that will be able to serve 25 communication lines. The hardware system should conform to all availability requirements as listed in Appendix D.**
   * Factor: Efficiency
10. 🖥️ **The “Super-lab” software package developed for the Linux \_\_\_\_\_\_ operating system should be compatible with applications in the Windows NT environment.**

* Factor: Compatibility

**2.3 ISO/IEC 25010:2011 Model**

a. 📋 **List the factors included in the ISO/IEC model.**

* Answer: The factors in the ISO/IEC 25010:2011 model include:
  * Functional Suitability
  * Performance Efficiency
  * Compatibility
  * Usability
  * Reliability
  * Security
  * Maintainability
  * Portability

b. 🔄 **Discuss the similarity of the ISO/IEC model with McCall’s model.**

* Answer: The ISO/IEC 25010:2011 model shares significant similarities with McCall's model. Four factors from ISO/IEC 25010 (Functional Suitability, Usability, Reliability, and Maintainability) were also present in McCall's model, showing a continuation of fundamental quality considerations.

**2.4 Requirements for Control Unit**

a. ⚙️ **To which of McCall’s factors do the above requirements belong?**

* Answer: The requirements belong to the McCall's factor of "Reusability."

b. 🤔 **Explain your answer.**

* Explanation: The requirements mention adaptability for different variations of washing machine models and the use of the control module for a dishwasher model planned in the future. These requirements relate to reusability as they emphasize the potential for the control unit to be used in various contexts.

**2.5 Testability and Verifiability**

a. 🔄 **Do you agree that testability and verifiability are actually different terms for the same factor?**

* Answer: No, testability and verifiability are not the same factors.

b. 📋 **Explain your reasoning.**

* Explanation: Testability focuses on how easily a software system can be tested to ensure its correctness and performance. Verifiability, on the other hand, is about the ability to verify and validate that the software meets its requirements and specifications. While they are related, they address different aspects of software quality, with testability being more about practical testing, and verifiability focusing on overall verification and validation processes.



