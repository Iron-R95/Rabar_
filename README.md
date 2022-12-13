# Postman  ![postman-logo-icon-orange](https://user-images.githubusercontent.com/43212219/206572553-5f96ba62-267a-485a-9434-00cc25e31c21.svg)


###### Introduction to the Postman world

-------

### Table of contents

...

...


...

--------
### 0. Intro

Postman is more than just an API-client that Postman is known for. Postman is a platform with a set of very useful tools that will make creating and managing APIs easier, and besides, Postman can save developers a lot of time and effort.

---------

### 1. Installation

Developers can use Postman in different ways, Postman can be used both as a web-app and as a Desktop-app, in addition, Postman is available for different operating systems such as Linux, Windows, etc.

And developers can also use Postman without having to register, but registration is recommended as it has some advantages, e.g. data backup, because Postman is cloud-based or registration is mandatory if developers want to set up a public workspace or network. I've already registered so that I can show all the important parts of Postman in the course of this tutorial.

The following screenshot shows what Postman looks like after installation, the developer can register or log in directly or at the bottom left there is also the possibility to use Postman directly without an account.

![Screenshot from 2022-12-08 20-56-03](https://user-images.githubusercontent.com/43212219/206555066-4ce9d7b4-42e2-439d-8533-b6f45260aeec.png)

---------

### 2. API-Repository

Developers can store, catalog and collaborate on one central platform. Postman provides us with a cloud-based and centralized repository throughout the API-Lifecycle, so we will have no any kind of problem by storing and managing of API specifications, tests, workflow, documentation, etc. And it doesn't matter if we have only one API or multiple APIs, we can very well organize and simplify everything around API world with Postman-API-Repository.


#### 2.1. API-Network

 ##### 2.1.1. Private API-Network
 
Teams and organizations can set up a private API network with Postman, which is only visible to authorized people and supports creating API versions.
 

 ##### 2.1.2. Public API-Network
 
 According to Postman, Postman's Public-API-Network is the world's largest public API-Hub, which many well-known companies like Microsoft, Google, etc.    are on. With the help of Public-API-Network we can release Worksapces, APIs, and other things worldwide

---------
### 3. Workspace

When we start postman, the first thing we have to do is create a workspace so that we can use the postman tools at all.

There are four workspace types in postman, these are:

+ **Personal Workspace**: As the name suggests, this is mainly personal and it contains all the tools we need to build, manage APIs. Everything in this area happens in real time, so we can easily switch between the Postman-instances, web- and desktop-app at any time.

+ **Team Workspace** (more than 3 members -> Pro or Enterprise edition): This allows creating a workspace for multiple people, and even assign them specific roles like admin, editor and viewer.

+ **Private Workspace** (only available in the Pro and Enterprise editions): There is the possibility that not all team members have access, but only members who receive an invitation.

+ **Partner Worspace**: Is similar to a private workspace, you can not only invite team members but also external users as partners.
Unlike the other workspaces, we cannot create a partner workspace directly, it is invisible at first. For this you have to go through a few steps first, see how to create [Partner-Workspace](https://blog.postman.com/introducing-partner-workspaces/) via Postman.

+ **Public Workspace**: We can publish or make our APIs available worldwide by setting up a public workspace.


The following image shows how to create a workspace, we simply have to click on workspace in the top left of the Postman web or desktop app, then give the workspace a name and next select the workspace type, e.g. Personal and finally click on Create Workspace.

![create_workspace](https://user-images.githubusercontent.com/43212219/207112977-c257b31f-4aa2-497a-a840-973af1fc78c2.png)


-------

### 4. Tools

We have the ability to manage the API-Lifecycle from design to testing, documenting, API-mocking and etc. all of this can be done with the helpful and user-friendly tools of Postman. In this section I will introduce the Postman-Tools and make a small example of it so that we can get an idea of them.

If we now go to our already created workspace, we will see the tools (Collections. APIs, Environments, Mock Servers, Monitors and Flows) on the left side. We will look at these tools next by using examples.

![Untitled](https://user-images.githubusercontent.com/43212219/207124332-b74adea7-8454-4a5c-93aa-20d1ea6f373e.png)




#### 4.1. API-Client

The foundational tool for which POstman is well known among developers. No matter if we want to test or debug the APIs or define simple and complex API-Requests for HTTP, REST, GraphQL and WebSocktes, we can do all these with Postman API Client. In addition, the API client can automatically recognize a lot more, for example the language of the response or authentication types to the server.

First we should create a collection by simply clicking the Plus button, then a collection will be automatically generated, we can name it whatever we want, in my case it's called My Collection.

we can now click Add a request to make an API call.

![coolll](https://user-images.githubusercontent.com/43212219/207129448-77515cad-5744-4ae6-ab11-5d4dd201158a.png)


Here I create an API-request called FetchUsers because I want to fetch a List of User. We now have the ability to use different HTTP methods(1) and we can call any API URL(2), for that I used the https://gorest.co.in/  to get back a list of test users.

![MS Paint _ Microsoft Paint Online](https://user-images.githubusercontent.com/43212219/207147530-339cda91-33d9-4c30-bb9b-dc2f4dd4f420.png)

If we now click on send, we get back a JSON file in pretty-print as a response. We can also change the representation on different data structures.

![Screenshot from 2022-12-12 21-28-51](https://user-images.githubusercontent.com/43212219/207148688-a2386719-2ede-4377-bd50-833164d67a46.png)

We can also call google.com and display it as a Perview.

![Screenshot from 2022-12-12 21-35-13](https://user-images.githubusercontent.com/43212219/207149181-dcdf04dd-cf54-4dd1-904f-5f8070693f64.png)

If we want to use an HTTP-Post, then we can enter the data directly as a body, and if authentication against the server is required, as in our example, this can be set under Authorization, there are different types.

There are also other options such as :

+ Params: here we have the possibility, for example, to enter query params. Alternatively, we can put it directly at the top of the Uri
+ Headers: different headers e.g. Content-Type etc.
+ Body: is needed if we want to use HTTP post
+ Pre-request-Script: here we can run some code before the request is made
+ Tests: you can also write tests for the API request 
+ Settings: various settings e.g. HTTP/HTTPs or requests-limiting etc.

![Screenshot from 2022-12-12 21-40-51](https://user-images.githubusercontent.com/43212219/207150074-e418138b-3e8c-4cd5-82c8-0034261cd499.png)

---------------

API-Documentation

We can write parallel documentation for the request. The documentation tool supports plain-text markdown languages etc.

![Screenshot from 2022-12-13 12-41-10](https://user-images.githubusercontent.com/43212219/207309682-1dcf710c-7109-4af7-acad-c362b9e668c1.png)

![Screenshot from 2022-12-12 22-08-00](https://user-images.githubusercontent.com/43212219/207319557-ed6a3762-4f5a-4217-858c-ee66e3e81089.png)



Postman automatically writes the parameters to the documentation, and we can also rewrite them however we want.

![Screenshot from 2022-12-13 12-40-15](https://user-images.githubusercontent.com/43212219/207309516-21c793d7-b2d4-4194-83e5-557339feee82.png)




---------
#### API-Design


We can also specify in Postman how our API-Structure should be, for that Postman provides us with various Schema-Types such as OpenAPI, GraphQL etc. and we can also choose the formatting as YAML or JSON. To learn more about this just read the API-Design [here](https://learning.postman.com/docs/designing-and-developing-your-api/developing-an-api/defining-an-api/).

![Screenshot from 2022-12-12 22-01-14](https://user-images.githubusercontent.com/43212219/207153852-6e05aa75-60e7-477d-a2fb-8b6dc9e86026.png)







-------------------
#### AP-Testing

Postman allows Test-Scripts to be written in JavaScript to verify that the APIs are working as they should.  To learn API-Testing, just read this [documentation](https://learning.postman.com/docs/writing-scripts/test-scripts/)

------

#### Mock-Server

If we don't have real API-servers, we don't have to worry because Postman has the ability to simulate individual API servers, so we can do whatever we want. we can also simulate the network latency in the mock server. to learn more about Postman mock servers, you can read this [documentation](https://learning.postman.com/docs/designing-and-developing-your-api/mocking-data/setting-up-mock/).


![Screenshot from 2022-12-13 14-02-12](https://user-images.githubusercontent.com/43212219/207325626-3ebf6c01-82cc-4463-8d45-199c14ecd303.png)



-------
#### Monitoring

With [Postman-Monitors](https://learning.postman.com/docs/monitoring-your-api/intro-monitors/) we can create a graphical representation of the state of our APIs. So we can check at any time whether the APIs are healthy or have enough performance.

We can also determine when to run the monitoring process and also be notified by email if there is any error.

![Screenshot from 2022-12-13 14-17-54](https://user-images.githubusercontent.com/43212219/207328654-8b126006-b2af-4bba-a6f9-b4dd06ffffaf.png)


![Screenshot from 2022-12-13 14-24-27](https://user-images.githubusercontent.com/43212219/207331425-5d43b769-3a08-4bdf-8cde-2ce46e006ea0.png)


------


#### Flows

Postman Flow is a relatively new feature that allows us to create API-Workflows to map and execute various actions together. There are widgets for that, which we can simply move back and forth using drag-drop.

![Screenshot from 2022-12-13 14-31-12](https://user-images.githubusercontent.com/43212219/207336612-9074a538-dc46-44d1-911b-17d2597f8bde.png)

An example of Postman-Team.

![Screenshot from 2022-12-13 14-37-56](https://user-images.githubusercontent.com/43212219/207338434-62d71e0e-2ac0-454c-84c0-609db72c3808.png)




----------

### Explore

With Postman-Explor we can find big companies worldwide that provide their APIs and also teams, workspaces, collections, flow etc.


![Screenshot from 2022-12-13 14-42-49](https://user-images.githubusercontent.com/43212219/207341615-84066d87-9995-4da8-953a-c225955dea49.png)


![Screenshot from 2022-12-13 14-43-42](https://user-images.githubusercontent.com/43212219/207341728-c6502229-43b2-487e-95f9-4abe7e735f54.png)



