# Software Product Quality Matrices

#### 📚 Software Product Quality Metrics 📊

**Motto**

* "You can’t control what you can’t measure." - Tom DeMarco (1962) 🎯

***

#### Objectives of Software Quality Metrics 🎯

**Monitoring and Control 📈**

* **Purpose**: Assist management in overseeing the development and maintenance of software systems.
* **Focus Areas**:
  * Observing software product conformance to functionality, regulations, and conventions.
  * Providing data for process improvement.

**Process Improvement 🔍**

* **Data Utilization**:
  * Identify low-performance areas needing enhancement.
  * Validate achievements of process improvement proposals.

**Date: December 24, 2023 🗓️**

***

#### Metrics' Required Characteristics 📝

<figure><img src=".gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

**Quality Metrics Characteristics ✨**

* **Essentials**:
  * Relevance
  * Validity
  * Reliability
  * Comprehensiveness
  * Mutual Exclusivity

**Implementation Characteristics 💡**

* **Key Aspects**:
  * Simplicity and ease of use.
  * No need for independent data collection.
  * Immunity to biased intervention by interested parties.



#### Implementation of Software Quality Metrics 💻

* **Extensive Research**: Numerous books, chapters, journals, and conference papers dedicated to software quality metrics.
* **Standard Framework**: Detailed in ISO/IEC Std. 9126 (2002–2004).
* **Key Focus Areas**:
  1. Implementation of Software Quality Metrics
  2. Product Metrics Classification
  3. Software Product Size Metrics
  4. Software Attribute Metrics

***

**Implementation of Software Quality Metrics 🛠️**

* **Activities Involved**:
  * Defining relevant and adequate metrics.
  * Regular application across units and project teams.
  * Metrics data analysis by the Corrective Action Board (CAB).
  * Responsive actions based on analysis results.
* **Detailed Discussion**: To be covered in further slides.

***

**Definition of Software Quality Metrics 📐**

* **Four-Stage Process**:
  1. **Listing Attributes**: Measuring software quality, team productivity, etc.
  2. **Defining Metrics**: Ensuring metrics measure required attributes and comply with standards.
  3. **Setting Comparative Targets**: Based on standards and past performance for benchmarking.
  4. **Determining Application Processes**: Reporting methods, data collection, and frequency.



#### Application of the Metrics 📊

**Implementing Metrics 🚀**

* **Assignment of Responsibilities**: For reporting and metrics data collection.
* **Team Instruction**: Educating the team about new metrics.
* **Follow-Up** 🔄:
  1. **Problem Solving Support**: Assisting with application problems and providing additional information.
  2. **Control of Reporting**: Ensuring completeness and accuracy in metrics reporting.

***

#### Analysis of Metrics Data by the Corrective Action Board (CAB) 📈

<figure><img src=".gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

* **Role of CAB**: Analyze metrics results as a crucial part of the SQA process.
* **Tools Used**: Statistical methods to identify significant outcomes.
* **Objective**: Facilitate process improvements through analysis.

***

#### Taking Action in Response to Metrics Analysis Results 🛠️

<figure><img src=".gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

**Comparative Analysis 📉**

* **Comparison of Project Metrics**: Analyzing metric results against predefined indicators and past projects.
* **Evaluating Metrics Effectiveness**: Assessing how well the metrics meet their objectives.

**Sample Questions for SQA Process 🤔**

* **Quality of Service**: Differences in HD teams’ service quality.
* **Impact of Development Tools**: Contribution of new tools to software quality.
* **Team Productivity**: Effects of reorganization on specific team’s productivity.

**Initiating Actions 🚦**

* **CAB's Role**: Leading the response to metrics analysis and organizational developments.



**2. Product Metrics and Their Classification 📊**

**Software Process Metrics 🔄**

* **Quantitative Representation**: Metrics reflect the software processes as experienced by developers and maintainers.
* **Examples**: Prerelease defects, percent of modified code lines, defect density.

**Software Product Metrics 📏**

* **User Experience Quantification**: Metrics represent product attributes as experienced by users in application, adaptation, or change.
* **Attributes**: Size, effectiveness, productivity, reliability.
* **Classification**:
  1. **Software Product Size Metrics**
  2. **Software Attributes Metrics**

***

#### 3. Software Product Size Metrics 📐

**Purpose of Measurement 🎯**

* **Resource Estimation** 📊: Needed for estimating development resources in planning stages.
* **Performance Comparison** ⚖️: Used in metrics of productivity, quality (defect rates), etc.

**Approaches 🚀**

1. **Thousands Of Lines of Code (KLOC)** 📝:
   * Physical size of software (lines of code or software statements).
   * Simple but can be inaccurate in early stages.
2. **Function Points (FPs)** 🎯:
   * Part of functional size measurement (FSM) methods.
   * Involves counting software inputs/outputs, transactions, logical file systems, and evaluating complexity.

**Questions for Consideration ❓**

* Average logical statements per function point?
* Average productivity per staff member in function points per month?

***

#### 4. Software Product Attribute Metrics 🌟

**ISO/IEC Technical Reports: 10 Attributes 📚**

1. **Software Functionality** 💡
2. **Software Reliability** 🛡️
3. **Software Usability** 👍
4. **Software Efficiency** 🚀
5. **Software Maintainability** 🔧
6. **Software Portability** 🌍
7. **Software Effectiveness** 🎯
8. **Software Productivity** ⏱️
9. **Software Safety** 🛑
10. **Software Satisfaction** 😊

***

#### Entities and Attributes 🔍

**Understanding Attributes 📊**

* **Definition**: Characteristics or properties of entities.
* **Example**: A person (entity) can be described by attributes like height, eye color, IQ, etc.
* **Software Entities**: Described by attributes such as size, cost, response time, defects, reliability.

**Resource Measures( Entities )**

<figure><img src=".gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

***

**Product Measures( Entities )**

<figure><img src=".gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>



Thousands Off Lines of Code (KLOC):

<figure><img src=".gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>



**Purpose of Measurement 🎯**

* **Development Resource Estimation**: Estimating resources in the proposal or planning stages.
* **Performance Comparison**: Used in productivity, quality metrics, and others.

**Approaches 🚀**

1. **Thousands Of Lines of Code (KLOC)**:
   * Represents physical completed size (e.g., lines of code).
   * Simple but can be inaccurate in early development stages.
   * Relies on evaluator experience and project specifications.
2. **Function Points (FPs)**:
   * Part of functional size measurement (FSM) methods.
   * Counts software inputs/outputs, transactions, and logical file systems.
   * Evaluates complexity and assigns factors.
   * Questions to Consider:
     * Average logical statements per function point?
     * Staff productivity in function points per month?

\
\


<figure><img src=".gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>



#### Function-Oriented Metrics – Weighting Factors 📊

**The 14 General Characteristics 🌟**

1. **Data Communications**: Are data communications required?
2. **Distributed Functions**: Are there distributed processing functions?
3. **Performance**: Is performance critical?
4. **Heavily Used Configuration**: Will the system run in a heavily utilized environment?
5. **Transaction Rate**
6. **Online Data Entry**
7. **End-user Efficiency**
8. **Online Update**
9. **Complex Processing**
10. **Reusability**
11. **Installation Ease**
12. **Operational Ease**
13. **Multiple Sites**
14. **Facilitation of Change**

***

**Calculating Weighting Factors 🔢**

#### Function-Oriented Metrics 📈

<figure><img src=".gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

**Information Domain Characteristics 🖥️**

* **Characteristics Determined**:
  * Number of user inputs (EI)
  * Number of user outputs (EO)
  * Number of user inquiries (EQ)
  * Number of files (ILF)
  * Number of external files (EIF)

**Weighting Factors ⚖️**

* **Complexity Assessment**: Assigning complexity values (simple, average, complex) to each count.
* **Function Points Calculation**: Using counts and weighting factors to determine function points.

<figure><img src=".gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

\


<figure><img src=".gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (49).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (51).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (52).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (53).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>
