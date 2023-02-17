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

C -> Create -> Post
R -> Read  -> Get
U -> Update -> Put
D -> Delete -> Delete


If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

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


#### How does this subject matter as it relates to what I am studying?
We are currently building full stack projects incorporating CRUD. 


#### Things I want to know more about:
How to refactor routes.  