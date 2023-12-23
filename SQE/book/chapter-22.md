# Chapter 22

_**Review Questions**_

**Q 22.1 ) An SCR relating to changes in only two of the software source SCIs has been approved. However, the software test plan prepared by the Testing Unit included nine of the system’s software source SCIs. • Explain in your own words why it may not be sufficient only to test the two SCIs specified in the SCR after they were changed**

**Answer :**&#x20;

**Question: Why might testing only the two Software Configuration Items (SCIs) mentioned in a Software Change Request (SCR) not be enough?** 🤔

Think of the software system like a spider web 🕸️. Each thread (SCI) is connected to others. Now, let's say you only fix two threads in the web that you think are broken (the two SCIs mentioned in the SCR).

Here's why just fixing those two threads might not be enough:

1. **Connected Threads:** Even if you only touched two threads, they're connected to others. Fixing them might accidentally change how the other threads (SCIs) behave (🔗➡️🔗).
2. **Hidden Problems:** If you don't check the threads around the ones you fixed, you might miss some other issues. It's like fixing a part of a net and not noticing another part is about to break (🔍🕳️).
3. **Complex Webs:** Software systems are complex, like really intricate spider webs. A small change in one place can have a big impact somewhere else (🕸️🧩).
4. **Expert Spiders:** The Testing Unit, like expert spider-web makers, thought it was important to check nine threads (SCIs). They probably had a good reason, like ensuring the whole web stays strong (🕷️👍).

In summary, testing only the two SCIs mentioned in the SCR might not be enough because it's like fixing only part of a spider web. To make sure the whole web is strong and doesn't have hidden weak spots, it's better to check all the parts that could be affected, just like the Testing Unit originally planned with nine SCIs. This way, you ensure the software system (the web) stays robust and reliable. 🕸️💻🔍





**Q 22.2)** **a. Why is there a need to examine the submitted Software Change Request (SCR)?** 🤔

Imagine you're playing a game where you want to change the rules. Before you do, you need to make sure the new rule won't ruin the game for everyone. This is like examining an SCR.

The SCC committee is like a group of referees who check the new rule (SCR) to ensure it:

* **Makes the game better:** They check if the change will improve the software system (👍).
* **Doesn't cause problems:** They make sure the new rule doesn't mess up other parts of the game (🚫).
* **Is actually needed:** They consider if this new rule is really necessary or just a nice-to-have (💡).

**b. Types of expected examination findings that need to be corrected** 🛠️

1. **Unclear Instructions:** Sometimes the new rule isn't explained well enough. It's like someone saying, "Let's add a twist!" but not explaining the twist (🤷‍♂️).
2. **Clashes with Current Rules:** The new rule might not fit with the existing rules of the game (🤔📚).
3. **Unexpected Mess-ups:** The new rule might accidentally make another part of the game less fun or broken (😱).
4. **Not Really Needed:** Sometimes, after thinking it over, the referees decide the new rule isn't really important for the game (🚫🤷‍♀️).
5. **Not Enough Resources:** Maybe there aren't enough game pieces or time to add this new rule (⌛🧩).
6. **Delays the Game:** The new rule might make the game take longer to finish (⏰).
7. **Not Keeping Up with Trends:** Sometimes, a rule might be outdated and doesn't fit with how people want to play the game now (📉).

In summary, examining the SCR is like double-checking a new rule in a game to make sure it's good, fits well, and actually improves the game. The SCC committee, like referees, need to fix any issues before saying, "Yes, let's play with this new rule!" 🎮👍



**22.3) The SQA unit periodic review of the activities of the organization’s |SCCA identified many shortcomings in the committee’s activities and decisions.**&#x20;

**a. List at least four different types of shortcomings.**&#x20;

**b. Suggest ways to prevent succession of each of the shortcomings mentioned in (a).**



**a. Types of Shortcomings in SCCA's Activities and Decisions** 🚩

1.  **Inadequate Examination of SCRs:** The SCCA didn't check the Software Change Requests (SCRs) thoroughly enough. It's like a chef not tasting the food properly before serving it (🔍📝).

    **Prevention:** Set clear rules for checking SCRs, like a recipe for the chef to follow every time (📖✅).
2.  **Not Following Procedures:** The SCCA sometimes skipped steps in their own rules, like a soccer player ignoring game rules (⚽🚷).

    **Prevention:** Stick to the rules strictly and train everyone to understand why they're important, like a soccer coach drilling the rules into the team (🏋️‍♂️📚).
3.  **Slow Decision-Making:** The SCCA took too long to make decisions, like a slow computer processing data (⏳💻).

    **Prevention:** Set specific time limits for decisions and keep everyone on track, like setting a timer for a game (⏰🏁).
4.  **Inconsistent/Biased Decisions:** The SCCA's choices sometimes seemed unfair or random, like a biased referee in a game (👨‍⚖️⚖️).

    **Prevention:** Use clear, fair criteria for all decisions, like a referee using a rulebook to make calls (📕🤝).

**b. Ways to Prevent These Shortcomings** 🛡️

* **For Inadequate Examination:** Implement detailed guidelines and checklists for examining SCRs, ensuring every aspect is covered (🔍📋).
* **For Not Following Procedures:** Regularly train the team on procedures and emphasize their importance for software quality (🎓📈).
* **For Slow Decision-Making:** Create a timeline for each decision-making step and hold regular meetings to keep things moving (⏱️🗓️).
* **For Inconsistent/Biased Decisions:** Develop objective evaluation criteria and make sure all decisions are transparent and based on these criteria (⚖️🔎).

In essence, improving the SCCA's work is like fixing a team's strategy in a game: make sure everyone knows the rules, follows them, makes quick and smart plays, and plays fairly. This way, the software (or the game) stays top-notch! 🌟💻🎮



**Topics for discussion**

**22.1) A developer’s success to complete a project, while successfully fulfilling the project requirements and being on schedule depends, to a great extent, on compliance to SCC procedures.**&#x20;

**a. While referring to the software change control tasks, explain in your own words the risks incurred with software quality by only partially complying with SCC procedures.**&#x20;

**b. It is widely accepted that by performing a full SCR process, the risks of failing to complete a software development project on schedule are substantially reduced. Explain**

**a. Risks of Partially Complying with SCC Procedures** 🚧

1.  **Incomplete Paperwork:** Just like missing pages in an instruction manual, incomplete documentation can leave people confused about the software changes (📄🤷‍♂️).

    **Risk:** Misunderstanding the changes can lead to mistakes in the software (⚠️🐛).
2.  **Uncontrolled Changes:** It's like adding ingredients to a recipe without measuring. Without full SCC compliance, changes can be random and unpredictable (🥄🧂).

    **Risk:** This can make the software unstable and unreliable (💥🖥️).
3.  **More Bugs:** Skipping steps in testing is like not checking your work in a math problem. This can lead to more errors in the software (🐞🔍).

    **Risk:** More bugs mean the software might not work correctly (🚫💻).
4.  **Lost Tracking:** Partial compliance can make it hard to track who did what, like a puzzle with missing pieces (🧩❓).

    **Risk:** If problems arise, it's hard to figure out where they started (🔍🤔).
5.  **Poor Teamwork:** Not following procedures can mess up communication, like a team playing without talking to each other (🗣️🤐).

    **Risk:** Miscommunications can delay or mess up the project (⏰🔄).

**b. Benefits of a Full SCR Process** ✅

1.  **Better Planning:** Doing a full SCR is like using a detailed map for a road trip. It helps in planning the project more accurately (🗺️📆).

    **Benefit:** This reduces the chances of the project getting delayed (🚗⌛).
2.  **Smart Choices:** It's like sorting tasks by importance. A full SCR helps prioritize changes and allocate resources wisely (📊🏆).

    **Benefit:** The project stays on track and important parts get attention first (🛤️👍).
3.  **Controlled Changes:** Fully documented changes are like well-written recipes. They make sure everything is done right (📖✅).

    **Benefit:** This keeps the software's quality high and prevents schedule slips (💡👌).
4.  **Better Teamwork:** Like a team huddle, a full SCR improves communication and collaboration (👥🤝).

    **Benefit:** Everyone understands the project better, reducing misunderstandings and delays (🗣️🚀).

In summary, skipping steps in SCC procedures is like trying to build something without all the instructions or tools. It can lead to mistakes, confusion, and a shaky final product. On the other hand, doing a full SCR process is like following a well-planned recipe or blueprint. It keeps everything organized, clear, and on track, making sure the project is successful and finished on time! 🏗️🕒🌟



**22.4) The software maintenance department provides services to 215 customers who use one or more of the company’s three popular software packages. From time to time, a maintenance team discovers that the software version installed in a customer’s site includes unrecorded changes that were not requested by an SCR, nor approved as part of an SCO.**&#x20;

**f. Who do you believe inserted the unrecorded changes and under what conditions could this have occurred?**&#x20;

**g. What effect could this event have on maintenance performance, and what is the expected influence on software quality from the perspective of the customer?**&#x20;

**h. What measures could be taken to make sure that no such unauthorized changes occur?**

#### f. Identifying the Source of Unrecorded Changes 🔍

Answer:&#x20;

**Who might have made the changes?**

1. **Software Maintenance Team** 🛠️:\
   The team itself may have made changes without proper documentation or approval, possibly due to a lapse in change management procedures or internal communication issues.
2. **Customer or Someone Within Customer's Organization** 👤:\
   Customers attempting DIY modifications or unauthorized personnel within the organization making changes without informing the maintenance team.
3. **Third Party (e.g., Hacker or Malicious Insider)** 👾:\
   Unauthorized changes could have been made by external parties, potentially with harmful intentions.

#### g. Impact on Maintenance and Software Quality 📉

**Effects on Maintenance Performance:**

* **Increased Workload for Maintenance Team** 🚧:\
  More time and effort needed to identify and rectify unrecorded changes, leading to delays in other maintenance tasks.

**Influence on Software Quality from Customer's Perspective:**

* **Potential Reduction in Software Quality** 💻:\
  Unrecorded changes may introduce new bugs or errors, affecting reliability and functionality, leading to customer dissatisfaction and operational disruptions.

#### h. Preventing Unauthorized Changes 🛡️

**Measures to be Taken:**

1. **Robust Change Management Process** 📋:\
   Establish formal procedures for requesting, reviewing, approving, and documenting all changes.
2. **Strict Access Controls and Permissions** 🔐:\
   Limit change capabilities to authorized personnel, with logged and monitored actions.
3. **Regular Audits and Reviews** 📊:\
   Regularly compare installed software versions with approved changes to detect unauthorized modifications.
4. **Training and Awareness Programs** 🎓:\
   Educate both the maintenance team and customers on proper procedures and the risks of unauthorized changes.
5. **Implement Version Control Systems** 🖥️:\
   Use these systems to track changes and manage software versions effectively.

By incorporating these measures, the software maintenance department can significantly reduce the occurrence of unauthorized changes, thereby enhancing maintenance efficiency and improving software quality from the customers' perspective. 🌟







