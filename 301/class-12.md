## CRUD

### [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

#### In your own words, describe what each group of status code represents:

* 100’s = Give information regarding a request.
* 200’s = Wahoo! We have success!
* 300’s = RuRoh. Let's look somewhere else.
* 400’s = Oh No! Something went wrong. We are missing something.
* 500’s = Error! Server overwhelmed or blocked

#### What is a status code 202? 
Accepted


#### What is a status code 308?
Permanent Redirect

#### What code would you use if an update didn’t return data to a client?

204

#### What code would you use if a resource used to exist but no longer does?

410

#### What is the ‘Forbidden’ status code?

403

## Videos
### [Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

#### Why do we need to pull our MongoDB database string out of our server and put it into our .env?

So we can deploy  from something other than localhost by pulling from our .env

#### What is middleware?


* a function that can only be applied using routes. We can access and modify request and response data using middleware.
* a function that will have all the access for requesting an object, responding to an object, and moving to the next middleware function in the application request-response cycle

#### What does app.use(express.json()) do?

"The app.use() function adds a new middleware to the app. Essentially, whenever a request hits your backend, Express will execute the functions you passed to app.use() in order."- (https://masteringjs.io/tutorials/express/express-json)

#### What does the /:id mean in a route?

it is a parameter we can access request.params.id It gives us access to whatever they pass in after the first slash


#### What is the difference between PUT and PATCH?

"PUT is a technique of altering resources when the client transmits data that revamps the whole resource. PATCH is a technique for transforming the resources when the client transmits partial data that will be updated without changing the whole data."- (https://byjus.com/gate/difference-between-put-and-patch-request/#:~:text=PUT%20is%20a%20technique%20of%20altering%20resources%20when%20the%20client,without%20changing%20the%20whole%20data.)

#### How do you make a default value in a schema?

Your schemas can define default values for certain paths. If you create a new document without that path set, the default will kick in.

#### What does a 500 error status code mean?

the server encountered an unexpected condition that prevented it from fulfilling the request

#### What is the difference between a status 200 and a status 201?

200: “Everything is OK.” This is the code that is delivered when a web page or resource acts exactly the way it's expected to. 201: “Created.” The server has fulfilled the browser's request, and as a result, has created a new resource

 #### Things I want to know more about:

 What rest is, and what are restful endpoints. 