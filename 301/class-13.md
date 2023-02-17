## [CRUD Basics](https://medium.com/geekculture/crud-operations-explained-2a44096e9c88)


"CRUD is an acronym that stands for Create, Read, Update and Delete"
They are the four major functions used to interact with database applications

* PUT replaces a resource (even if that resource doesn’t yet exist), while POST usually adds a new resource. They can both be used to Create new resources, but PUT is mainly used to Update existing resources.
* PATCH is used to Update part of a resource, whereas PUT is only used to Update an entire resource (by replacing it).
* POST is processed “according to the resource’s own specific semantics” (per the RFC), making it something of a catch-all. It can even have Update functionality, like when sent to an /updates/ subresource.




#### Which HTTP method would you use to update a record through an API?

Put

#### Which REST methods require an ID parameter?
 REST stand for Representational State Transfer, it is an HTTP method

 Put, Delete


(https://rapidapi.com/guides/rest-parameter-types)
 (https://www.cordra.org/documentation/api/rest-api.html)


Videos
### [Speed Coding: Building a CRUD API (Watch a Twitch streamer code an Express API in 20 minutes!)](https://www.youtube.com/watch?v=EzNcBhSv1Wo)

#### What’s the relationship between REST and CRUD?

* C -> Create -> Post
* R -> Read  -> Get
* U -> Update -> Put
* D -> Delete -> Delete


If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

[5 Steps for designing your REST API](https://www.wutsi.com/read/246/5-steps-for-designing-your-rest-apis)

##### 1. Identify your Object Model
In the REST world, they are called Resources. A Resource is an typed object with data. 
##### 2. Identify the URIs
A URI is a unique address assigned to resources, it's a way to identify Resources on the Internet.  
##### 3. Define the Representations
Next step is to define the content and the format of your resources. The most common formats are JSON, XML or Protobuf. For each resource in your Object Model, you must define a representation for a collection and single resource.
##### 4. Assign HTTP Methods
The next step is to define how to access your resources via HTTP. For that, you need to use the standard HTTP methods:

* GET to retrieve Resources
* POST to create or update a Resource
* DELETE to delete a Resource

Read All: (Get all...)
 router.get('/', (req, res, next)=>{

 });

 Read One: (Get one specific... by id)
 router.get('/:id, (req, res, next)=>{

 });

Create One:
 router.post('/', (req, res, next)=>{

 });

 Update One:
router.put('/:id', (req, res, next)=>{

});

 Delete One:
router.delete('/:id', (req, res, next)=>{

});

##### 5. What about Errors

For REST API, you should use HTTP status codes to report the status of each interaction with your API.  

#### How does this subject matter as it relates to what I am studying?
We are currently building full stack projects incorporating CRUD. 


#### Things I want to know more about:
How to refactor routes.  