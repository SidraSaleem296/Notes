# Testing

#### Software Testing 💻

**Understanding Software Testing**

* **Human Factor** 👥: Computer programs, created by humans, are prone to errors.
* **Necessity of Testing** 🔍: Integral to the software development lifecycle to avoid potential problems.
* **Implementation** 📝: Requires proper planning and correct implementation.

***

#### Software Testing - Definition 📖

* **Formal Process** 🧑‍🔬: Conducted by a specialized testing team.
* **Scope** 🌐: Involves examining software units or entire packages by running them on a computer.
* **Methodology** 📚: Performed based on approved test procedures and cases.

***

#### Clarifying Software Testing 🤔

* **Goal** 🎯: To find evidence of defects and establish confidence in the software's functionality.
* **Misconceptions** 🚫:
  1. Not equivalent to debugging.
  2. Not the same as quality assurance.

***

#### Testing Vs Debugging ⚙️

* **Testing** 🔎:
  * Objective: Identify problems in the product.
  * Role: Performed by testers without needing source code access.
* **Debugging** 🛠️:
  * Objective: Remove or fix bugs.
  * Role: Conducted by developers who need source code access.

***

#### Software Testing Vs Quality Assurance 📈

* **Role in QA** ✨: Testing is vital but not the sole component of QA.
* **Contribution** 🤝: Helps improve quality by identifying issues.
* **QA Standards** 📋: Sets benchmarks for the project team, including testers, for superior software development.

***

#### Exploring Software Testing 🔬

* **Key Aspects** 🌟:
  * Correctness with respect to requirements.
  * Performance under various conditions.
  * Robustness and error handling.
  * Installation and other facets of release.

***

#### Important Considerations in Testing 📍

* **Process Steps** 🔄:
  1. Detect system failures with carefully chosen test inputs.
  2. Identify and repair faults leading to failures.
  3. Re-test the module/system for verification.

\


#### Basic Questions on Testing 🤔

**Why to Test? 🔍**

* **Purpose** 🎯: To ensure the software functions correctly and fulfills its intended purpose.

**What to Test? 📊**

* **Scope** 📚: All components of the software application, including both data and programs.

**How Often to Test? 🔄**

* **Frequency** ⏲️: Testing is required whenever the source code is modified or newly developed.

**Who Tests? 👥**

* **Responsibility** 🧑‍💻: Involves programmers, testers, and customers (or third parties).

***

#### Why do Failures Occur? 🚫

**Failure Sources 🛠️**

* **Areas of Concern** 📝:
  * Specification
  * Design
  * Code
  * Other related factors

<figure><img src=".gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

***

#### Software Testing Objectives 🎯

**Direct Objectives ✅**

1. **Error Identification**: Revealing as many errors as possible.
2. **Quality Improvement**: Bringing software to an acceptable quality level after error correction and retesting.
3. **Efficiency and Effectiveness**: Conducting tests within budgetary and scheduling constraints.

**Indirect Objectives 🌐**

* **Error Record Compilation**: Gathering data on software errors for future error prevention strategies.

***

#### Software Testing Styles 🌟

**Incremental Testing Strategies 📈**

* **Test Incrementally**:
  * Unit Testing
  * Integration Testing
  * System Testing
* **Integration Testing Approaches**:
  * Bottom-up Testing
  * Top-down Testing
  * Big Bang Testing

#### Bottom-Up Integration Testing 📉

**Integrating Lower-Level Components 🔄**

* **Combining Components** 🧩: Lower-level components are merged into clusters to perform specific software functions.
* **Driver Utilization** 🚗: A control program (driver) is created for coordinating test case input and output.
* **Cluster Testing** 🧪: Each cluster undergoes testing.
* **Progressive Integration** ⬆️: After testing, drivers are removed, and clusters are combined, moving upward in the program structure.

<figure><img src=".gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

**Top-Down Integration Testing 📈**

**Structuring the Integration Process ⚙️**

* **Utilizing the Main Program as a Test Driver** 🚙: Stubs are used in place of components directly subordinate to the main program.
* **Sequential Component Replacement** 🔁: Subordinate stubs are individually replaced with real components, either depth-first or breadth-first.
* **Conducting Tests** 🧪: Testing occurs as each component is integrated.
* **Stub Replacement** 🔄: After testing each set, the stub is substituted with an actual component.
* **Regression Testing** 🛠️: Applied to ensure no new errors are introduced during integration.

<figure><img src=".gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

#### Stubs and Drivers: Example 🚀

**Web Application Testing Scenario 💻**

* **Module Overview** 📦:
  * **Module-A**: Login page of the web application.
  * **Module-B**: Home page of the web application.
  * **Module-C**: Print Setup.
  * **Module-D**: Log out page.
* **Module Interdependencies** 🔗: Highlighting the interconnected nature of Modules A, B, C, and D.

***

**Integration of Stubs and Drivers 🛠️**

* **Parallel Testing and Development** 🔄: Testing is conducted alongside the development process.
* **Module-A Testing Challenge** 🚧: Validating Module-A (login page) requires Module-B (home page), which may not be developed yet.
* **Stubs and Drivers in Action** 🧩:
  * Creating a dummy module for Module-B to facilitate testing of Module-A.
  * Using stubs and drivers to substitute for unavailable modules, ensuring continuous testing efficiency.
* **Example Usage** 📝:
  * Testing Module-D (log out page) with a stub or driver acting as Module-A (login page) in its absence.

\
**Big Bang Integration Testing 💥**

* **Testing Approach** 🌐: Tests the entire software at once by integrating all components or modules simultaneously.
* **Advantages** ✅: Complete development before testing starts.
* **Disadvantages** ❌: Time-consuming and challenging to trace failures due to late integration.

***

#### System Testing Process 🧪

1. **Plan** 📝:
   * Create Master Test Plan (MTP) and Detailed Test Plan (DTP).
   * Develop Detailed Test Cases (DTC).
2. **Execute** 🏃‍♂️: Implement the planned tests.
3. **Regress and Analyze** 🔍: Perform regression testing and analyze results.

***

#### What’s a Test Plan? 📊

* **Purpose** 🎯: Document describing testing objectives, scope, approach, and focus.
* **Includes** 📋:
  * Title, software identification, revision history.
  * Software product overview.
  * Testing priorities, focus, scope, and limitations.
  * Test environment specifications.

***

#### Detailed Test Plan 🗺️

* **Testing Aspects** 📈: Configuration, Security, Functionality, Performance, Environment.

***

#### Test Planning Objectives 🎯

* **Goals** 🏁: Establish tasks, identify unmet requirements, document overall approach.
* **Output** 📚: Comprehensive test plan.
* **Inspection** 🔎: Review by engineering team and senior managers.

***

#### Test Plan Overview 🔍

* **Who** 👤: QA team.
* **When** ⏳: During planning/design/coding/testing stages.
* **Why** 🤔: Divide responsibilities, plan for resources, timelines, and test coverage.

***

#### Test Planning Details 📝

* **QA Role** 🛠️:
  * Create, maintain, and analyze the document.
  * Get it reviewed and approved by project leads/managers.

***

#### Test Plan Structure 🏗️

* **Components** ⚙️:
  * Test objectives, strategies, and cases (procedure, data, expected result).
  * Procedures for handling problems.

***

#### Software Test Plan - Contents 📄

* **Covering** 📖: All types and phases of testing.
* **Guidance** 🧭: Directs who, why, when, and what in the testing process.
* **Development Phase** 🛠️: Concurrent with requirements and design phases.

<figure><img src=".gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

***

<figure><img src=".gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

#### Testing Basics 📊

* **Definition** 💡: Process of identifying defects through test cases and data.
* **Test Case** 🧾: A formal description of a starting state, response events, and expected outcomes.

**Testing Discipline Activities 🧪**

<figure><img src=".gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

**Test Case 📝**

* **What**: A set of inputs, preconditions, and expected outcomes to achieve specific testing objectives.
* **Who**: QA team.
* **When**: During planning, design, coding, and testing stages.
* **Why**:
  * Plan testing efforts, resources, and timelines.
  * Review and plan test coverage.
  * Track testing progress, defects, and software quality metrics.
  * Establish unified pass/fail criteria.
  * Differentiate between planned/systematic and ad-hoc testing.

**Test Case Structure 🔍**

* **Typical Layout**: Often presented in table format.
* **Components**:
  * **ID**: Unique identifier for each test case.
  * **Features/Steps/Input Values**: Details of what to do.
  * **Requirements**: The specific requirement being tested.
  * **Preconditions**: State of the software before testing.
  * **Steps**: Specific actions in the interaction.
  * **Expected Results/Output Values**: Predicted outcomes post-execution.
* **Repeatability**: Test cases must be repeatable and data-specific.

**Test Suite 📊**

* **Definition**: A document specifying the sequence of actions for executing multiple test cases.
* **Purpose**: Organizes test cases for execution; may be manual or automated (referred to as test scripts).
* **Organization**: Multiple Test Suites are sequenced to define test order, timing, responsibilities, etc.\


<figure><img src=".gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

**Detailed Test Cases:**

<figure><img src=".gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

**Test Case Bug Report**

<figure><img src=".gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>
