# **ISTQB Foundation Level Certification Exam Preparation**

## **Introduction**

**What you will learn in this first section**

- Why Testing?
- Causes of software defects
- Tester objectives
- Testing and debugging
- Principles of testing
- Test activities
- Retesting
- Resource triangle
- Completion criteria
- Static and dynamic testing
- Testing independencies
- Code of ethics

## **What is ISTQB**

- ISTQB, International Software Testing Qualification Board
- Founded in 2002
- Is a world wide **leader** in the certification of software testing
- The goal of ISTQB is to continually **improve** and advance the software testing **profession**
- **Certification** knowledge is based on **best practices**, the community of software testers and **continuously** researching in the subject matter.

## **What Will You Learn**

**Foundation level professionals should be able to:**

- Use a **common** language for **efficient** and **effective communication** with other **testers** and project **stakeholders**
- **Understand** established testing **concepts**, the fundamental test **process**, test **approaches**, and **principles** to support test **objectives**
- **Design** and **prioritise** tests by using established **techniques**
- **Analyse**f both **functional** and **non-functional** specifications at all test levels for systems with a **low** to **medium** level **complexitiy**
- **Execute** tests per agreed **test plans**, **analyse**, and **report** on the **results** of tests
- **Write** clear and **understandable** incident **reports**
- **Effectively** participate in **reviews** of **small** to **medium-sized projects**
- Be **familair** with different **types** of testing **tools** and their uses
- **Assist** in the **selection** and **implementation** process

## **Course Structure**

The course is divided into **6 sections** following the **ISTQB syllabus structure**, which consists of **6 chapters**.

## **Course Objectives**

1. **Remeber** - Recognize, remeber, and recall a term or concept
2. **Understand** - Can select the reasons or explanations for statments related to the topic and summarize, diffentiate, classify, and give examples.
3. **Apply** - Select the correct application of a concept or technique and apply it to a given context
4. **Analyze** - Separate information related to a procedure or techqniue into its constituent parts for better understanding and distinguish between facts and inferences.

## **Fundamentals of Testing - Section 1**

## **Section 1 Intro**

**What you will learn in this first section**

- Why testing?
- Causes of software defects
- Tester objectives
- Testing and debugging
- Principles of testing
- Test activities
- Retesting
- Resource triangle
- Completion critieria
- Static and dynamic testing
- Testing independencies
- Code of ethics

## **Why Testing is Necessary**

**People make mistakes due to fallibility but also other pressures including:**

- Attention to detail
- Time constraints
- Lack of knowledge
- Experience

Software (program code) is present everywhere.

From banking, e-commerce, cars, electrical appliances, arms, heating systems, and many more.

Failure results in financial loss, waste of time, loss of reputation or, in worst cases, injury and death.

Testing reduces the risk of software failure.

## **Causes of Software Defects**

**Error:** Humans make **mistakes** in code.

**Defect:** A problem casued by an **error**.

**Fault:** A **failure** of the system or component caused by a **defect**

**Failure:** Failures don't only happen due to **defects**, but also environmental conditions, hardware failures, etc.

All defects start with a human error (for example a typo, midunderstanding, lack planning, capability, etc.).

The tester's job is to expose the defect by causing a failure before the software gets to production

## **Objectives of Testing Software**

- Avoid and rectify errors.
- Ensure that key functional and non-functional requirements are examined.
- Testing is not about removing defects, but about notifying developers about them.
- Testing is also about reducing risk in releasing

Testing can give confidence in the quality of the software if it finds few or no defects.

Tests can and must be measured. Typical measurements are:

- Number of defects found
- Number of failures in a given time period (reliability)
- Usability testing
- Mantainability

## **Difference Between Testing and Debugging**

**Debugging** is a process used to identify casues of bugs in code and **correct them**.

**Testing** is the exploration of the system in order to **find defects**

![Testing vs Debugging](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/1.%20Test%20Strategy%20and%20Planning/assets/testing-vs-debugging.jpg)

## **Fundamental Principles of Testing**

1. Testing shows the presence of bugs
2. Exhaustive testing (testing all possible data combinations) is impossible
3. Early testing saves money
4. Defect clustering happens. If there is a bug in one part of the software, chances are there are other, related bugs nearby.
5. The 'pesiticde paradox': continuing to run the same tests won't find new bugs
6. Testing is context dependent. Testing is done differently in different context.
7. Software with no known errors is not necessarily ready to be shipped. Does it match user/business expectactions?

## **Five Fundamental Test Activities And Tasks From Planning To Test Closure**

1) Planning and Control: **Planning** - Verify the mission of testing. **Control** - Monitor, check progress, and take action.

2) Analysis and Design: Test **analysis** and test **design** - testing objectives to create test conditions and test designs.

3) Implementation and Execution: Activity where **test procedures** or scripts are in order, the **environment** is setup and **tests** are **run**.

4) Evaluating Exit Criteria and Reporting: Activity where **test execution** is assessed against the defined **objectives**.

5) Test Closure Activities: Occurs at project **milestones** such as **release**, **completion, cancellation,** or **maintainence** release has been complete.

![Five Fundamental Test Activities](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/1.%20Test%20Strategy%20and%20Planning/assets/test-activities.jpg)

## **Restesting and Regression Testing**

- Retest - running the tests again after they fail and the bugs have been in theory fixed

- Regression - running testing to check the cross impact of defect fixes in the whole functionality or system

![Retest and Regression](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/1.%20Test%20Strategy%20and%20Planning/assets/retesting-and-regression.jpg)

## **Resource Triangle**

Time, Cost, and Quality.

You can't have them all, you can only pick **two**.

You are given the options of ***Fast***, ***Good***, and ***Cheap***, and told to pick any two.

Here *fast* refers to the **time** required to deliver the product.

*Good* is the **quality** of the final product.

*Cheap* refers to the total **cost** of designing and building the product.

This triangle reflects the fact that the three properties of a project are interrelated, and it is not possible to optimize all three - **one will always suffer**.

In other words, you ahve three options:

1. Design something quickly and to a high standard, but then it will not be cheap.
2. Design something quickly and cheaply, but it will not be of high quality.
3. Design something with high quality and cheaply, but it will take a relatively longer time.

![Resource Triangle](https://github.com/kieferhax/Quality-Assurance-Engineering-Road-Map/blob/main/1.%20Test%20Strategy%20and%20Planning/assets/scope-triangle.png)

## **Completion Criteria**

Criteria you set at the beginning of a project that determines when it is safe to stop testing.

Exit criterion is conencted to the test coverage, test case design technique adopted, risk level of the product varies from one test level to another.

- Specified coverage has been achieved
- No showstoppers or critical defects
- There are very few known medium or low priority defects that don't affect the usage of the product
- If Exit criterion has not be meat, the test cannot be stopped.
- The Exit criterion has to be revamped or the time should be extended for testing based on the quality of the product
- Any changes to the test completion criterion must be documented and signed off by stakeholders.
- The test ware can be released upon successful completion of exit criteria.

## **Static and Dynamic Testing** 

**Static** - Testing where code is not executed: document specification analysis, reviews, even code itself, etc. Can be done as **review** by humans carrying out **manual** examination of documents or **Static Analysis** of the code and software models by using **automation** tools

**Dynamic** - Kind of testing that executes the program code with some **test data**. Dynamic testing is performed by executing **software under test** and comparing actual and expected results.

## **Testing Independnce**

Developers are least independent, wheras outsourced testing companies are most independent, because they don't take defects as criticism.

Several levels of independence can be defined as shown below:

- Tests designed by the person(s) who *wrote the software* under test
- Tests designed by another person(s) within the *developement team*
- Tests designed by a person(s) from a *different organizational group* or *test specialists*
- Tests designed by a person(s) from a *different organization or company*

## **Code of Ethics**

Involvement in software testing enables individuals to learn confidential and privileged information. A code of ethics is necessary, the ISTQB states the following code of ethics:

- Public: testers shall act consistently with the public interest
- Client and Employer: testers shall act in a manner that is in the best interests of their client and employer, consistent with the public interest.
- Product: testers shall ensure that the deliverable they provide meets the highest professional standards possible
- Judgement: testers shall maintain integity and independence in their professional judgement
- Management: test managers and leaders shall subscribe to and promote an ethical approach to the management of software testing
- Profession: testers shall advance the integrity and reputation of the profession consistent with the public interest.
- Colleagues: testers shall be fair to and supportive of their colleagues, and promote cooperation with software developers.
- Self: testers shall participate in lifelong learning regarding the practice of their profession and shall promote an ethical approach to the practice of the profession.

# **Summary**

This is what you have learned so far:

- Why testing is necessary
- Common casues for software defects
- What is testers objectives
- Differences between testing and debugging
- Fundamental principles of testing
- Five fundamental test activities and tasks for planning closure
- Why retesting is one of the most important tasks in testing
- Resource triangle: money, time, quality
- Definition of completion criteria
- When to carryout static and dynamic testing
- Why it is important to get testing independence
- Why the code of ethics is necessary

# **Section 1 Quiz**

1) A human action that produces an incorrect result is called:
    - An error

2)  A deviation of the software from its expected delivery or service is:
    - A failure

3) Which of the following statements are true?
    - Failures can be caused by environmental conditions such as radiation
    - Defects, bugs and faults are the same thing

4) Which of the following statements is true?
    - Testing can show failures that are caused by defects

5) Static tests are:
    - Reviews of documents of code

6) Which of the following statements apply to testing and which to debugging?
    1) Investigates the cause of a fault
    2) Identifies failures
    3) Confirms whether a failure has been fixed
    4) Fixes software if necessary
    5) Checks the defect has been fixed
    6) Steps through program code
        -  2 and 3 are testing; 1, 4, 5, 6 are debugging


7) Who would usually perform debugging activities?
    - Developers


8) An unlikely objective for a test is
    - To prove there are zero defects.

9) Which is not a testing principle?
    - Functional testing

10)  The Test Closure phase of a testing project begins when
    - The exit criteria have been met

11) Which activity in the fundamental test process creates test suites for efficient test execution?
    - Implementation and execution

12) During which fundamental test process activity do we determine if more tests are needed?
    - Evaluating exit criteria and reporting

13)  Which activities from part of test planning?
    - Defining the overall approach to testing
    - Determining the required resources
    - Implementing the test strategy

14) Independence in testing means
    - Someone other than the developer designing the tests

15) Meeting between developers and testers
    - Are for constructive communication of defects

16) One key reason why developers have difficulty testing their own work is:
    - Lack of objectivity

17) Which of the following is a benefit of independent testing?
    - Independent testers see other and different defects and are unbiased

18) Which of the following has the highest level of independence? Test cases which are designed by:
    - A person from a different organization

19) Which of the following is not part of the Code of Ethics?
    - Financial

20) Which, in general, is the skill least required of a good tester?
    - Able to write software
