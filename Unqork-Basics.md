
<br>

# Unqork Basics
------------------------------------------------------------------------------------------------------------------
## Table of Contents
1. [Environment Basics](#unqork-environment-basics)
2. [Overview of Modules and Components](#overview-of-modules-and-components)
3. [Components: basic structuring and usage](#components-basic-structuring-and-usage)



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
 Regular Expression Pattern <br> (Client Side Form Valid) | ^[a-zA-Z]*$
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
        
### Modules Overview:
#### Intro to the Module Editor:
The module editor is what is used to change the display, function, and purpose of a module.
The module editor contains the **Components library** (seen in components overview), which will contain 
all of the smaller building blocks which will affect how the module functions.

<"img src="https://docs.unqork.io/Content/Resources/Images/AppBuild_Primary_Fields_Intro.jpg"  width="300" height="300"> <br>
![](https://docs.unqork.io/Content/Resources/Images/AppBuild_Primary_Fields_Intro.jpg)

<br>

### Components Overview:
####  Intro to the Components Library:
Components are the smallest building block when creating applications and they range in purpose. 
They range from simple input fields to complex api plug in components. Each component has its own set of properties 
that affect how the component functions.

#### ***Primary Fields:*** 
* Text Field
* Text Area
* Checkboxes
* Multi-Select Dropdown
* Radio Buttons
* Dropdown
* Number
* Date Input
* Single Checkbox
* [Ex images](https://academy.unqork.com/path/associate-configurator/introduction-to-primary-fields/589015)
* ***Note turn these to links in the docs***

#### ***Secondary Fields:***
* Protected Field 
* Button 
* Email 
* Phone Number 
* Intl Phone Number 
* Address 
* Hidden 
* Signature 
* [Ex images](https://academy.unqork.com/path/associate-configurator/introduction-to-secondary-fields/590614)

#### Display and Layout
* Grid Systems 
* HTML Element 
* Content 
* Data Grid 
* Matrix 
* Columns 
* Panel
* Table
* Advanced Data Grid
* Navigation
* View Grid
* Field Group
* Rich Text Editor
* Repeater


#### Data and Event Processing
* File
* Data Mapper
* Decisions
* Initializer
* Plug-in
* Calculator
* Data Table
* Data Workflow
* Checkpoint
* Timer
* Plaid
* File Storage
* Browser Storage


#### Charts and Graphs
* KPI
* Chart


<br> 


### Resources Used:
* [Associate Configuator](https://academy.unqork.com/path/associate-configurator)
    * [Intro to Primary Fields](https://academy.unqork.com/path/associate-configurator/introduction-to-primary-fields)
    * [Intro to Secondary Fields](https://academy.unqork.com/path/associate-configurator/introduction-to-secondary-fields)
* [Unqork Docs - Intro to Modules](https://docs.unqork.io/Content/A01-ModEditor-General/A01007-Module_Introduction.htm?Highlight=module%20editor)

<br>
<br>
<br>


## Components: Basic Structuring and Usage
-------------------------------------------------------------------------------------------------------------------
### Basic Data Types and Structures:
In Unqork data is categorized into 3 basic types ...

* **Numbers**
* **Strings**
* **Booleans**

Numbers can be further specified based on expected decimal value 
* **Integers**
* **Decimals**

The data type of input is specified in the **Component Configuration** ...

<br>

### The Component Configuration Window
#### General
Setting             |           Description
:------------------:|:------------------------:
Active              |   By default this toggle is set to 'ON', which means that the component is visible and accessible by other components
Property Id         |   Id's must use camelCase, A Property ID is the unique field ID used by Unqork to track and link components in your module
Field Tags          |   Field Tags are one-word labels used to identify a group of components. Field Tags let you target two or more components using a single Decision or Initializer. 
Settings Tab        |   Selecting this tab shows the component's Display, Data, Actions, and Validation settings panels as applicable.
Permissions Tab     |   Selecting this tab shows the component's role-based access control (RBAC) settings.
Notes Tab           |   This tab is used for component documentation
Cancel Button       |   
Save Button         |


<br>

#### Display
Setting             |           Description
:------------------:|:------------------------:
Label Text          |   Applies label text for the input component
Tooltip             |   A short hint that appears when an end-user positions their cursor over the  (Tooltip) icon. Tooltips can display across more than one line.
Placeholder Text    |   Provides text inside of the input area of the text input component
Helper Text         |   Provides additional information for the input, unlike the tooltip helper text stays visible under the component
Hide Label          |   This toggle hide the label
Disable User Input  |   This toggle prevents user input
Read Only View      |   This toggle makes the component into 'display only'
Hide Field          |   This toggle hides the field


<br>

#### Validation
Setting             |           Description
:------------------:|:------------------------:
Required            |   This toggle makes component input required for form submission
Min/Max Length      |   These values define the min and max of characters for the input



<br>

### Primary Fields

<br>

### Secondary Fields

<br>

### Layout and Display
#### Intro to the Grid System

<br>

### Data and Events Processing
#### Triggering w/ buttons

<br>

### Charts and Graphs

<br>

### Building a basic application
* [Hello World](https://academy.unqork.com/developer-guide/1149556/scorm/l45tk7tmcr6x)
* [Unqork User Manual - 20 min App](https://docs.unqork.io/Content/A00-Unqork_Platform/A00003-Unqork_In_20_Minutes.htm)

### Resources Used:
* [Associate Configuator](https://academy.unqork.com/path/associate-configurator)
    * [Intro to Primary Fields](https://academy.unqork.com/path/associate-configurator/introduction-to-primary-fields)
    * [Intro to Secondary Fields](https://academy.unqork.com/path/associate-configurator/introduction-to-secondary-fields)
    * [Intro to data types](https://academy.unqork.com/path/associate-configurator/introduction-to-data-types)
    * [Layout and display](https://academy.unqork.com/path/associate-configurator/introduction-to-display-and-layout)
    * [Intro to data and event processing](https://academy.unqork.com/path/associate-configurator/introduction-to-data-and-events-processing)
    * [Triggering w/ buttons](https://academy.unqork.com/path/associate-configurator/triggering-with-buttons)

* [Unqork Docs - Components Library](https://docs.unqork.io/Content/A02-ModEditor-Primary/A02000-Primary_Fields_Introduction.htm)
    * *Contains the same content* 


<br>
<br>
<br>
<br>


## Intro to APIs
-------------------------------------------------------------------------------------------------------------------
stuff here

<br>

### Resources Used:
* [Associate Configuator](https://academy.unqork.com/path/associate-configurator)
    * [Intro to APIs](https://academy.unqork.com/path/associate-configurator/what-is-an-api)

<br>
<br>
<br>
<br>



## Form Basics
--------------------------------------------------------------------------------------------------------------------
Data Validation
Text Fields
https://docs.unqork.io/Content/A01-ModEditor-General/A01201A-Regex_In_Unqork.htm

<br>
<br>
<br>
<br>


## Server Side execution
--------------------------------------------------------------------------------------------------------------------
Data Security

<br>
<br>
<br>
<br>


## Writing Transforms (Converting data/file types)
--------------------------------------------------------------------------------------------------------------------
https://docs.unqork.io/Content/A01-ModEditor-General/A01018B-Writing_Transforms_Using_JSON_and_Nunjucks.htm

<br>
<br>
<br>
<br>

