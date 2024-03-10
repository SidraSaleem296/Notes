# Levels of Testing

**Agenda** 📅

* 🧩 Levels of Testing
* 🔍 Component Testing
* 🚧 Stubs and Drivers
* 🔬 Unit Testing
  * Key Points for Unit Testing
  * 🛠️ Tools for Unit Testing
* 🌐 Integration Testing
  * Approaches to Integration Testing
  * 🆙 Bottom-Up and 🔝 Top-Down Integration Testing
  * 💥 Big Bang and 📲 Ad-Hoc Integration Testing

***

#### **Levels of Testing** 📊

**Component Testing 🧱**

* Tests individual software components in isolation.
* Uses **stubs and drivers** for simulation.
* Objectives include reducing risks, verifying behaviors, building confidence, finding, and preventing defects.

**Stubs vs. Drivers 🚀🔙**

* **Stubs**: Mimic called functions, used in Top-Down Integration.
* **Drivers**: Mimic calling functions, used in Bottom-Up Integration.

#### Stubs vs Drivers Comparison Table 🛠️

| **Aspect**                | **Stubs**                                                                                                                     | **Drivers**                                                                                                             |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| **Definition**            | Stubs are simulated implementations of lower-level modules or components that a unit under test depends on.                   | Drivers are simulated implementations of higher-level modules that call a lower-level module or component to be tested. |
| **Purpose**               | Used to mimic the behavior of child components not yet developed or integrated, allowing the testing of higher-level modules. | Used to simulate the behavior of parent components, enabling the testing of lower-level modules in isolation.           |
| **Usage in Testing**      | Commonly used in Top-Down Integration Testing where testing starts from the top layers of the application.                    | Predominantly used in Bottom-Up Integration Testing, where testing begins with the lowest layers.                       |
| **Functionality**         | Stubs provide predefined responses to the calls made by the module under test.                                                | Drivers make calls to the module under test and can provide input data for testing.                                     |
| **Complexity**            | Stubs are usually simpler, as they only need to simulate specific functionalities or outputs.                                 | Drivers can be more complex, as they may need to initiate and manage the execution of a module or component.            |
| **Integration Direction** | Facilitate the testing of higher-level functionalities before the lower-level components are developed.                       | Facilitate the testing of foundational components before the higher-level functionalities are developed.                |
| **Example**               | A stub could simulate a database response for a data retrieval method in a service layer being tested.                        | A driver could simulate a user interface or controller to test the interaction with a back-end service.                 |

**Unit Testing 🧪**

* Focuses on individual parts for functionality, aiming to identify and fix defects early.
* Often performed by developers to ensure reusability and facilitate changes.

**Key Points for Unit Testing ✅**

* Functional aspects, boundaries, termination behavior, expected outputs, and inputs, interaction with other modules.

**Tools for Unit Testing 🛠️**

* Junit, Nunit, JMocKit, EMMA, PHPUnit.

***

#### Unit Testing vs Component Testing 🤔

| **Aspect**         | **Unit Testing**                                                                                          | **Component Testing**                                                                                                    |
| ------------------ | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| **Definition**     | Testing of individual units or components of a software, typically by the developers.                     | Testing of individual components or sets of related components as a group, often after unit testing.                     |
| **Scope**          | Narrow, focuses on a specific unit of the software.                                                       | Broader than unit testing, focuses on the functionality and performance of a component or a group of related components. |
| **Isolation**      | Tested in isolation from the rest of the system, often using stubs or mocks to simulate other components. | Tested in a context that is closer to real-world use, may still use stubs or drivers to simulate interacting components. |
| **Objective**      | To validate that each unit of the software performs as designed.                                          | To verify the interface and interaction between components and detect any defects in the integration.                    |
| **Performed by**   | Primarily developers.                                                                                     | Developers or testers, depending on the organization's process.                                                          |
| **Tools**          | JUnit, NUnit, PHPUnit, etc.                                                                               | Similar tools as unit testing, but also includes integration testing tools for more complex scenarios.                   |
| **Testing Method** | White-box testing, where the internal structure/design is known to the tester.                            | Can be both white-box or black-box testing, depending on whether the internal details of the component are known or not. |
| **When Performed** | After a unit or piece of code is written, before integration.                                             | After unit testing, before system testing.                                                                               |
| **Complexity**     | Low, tests the smallest parts of an application independently.                                            | Higher, as it may involve multiple components and their interactions.                                                    |
| **Focus**          | Functional correctness of the unit.                                                                       | Functional and non-functional behaviors of the component, including performance and scalability.                         |

#### **Integration Testing** 🔄

* Combines units, components, products to find interface defects.
* Types of approaches: **Top-Down**, **Bottom-Up**, **Big Bang**, **Ad-Hoc**.

**Integration Testing Approaches 🛤️**

* **Top-Down**: Tests top modules first, using stubs for missing ones.
* **Bottom-Up**: Starts with the lowest units, using drivers for simulation.
* **Big Bang**: Integrates all components at once, convenient for small systems.
* **Ad-Hoc**: Informal, without planning or documentation, integrating components as they are completed.

#### Integration Testing Approaches Comparison 🛠️

| **Aspect**         | **Top-Down**                                                                                         | **Bottom-Up**                                                         | **Big Bang**                                                                         | **Ad-Hoc**                                                             |
| ------------------ | ---------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- | ------------------------------------------------------------------------------------ | ---------------------------------------------------------------------- |
| **Starting Point** | Begins with the highest-level modules and works down.                                                | Begins with the lowest level modules and integrates upwards.          | All modules or components are integrated simultaneously.                             | Components are integrated as they are completed, without a set order.  |
| **Stubs/Drivers**  | Uses **stubs** to simulate lower-level modules not yet integrated.                                   | Uses **drivers** to simulate higher-level modules not yet integrated. | Not applicable, as all components are integrated at once.                            | May use stubs or drivers, but not systematically.                      |
| **Ideal For**      | Projects where top-level design details are crucial.                                                 | Projects where bottom-level functionalities are critical.             | Small systems or projects where a quick overview is needed.                          | Quick, informal testing with no specific plan or documentation.        |
| **Testing Focus**  | Testing the integration from top to bottom, ensuring major functionalities work before going deeper. | Focuses on data flow and control flow from the bottom up.             | Tests the overall system functionality and interaction at once.                      | Testing based on convenience or immediate need, rather than structure. |
| **Advantages**     | Facilitates early identification of high-level design issues.                                        | Allows early testing of basic functionalities and data processing.    | Simplifies the process by testing everything at once; good for smaller systems.      | Flexible and can adapt to project needs without formal planning.       |
| **Disadvantages**  | May delay testing of lower-level components and their interactions.                                  | Higher-level functionalities are tested late in the cycle.            | Risk of missing interactions and integration issues due to simultaneous integration. | Lack of planning can lead to missed defects and inefficiencies.        |

***

Now, let's make this learning process even more interactive with some **technical but tricky questions** about the lecture:

1. **Why are stubs specifically used in Top-Down Integration Testing?** 🤔
2. **Can you describe a scenario where Component Testing might not be sufficient and Integration Testing becomes necessary?** 💡
3. **What is the main advantage of using drivers in Bottom-Up Integration Testing?** 🚀
4. **In what situations might Big Bang Integration Testing be preferred over other approaches?** 🌟
5. **How does Unit Testing contribute to reducing the overall cost of testing in the software development life cycle?** 💰





1. **Why are stubs specifically used in Top-Down Integration Testing?** 🤔
   * Stubs are used in Top-Down Integration Testing to simulate the behavior of lower-level modules that have not yet been developed or integrated. This allows testers to focus on testing the functionality of the higher-level modules first, ensuring that the major parts of the system work correctly before the lower-level details are finalized. Stubs essentially provide a temporary implementation that mimics the interface and outputs of the undeveloped modules, facilitating the testing process without waiting for the entire system to be built.
2. **Can you describe a scenario where Component Testing might not be sufficient and Integration Testing becomes necessary?** 💡
   * Component Testing might not be sufficient in scenarios where the components or modules need to interact with each other to perform a complete function or feature. For instance, in a web application that includes a user registration module, a login module, and a profile management module, each module might work perfectly when tested individually (Component Testing). However, Integration Testing becomes necessary to ensure that the user can register, log in, and then access and modify their profile seamlessly. This tests the data flow and interaction between these modules, uncovering issues that would not be evident when modules are tested in isolation.
3. **What is the main advantage of using drivers in Bottom-Up Integration Testing?** 🚀
   * The main advantage of using drivers in Bottom-Up Integration Testing is that they enable the testing of lower-level modules even when the higher-level modules they interact with are not yet developed or integrated. Drivers simulate the calling environment for the lower-level modules, allowing developers and testers to verify the functionality of these foundational components early in the development process. This approach ensures that the basic building blocks of the application are working correctly before they are integrated into the larger system, facilitating a smoother integration process as development progresses.
4. **In what situations might Big Bang Integration Testing be preferred over other approaches?** 🌟
   * Big Bang Integration Testing might be preferred in smaller projects or systems where the number of components and their interactions are limited and manageable. This approach can also be beneficial when the development team has a tight deadline and needs to quickly integrate and test all components together to ensure the system works as a whole. Since Big Bang Integration Testing involves integrating all components at once, it can save time in planning and executing phased integration tests. However, it requires a well-coordinated effort and thorough understanding of the system to effectively identify and troubleshoot integration issues.
5. **How does Unit Testing contribute to reducing the overall cost of testing in the software development life cycle?** 💰
   * Unit Testing contributes significantly to reducing the overall cost of testing in the software development life cycle by catching and fixing errors early in the development process. When developers test individual units of code before they are integrated into larger components, defects can be identified and corrected immediately, preventing the propagation of these errors to later stages of development. This early detection reduces the need for more complex and time-consuming fixes during integration or system testing phases. Additionally, well-designed unit tests can be automated and reused throughout the development lifecycle, offering continuous validation of code integrity as changes are made, thereby maintaining quality and reducing regression testing efforts and costs.
