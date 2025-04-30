**Content:**
 <a id="x"></a>

* [Introduction](#1)
* [Aligning test activities with SDLC activities](#200)
* [Test Analysis](#2)
* [Test Design](#3)
* [High-Level & Low-Level Test Cases](#4)
* [Low-Level Test Cases Advantages & Disadvantages](#5)
* [High-Level Test Cases Advantages & Disadvantages](#6)
* [Design of Test Cases](#7)
* [Test Implementation](#8)
* [Test Execution](#9)



 <a id="1"></a>

## Introduction
The Software Development Life Cycle (SDLC) is a crucial framework that outlines the various stages involved in developing software applications. This structured process ensures that software is created efficiently, meets user requirements, and maintains high quality throughout its lifecycle.  <br>

Review from the Foundation Level:
* The [SDLC](https://github.com/BeatrizBravo/ISTQBpreparation/blob/main/subjects/2-Life-cycles.md), chapter 2 . <br><br>
* And review the ['Test Process'](https://github.com/BeatrizBravo/ISTQBpreparation/blob/main/subjects/1-Fundamental.md#test-process) , Chapter 1.

<br><br>

In the ISTQB® Foundation Level syllabus, the test process includes several important steps:
1. Test Planning: Deciding what to test and how to do it. 
2. Test Monitoring and Control: Keeping track of the testing progress.
3. Test Analysis: Looking at what needs to be tested.
4. Test Design: Creating the tests.
5. Test Implementation: Setting up the tests.
6. Test Execution: Running the tests.
7. Test Completion: Finishing up the testing process.
<br>

In the Advanced Level Test Analyst syllabus, we dive deeper into the activities that are especially important for Test Analysts. This helps to make the testing process fit better with different ways of developing software. <br><br>
The main focus for a Test Analyst is on:
* Test Analysis: Figuring out what needs testing.
* Test Design: Planning how to test it.
* Test Implementation: Getting the tests ready.
* Test Execution: Actually running the tests.<br>
<br>

[Back to content](#x)

![SDLC and Process](https://github.com/BeatrizBravo/ISTQBpreparation-advance/blob/main/Resources/sdlc-process.png?raw=true)
<br>

[Back to content](#x)

<a id="200"></a>

## Aligning test activities with SDLC activities
Test activities must be aligned with the chosen SDLC whose nature may be sequential, iterative, incremental, or a hybrid of these.  <br>

For example: <br> <br>
** in the ***sequential V-model***, the test process applied to the system test level could align as follows:
* System test planning occurs concurrently with project planning, and test monitoring and control continues until test completion. This will influence the schedule inputs provided by the Test Analyst for project management purposes.
* System test analysis and design aligns with documents such as the system requirements specification, system and architectural (high-level) design specification, and component (low- level) design specification. “What and how to test”
* Implementation of the system test environment might start during system design, though the bulk of it typically would occur concurrently with coding and component testing, with work on system test implementation activities stretching often until just days before the start of system test execution.
* System test execution begins when the entry criteria are met or, if necessary, waived, which typically means that at least component testing and often also component integration testing have met their exit criteria. System test execution continues until the system test exit criteria are met.
* System test completion activities occur after the system test exit criteria are met.

** in the  ***Iterative and incremental models*** may not follow the same order of activities and may exclude some activities. For example, an iterative model may utilize a reduced set of test activities for each iteration. Test analysis, design, implementation, and execution may be conducted for each iteration, whereas high-level planning is done at the beginning of the project, and completion tasks are done at the end. <br>
In Agile software development, it is common to use a less formalized process and a much closer working relationship with project stakeholders that allows changes to occur more easily within the project. There may not be a well-defined Test Analyst role. There is less comprehensive test documentation, and communication is shorter and more frequent. <br> <br>
Agile software development involves testing from the outset. This starts from the initiation of the product development as the developers perform their initial architecture and design work. *Reviews may not be formalized* but are continuous as the software evolves. Involvement is expected to be throughout the project and Test Analyst tasks are expected to be done by the team.
 <br> <br>
Iterative and incremental models range from Agile software development, where there is an expectation for change as the customer requirements evolve, to hybrid models, e.g., 
iterative/incremental development combined with a V-model approach. **_In such hybrid models_**, Test Analysts should be involved in the planning and design aspects of the sequential activities, and then move to a more interactive role during the iterative/incremental activities. <br> <br>
Whatever the SDLC being used, Test Analysts need to understand the expectations for involvement as well as the timing of that involvement. Test Analysts provide an effective contribution to software quality by adjusting their activities and their moment of involvement to the specific SDLC rather than sticking to a pre-defined role model.

<br>

[Back to content](#x)


<a id="2"></a>

# Test Analysis

 During test planning, the scope of the testing project is defined. <br>
 During test  analysis, Test Analysts use this scope  definition to:
*  Analyze the test basis Identify defects of various types in  the test basis
*  Identify and prioritize test conditions  and features to be tested
*  Capture bi-directional traceability  between each element of the test
*  basis and the associated test  conditions
*  Perform tasks associated with risk based testing
<br>

In order for Test Analysts to proceed **effectively** with test analysis, the following **entry criteria** should be met:
* There is a body of knowledge (e.g., requirements, user stories) describing the test object that can serve as its test basis.
* This test basis has passed review with reasonable results and has been updated as needed after the review. Note that if high-level test cases are to be defined, the test basis may not yet need to be fully defined. In Agile software development, this review cycle will be iterative as the user stories are refined at the beginning of each iteration.
* There is an approved budget and schedule available to accomplish the remaining testing tasks for this test object.
<br>

Test conditions are typically identified **by** analysis of the test basis in conjunction with the test objectives (as defined in test planning). In some  situations, where documentation may be old or non-existent, the test conditions may be identified by discussion with relevant stakeholders (e.g., in workshops or during iteration planning). In Agile software development, the acceptance criteria, which are defined as part of user stories, are often used as the basis for the test design.
<br>

While test conditions are usually specific to the item being tested, there are some standard considerations for the Test Analyst.
* It is usually advisable to define test conditions at differing levels of detail. Initially, high-level conditions are identified to define general targets for testing, such as “functionality of screen x”. 
Subsequently, more detailed conditions are identified as the basis of specific test cases, such as “screen x rejects an account number that is one digit short of the correct length”. 
Using this type of hierarchical approach to defining test conditions can help to ensure the coverage is sufficient for the high-level items. This approach also allows a Test Analyst to start working on defining high-level test conditions for user stories that have not yet been refined.
* If product risks have been defined, then the test conditions that will be necessary to address each product risk should be identified and traced back to that risk item.

<br>

The application of test techniques (as identified within the test strategy and/or the test plan) can be helpful in test analysis activities and may be used to **support** the following objectives: 

* Identifying test conditions
* Reducing the likelihood of omitting important test conditions 
* Defining more precise and accurate test conditions

**After** the test conditions have been **identified** and refined, **review** of these conditions with the **stakeholders** can be conducted to ensure the requirements are clearly understood and that testing is aligned with the goals of the project. <br>

At the conclusion of the test analysis activities for a given area (e.g., a specific function), the Test Analyst should know what specific tests must be designed for that area.<br>

[Back to content](#x)

<a id="3"></a>

# Test Design
Still adhering to the scope determined during test planning, the test process continues as the Test Analyst designs the tests which will be implemented and executed. Test design includes the following **activities**:

* Determining in which test areas low-level or high-level test cases are appropriate
* Determining the test technique(s) that will enable the necessary coverage to be achieved. The techniques that may be used are established during test planning.
* Using test techniques to design test cases and sets of test cases that cover the identified test conditions
* Identifying necessary test data to support test conditions and test cases
* Designing the test environment and identifying any required infrastructure including tools Capturing bi-directional traceability (e.g., between the test basis, test conditions and test cases)

**Prioritization criteria identified** during risk analysis and test planning should be applied throughout the process, from analysis and design to implementation and execution. <br>

Depending on the types of tests being designed, one of the entry criteria for test design may be the availability of tools that will be used during the design work. <br>


During test design, the Test Analyst must consider at least the following:

* Some test items are **better addressed** by defining only the **test conditions** rather than going further into the definition of test scripts, which give the sequence of instructions required to execute a test. In this case, the test conditions should be defined to be used as a guide for unscripted testing.
* The pass/fail criteria should be clearly identified.
* Tests should be designed to be **understandable by other testers,** not just the author. If the author is not the person who executes the test, other testers will need to read and understand previously specified tests in order to understand the test objectives and the relative importance of the test. 
Tests must also be understandable for **other stakeholders** such as developers (who may **review** the tests) and auditors (who may have to approve the tests).
* Tests should cover all types of interaction with the test object and should not be restricted to the interactions of people through the user-visible interface. They may also include, for example, interaction with other systems and technical or physical events.
* Tests should be designed to test the interfaces between the various test items, as well as the behaviors of the items themselves.
* Test design **effort must be prioritized** and balanced to **align** with the **risk** levels and **business** value.

<br>

[Back to content](#x)

<a id="4"></a>

# High-Level & Low-Level Test Cases


<a id="5"></a>
## Low-Level Test Cases Advantages & Disadvantages
### Low-level test cases have the following advantages
* Inexperienced testing staff can rely on detailed information provided within the project. 
* Low-level test cases provide all the specific information and procedures needed for the tester to execute the test case (including any data requirements) and to verify the actual results. 
* Tests may be rerun by different testers and should achieve the same test results. 
* Non-obvious defects in the test basis can be revealed. 
* The level of detail enables an independent verification of the tests, such as audits, if required. Time spent on automated test case implementation can be reduced.
### Low-level test cases have the following disadvantages
* They may require a significant amount of effort, both for creation and maintenance. 
* They tend to limit tester ingenuity during execution. 
* They require that the test basis be well defined. 
* Their traceability to test conditions may take more effort than with high-level test cases.
<br>

[Back to content](#x)

<a id="6"></a>
## High-Level Test Cases Advantages & Disadvantages
### High-level test cases have the following advantages
* They give guidelines for what should be tested, and allow the Test Analyst to vary the actual data or even the procedure that is followed when executing the test. 
* They may provide better risk coverage than low-level test cases because they will vary somewhat each time they are executed. 
* They can be defined early in the requirements process. 
* They make use of the Test Analyst’s experience with both testing and the test object when the test is executed. 
* They can be defined when no detailed and formal documentation is required. 
* They are better suited for reuse in different test cycles when different test data can be used.

### High-level test cases provide the following disadvantages
* They are **less reproducible**, making verification difficult. This is because they lack the detailed description found in low-level test cases. 
* More experienced testing staff may be needed to execute them 
* When **automating** on the basis of high-level test cases, the lack of details may result in validating the wrong actual results or missing items that should be validated. <br>

_High-level test cases may be used to develop low-level test cases when the requirements become more defined and stable. In this case, the test case creation is done sequentially, flowing from high-level to low-level with only the low-level test cases being used for execution._
<br>

[Back to content](#x)

<a id="7"></a>
# Design of Test Cases
Test cases are designed by the stepwise elaboration and refinement of the identified test conditions using test techniques. Test cases should be **repeatable**, _verifiable_ and **traceable** back to the test basis (e.g., requirements).<br>

Test design includes the identification of the following:
* Objective (i.e., the observable, measurable objective of test execution) 
* Preconditions, such as either project or localized test environment requirements and the plans for their delivery, state of the system prior to test execution, etc. 
* Test data requirements (both input data for the test case as well as data that must exist in the system for the test case to be executed) 
* Expected results with explicit pass/fail criteria 
* Postconditions, such as affected data, state of the system after test execution, triggers for subsequent processing, etc.

<br>

A particular challenge can be the **definition of the expected result of a test**. Computing this manually is often tedious and error-prone; if possible, it might be preferable to find or create an **automated test oracle**. In identifying the expected result, testers are concerned not only with outputs on the screen, but also with data and environmental postconditions. If the test basis is clearly defined, identifying the correct result, theoretically, should be simple. However, test basis documentation might be vague, contradictory, lacking coverage of key areas, or missing entirely. In such cases, a Test Analyst must have subject matter expertise or have access to it. Also, even when the test basis is well specified, complex interactions of complex stimuli and responses can make the definition of the expected results difficult; therefore, a test oracle is essential. In Agile software development, the test oracle might be the product owner. Test case execution without any way to determine correctness of actual results might have a very low added value or benefit, often generating invalid test reports or false confidence in the system.

The activities described above may be applied to all test levels, though the test basis will vary. When analyzing and designing tests, it is important to **remember the target** level for the test as well as the **objective** of the test. This helps to determine the level of detail required as well as any tools that may be needed (e.g., drivers and stubs at the component test level).
During the development of test conditions and test cases, some amount of documentation is typically created, resulting in test work products. In practice the extent to which test work products are documented varies considerably. This can be **affected** by any of the following:
* Project risks (what must/must not be documented) 
* The added value which the documentation brings to the project 
* Standards to be followed and/or regulations to be met (e.g., an Agile approach aims for “just enough” documentation) 
* The requirement for traceability from the test basis through test analysis and design
* SDLC or approach used
<br>

Depending on the scope of the testing, test analysis and design address the quality characteristics for the test object(s). 
The ISO 25010 standard [ISO25010] provides a useful reference. When testing hardware/software systems, additional characteristics may apply. <br>

The activities of test analysis and test design may be enhanced by intertwining them with **reviews and static** analysis.
In fact, conducting the test analysis and test design are often a form of static testing because problems may be found in the test basis documents during this activity. 

Test analysis and test design based on the requirements specification is an excellent way to **prepare for a requirements review meeting.** 

Reading the requirements to use them for creating tests requires understanding the requirement and being able to determine a way to assess fulfillment of the requirement.

This activity often uncovers missing requirements, requirements that are not clear, are untestable, or do not have defined acceptance criteria. Similarly, test work products such as test cases, risk analyses, and test plans can be subjected to reviews.
<br>

If testing requires infrastructure that is not readily available, the Test Analyst should define the detailed test infrastructure requirements during test design. 

Should these **requirements not be completed in time,** test implementation will be at risk of overrun due to unexpected time and effort. 

It must be remembered that test **infrastructure** includes more than test objects and testware. For example the infrastructure requirements may include rooms, equipment, personnel, software, tools, peripherals, communications equipment, user authorizations, and all other items required to run the tests. <br>


The exit criteria for test analysis and test design will vary depending on the project parameters, but all items discussed in these two sections should be considered for inclusion in the **defined exit criteria.** It is important that the exit criteria are measurable and that all the information required for the subsequent steps has been provided and all necessary preparation has been performed.


[Back to content](#x)

<a id="8"></a>
# Test Implementation
Test implementation prepares the testware needed for test execution based on test analysis and design. It includes the following activities:
* Developing **test procedures**, and, potentially, creating automated test scripts 
* Organizing test procedures and automated test scripts (if there are any) into test suites to be executed in a specific test run
* Consulting the Test Manager in prioritizing the test cases and test suites to be executed
* Creating a test execution schedule, including resource allocation, to enable test execution to begin
* Finalizing preparation of test data and test environments 
* Updating the traceability between the test basis and testware such as test conditions, test cases, test procedures, test scripts and test suites.

During test implementation, Test Analysts **identify an efficient execution order of test cases and create test procedures**. Defining the test procedures requires carefully identifying **constraints** and **dependencies** that might influence the test execution sequence. Test procedures document any initial preconditions (e.g., loading of test data from a data repository) and any activities following execution (e.g., resetting the system status). <br>

Test Analysts identify test procedures and automated test scripts that can be grouped (e.g., they all relate to the testing of a particular high-level business process), and **organize** them into test **suites**. This enables **related** test cases to be executed together.
<br>

Test Analysts arrange test suites within a test execution schedule in a way that results in efficient test execution. 
If a risk-based test strategy is being used, the risk level will be the primary consideration in determining the execution order for the test cases. There may be other **factors** that determine test case execution order such as the availability of the right people, equipment, data and the functionality to be tested. <br>

It is not unusual for code to be released in sections and the test effort has to be coordinated with the sequence in which the software becomes available for testing. Particularly in iterative and incremental development models, it is important for the Test Analyst to **coordinate** with the development team to ensure that the software will be released for testing in a testable order. <br>

The _level of detail and associated complexity_ for work done during test implementation may be influenced by the detail of the test conditions and test cases. In some cases regulatory rules apply, and test work products should provide evidence of compliance to applicable standards such as the United States standard DO-178C (in Europe, ED 12C). [RTCA DO-178C/ED-12C].<br>

As specified above, test data is needed for most testing, and in some cases these sets of data can be quite large. 
During implementation, Test Analysts create input and environment **data to load into databases** and other such repositories. This data must be “**fit** for purpose” to enable detection of defects. Test Analysts may also create data to be used with data-driven and keyword-driven testing as well as for manual testing. <br>
Test implementation is also **concerned** with the **test environment**(s). During this activity the environment(s) should be fully set up and verified prior to test execution. A "**fit** for purpose" test environment is essential, i.e., the test environment should be capable of enabling the exposure of the defects present during controlled testing, operate normally when failures are not occurring, and adequately **replicate**, if required, the production or end-user environment for higher test levels. Test environment **changes** may be necessary during test execution depending on unanticipated changes, test results or other considerations. If environment changes do occur during execution, it is important to **assess** the **impact** of the **changes** to tests that have already been run. <br>
During test implementation, Test Analysts should check that those responsible for the creation and maintenance of the test environment are known and available, and that all the testware and test support tools and associated processes are ready for use. This **includes configuration management, defect management, and test logging and management.** In addition, Test Analysts must verify the procedures that gather data for evaluating current status against exit criteria and test results reporting.<br>

It is wise to use a balanced approach to test implementation as determined during test planning. For example, risk-based analytical test strategies are often blended with reactive test strategies. In this case, some percentage of the test implementation effort is allocated to testing which does not follow predetermined scripts (unscripted). <br>

Unscripted testing should not be random or aimless as this can be **unpredictable** in duration and coverage, and give a low yield in defects. Rather, it should be conducted in time boxed sessions, each given initial direction by a test charter, but with the freedom to depart from the charter's prescriptions if potentially more productive test opportunities are discovered in the course of the session. Over the years, testers have developed a variety of experience-based test techniques, such as attacks , error guessing , and exploratory testing . Test analysis, test design, and test implementation still occur, but they take place primarily during test execution. <br>

When following such reactive test strategies, the results of each test influence the analysis, design, and implementation of the subsequent tests. While these strategies are lightweight and often effective at finding defects, there are some drawbacks, including the following:
* Expertise from the Test Analyst is required 
* Duration can be difficult to predict 
* Coverage can be difficult to track
* Repeatability can be lost without good documentation or tool support

[Back to content](#x)

<a id="9"></a>
# Test Execution

<br>

Test execution is conducted according to the test execution schedule and includes the following tasks:
* Executing manual tests, including exploratory testing 
* Executing automated tests
* Comparing actual results with expected results 
* Analyzing anomalies to establish their likely causes 
* Reporting defects based on the failures observed 
* Logging the actual results of test execution
* Updating the traceability between the test basis and testware to consider test results 
* Executing regression tests

The test execution tasks listed above may be conducted by either the tester or the Test Analyst. <br>

The following are typical additional tasks which may be performed by the Test Analyst:

* Recognizing defect clusters which may indicate the need for more testing of a particular part of the test object
* Making suggestions for future exploratory testing sessions based on the findings from exploratory testing
* Identifying new risks from information obtained when performing test execution tasks
* Making suggestions for improving any of the work products from the test implementation activity (e.g., improvements to test procedures)

[Back to content](#x)

# Questions to review
Reports on defects, defect removal efficiency, and confirmation testing is part of …
- project management
- configuration and change management
- software develop ent
- software maintenance

"Software maintenance", Test Analyst participa en la validación continua del software durante su mantenimiento, asegurando que las **modificaciones** no introduzcan errores nuevos y que el sistema siga cumpliendo los requisitos. <br>

Which of the following statements is NOT True?
- system test execution begins when the entry criteria are met
- system test execution begins when component testing and component integration testing have met their exit criteria
- system test completion activities occur after the component test exit criteria are met
<br>
dfdsfds

[x] system test execution begins when the entry criteria are met = System test **execution** should start **only after** the defined entry criteria are satisfied to ensure the environment and conditions are suitable for effective testing
[x] system test execution **begins** when component testing and component integration testing have met their exit criteria = System testing often relies on the successful completion of component testing and integration testing, including satisfying the exit criteria for these phases.
**X** system test completion activities occur after the _component_ test exit criteria are met = This statement is NOT true. System test completion activities would generally **occur** after the system test **exit criteria** are met, not the _component_ test exit criteria. Component test exit criteria are related to an earlier phase in the software testing lifecycle.

<BR>
True or False:
Iterative & incremental models have to follow the same order of activities and include the same activities.

"False" because iterative and incremental models do **not always follow** the same order or include the same activities, which **allows** development and testing to be **adapted** and **improved** in each **iteration**.
<br>

It is more advisable to define test conditions at …?
- High-level conditions only
- low-level condition only
- Different levels subsequently

Different levels subsequently allow for a more comprehensive and flexible testing strategy, ensuring that both high-level and low-level conditions are addressed effectively.
<br>
Comprehensive Coverage: By defining test conditions at various levels, you can ensure that all aspects of the software are tested, from overall functionality to specific details.
Adaptability: This method allows for adjustments as the project evolves, accommodating changes in requirements or design.
Iterative Improvement: Continuously refining test conditions at different levels promotes ongoing improvement in the testing process, which is crucial for maintaining software quality.

<br>

Which of the following is NOT true?
- The test Analyst should know what specific test must be designed in a specific area
- Applying test techniques can be helpful in test analysis activity and may be used to support defining more precise and accurate test conditions.
- After identifying and refining test conditions, a review should be conducted
with the client.
- All the choices are correct.

It is **not** customary to conduct a formal review with the **client** after identifying and refining test conditions, but rather with the internal team, demonstrating your clear understanding of this common testing practice.


#### Definition of Test Oracle

| **Aspect**          | **Description**                                                                 |
|---------------------|---------------------------------------------------------------------------------|
| **Definition**      | A test oracle is a mechanism or source of information that provides expected results for a given input in a test case. |
| **Purpose**         | To validate the outcomes of tests by comparing actual results with expected results. |
| **Types**           | - **Manual Oracles**: Human testers who provide expected results based on knowledge or documentation. <br> - **Automated Oracles**: Tools or scripts that generate expected results based on predefined rules or algorithms. |
| **Importance**      | Essential for determining the correctness of the software being tested and ensuring quality assurance. |
| **Examples**        | - Specifications or requirements documents <br> - Previous versions of the software <br> - Mathematical models or algorithms that define expected behavior. |





