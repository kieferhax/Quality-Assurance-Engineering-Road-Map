# **ISTQB Foundation Level Certification Exam Preparation**

## **Introduction**

**What you will learn in this second section**

- Software Testing Methodologies; Waterfall, V-Model,  and Iterative
- What is unity or component system testing
- What does integration, system and acceptance mean
- Difference between functional and non-functional testing
- What is structural testing
- Change-related testing
- Maintenance testing 

## **Life Cycle Models**

**Sequential Life Cycle Models**

In sequential models the entire system is built in a single sequence of activities that successively define, build, test, and implement the software.

Examples are waterfall, Structured System Analysis and Design Model (SSADM), the V-model, and the W-model.

**Iterative-Incremental (Agile) Life Cycle Models**

In iterative-incremental development models, systems are built in a series of short development cycles which deliver working systems in a number of separate increments that can later be integrated together.

Agile development is a term for several methodologies including Scrum, Crystal Clear and many more.

Each has its specific approach but all share the common vision and core values as continuous planning, testing, integration, for the project and software. Is adaptable and focuses on empowering people to collaborate and make decisions together quickly and effectively.

## **Life Cycle Model Categories**

Testing does not exist in isolation.  Test activities are related to software development activities. Different development life cycle models, methodologies, need differetn approaches to testing.

There are many system development life cycle models, which fall into two main categories:

**Sequential**

- Waterfall
- V-model

**Iterative-Incremental (Agile)**

- Rapid Application Development (RAD)
- Rational Unified Process (RUP)
- Extreme Programming (XP)
- Scrum
- Cynamic Systems Development Method (DSDM) Atern

## **Waterfall Model**

Life cycle through which a project goes.  Squential or linear design process. Testing is carried out at the end.

1) Initiation
2) Analysis
3) Design
4) Build
5) Test
6) Deploy

This is the traditional approach to systems development.  Each stage is quite separate, carried out by specialists, and each must complete before the next begins. Each stage outputs a deliverable which is input to the next step.

All testing is done at the end, after the code is developed. Therefore this model does not allow for early testing, as recommended in the principles earlier.

## **V-model**

There's many variations of V-model, with slightly different numbers and descriptions of levels.  The ISTQB Foundation exam syllabus refers to a model with 4 test levels:

1) Component Testing
2) Integration Testing
3) System Testing
4) Acceptance Testing

The goes on to describe two different integration test levels, so in this demonstration, I'll describe a V-model with 5 levels of testing instead:

1) Component Testing
2) Component Integration Testing
3) System Testing
4) System Integration Testing
5) Acceptance Testing

**V-Model**

*Static*

- Business Requirements
- Interface Specifications
- Systems Specifications
- Design Specifications
- Component Specifications
- Source Code
- Object Code

*Dynamic*

- Component Testing
- Component Integration Testing
- System Testing
- System Integration Testing
- Acceptance Testing

Although the similarities with the sequential method as in waterfall, the V-model includes a number of different test levels, each corresponding to a development stage. This allows testing activities to be fully integrated with other tasks in the project life cycle.

Mini cycles show the purpose of each test level, and show the importance of catching defects early.

The V-model also shows how static testing can be carried out during the development stages, before the code is written. Documents are identified which can be reviewed to trap faults as early as possible.

## **Iterative-Incremental (Agile) Models**

A software design model where the stages are ongoing opposite to the watefall method. Testing occurs as part of each sprint.

Agile development is an umbrella term for several iteative and incremental software development methodologies.

Most popular agile methodologies are: Scrum, Crystal Clear, XP (Extreme Programming), DSDM, and FDD.

Typically, development teams work closely together with fewer formal documents and more emphasis on face-to-face communication.

This minimises overall risk and allows the project to adapt to changes quickly.

## **Unity or Component Testing**

Tests individual units or pieces of code for a system. the aim of component testing is to determine whether an individual functino works properly in isolation before integration with the system and combining it with other components.

Component testing is different from all later test stages as it is **not** done by testers but by the developers of the code, the the developer's environment using IDE, debugging tools and test frameworks incorporating stubs and drivers.

## **Integration Testing**

Performed to ensure that two modules operate together correctly.  The aim is to test all major interfaces and interactions between the individual components, and to uncover communication failures between components.

It should **not** test teh functionality within the component (by this time it has already been done by component testing), only focusing how it communicates with each other.  It is normally performed by developers in the development environment.

V-model document: **Design Specification** and **Component Integration** testing.

## **System Testing**

Tests the various parts of the application to ensure they are working together within a system of work.  This tests the behavior of an end-to-end integrated ssytem as defined by the scope of a development project. It is usually conducted by independent testers.

System testing may include tests based on risks, requirements, business processes, use cases or high level text descriptions, models, or system behavior, interactions with the operating system and system resources.

The test environment should be as close to the production environment as possible in order to minimize the risk of environment-specific failures not being found in testing.

V-model document: **System Specification** and **System Testing**

## **System Integration Testing**

Most computer systems will link with other systems, either internally to the organization or externally.

The purpose of system integration testing is to expose defects in the interfaces and interactions between systems and between hardware and software.

It is normally carried out once system testing is completed by independent system testers in a near live environment.

When testing links with external systems, testers may control only their own side of the interface, which might be considered a risk, as their test system may be linked to an external production system.

Workflow implementation of business processes may involve a series of systems, where cross platform issues may be significant.

## **Acceptance Testing**

To determine whether the product indeed satisifies its specification and user story requirements.

The purpose of acceptance testing is to establish confidence and main focus is ensuring it is fit for purpose, not finding defects.

Acceptance can be carried out by real business users or by independent testers representing users.

Acceptance testing is normally the final stage of testing before deploymebnt.

V-model document: **Business Requirements** and **Acceptance Testing**

## **Functional Testing**

Testing what the system does, based on analysis of specified requirements.

Functinoal testing is concerned with WHAT the system must do to achieve its objectives, as defined in business requirements, functinoal specifications, use cases, business process models, etc.

It considers the external behavior of the software, hence is black-box testing.

Functional testing is usually associated with data manipulation, such as input, validation, processing, storage, and output.

## **Non-Functional Testing**

Testing how well the system meets the required software characteristics such as performance and usability.

It tests the attributes of a system that do not relate to functinoality.  It is concerned with how well the system works.

It considers constraints on the functionality on how, how often, who, or where a function can take place.

Non functional testing includes:

- Performance
- Load
- Stress
- Usability
- Accessibility
- Maintainability
- Reliability
- Portability

## **Structural Testing**

Testing that takes into account the internal mechanism (structure) of a system or component.  Types include branch testing, path testing, and statement testing.

Structural testing, it is sometimes called glass box, usually follows specification-based tests to ensure thoroughness of coverage. 

Full structured testing is very thorough but time consuming, and is often mandated in safety-critical systems such as life support machines.

Coverage measurement applies at all levels, as any aspect of a system which can be represented in a structural diagram and can be used as the basis for structural testing.

- Program code design: coverage of statement, decisions, and paths.
- Component hierarchy diagram: coverage of component interfaces.
- Web pages structure: coverage of page navigation

## **Change-related Testing**

Testing a system following modifications or corrections: includes re-testing and regression testing.  This is testing following a change or fix to the software or environment. This should involve two types of test:

**Re-testing** or confirming testing, that **Reruns** test cases that previously failed in order to verify the success of corrective actions.

**Regression Testing** of a previously tested program following modification to ensure that defects have not been introduced or uncovered in unchanged areas of the software as a result of the changes made. An estimated 20% - 50% of changes introduce new defects. It may be performed at all test levels and types, including functinoal, non-functinoal and structural testing. Regression should take place at all stages of testing after a functinoal improvement or repair.

**Automation** testing, this is an advanced level for new testers. Retesting and regression should be repeatable, so they can re-run every time there is a change or fix.  It is essential to automate both re-testing and regression tests. Automation is not a full substitute to manual testing as not 100% automation testing can be achieved and it shouldn't

## **Maintenance Testing**

Once deployed, as software systems are in service for years or decades, during this time the operational system, its configuration data, and or its environemnt are often corrected, changed, or extended.

The testing of these cahnges is called maintenance testing, and is triggered by:

- Planned enhancements or upgrades to business systems.
- Corrective and emergency changes
- Changes to the operating environment such as system upgrades.
- Upgrade of commercial-off-the-shelf software
- Migration of applications from one platform to another
- Retirement of legacy software systems

## **Summary**

**This is what you have learned so far:**

- Waterfall Model
- V-Model
- Iterative Model
- Unity or Component Testing
- Integration Testing
- System Testing
- Acceptance Testing
- Functinoal Testing
- Non-Functional Testing
- Structural Testing
- Change-related Testing
- Maintenance Testing

## **Section 2 Quiz**

1) Which of the following describes how testing activities can occur in parallel with development activities?
    - V-Model

2) In iterative development models, which of the following is true?
    - Regression testing is increasingly important on all iterations after the first one

3) Validation involves which of the following?
    - Checking that the right product has been built

4) Testing interfaces to external organisations is most likely to occur in which part of the life cycle?
    - System Integration Testing

5) Navigation of a web site might be tested as part of:
    - Usability Testing

6) In Test-Driven Development, when should a set of test scripts be written for a component?
    - Before the code is written

7) When conducting Component Integration testing, functional integration
    - Selects a specific area of functional capability in the system


8)  Integration testing, where no incremental testing takes place prior to combining all the system’s components, is called
    - Big Bang Testing

9) A Use Case makes a good:
    - Test Basis

10) Specially-written software that replaces a called component during component integration testing is called what?
    - Stub

11) Which of the following is untrue of user acceptance testing?
    - The main purpose is to find defects in the system

12) Testing following modifications, migration, or retirement of the software is
    - Maintenance Testing

13) Which of the following statements about testing are true?
    - Structural testing is equivalent to white box testing

14) Functional testing would test which of the following?
    - The system will produce a weekly order report

15) A regression test:
    - Checks unchanged areas of software for unexpected side effects.

16) The difference ebtween re-testing and regression testing is:
    - Re-testing is running a test again. Regression testing looks for unexpected side effects

17) Regression testing should be performed: 
    - After the software has changed
    - When the environment has changed

18) Which of the following defines the scope of maintenance testing?
    - The size and risk of any changes to the system