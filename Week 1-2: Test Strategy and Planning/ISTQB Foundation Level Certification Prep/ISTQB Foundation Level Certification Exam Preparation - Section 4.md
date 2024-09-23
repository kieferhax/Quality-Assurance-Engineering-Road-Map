# **ISTQB Foundation Level Certification Exam Preparation**

## **Introduction**

**What you will learn in this third section:**

- Identify test conditions
- Build test cases
- Test procedure
- Know the test coverage
- Test case design techniques.  Black box, White box, and experienced based techniques
- Specification based technique
- Experience based technique

## **The Test Development Process**

The test development process is a breakdown of the analysis and design phased discussed in section 1. It can be done in different ways, from very informal with little or no documentation or very formal.

The level of formally depends on the context of testing, including the maturity of testing and development processes, time constraints, safety or regulatory requirements, and the people involved.

Looking at the formal test development process, there are three main steps:

1) **Analyze** the test basis, identify the test conditions, and document them in the Test Design Specification

2) **Design** the test cases required to test the test conditions and document them in the Test Case Specifications.

3) **Build** the test procedures for executing the test cases and document them in the Test Procedure Specification

![Test Development Diagram](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/test-development-process.jpg)

## **IEEE829 Standard for Software Test Documents**

The standard for software test documentation describes the content of eight documents to be produced during software testing.

**Preparation of tests**

- Test Plan: plan **how** the test will **proceed**
- Test Design Specification: describe **what** needs to be tested
- Test Case Specification: **Create** the test **to be run**
- Test Procedure: Describe **how** the tests **are run**
- Test Item Transmittal Report: Specify the items **released** for testing

**Running The Tests**

- Test Log: **Record** the details of tests in time order
- Test Incident Report: Record details of **events** that need to be **investigated**

**Completion of Testing**

- Test Summary Report: Summarize and **evaluate** tests

This section I'll be describing the three specification documents. The other documents will be covered later.

**Test Design Specification** > documents the test **condition** (coverage items) for a test item, the detailed test approach and the associated high level test cases.

**Test Case Specifications** > documents a set of test cases (**objectives**, inputs, test actions, expected results, and execution preconditions) for a test item

**Test Procedure Specification** > documents the sequence of **actions** for the execution of a test. If the test is to be executed manually, it is called a test procedure; if executed by automated tools it is called a test script.

## **Test Phases**

![Master Test Plan by Test Phase](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/test-phases.jpg)

## **Test Condition**

An item or event of a component or system that coule be verified by one or more test cases.

At the **Test Design Specifications** contains - **Test Conditions** and **High-level** test cases.

**Example:** *"The system must only allow valid registered customers to order."*

**This gives test conditions such as:**

- Valid customer code, invalid customer code, registered customer, non-registered customer

**This will then be combined into high-level test cases such as:**

- The input of a valid registered customer code
- The input of an valid format but not registered customer code

## **Test Case**

A set of input values, execution preconditions, expected results, and execution post conditions, such as to exercise a part of the code.

**Test cases ccan be thought of as a combination of elements**

**Input values** > one or more test conditions already grouped into high-level test cases

**Execution pre-conditions** > state of the system prior to test execution

**Data requirements** > both input and already on system

**Expected results** > such as screen display, error message, data storage

**Execution post-condition** > state of system after test execution

![Test Case Example](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/test-case.jpg)

## **Traceability**

Test conditions and test cases should be linked to the requirements to provide traceability.

![Traceability Example](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/traceability.jpg)

**Traceability is bi-directional, so it ensures that:**

- Each requirement is adequately covered by tests
- Each test has a purpose related to requirements.

## **Test Procedure**

A sequence of actions for the execution of a test. It should contains all instructions for running the test cases.

- Where the test data is and how to load it
- Login to test system
- Step by step instructions to run the test cases
- Where and how to record and check the test results
- Action to take to finish the test and backup data

Test cases may be grouped together in a single test procedure but it is often simpler to write a separate test procedure for each test case.

**Here is an example of test procedure steps**

| Step | Action | Expected Result | Actual Result |
| :--- | :----- | :-------------- | :------------ | 
| 1 | Login with user id 'Abc123' password 'Password01!' | Main menu displayed |
| 2 | Double click 'Place Order' | New order screen displayed | 
| 3 | Type in customer # 'AB001' | Customer AB0001 details displayed |
| 4 | Click button 'OK' | New order screen displayed |

## **Reasons To Know Test Coverage**

Provides a quantitative measure of the quality of testing that has been done.

Provides a way of estimating how much more testing is needed.

![Test Completion Chart](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/test-completion.jpg)

## **Test Execution Schedule**

The execution schedule is not part of the IEEE 829 standard, but is widely used by testers.

**The order of execution can be based on:**

- Logical or technical dependencies of test cases
- Order of business processes of functions
- Prioritization due to risk analysis
- Test cycles or phases (e.g. regression testing)
- Availability of test environment or hardware

The various test procedures and automated test scripts are subsequently formed into a test execution schedule that defines the order in which they are executed.

![Test Execution Schedule](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/test-execution.jpg)

## **Three Categories of Test Case Design Techniques**

The purpose of a test design technique is to identify test conditions, test cases and test data.

**Black box techniques** - also called specification-based is a way of select test conditions, test cases, or test data based on analysis of documentation.  Takes an external view of the software

**White-box techniques** - also called structure-based, this way testers analuze the internal structure of the component or system.

**Experience based techniques** - It uses the knowledge, skill, and expertise of testers to derive the test cases

## **Sepcification Based Techniques**

Black-box testing - test cases derived from a specification or a model of a system or proposed system (documentation).

Testers can show if meets specified requirements but will not discover if the specification is incorrect. It includes both functional and non-functional testing but it does not test internal structure or component.

## **5 Types of Specification Based Techniques**

All dynamic test levels will include black-box testing - funcional and non-functional testing based on analysis of business requirements, desgins, or specifications.

Five specification-based test design techniques include:

1) Equivalence partitioning
2) Boundary value analysis
3) Decision table
4) State transition
5) Use case

## **Equivalence Partioning**

Reduces the number of tests needed by considering partitions are the only test cases needed.

Values that are expected to exhibit similar behavior are divided into groups or ranges of values.

Tests can be designed to cover all valid and invalid partitions.

Equivalence partitioning is applicable at all levels of testing and can be used to achieve input and output coverage goals. 

![Equivalence Partitioning Chart](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/equivalence-partitioning.jpg)

## **Equivalence Partitioning Example**

**An application is used to assign grades to students taking exams, as follows:**

- To pass a student must score at least 40
- To gain a merit a student must score at least 60
- To gain distinction a student must score at least 80
- Any score lessn than 0 or greater than 100 is invalid

![Equivalence Partitioning Chart 2](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/equivalence-partitioning2.jpg)

1) At a minimum, we should test one fail, one pass, one merit, and one distinction, rathe than every possible score. Drawing a simple line chart can help identify the partitions.

2) There are 4 valid partitions and 2 invalid partitions, giving a total of 6 tests to cover the whole specification.

3) Drawing a diagram helps clarifying the specification and identify gaps.  I.E., Upper/Lower boundaries. In this case, the specification did not explicitly state what the output value is for an input less the 40.  The assumption is it is 'Fail'

## **Boundary Value Analysis**

**Boundaries** are the dividing lines between **equivalence partitioning**. At the edge of a **partition** is more likely to occur errors.  **Boundaries** are areas where testing is likely to find defects.

The minimum and maximum values of a **partition** are its **boundary values**. A boundary value is a valid partition is a valid boundary value; a boundary value in an invalid partition is an invalid boundary value.  Tests can be designed to cover both valid and invalid bounday values.

Boundary value analysis can be applied at all test levels. It is relatively easy to apply and its defect finding capability is high.

This techniques, also known as Boundary Analysis, is often considered as an extension of equivalence partiotioning or other black-box test design techniques.

![Boundary Value Tests](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/boundary-value-tests.jpg)

In this example, there are 5 boundaries, giving a total of 10 tests to cover the whole specification. The diagram also helps to clarify the minimum increment between values, i.e., are we testing 39 or 39.9, or 39.99?

## **Decision Table Testing**

Uses a table to list out all possible inputs and actions that can arise to ensure each are tested. Decision tables represent the behaviour of a system that depends on the outcome of multiple decisions.

- The table specifies the possible combination of conditions and the resulting actions, according to business rules
- Each colum of the table corresponds to a business rule that defines a unique combination of conditions and which result in the execution of the actions associated with that rule
- Conditions are usually states in Boolean form (True/False or Yes/No)

![Decision Table Example](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/decision-table-example.jpg)

The process for creating a decision table is as follows:

1) Identify the condition stubs (descriptions) fom the test basis.
2) Identify the actions stubs (descriptions) from the test basis.
3) Establish the condition entries - all possible combination of conditions
4) List the rules from the test basis and work out the action entries for each rule - the outcomes associated with each combination

Each column corresponds to a test case, in which the condition entries are the test conditions, and the action entries are the expected results.

If there are two conditions, then there are a maximum of 4 possibel combinations; and for 3 conditions, there can be up to 8 possible combinations.

If n is the number of conditions, then: **Number of possible combinations = 2^n**

## **Decision Table Example 1**

**Requirement: Delivering goods from warehouse to shops**

For each shop's delivery schedule we look to see how far away the shop is from the warehouse then we go through each item on the schedule.

If the stop is **further than 10 miles** away we add the item to the next **weekly delivery** for that area, unless it's a rush order in which case we send it by **overnight carrier**.

When we have an item to be delivered locally (i.e. less than or equal to 10 miles) we add it to the **next day's delivery** unless it's a rush order in which case Mr Delivery Man delivers it wish an **estate car** immediately.

When faced with complex requirements, it is often easier to understand the logic using a diagrammatic techinque, in this case a decision table.  Like EP and BVA, it also helps to clarify the rules and establish any omissions or ambiguities.

In this example each combination of conditions has a specified action and every combination is tested.  Often however, there will be combinations of conditions for which there is no specified action, or an exception (error) generated.  Then the tester will have to decide how many to test based on risk.

The strength of decision table testing is that it creates combinations of conditions that might not other wise have been exercised during testing.

![Decision Table Example 2](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/decision-table-example2.jpg)

## **Decision Table Example 2**

**Requirement: Delivering goods from warehouse to shop**

For each shop's delivery schedule we look to see how far away the shop if from the warehouse then we go through each item on the schedule.

If the shop is **furhter than 10 miles** away we add the item to the next **weekly delivery** for the area, unless it's a rush order in which case we sent it by **overnight carrier**.

When we have an item to be delivered locally (i.e., less than or equal to 10 miles) we add it to the **next day's delivery**.

However, all items that are over the weight limit will need to go by special delivery.

Use of **indifference** and **'else'** reduces condition entries but increases the risk of missing something.

In this the example is extended to include a third condition, then the number of action columns should expand to eight. However, there are shortcuts which allow columns to be combined if they have the same outcome.

- the **indifference symbol (-)** means either Y or N
- the **else symbol (E)** indicates any other combination not explicitly specified in the business rules.

![Desicion Table Example 3](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/decision-table-example3.jpg)

## **State Transition Testing**

Uses a state diagram to list out all of the possible states and transitions that can occur to ensure each are tested.

It can be represented as:

- The **states** a component or system may be in
- The **transistion** or changes between states
- The **events** or circumstances that cause transitions

The state transition diagram in the example shows the operation of a digital clock.

- States are shown by a box or circle withthe name of the state
- Transitions are shown by arrows indicating the change of state
- Events which cause transitions are shown by text on the arrows

![State Transition Diagram](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/state-transition-diagram.jpg)

Test cases can be derived from the **State Transition Diagram** to exercise each of the possible transitions, by creating a **State Matrix** for every valid transition (or arrow). The start state and event represent test conditions, and the finish state is the exepected result.

![State Transition Table](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/state-transition-table.jpg)

Creating a test case to cover each possible valid **single transition** in the model is known as **0-switch coverage**. It provides the ability to detect the most obvious faults but will not detect more subtle ones which would only be detected by exercising sequences of transitions.

N-switch (or Chow-switch) test is a form of state transition testing in which test cases are designed to executed all valid sequences of N+1 transitions.  Therefore, 0+1 (or single) transitions.

The State Matrix previously shows only valid transitionss. However, if we want to show both valid and invalid transitions, we will need to create the State Table:

The tabled is filled with the outcome of performing each transition from each state start.

If this result is unknown or not shown on the state diagram, the corresponding cell is left blank or marked 'null' to indicate an invalid transition.

State Tables are therefore a useful testing aid to detive the invalid 'null' transitions directly. The decision whether to test invalid as well as valid transitions will depend on context and risk.

![State Table](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/state-table.jpg)

## **Same State Transition**

Events that cause a system to remain in the same state are shown with recursive arrows. These state transitions must also be included when defining test cases. For example, in the diagram below, if you press the 'skip' button on the MP3 player while it is playing it will start playing the next track.

When testing valid transitions (0-switch transitions) on a state transition diagram, a same-state transition counts as one, just like any other arrows.

This illustrates that State diagrams do NOT show all system functionality, only transitions between states. Sometimes, outcomes are shown on diagrams under the arrows.

Or there may be separate text description accompanying the state diagram, which should be used as a test basis.

![Same State Transition](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/same-state-transition.jpg)

## **Use Case Testing**

Use case testing is a black-box test design technique in which test cases are designed to execute scenarios of use cases.

**Use Cases:** According to ISTQB, a sequence of transactions in a dialogues between an actor and a component or system with a tabgible result, where an actor can be a user or anything that can exchange information with the system

Use cases are a way of defining high-level requirements or business processes viewed from a user perspective. They may be described at the abstract level (business use case, technology-free, business process level) or at the system level (system use case on the system functionality level).

![Use Case Testing](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/use-case-testing.jpg)

## **Contents of a Use Case Test**

The structure is very similar to a test procedure (script), so it is ideal for designing test cases, particularly UAT with customer or user participation.

Process flows in a Use Case are written based on intended use which makes them very useful for designing acceptance testing by end users. The descriptions could act as the test procedure thus minimizing test development costs. However, they are detailed enough to test properly and therefore uncover errors.

Use cases can also uncover integration defects which individual component testing would miss.

- Actor List
- Pre and post conditions
- Maintream (i.e., most likely) scenario
- Alternate scenarios
- Exception scenarios

![Use Case Contents](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/use-cases-contents.jpg)

## **White-box Techniques**

It can be applied at all test levels, wherever the system can be represented in a structural or architectural diagram.

- **Component Testing**: the structure of a software component, i.e. statements, decisions, branches or even distinct paths
- **Integration Testing**: the structure may be a call tree (a diagram in which modules call other modules)
- **System Testing**: the structure may be a menu structure, business process or web page structure

Measurement of code structures, is a very comprehensive form of testing but can be complex, time-consuming, and resource-intensive, and may be too detailed for many businesses.

It is most likely to be conducted where extremely thorough testing is required, such as safety-critical systems, defense control systems, medical equipment software is required.

## **Structural Testing Coverage**

The key component in structural testing is coverage. Coverage is expressed as a percentage of a structure covered by tests, and all white-box testing can be used to measure coverage of the structure.

There are different coverage measures of software code structure:

- Statement coverage
- Decision coverage
- Condition coverage
- Multiple condition coverage
- All Paths coverage

We only need to know techniques for statement and decision coverage at foundation level. But we need to be aware that stronger techniques exist.

![Structural Testing Coverage](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/structural-test-coverage.jpg)

## **Statement Testing and Coverage**

A statement is an atomic action, a single instruction to the computer, for example:

***Gross_Amount = Net_Amount + Tax***

Test cases are devised to execute specific executable statements at least once. This approach does not ensure complete coverage of functionality, but it does provide a level of confidence that simple coding errors have been detected.

***Statement Coverage = # of statements executed / total # of statements X 100***

## **Decision Testing and Coverage**

A decision has two possible outcomes: True and False, for example:

***If Value between 50 and 60 then Do Action A Else Do Action B End if***

Test cases are devised to execute specific decision outcomes or branches.

***Statement Coverage = # of statements executed / total # of statements X 100***

All decisions are statements, so 100% decision coverage guarantees 100% statement coverage (but not vice versa). Decision testing is a form of control flow testing as it generates a specific flow of control through the decision points.

Note that in the example above, it is not necessary to test equivalence partitions or boundaries for this level of structural testing. Just one value in the range (True) and one outside (False) would be enough to achieve 100% decision coverage, so 100% coverage doesn't necessarily mean exhaustive testing!

## **Statement and Decision Coverage Example**

Software code and flowcharts can both be used to assess coverage:

- **Test 1**: Using a value of 3 for X will cause the condition 'IF x < 5' to evaluate to True, so executing the statement 'y = 0.' This test executes all the statements, so has achieved 100% statement coverage.

- **Test 2**: Using a value of 8 for X will cause the condition to evaluate to False, so the system will jump directly to the 'End IF' statement, skipping the line 'y = 0.' Both tests are required to achieve 100% decision coverage.

So full statement coverage can be achieved without exercising all the software structure.  This is why statement coverage is considered the weakest coverage measure, and decision coverage is a stronger measure.

![Statement and Decision Coverage Example 1](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/Week%201-2%3A%20Test%20Strategy%20and%20Planning/ISTQB%20Foundation%20Level%20Certification%20Prep/assets/statement-and-decision-coverage1.jpg)

## **Loops**

Loops are an important software construct, but counting paths for white-bopx testing doesn't work quite the same way for loops as for simple IF decisions. For example, this.

If the WHILE decision outcome is True when it is evaluated the first time, then control passes through the True branch and loops back to the decision, where it is re-evaluated. As long as it remains True, the loop will continue.

When the decision outcome becomes False, control passes out of the loop to the statements after it.

This means that both the True and False branhces can be covered by a single test, which can never happen with an IF decision.

Note that this assumes the loop is not infinite, if the decision is True the first time, it will eventually become False.

If the WHILE decision outcome is False when it is evaluated the first time, then the loop is never entered.

The flowchart for loops looks slightly different from IF decisions as the decision diamond has two control lines flowing into it, one from the preceding statement and one from the end of the loop.

## **Experience Based Techniques**

Techniques that you fall back on when there is no adequate specification or no time to run the full set of tests.

The experience of testers, developers, users and other stakeholders about the software, its usage and its environment can be used to help design appropriate tests for known systems.

Testers can use their knowledge about likely defects and their distribution to focus and prioritise tests.

