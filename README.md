## Aiden Waring - CAB012027

## T2A1 - Workbook

---

#### Introduction

As a developer (dev) you are sometimes required to prove your knowledge to prospective clients and employers.

A common way clients assess this for a specific project is to release a Request for Quotation (RfQ). A RfQ can take many forms, but in general it is a questionnaire covering technical and commercial topics. This Workbook emulates the technical section of a RfQ.

#### Brief

The ACME Corporation is interested in building a marketplace web application (app) using Rails for one of it’s product lines. To help it choose the vendor who will undertake the project they have released a RfQ. As an aspiring junior dev at an up and coming Sydney software startup (CAx-Dev) your manager has assigned you to assist with preparation of the RfQ response.

You are assigned (required) to complete all the questions from the technical section of the RfQ - which are presented below.

Being a highly valued junior dev you are expected to continue working on your other ongoing projects and schedule time for this project accordingly.

#### Questions

##### Details:

ACME Corporation is looking for devs with an understanding of Rails. The following set of questions relate to this RfQ-requirement.

## Q1

Describe the architecture of a typical Rails application. [200-300]

**Answer:**

Ruby on Rails is a software framework used for web development. An extension of the Ruby programming language, Ruby on Rails (or Rails as it is often called) utilises Ruby and combines it with HTML, CSS and JavaScript to create a web application that runs on a web server.
Rails applies the model-view-controller (MVC) software design pattern for it's architecture. This architectural pattern separates the application into three primary components: model, view and controller - each with it's own responsibilities.

As per the Rails API, the model layer represents the central component of the design pattern. It  manages the behaviour and data of the data of the application. The model contains the data of the application and it's links to databases, the business logic and the current state of the application. Each of the programs references to data stored in the database and it's structure works independently of the user and their interfaces. Rails separation of model information and data representation from the rest of the application ensures minimal repetition of data handling.
[Reference](https://api.rubyonrails.org/)

The view layer represents the user interface presented to the user. The view does not perform any processing, rather it is passed information from the rest of the application to the appropriate user. 

The controller layer handles the user interface and application logic. While the view visually represents data it has been given on screen for the user, the controller manages client requests for certain information, retrieves the relevant information and directs the user to a view, where that information can be visually represented.

Separating these responsibilities adheres to the strong design philosophy rules. The first of which is that the separation of concerns within the application increases re-usability, as a model can be reused and queried in different ways for different views. Code is easier to maintain, as each application component has a low dependency on others. This makes parts of the application easier to edit or change without concern of impacting other functions. MVC component seperation also improves the scalability of the app. [Glenn Goorich in 'Rails: Novice to Ninja'](https://www.sitepoint.com/model-view-controller-mvc-architecture-rails/), states that "...for example, if your application begins experiencing performance issues because database access is slow, you can upgrade the hardware running the database without other components being affected."

Rails also follows the "Convention Over Configuration" rule, which is also known as Coding by convention. This is a design paradigm that attempts to simplify designing Rails applications using its framework by streamlining development steps and decreasing the number of decisions made by a developer. This means, that it has already taken a few decisions for you and you don’t have to worry about those things until you follow ROR conventions. [Reference](https://medium.com/@SravanCynixit/overview-of-ruby-on-rails-architecture-9902de7c93f9)



## Q2

Identify a database management system (DBMS) commonly used in web applications (including Rails) and discuss the pros and cons of this database.[150-200]

**Answer:**

A database management system (DBMS) is software 
for managing databases. PostgreSQL is a popular database management system chosen by many developers for use with their web applications. PostgreSQL provides many advantages to its developed web application, though not without its setbacks.

##### Advantages:

- Cost
One of PostgreSQL's major advantages is that the DBMS is completely open source. This grants "[permission to use, copy, modify, and distribute this software and its documentation for any purpose, without fee, and without a written agreement..."](https://opensource.org/licenses/postgresql). ["The term open source refers to something people can modify and share because its design is publicly accessible."](https://opensource.com/resources/what-open-source) As the code is publicly available it means that there will always be opportunities to make changes and improvements to the code base where projects require them.  Developers can develop their own modules and propose them to the open source community.

- Cost
This means that developers that may chose to implement PostgreSQL as their chosen DBMS for their web application may do so for free: no royalties or licensing costs and restrictions to consider as part of their project's scope. 

- ACID Support
In computer science, ACID is a collection of properties that ensure database transactions are processed reliably. PostgreSQL is compliant with this design principles. The acronym ACID details the desirable properties for transactions within a database. ACID stands for atomicity, consistency, isolation and durability. These principles ensure that PostgreSQL operations are resilient to fault, such as crashes, failed transactions and unexpected hardware & software interruption. 

- Relational DBMS Design
PostgreSQL is an object-relational database, while MySQL is a purely relational database. This means that PostgreSQL includes features like table inheritance and function overloading, which can be important to certain applications. PostgreSQL also adheres more closely to SQL standards. For example, "PostgreSQL handles concurrency better than MySQL."[Reference](https://developer.okta.com/blog/2019/07/19/mysql-vs-postgres)

##### Disadvantages:

- Less Hosts
As PostgreSQL is considered a smaller and less used DBMS compared to another service such as MySQL, it is less supported on various web hosting platforms. 

- Performance
Studies have also shown that PostgreSQL performs slightly slower compared to alternative DBMS options when performing specific operations (comparatively low reading speed). [Reference](https://www.xplenty.com/blog/postgresql-vs-mysql-which-one-is-better-for-your-use-case/)

## Q3

##### Details:

ACME Corporation is very big on project management, documentation and process. This will be a key metric in their decision to award the project. The following set of questions relate to this RfQ-requirement.

Discuss the implementation of Agile project management methodology. [200-300]

**Answer:**

Agile is a type of project management methodology often used in software development that focuses on the idea of iterative development, adaption and user feedback. [Reference](https://www.atlassian.com/agile/project-management)

The fundamentals of the Agile methodology stems from the [Agile Manifesto](http://agilemanifesto.org/): a document created in 2001 by leaders in the software development industry. This document discusses their frustrations with older, less flexible methods back then and wrote to "uncover a better way of developing software". The core values of the proposed Agile method are:

- Individuals and interactions over processes and tools over processes and tools
- Working software over comprehensive documentation
- Customer collaboration over contract negotiation
- Responding to change over following a plan

These values and their 'Twelve Principles of Agile Software' helped define a new way of approaching software development. Over the years many different organisations have helped further these core values and found ways to implement these strategies into their project delivery. The growing use of Agile has helped better define it's processes. Several different types of Agile methodologies have been created, while similar, are designed for different delivery models.

The implementation of the Agile methodology is first determined by your delivery objective. Teams who work continuiously on a project with continuious release methodlogy often chose to implement the Kanban methodology, which focuses on visual representations of work to maximize efficiency and highlight where work is needed. Teams who are delivering a product or service by a certain deadline may chose to use Agile in the 'Scrum' framework. In a scrum, teams work in a several interval phases named sprints, during which their goal is to create an interative loop of developing the software and gathering feedback, using this as input for their next sprint.[Reference](https://www.atlassian.com/agile/kanban/kanban-vs-scrum)

If we take a look at using scrum as an example, after determining that scrum is chosen to be the preferred delivery methodology, implementing it as part of managing the project is as follows:[Reference](https://www.scrumguides.org/scrum-guide.html)

#### 1. Defining Scrum Team

This phase begins with determining the product owner (often the end user or client). Followed by determining the scrum master (often a senior developer of project manager). This is then followed by establishing the scrum team members (often the development staff involved in the project which includes programmers, testers, team leads).

#### 2. Sprint Objectives 

A product backlog is created. This is a tool to systematically list all features that should be implemented during the development process. Ordered by priority, these required items are each known as a "user story". 

#### 3. Sprint Planning

The duration of the sprint is determined. The sprint's duration is relative to how often the team will receive feedback from the client as this is done between sprints. Shorter sprints result in customer feedback being given more frequently whereas longer sprints allow the team to work on items more thoroughly. Sprints are often two weeks in duration by default.

The selected team for the scrum choses the most important user stories (MVPs) to work on. A sprint backlog is created which consists of items to be completed in the next sprint.
    
#### 4. Sprinting

Scrum meetings or standup meetings (standups) are held typically at the start of each work day during the sprint for developers to update team leads and project managers. Each member discusses the current project's status, where they are at with their objectives, completed items, identified problems and roadblocks.
Work begins on the selected user stories. User stories are organised into cards, and as the sprint progresses are moved into categories: to-do, in progress, testing and done. Project management software platforms such as Atlassian JIRA and Trello are often used to organise these.

#### 5. Sprint Testing & Demonstration

As part of the full life-cycle testing process that agile uses, internal testing is performed on items delivered during the sprint. Once this is completed, the product is often demonstrated to either a test group or client for further user feedback.

#### 6. Sprint Retrospective

Once the previous segment has completed, the team reflects on the performance of the sprint and undergo an analysis on what worked and what did not. Suggestions on how to improve and given and the team takes construcive criticism in an analysis to provide to the scrum master. These improvements can be implemented for the next sprint.

#### 7. Next Cycle of Sprints

Taking into consideration the feedback from the testing and retrospective, the next sprint begins with developers working on the sprint backlog. This process is repeated until a complete end product is delivered.

## Q4

Provide an overview and description of a standard source control workflow. [100-200]

**Answer:**

Source control workflow refers to the recommended steps and procedure adhered to in a source control environment. Developers utilising a source control system can contribute and work in different ways. The workflow concept is a design that defines the rules versioning, branching and the control of the master branch.
[Reference](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)

A popular standard workflow practiced by developers is the centralized workflow.
In a centralized workflow, developers all contribute to a shared repository (as opposed to fork-pull workflow. This central repository is often created and hosted on source control hosting services such as Bitbucket or GitHub.

Problems arise when publishing or "pushing" to the central repository without following a source control workflow. The centralized workflow, sometimes referred to as feature branch workflow, ensures that all code changes are made in new, feature-specific branches instead of master. These feature branches are created on the repository for code changes. Developers will make changes and edit files committing locally and synchronising upstream at a convenient time. Reviewed changes can then be "pulled" back into the shared repositories master branch by initiating a pull request. The request can then either be accepted or denied. Accepted pull requests then see new code "merged" into the master branch. 

This segmentation of new code and it's staged change control methodology ensures that the master branch remains valid, stable and conflict-free. This approach is often employed by organisations for in-house development.
[Reference](https://git-scm.com/book/en/v2/Distributed-Git-Distributed-Workflows)

## Q5

Provide an overview and description of a standard software testing process (e.g. manual testing). [100-200]

**Answer:**

Software testing is the process of evaluating the functionality of software and its quality, identifying bugs and errors that may disrupt the user experience.[Reference](https://www.toolsqa.com/software-testing/test-process-in-software-testing/)
There are three popular approaches to testing: white box, black box and grey box testing. Each one refers to the amount of visibility the individual testing the application has to the application's code. White box testing has a user internal to the design and programming of the software create the test cases. Black box testing is performed by users without looking at the code, where the input and output of the user's experience defines the test cases. Grey box testing is performed by a user who does not have access to the code but rather access to the code's documentation which is to be used to create test cases.[Reference](https://www.softwaretestingmaterial.com/software-testing/)

Regardless of the approach, the method of testing software for error can be performed in a variety of different ways. For this example manual testing will be discussed.

Manual testing is a process of manually executing test cases without the use of testing tools. This is done by comparing the current behaviour of the software to the expected behaviour of the software. A test plan is produced before testing begins. This outlines the approach which the tester will take to completing the testing and to ensure that no part of the code has been overlooked. Each operation within the program that a user can undertake is considered a 'test case'. This test case identifies the code segment or application component being tested and what the expected outcome of the operation should be. Any differences identified between the expected outcome and the result of the test are noted as a discrepancy or defect. These are logged to be provided back to the developer for feedback. For each identified discrepancy that has been identified and fixed, a re-evaluation should occur, where the tester performs the same use case test to ensure that the problem has since been resolved and that the expected outcome matches the fixed result. This process is repeated for the entirety of the application. Automation is often used to coincide with manual testing as while manual testing is effective, it is also time consuming.

## Q6

##### Details:

Having suffered several cyber attacks in the past and resultant remedial audits ACME Corporation takes compliance, security and privacy very seriously. The following set of questions relate to this RfQ-requirement.

Discuss and analyse requirements related to information system security and how they relate to the project.[100-200]

**Answer:**

## Q7

Discuss common methods of protecting information and data and how you would apply them to the project.[100-200]

**Answer:**

## Q8

Research what your legal obligations are in relation to handling user data and how they can be met for the project.[100-200]

**Answer:**



## Q9

##### Details:

ACME Corporation has specifically requested the app to be based on a relational database. The next set of questions relate to this RfQ-requirement.

Describe the structural aspects of the relational database model. Your description should include information about the structure in which data is stored and how relations are represented in that structure.[100-200]

**Answer:**

## Q10

Describe the integrity aspects of the relational database model. Your description should include information about the types of data integrity and how they can be enforced in a relational database.[100-200]

**Answer:**

# Q11

Describe the manipulative aspects of the relational database model. Your description should include information about the ways in which data is manipulated (added, removed, changed, and retrieved) in a relational database.[100-200]

**Answer:**



## Q12

##### Details:

The efficiency of an app (i.e. site) and the algorithms used are of the utmost importance. The next set of questions relate to this RfQ-requirement.

Identify and explain the workings of TWO sorting algorithms and discuss and compare their performance/efficiency (i.e. Big O).[300-500]

**Answer:**

## Q13

Identify and explain the workings of TWO search algorithms and discuss and compare their performance/efficiency (i.e. Big O).[300-500]

**Answer:**


## Q14


##### Details:

Companies (including ACME Corporation) value previous project experience and case studies. The following set of questions relate to this RfQ-requirement.

Conduct research into a marketplace website (app) and answer the following parts:  
a. List and describe the software used by the app.
b. Describe the hardware used to host the app.
c. Describe the interaction of technologies within the app.
d. Describe the way data is structured within the app.
e. Identify entities which must be tracked by the app.
f. Identify the relationships and associations between the entities you have identified in part (e).
g. Design a schema using an Entity Relationship Diagram (ERD) appropriate for the database of this website (assuming a relational database model).[50-100]

**Answer:**

