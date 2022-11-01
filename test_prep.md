# Concept Overviews
* [Workflow](#workflow)
* [RBAC](#rbac)
* [Remote Executes](#remote-executes)
* [Dashboards](#dashboards)
* [Transforms](#transforms)
* [APIs](#apis)

## Workflow

## RBAC

## Remote Executes

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

#### External
* [DocuSign]()
* [SendGrid]()

<br>

## Plugins in Unqork
The Plugin componenet is what is used in unqork to interact with apis and to 'plugin' functionality from another application/module. 

Examples of plugin usage are: 
- Frontend modules getting (parts of) submission data to display in a viewgrid component (ususally excluding sensitive info like password data)
- Server side modules calling external apis in order to provide functionality like in ... [api examples](#api-examples) and [common unqork examples](#common-unqork-examples)

Plugin components are often used to manipulate submission data from frontend modules. In this ex a plugin will be used to GET submission data from a login page and display it in a viewgrid component

plugins have 5 basic request types



