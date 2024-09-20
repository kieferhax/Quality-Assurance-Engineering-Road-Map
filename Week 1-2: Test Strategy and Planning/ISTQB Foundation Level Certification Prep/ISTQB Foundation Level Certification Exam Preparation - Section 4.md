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

## **Traceability**

Test conditions and test cases should be linked to the requirements to provide traceability.

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

## **Test Execution Schedule**

The execution schedule is not part of the IEEE 829 standard, but is widely used by testers.

**The order of execution can be based on:**

- Logical or technical dependencies of test cases
- Order of business processes of functions
- Prioritization due to risk analysis
- Test cycles or phases (e.g. regression testing)
- Availability of test environment or hardware

The various test procedures and automated test scripts are subsequently formed into a test execution schedule that defines the order in which they are executed.

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

## **Equivalence Partitioning Example**

**An application is used to assign grades to students taking exams, as follows:**

- To pass a student must score at least 40
- To gain a merit a student must score at least 60
- To gain distinction a student must score at least 80
- Any score lessn than 0 or greater than 100 is invalid

| Invalid | Fail | Pass | Merit | Distinction | Invalid |
| :-----: | :--: | :--: | :---: | :---------: | :-----: |
|  -1     |  20  |  40  |  60   |     80      |   101   |

1) At a minimum, we should test one fail, one pass, one merit, and one distinction, rathe than every possible score. Drawing a simple line chart can help identify the partitions.

2) There are 4 valid partitions and 2 invalid partitions, giving a total of 6 tests to cover the whole specification.

3) Drawing a diagram helps clarifying the specification and identify gaps.  I.E., Upper/Lower boundaries. In this case, the specification did not explicitly state what the output value is for an input less the 40.  The assumption is it is 'Fail'

## **Boundary Value Analysis**

**Boundaries** are the dividing lines between **equivalence partitioning**. At the edge of a **partition** is more likely to occur errors.  **Boundaries** are areas where testing is likely to find defects.

The minimum and maximum values of a **partition** are its **boundary values**. A boundary value is a valid partition is a valid boundary value; a boundary value in an invalid partition is an invalid boundary value.  Tests can be designed to cover both valid and invalid bounday values.

Boundary value analysis can be applied at all test levels. It is relatively easy to apply and its defect finding capability is high.

This techniques, also known as Boundary Analysis, is often considered as an extension of equivalence partiotioning or other black-box test design techniques.

| Invalid | Fail   | Pass    | Merit   | Distinction | Invalid |
| :-----: | :----: | :-----: | :-----: | :---------: | :-----: |
|   < 0   | 0 - 39 | 40 - 59 | 60 - 79 | 80 - 100    | > 100   |

In this example, there are 5 boundaries, giving a total of 10 tests to cover the whole specification. The diagram also helps to clarify the minimum increment between values, i.e., are we testing 39 or 39.9, or 39.99?

## **Decision Table Testing**

Uses a table to list out all possible inputs and actions that can arise to ensure each are tested. Decision tables represent the behaviour of a system that depends on the outcome of multiple decisions.

## **Decision Table Example**
![Decision Table Example](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/1.%20Test%20Strategy%20and%20Planning/assets/decision-table-example.jpg)
