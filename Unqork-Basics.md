
<br>

# Unqork Basics
------------------------------------------------------------------------------------------------------------------
#### Official Resources:
* [Training Environment](https://training.unqork.io)
* [Unqork Academy](https://academy.unqork.com/)
    * [Associate Configurator](https://academy.unqork.com/path/associate-configurator)
    * [Developer Guide](https://academy.unqork.com/developer-guide)
* [Unqork Docs](https://developers.unqork.io/)
* [Unqork User Manual](https://docs.unqork.io/Content/LandingPages/Landing_UserManual.htm)
* [Unqork YouTube Channel](https://www.youtube.com/channel/UC4fU3i-_WG4yDn8e2LeYgPQ)

#### Common Resources:
* [M.D.N.](https://developer.mozilla.org/en-US/)
* [HTML5 cheat sheet](https://quickref.me/html)
* [CSS3 cheat sheet](https://quickref.me/css)


<br>


#### Useful stuff:
Tool        | Formula/URL | 
:----------:|:-------------:
 Devtools Console Angular Command   |   angular.element('.unqorkio-form').scope().submission   
 Send Grid API Docs                 |   https://sendgrid.com/docs/api-reference/    
 Module Submission Path             |   =concatenate('/#/display/',moduleId,'/',submissionId,'/',moduleId    
 MomentJS Formula                   |   =moment(moment(),'diff',moment(a),'years')
 HTML Anchor Tag                    |   \<a href="">\</a>
 SSN Formula                        |   ssn=CONCATENATE("***-**-",GET(ssn,5),GET(ssn,6),GET(ssn,7),GET(ssn,8))
 Delete/Get Workflow submission Endpoint |  /fbu/uapi/workflows/{workflowId}/submissions/{submissionId}
 App ID for Weather API             |   4e25461876c6722efa0f107814b65203
 

<br>
<br>
<br>
<br>


## Unqork Environment Basics
-----------------------------------------------------------------------------------------------------------------------
### File system navigation
Unqork uses element configuration as apposed to code in order to develop applications. <br>
Although Unqork functions on top of an abstraction of the low level code, it is structured in a familiar way . . .


Common Term     |  Unqorks Term |
:--------------:|:------------------:
Environment/Organizations | Environment
Repository      | Workspace
Folders         | Application
Files           | App elements: *Modules, Workflows, Data Collections*

Navigation Demo: [Unqork Bootcamp - Intro to the Platform](https://academy.unqork.com/path/bootcamp/unqork-101-and-102/653995)

<br>


### Workspaces:
When you log in to the ***Unqork Designer platform***, Unqorks IDE, the default landing page is your companies environment in workspaces. Workspaces is the entry point into the Unqork Designer platform.

Like a repository, **Workspaces** house single or multiple projects based on the needs and preferences of your organization. 

<br>

### Applications:
Within workspaces you can create applications. **Applications** house and organize associated **elements** . . .


#### Application Elements:

Element Type    | Description
:---------------:|:-----------------------:
Modules         |   Modules are the equivilant of code files. Modules contain the **low level** rules of an application and can <br> configure client side display and server side execution.
Workflows       |  Workflows are like the **higher level** pseudo-code of the application. They configure and link the logic between modules similar to Model–view–controller (MVC) is a software architecture.
Data Collections |  Data collections are static data referenced by your applications.

<br>

### Resources Used:
* [Unqork Academy - Introducing the Platform](https://academy.unqork.com/introducing-the-unqork-platform?next=%2Fintroducing-the-unqork-platform%2F657299.)
* [Unqork Dev Guide - Setup & Nav](https://academy.unqork.com/developer-guide/1149553/scorm/6cesnexaguka)


<br>
<br>
<br>
<br>


## Overview of Modules and Components
---------------------------------------------------------------------------------------------------------------------
### Vocabulary:
* **Modules:** modules are building blocks of *Applications*, 
    * use cases of modules:
        * A Sign in page
        * A Survey/Feedback page
* **Components:** components are the building blocks of *Modules*,
    * use cases of componenets:
        * A text input field
        * A radio input field (multiple choice)

<br>

### Components Overview:
####  Intro to the Components Library:
#### ***Primary Fields*** 
``` 
    insert examples and screenshots here
```
#### ***Secondary Fields***
``` 
    insert examples and screenshots here
```

<br> 

### Modules Overview:
#### Intro to the Module Editor:
``` 
    insert examples and screenshots here
```

<br>

### Resources Used:
* [Associate Configuator](https://academy.unqork.com/path/associate-configurator)
    * [Intro to Primary Fields](https://academy.unqork.com/path/associate-configurator/introduction-to-primary-fields)
    * [Intro to Secondary Fields](https://academy.unqork.com/path/associate-configurator/introduction-to-secondary-fields)


<br>
<br>
<br>


## Basic Structuring
-------------------------------------------------------------------------------------------------------------------
### Basic Data Types and Structures:
In Unqork data is categorized into 3 basic types ...

* **Numbers**
* **Strings**
* **Booleans**

Numbers can be further specified based on expected decimal value 
* **Integers**
* **Decimals**

<br>

### Layout and Display

<br>

### Data and Events Processing

<br>

### Triggering with buttons

<br>

### Building a basic application
* [Hello World](https://academy.unqork.com/developer-guide/1149556/scorm/l45tk7tmcr6x)
* [Unqork User Manual - 20 min App](https://docs.unqork.io/Content/A00-Unqork_Platform/A00003-Unqork_In_20_Minutes.htm)

### Resources Used:
* [Associate Configuator](https://academy.unqork.com/path/associate-configurator)
    * [Intro to data types](https://academy.unqork.com/path/associate-configurator/introduction-to-data-types)
    * [Layout and display](https://academy.unqork.com/path/associate-configurator/introduction-to-display-and-layout)
    * [Intro to data and event processing](https://academy.unqork.com/path/associate-configurator/introduction-to-data-and-events-processing)
    * [Triggering w/ buttons](https://academy.unqork.com/path/associate-configurator/triggering-with-buttons)


<br>
<br>
<br>
<br>


## Intro to APIs
-------------------------------------------------------------------------------------------------------------------


<br>

### Resources Used:
* [Associate Configuator](https://academy.unqork.com/path/associate-configurator)
    * [Intro to APIs](https://academy.unqork.com/path/associate-configurator/what-is-an-api)

<br>
<br>
<br>
<br>




