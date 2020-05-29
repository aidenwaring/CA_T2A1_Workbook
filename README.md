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





## Q3

##### Details:

ACME Corporation is very big on project management, documentation and process. This will be a key metric in their decision to award the project. The following set of questions relate to this RfQ-requirement.

Discuss the implementation of Agile project management methodology. [200-300]

**Answer:**

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

