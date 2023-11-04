# Lecture 9

📝 **Task Analysis**

Task descriptions are a means for designers to delineate and understand the tasks the user performs. They help us analyze:

* 🤔 What people are doing
* 🎯 What they are trying to achieve
* ❓ Why they are trying to achieve it
* 🚀 How they are going about it

Task descriptions are written by designers and can be shared with the client to ensure understanding. They can also be shared with programmers to help design the software.

🔍 **Task Analysis- Decomposition**

👉 The difference between:

* **Goal**: The state of the system that a human wants to accomplish.
* **Task**: Activities required to achieve a goal, often consisting of subtasks.
* **Actions**: Steps required to complete a task.

For example, recording a TV program can involve asking a friend, pressing 'Rec' on the PVR, setting the timer manually, or using an on-screen TV guide.

📊 **Task Analysis**

* Task analysis techniques support user-centered design.
* They inform us about how users use existing products and may interact with future ones.
* Can be used to improve current design, identify problems with new design, and develop training materials and manuals.

🔄 **Task Analysis**

Task analysis is crucial in systems development but varies in focus:

* During understanding, it aims to be device-independent to understand the essential nature of the work.
* During design and evaluation, it focuses on achieving work using a particular technology (device-dependent).

🛠️ **Practical Task Analysis**

* Develop concrete, detailed examples of tasks users perform or want to perform.
* Determine what the user wants to do, not how to do it.
* No assumptions about the interface, allowing for design alternatives.
* Task descriptions are very specific, context-specific, and user-specific.

📊 **Hierarchical Task Analysis (HTA)**

Two techniques:

* **HTA**: Concerned with the logic of a task, structure tasks within hierarchies.
* **GOMS**: Focuses on cognitive analysis of tasks and procedural knowledge.

HTA aims to describe actions, structure them hierarchically, describe the order of subtasks, and analyze existing systems.

🌲 **HTA**

HTA uses graphical representation based on a structure chart notation:

* Represents sequences of tasks, subtasks, and actions hierarchically.
* Includes notational conventions for iteration and selection.
* Helps understand task structures effectively.

📋 **Procedure for HTA**

* Define the task title and overall goal.
* Identify the first level of subtasks (less than 10).
* Break down subtasks further when needed (less than 10 steps each).
* Describe the order of subtasks and steps in plans.

🔄 **Stages of HTA**

1. Starting the analysis: Specify the main task, break it down, and draw layered plans.
2. Progressing the analysis: Decide on the level of detail and decomposition method.
3. Finalizing the analysis: Check consistency and have a second person review it.

📜 **Textual HTA Description**

Example of hierarchical structure:

* Invert a portion of an image:
  * Zoom display to area of interest
  * Select the Lasso Tool
  * Select the subregion of the image
  * Select Invert from the Image menu

🔍 **Refining the Description**

Heuristics for improving HTA:

* Paired actions, restructuring, balancing, and generalizing.

🔀 **HTA Structure Chart Notation**

Visual representation of HTA tasks using a structure chart notation.

📄 **Hierarchical Task Analysis**

Example of hierarchical task analysis for inverting an image.

1. Invert a portion of an image: 1.1 Zoom display to area of interest 1.1.1 Select the zoom tool from the toolbox 1.1.2 Specify the zoom region using the tool 2. Select the Lasso Tool 3. Select the subregion of the image: 3.1 Point and click around the area of interest 3.2 Adjust the "rubber band" to accurately select the region 4. Select Invert from the Image menu

🎯 **Task Analysis - Critical Thinking**

Requirements that might emerge from task analysis:

* Distinctive, non-annoying bell sound
* Easily accessible door mechanism
* Highly learnable means of selecting a program

🧩 **GOMS - Goals, Operators, Methods, Selection Rules**

GOMS provides predictive, descriptive, and prescriptive models for tasks.

📊 **GOMS: Classification**

GOMS stands for Goals, Operators, Methods, and Selection Rules, offering predictive, descriptive, and prescriptive modeling.

🎯 **Goals**

Goals represent what the user wants to achieve, often structured hierarchically.

🛠️ **GOMS Output Uses**

GOMS output is used to ensure goals are achieved quickly, assess functionality coverage and consistency, and determine operator sequences.

🔄 **How to Do GOMS Analysis**

Steps for GOMS analysis:

1. Generate a task description.
2. Evaluate the task description.
3. Apply results to UI.
4. Iterate as needed.

❌ **Disadvantages of GOMS**

Disadvantages of GOMS include complexity, time and effort, unrealistic assumptions, and limited consideration of user mistakes.

🌐 **GOMS Family of Models**

Various GOMS techniques include MHP, KLM, CPM-GOMS, and CogTool, tailored for different applications.

Various techniques have been developed within the GOMS framework to address different aspects of human-computer interaction. Some of the notable techniques include:

1. MHP (Model Human Processor): MHP is a theoretical model that attempts to describe the structure and function of the human information processing system. It provides a framework for predicting the time it takes a person to carry out cognitive tasks. This model is often used to estimate the time it takes for a user to perceive, process, and respond to information presented on a computer screen.
2. KLM (Keystroke-Level Model): KLM is a simplified GOMS technique that focuses on predicting the time it takes for a skilled user to perform specific tasks by counting the number of cognitive and motor operations required. It involves estimating the time for different types of actions, such as keystrokes, mouse clicks, and pointing actions. KLM is commonly used for predicting the efficiency of simple interactive tasks.
3. CPM-GOMS (Cognitive Perceptual Motor - GOMS): CPM-GOMS is an extension of the traditional GOMS model that incorporates cognitive, perceptual, and motor processes. It is used to analyze complex human-computer interaction tasks that involve both cognitive and physical actions. CPM-GOMS allows for a more detailed analysis of the interaction process and can provide insights into the cognitive and perceptual demands of a task.
4. CogTool: CogTool is a software tool that integrates GOMS analysis with predictive modeling to evaluate the usability of interactive systems. It allows designers to simulate and analyze user interactions with a system based on GOMS principles. CogTool can help identify usability issues and optimize the design of user interfaces by providing quantitative predictions of task completion time and potential user errors.

🖥️ **KLM: Keystroke-Level Model**

KLM is a simplified GOMS technique that predicts execution time based on keystrokes, pointing, and cognitive operations.

💡 **KLM Example**

Example of KLM analysis for editing a manuscript.
