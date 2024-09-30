# **ISTQB Foundation Level Certification Exam Preparation**

## **Introduction**

**What you will learn in this third section:**

- Learn to identify risk and its levels and types of risks
- The role of test lead
- The tester tasks
- Learn what test approach means and how to use it
- The importance of master test plan
- The standard for software testing documentation - IEEE829
- Test planning activities
- Determine the entry and exit criteria
- Test estimation
- Test control

## **Test Organization and Independence**

The effectiveness of finding defects by testing and reviews can be improved by using independent testers.

Development staff may participate in testing, especially at the lower levels, but their lack of objectivity often limits their effectiveness.

For large, complex or safety critical projects, it is usually best to have multiple levels of testing, with some or all of the levels done by independent testers.

**The benefit of independent testers include:**

- They will see other and different defects, and are unbiased
- They verify assumptions made during specification and implementation of the system
- They bring experience, skills, quality, and standards

**Drawbacks include:**

- Isolation from the development team, leading to possible communication problems.
- They may be seen as a bottleneck or blamed for delays in release
- They may not be familiar with the business, project, or systems
- Developers may lose a sense of responsibility for quality

## **Task of the Test Leader and Tester**

Most test teams consist of two distinct toles, test leader and tester.

The activities and task performed by people in these two roles depend on the project and product context, the people in the roles, and the organization.

**Test Leader**

- Send timely status reports
- Flexability
- Assist team in the deliverables
- Timely work allocation

**Tester**

- Send timely status reports
- Flexability
- Complete assigned tasks
- Discuss issues with Leads

![Tasks of the Test Leader and Tester]()

## **Typical Test Leader Tasks**

The role of the test leader or test manager, may be performed by a project manager, a development manager, a quality assurance manager, or the manager of a test group.

Typically the test leader plans, monitors, and controls the testing activities and tasks described below:

- Write or review the test policy and strategy for the organization
- Coordinate the plan with project managers and others
- Contribute the testing perspective to other project activities
- Plan the tests, approaches, estimating the time, effort, and cost of testing, acquiring resources, defining test levels, cycles, and planning incident management 
- Assess the test objectives, context, and risks
- Initiate the specification, preparation, implementation, and execution of tests.
- Monitor the test results and check the exit criteria
- Adapt planning based on test results and progress and take any action necessary to compensate for problems.
- Write test summary reports based on the information gathered during testing

## **Tasks of the Tester**

Testers or Test Analysts, who work on test analysis, test design, specific test types or test automation may be specialists in these roles. 

Typically testers at the component and integration level would be developers, testers at the acceptance test level would include business experts and users. 

Typical tester task include:

- Review and contribute to test plans
- Analyze and review user requirements, specifications, and models for testability
- Create test specifications
- Set up the test environment with appropriate technical support
- Prepare and acquire test data
- Implement tests on all test levels, execute and log tests
- Evaluate results and record incidents
- Use test tools as necessary and automate tests
- Measure performance of systems as necessary
- Review tests developed by others

## **Planning Activities**

Planning is the first test activity to be carried out at each test level, but it is a continuous process and is performed throughout the life cycle.  

Feedback from test activities is used to recognize changing risks so that planning can be adjusted. 

Planning is a lot more than scheduling:

- Determining the scope and risks and identifying the objectives of testing
- Defining the overall approach to testing, including definition of the test levels, and entry and exit criteria
- Linking into other software life cycle activities, such as acquisition, development, operation, and maintenance
- Assigning resources for the different activities defined
- Deciding testing tasks, roles, schedule, and evaluation of test results
- Defining the amount, level of detail, structure and templates for the test documentation
- Selecting metrics for monitoring and controlling testing
- Setting the level of detail for test procedures

## **Levels of Planning**

Test planning may be documented in a hierarchy of documents, each one refining the approach taken to testing projects within an organization.

**Test Policy:** "A document characterizing the Organization's philosophy towards software testing. It is set at the highest level of the organization and is the overall approach to quality of the organization and is the overall approach to quality assurance giving general guidelines for all project testing. It may be the IT department's philosophy if there is no organizational document.

**Test Strategy*:** A high-level description of the test levels to be performed and the testing within those levels for an organization or programme. A division or programme sets out their testing strategy based on the Test Policy and identified risks.

There are two main aspects:

- Risks to be resolved by testing the software
- Testing approach used to address the risk

**Test Plan:** A document describing the scope, approach, resources, and schedule of intended test activities. Each project adapts the strategy to create a test plan for that particular project

![Levels of Planning Tree Diagram]()

There may be further plans for test levels, maintenance testing, regression testing, static testing, etc., not all show here.

## **Levels of Planning IEEE 829-1998**

Standard for Software Development Documentation

Most business adopt the IEEE standard 829-1998 Test Plan outline for documenting test planning, but even the standard is not being used, the approach to test planning should be the same.

The new standard is **ISO/IEC/IEEE 29119** but for the ISTQB exam, learning 829 should be sufficient for now.

Little something to help you memorising all this:

- S - Scope
- P - People
- A - Approach
- C - Criteria
- E - Environment needs
- D - Deliverable
- I - Identifier and introduction
- R - Risks and contingencies
- T - Testing and tasks and schedule

## **IEEE 829 Test Plan Content**

![IEEE 829 Test Plan Content]()

![IEEE 829 Test Plan Content Continued]()

## **Entry Criter**

Entry criteria define when to start testing such as at the beginning of a test level or when a set of tests is ready for execution.

Typically entry criteria might include:

- Test environments and tools configured and available and ready
- Testable code available
- Test data available, including configuration data, logins, etc.
- Test summary report or evidence available from previous testing, including quality and coverage measures.
- Third-party software delivered and software licenses bought

Entry criteria for one test level might match the exit criteria of the previous level. Some examples:

- 80% of system tests complete (for entry to UAT)
- Unit testing is completed with branch coverage reports (for entry to system testing)
- All documentation is present and has been signed off

## **Exit Criteria**

Exit criteria define when to stop testing at the end of a test level or when a set of tests has a specific goal.

This decision should be based on a measure of software quality achieved as a result of testing, rather than just on time spent testing.

**Typical exit criteria may consist of:**

- Measures of testing **thoroughness**. i.e., coverage of code, requirements, functinoality, **risk**, or cost
- **Estimates of defect density** or reliability
- **Residual risks** such as **number of defects** outstanding or requirements not tested

**Typical examples are:**

- All paths coverage of code, high and medium risk areas completed.
- No outstanding high-severity incidents, all security testing completed successfully
- Non-functional measures such as usability in acceptance testing

## **Test Approaches**

The test approach should be set out in the Test Strategy, then refined and implemeneted in test plans and test designs for a specific project.

It is the starting point for planning test activities, choosing test design techniques, and defining entry and exit criteria.

**Test approaches may be:**

- Preventative, where tests are designed as early as possible
- Reactive, where test design comes after the software has been produced

**Typical test approachs include:**

- Analytical approaches, such as risk-based testing where testing is directed to areas of greatest risk
- Model-based approaches, such as stochastic testing using statistical information about failure rates (such as reliability growth models) or usage (such as operational profiles).
- Methodical approachs, such as failure based (including error guessing and fault attacks), check-list based, and quality characteristic based.
- Process or Standard-compliant approaches, such as those specified by industry standards or the various agile methodologies
- Dynamic and heurisitc approaches, such as exploratory testing where testing is more reactive to events than pre-planned, and where execution and evaluation are concurrent tasks
- Consultative approaches such as those where test coverage is driven primarily by the advice and guidance of technology and/or business domain experts outside the test team
- Regression-averse approaches, such as those that include reuse of existing test material, extensive automation of functinoal regression tests, and standard test suites.

**Choosing an approach** - Different approaches may be combined, for example, a risk-based dynamic approach. The selection of an approach depends on:

- Context, type of system and technology
- Risks, hazards, safety, and regulations
- Available resources and skills
- Testing objectives

## **Test Estimating**

Test managers need to estimate the time, effort, and cost of testing tasks in order to plan test activities, identify resource requirements and draw up a schedule. 

Two possible approaches are:

- The metrics-based approach: based on analysis of similar project or on typical values
- The expert-based approach: based on assessment by the owner of the task or domain experts

![Test Estimating]()

## **Metrics-Based Estimation Example**

Testing is much more difficult to test than other project activities such as requirements analysis and development.

Standard Percentages uses industry or company-based historical data to calculate the proportion of the time testing stages takes for different project types.

Then if you can size the overall project, you can work out how much testing effort is required, without estimating the testing tasks directly.

Alternatively, if you can obtain more accurate estimates for a non-testing part of the project, you can apply the appropriate proportions.

For example, using the figures here, if the development manager provides an estimate of 40 days for coding and unit testing, then that is equivalent to 60% of the total development and testing time, so system and integration testing (25%) would be 17 days and acceptance testing (15%) 10 days.

*Not all projects are the same. A package purchase would require integration and acceptance rather than unit testing.*

![Standard Percentages Using Work Distribution Model]()

## **Expert-based Estimation Example**

Experience is still the most widely used approach. Asking the task owner means they are more likely to commit to a deadline and also think through every detail of the job (i.e., remebering about setting up test data, etc.).

Breaking a large task into bite-sized chunks makes it easier to understand and leads to more accurate estimates.

![Expert-based Estimation Example]()

## **Factors to Consider When Estimating**

**The testing effort may depend on a number of factors, including:**

- Product factors, such as **quality** of the specification, **size**, and **complexity** of the product and requirements for **reliability**, **security**, and **documentation**
- Development process factors and the **stability** of the organization, **tools** used, **test process**, **skills** of the people involved, and **time pressure**
- Quality factors, for example the **number of defects** and the amount of **rework** required

Functionality forms the core approach to estimating but all sorts of **environmental** factors come into play too.  **Rework** is a major consideration: filling incident reports, retesting, changing documents can tak an equivalent time to the intial tests.

## **Test Progress Monitoring**

Throughout a project, the progress of test activities should be monitored and checked frequently in order to:

- Provide feedback and visibility about testing to stakeholders and managers
- Assess progress against estimated schedule and budget in the test plan
- Measure testing quality, such as number of defects or coverage achieved, against exit criteria
- Assess the effectiveness of the test approach with respect to objectives
- Collect data for future estimation

The metrics used to measure progress should, if possible, be based on objective data (i.e., numerical analysis of test activity) rather than subjective opinion. These metrics may be collected manually or automatically using test tools such as test management tools or defect trackers

The test manager may have to report on deviations from the test plans such as running out of time before completion criteria is achieved.

**Common test metrics include:**

- Percenteage of work done in test case and environment preparation
- Test case execution - number of test cases run/not run, test cases passed/failed
- Defect information - defect density, defects found and fixed, failure rate and retest results.
- Coverage of requirements, risk or code
- Data of test milestones
- Testing costs, including the cost compared to the benefit of finding the next defect or to run the next test

The best metrics are those that match the exit criteria (i.e., coverage, risk, and defect data) and estimates (i.e., time and cost) defined in the test plan

## **Typical Progress Metrics**

Plotting a graph (using  a test planning tool or spreadsheet) is a great way to monitor test activity against the plan. The graph below is typical, and allows test managers to check the number of tests passed does not diverge too far from the number executed.

![Typical Progress Metrics]()

## **Number of Incident Reports**

Other graphs commonly used by test managers is to show how fast incidents are dealt with as they are raised. If the lines do not start to converge towards the end of the project, test managers can take appropriate action such as adding more resources to fix or address quality problems.

![Typical Number of Incident Report Metrics]()

## **Test Control**

If test monitoring shows that progress is slipping from planned targets, or that exit criteria are not being met, then test managers may have to take some guiding or control actions to get back on track. Options for actions may often be limited, but might include:

- Re-prioritize testing activities (i.e., focus testing on high-risk objectives)
- Change test schedule (i.e., allocate more time to testing)
- Re-assign resources (i.e., assign more testers, or more developers working on fixes)
- Set entry criteria for deliverables from developers (i.e., set minimum quality levels at start of testing)
- Adjust exit criteria (i.e., re-assess acceptable quality measures)

## **Test Reporting**

Test Managers will report regularly on test progress to Project Managers, project sponsors, and other stakeholders. The report should be a summary of test endeavour, including what testing actually occured, statistics on key metrics, and dates on which milestones were met.

Reports will be based on metrics collected from testers and may be considered using spreadsheets or test management tools. It is then analyzed by project stakeholders to support recommendations and decisions about the future actions:

- Assessment of defects remaining
- Economic benefit of continued testing
- Outstanding risks
- Level of confidence in tested softwaer
- Effectiveness of objectives, apprach and tests

## **Test Summary Report**

The Test Summary Report is part of the IEEE standard 829-1998, and is used to summarize test activity at the end of a test level. The outline of the standard report is as follows:

![Test Summary Report]()

## **Configuration Management**

The purpose of configuration management is to establish and maintain the integrity of system products throughout the project life cycle.

It applies to all products connected with software development (such as software components, data, and documentation) and testing (such as test plans, test specs, test procedures, and test environments).

Configuration management is therefore more that just version control, it's also about knowing what versions are deployed in different environments at different times.

It ensures that every item of test-ware (software and test documentation) is uniquely identified, version controlled, tracked for changes, related to each other and related to development items.

Although these items may be physically stored in many locations, configuration management describes and links them in a common controlled library. This ensures that all identified documents and software items are referenced unambigously in test documentation, which avoids tests being run against the wrong software version.

## **Risk and Testing**

As ISTQB glossary quotes - *"A factor that could result in future negative consequences; usually expressed as impact and likelihood.""*

Risk-based testing is seen as the best approach to enabling the best testing to be done in the time available. This section covers measuring, categorizing, and managing risk in relation to testing.

A risk is a specific event which would cause problems if it occurred. Individual risks can be assessed in terms of:

- Likelihood - the probability of the event, hazard, or situation occurring
- Impact - the undesirable consequences if it happens, for example financial, rework, embarassment, legal, safety, or company image

Two types of risks are: project risk and product risk

## **Project Risks**

Project risks are the risks that affect the project's or test team's capability to deliver its objectives such as:

**Technical Issues**

- Problems in defining the right requirements
- The extent that requirements can be met given existing constraints
- Test environment not ready on time
- Poor quality of design, code, or tests
- Late data conversion or migration planning

**Organizational Factors**

- Skill, training, and staff shortages
- Personnel issues
- Political issues, such as problems with testers communicating their needs and test results, or failure to follow up on information found in testing and reviews
- Unrealistic expectations of testing

**Supplier Issues**

- Failure of a third party
- Contractual issues

## **Product Risks**

"Product" means the software or system. Potential failures in the software are known as product risks, as they are a risk to the quality of the system. product risks include:

- Failure-prone software delivered
- Potential for software or hardware to cause harm to an invidual or company
- Poor software characteristics (i.e., functionality, reliability, usability, performance)
- Poor data integrity and quality (i.e., data migration issues, data conversion problems, data standards violation)
- Software does not work as intended

## **Risk Assessment Matrix**

For each risk identified, its likelihood and impact must be assessed. These may be numerical measures (i.e., 1-10) or simply Low, Medium, and High. Combining lielihood and impact measures into an overall risk measurement allows risks from different areas to be compared, assessed, and prioritized. Risk and their assessments should be recorded in the test plan, perhaps using a matric like this:

![Risk Assessment Matrix]()

Once a risk has been assessed, there are two possible actions which can be put in place to reduce the risk:

- Mitigation - preventative or proactive action to reduce the likelihood of the risk happening
- Contingency - emergency or reactive approach to reduce the impact if the risk happens

## **Risk-based Testing**

A risk-based approach to testing provides proactive opportunities to reduce the levels of product risk, starting in the initial stages of a project. It involves the identification of product risks and their stages of a project. It involves the identification of product risks and their use in guiding test planning and control specification, preparation and execution of tests.

Risk-based testing draws on the collective knowledge and insight of the project stakeholders to determine the risks and the levels of testing required to address those risks. For example, developers can identify the most complex code, users may describe the most used functions, managers may highlight the areas with the biggest financial impact, etc.

![Risk-based Testing]()

In a risk-based approach, the risks identified may be used to:

- Determine the test techniques to be employed, i.e.:
- White-box testing for safety critical systems
- Usability testing for customer input screens
- Security testing for e-commerce system

- Determine the extent of testing to be carried out, i.e.:
- What to test, and not to test
- What to test first, and last
- What to test most, and least

- Prioritize testing in an attempt to find the critical defects as early as possible, i.e.:
- Use tracability matrix to link test design to priority requirements
- Create test execution schedule to run tests in the most efficient order
- Focus on defect clusters

- Determine whether any non-testing activities could be employed to reduce risk i.e.:
- Provide training to inexperienced designers
- Improve documentatino

In addition, testing may support the identification of new risks, help to determine what risks should be reduced, and lower uncertainty about risks.