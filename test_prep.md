# Concept Overviews
* [Workflow](#workflow)
* [RBAC](#rbac)
* [Remote Executes](#remote-executes)
* [Dashboards](#dashboards)
* [Transforms](#transforms)
* [APIs](#apis)

# example program/app
https://training.unqork.io/workspaces/5ec846299cc11b020f495f2c/applications/635c216cb1634555964efe54/modules 

## Workflow

## RBAC

## Remote Executes

### EX : delete submissions from viewgrid/dashboard
Steps in creating a remote execute ([link to ex](https://docs.unqork.io/Content/G-Common_Configs/G01-Dashboards/G01012-Dashboard_Remote_Delete.htm?Highlight=delete%20submission))
- create the frontend module
- create the RE to get submissions
 - within this module, original data from the submission can be ommited (for security purposes) and then used for the api response
- create the dashboard module
- create the RE for deleting the submission/s


for step one in creating a frontend module for submissions, all input fields should be toggled to 'store in database'. this includes all hidden fields that contain important information as well

for step 2, creating a remote execute to get submissions, a plugin must first be created.
plugin configuration
- should be descriptively named (pluginGetSubmissions)
- should be correct service type (Unqork > list submissions for dashboard)
- should be correct request type (GET)
- input parameters are
 - Mapping
  - workflowId ... or ... moduleId (PropertyId = 'hiddenField or copy paste')
  - fields (PropertyId = 'input1,input2,input3') 

Afterwards an initializer component can be created and set to 'new submission', it will triger the plugin

A hidden field can be created (stored in db) to store the response. From here the response from the plugin can be output to the hidden field directly or a data workflow can be used to filter the plugin's response

if a dwf is used, the plugin is used as the input and the hidden field is used as the output. the dwf van be configured to filter data by using an 'omit keys' operator in between the input and output.

<br>

## Dashboards


## Transforms

## APIs 
A common way to first understand what APIs (Application Programming Interfaces) are is with the analogy of a restaurant and a waiter. <br>
In the analogy, you, the ***Client***, ***request*** an item from the menu. The waiter is the ***interface*** between you and the kitchen. <br>
* You will ***REQUEST*** an item to the waiter
* The waiter will then tell the kitchen your request
* When done, the waiter will bring the kitchen's ***RESPONSE***

In reference to Apis, this is known as the ***Request/Response Cycle***:

![image](https://user-images.githubusercontent.com/99841849/199265199-5ae84c17-af69-474f-81e6-13d3dfb07893.png)
*APIs are what make the process easier for the 'client's' by abstracting (hiding) complex details; they provide an interface/simplified way to interact with databases and third-party applications. Programmers regularly leverage and include many different APIs to create their own applications and services.*

<br>

### API Examples
Common examples of APIs used are:
* [Open Weather](https://openweathermap.org/)
  * Used for accessing weather information from a database
* [Google's Font API](https://developers.google.com/fonts?csw=1)
  * Provides an easy way to import font styles into CSS files
* [Google Maps](https://developers.google.com/maps)
  * If you've ever seen an interactable location map on a companies website, chances are they used Google's maps api
* [Twitter Bot API](https://developer.twitter.com/en/docs/tutorials/how-to-create-a-twitter-bot-with-twitter-api-v2)
  * Allows for accounts like '@everyShrekMovieScene' or '@aceCourtBotRender'
* [Facebook Login](https://developers.facebook.com/docs/facebook-login/)   
* [Google Login](https://developers.google.com/identity/sign-in/web/sign-in)
* [Twitter Login](https://developer.twitter.com/en/docs/authentication/guides/log-in-with-twitter)

<br>

## Basic API Requests
#### GET
retrieves existing data/resource

#### PATCH
makes changes to parts of a resource

#### POST 
creates new resources

#### PUT
update existing resources

#### DELETE
deletes resources

<br>

### Common Unqork APIs
#### Internal
* [api doc](https://developers.unqork.io/#tag/Applications)

#### External
* [DocuSign](https://developers.docusign.com/)
* [SendGrid](https://docs.sendgrid.com/for-developers/sending-email/api-getting-started)

<br>

## Plugins in Unqork
The Plugin componenet is what is used in unqork to interact with apis and to 'plugin' functionality from another application/module. 

Examples of plugin usage are: 
- Frontend modules getting (parts of) submission data to display in a viewgrid component (ususally excluding sensitive info like password data)
- Server side modules calling external apis in order to provide functionality like in ... [api examples](#api-examples) and [common unqork apis](#common-unqork-apis)




# App Example 
### Concepts
* APIs
* Dashboards
* REs
* RBAC
In the following example a frontend module (login page) will provide submission data to be displayed in another module (dashboard), which will display parts of the submission data in a viewgrid. The dashboard module will call a server side module using a plugin w/ a GET request. 

* [Training env: Dashboard Practice VA](https://training.unqork.io/workspaces/5ec846299cc11b020f495f2c/applications/635c216cb1634555964efe54/modules)




