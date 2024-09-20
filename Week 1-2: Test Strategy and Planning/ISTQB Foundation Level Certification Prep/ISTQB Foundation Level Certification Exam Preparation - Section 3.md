# **ISTQB Foundation Level Certification Exam Preparation**

## **Introduction**

**What you will learn in this third section:**

- Static testing techniques
- Importance of reviews
- Typical types of defects found in reviews
- Carry out a basic and formal review
- Roles and types of reviews
- Informal, walk-through, Technical and inspection reviews
- Success factors of reviews
- What is a static analysis
- Benefits of reviews
- Use of static analysis tools

## **Static Testing Techniques**

Static testing is the examination of program source code or other project documentation, without the execution of the code, to find defects. The two types of static testing are:

**Reviews** - Done by humans are the manual examination of documents

**Static analysis** - Done by tool is the automated analysis of source code and software models.

As opposed to dynamic testing which is performed by executing software under test and comparing actual and expected results.

Reviews and static analysis have the same objective as dynamic testing in finding defects. Static testing is a complementary technique. It finds causes of failures (defects) directly, while dynamic testing failures which may be caused by defects.

![Static Testing Techniques]()

## **Reviews**

Typical written project document or software product that can be reviewed are:

- Business requirements
- Functional requirements
- System and database designs
- Source code
- Test plans, test cases, and scripts
- User guides, help text
- Web pages

The benefits of reviewing as early as possible are simple.  Easier and cheaper to fix.

- Early defect detection and correction
- Increase develpoment productivity
- Reduced development cost and timescales
- Fewer defects in code
- Reduced time and cost of dynamic testing
- Improve communication between testers, analysts, developers, and users

## **Types of Defects Found in Reviews**

The aim of reviews is to check and improve the quality of project products.  Such as verification and validation of documents and completeness and conformance to standards.

- Errors (Human)
- Omissions
- Additions
- Inconsistencies
- Ambiguities
- Readability
- Terminology
- Spelling
- Grammar
- Layout
- Structure

## **Basic Review Process**

A good review will also include causal analysis to learn from issues and bring about process improvement. By involvoing a number of reviewers in a controlled manner consensus can be reached on subjects such as best design practice.

Reviewers are better than dynamic testing at finding some types of defects, such as checking standards, identifying inconsistencies in requirements and designs, assessing maintainability and checking interface specifications.

## **Formal Review Process**

The way review works depends on the agreed objectives, the intention is to find defects, gain understanding, educate testers and new team members or discussion and decision by consensus.

Here's a typical formal review process:

- **Planning** - Moderator defines criteria and what to review. Allocate resources. Define entry and exit criteria.

- **Kick-off** - Document distributed to reviewers 1 to 3 days in advance. Objectives, process, and document explained to participants.

- **Individual preparation** - Reviewers read and note any potential defects, questions and comments. Compare product to predecessor products, standards, guidelines, and best practices.

- **Review Meeting** - Participants discuss the document, note defects, and log findings. Moderator ensures discussion is kept on track and remain in objective. Some review only dfect is discussed others may discuss alternative solutions

- **Rework** - Following the meeting, the author corrects the document based on the defects found and updates the status of the defects

- **Follow-up** - Moderator ensures document is now corrected and collect metrics such as times spent reviewing, defect density and breakdowndefects by business area or severity. This info will be used to find recurring issues.

## **Review Roles**

**Manager** - decides what to review, allocate time and determines wether objectives have been met.

**Moderator** - or **leader**, manage the mead, including planning, motivating, facilitating meetings, training reviewers, and monitoring the process.

**Author** - prepares the material to be reviewed, participates in discussion during the review meeting and incorporates the agreed changes afterwards.

**Reviewers** - aka **checkers** or **inspectors** are responsible for finding defects. Stakeholders should have technical or business background. Ideally from different areas and focus, such as Business users, developers, analysis, IT operations, testers, and compliance officers.

**Scribe** - or **recorder**, documents all the issues, problems, and open points that were identified during the meeting

## **Four Types of Review**

- **Informal** - one to one discussion with no formal process. For example 'buddy reviews', pair programming, design review or code by a technical team leader

- **Walk-through** - Led by the author taking you through the scenarios, dry runs and peer group. Useful and highly visual via storyboarding, workflows, etc. Seen as more passive approach presenting the information finding defects but not proposing solution. Opportunity for testers to analyze and query the document

- **Technical Review** - It's a defined defect-detection process involving both peers and technical experts. Led by morderator and vary from informal to very formal. The goal is to review from technical and specialist viewpoint. To discuss, make decisions, evaluate alternatives, find defects, solve technical problems, and check conformance to specification plans, regulations, and standards.d

- **Inspection** - It's a very thorough, formal process designed to detect defects in documents and program source code, using rules, checklists and entry and exit criteria. Inspection is led by a trained moderator. Also involve causal analysis, looks at common casues of defects and provides feedback to improve future development and inspection processes.

## **Informal Review**

Main pupose is to find defects and uses no real formal process.

## **Walkthrough**

Very useful for highly visual products via storyboarding, workflow tools, etc.

Walkthrough should find defects but not propose solutions - this is the author's task after the meeting.

## **Technical Review**

Enable decision making, finding defects, solving technical problems, and checking conformance of document

## **Inspection**

Main purpose is to find defects and process improvement.

The inspection process is a very thorough, formal process designed to detect defects in documnet and program source code, using rules, checklists, and entry/exit criteria.

## **Success Factors for Reviews**

For any type fo review to be successful, it must have clear, predefined objectives and must involve the right people for the review objectives.

This includes testers who are valued reviewers and can contribute to the review and also learn about the product which enables them to prepare tests earlier.

- Each review should have predefined and agreed objectives.
- Any defects should be welcome
- Conducted in an atmosphere of trust
- Techniques are suitable to work-product type
- Emphasis on learning
- Management support

## **Static Analysis**

Used to find defects in software source code and software models.

The objective of static analysis is to find defects in software source code and software models, but not written documents. It requires the use of tools and is performed without actually executing the software being examined by the tool. Static Analysis finds defects rather than failures.

Static analysis does not test functionality but can locate structural defects that are hard to find in dynamic testing.

## **Benefits of Static Analysis**

- Early detection of issues prior to text execution.
- Early warning about suspicious code or design.
- Identification of defects not easily found by dynamic testing.
- Improved mantainability
- Prevention of defects

## **Use of Static Analysis Tools**

Static analysis tools are typically used by developers to check against pre defined rules of programming standards, before, during component (unit) and integration testing.

Many of these tools provide a graphical representation of the code and this can be useful for testers to help pinpoint where are the complex source code, which might indicate possible defect clustering helping you focus on dynamic testing.

## **Summary**

**This is what you've learned so far**

- Two main static techniques
- Reviews
- Types of defects found in reviews
- Basic review process
- Formal review process
- Review roles
- Four types of reviews
- Informal Review
- Walkthrough Review
- Technical Review
- Inspection
- Success factors for reviewers
- Static Analysis and its benefits
- Use of static analysis tools

## **Section 3 Quiz**

1) Typical defects that are easier to find in reviews than in dynamic testing are:
    - Deviations from standards
    - Requirements and design defects
    - Insufficient maintainability and incorrect interface specifications


2) Q2. What common objective is shared by static testing and dynamic testing?
    - Identifying defects

3)  In a walkthrough, the scribe should not also be the
    - Author

4) The following characteristics define a technical review:
    - Have a documented, defined fault-detection process
    - Include peers and technical experts
    - May have no management participation
    - May correct issues as they arise

5)  A developer who desk-checks his or her own code by visually stepping through is execution is performing:
    - An informal review

6) A moderator who is not also the author is mandatory in
    - An inspection

7) What type of review requires formal entry and exit criteria, and keeps metrics?
    - Inspection

8) Reviews are worthwhile because:
    - They reduce costs by removing defects before test execution

9)  One of the defining characteristics of walkthroughs is that they are led by:
    - The author

10) In a formal review, reviewers are each assigned a focus so that:
    - We exploit individuals' expertise
    - Responsibilities are defined clearly
    - Each has a smaller task

11)  Static analysis can detect which of the following more easily than dynamic testing?
    - Parameter type mismatches

12)  Which of the following statements about compilers is true in testing?
    - May provide some similar functionality to a static analyser

13) Which of the following is true of static analysis?
    - Finds defects rather than failures

14) What can static analysis NOT find?
    - Whether the value stored in a variable is correct

15) Static analysis tools are:
    - Able to provide quality information about source code