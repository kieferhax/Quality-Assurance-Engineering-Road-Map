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

![State Transition Diagram]()