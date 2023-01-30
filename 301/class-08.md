Reading

### [API Design Best Practices](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design)


#### How does this subject matter as it relates to what I am studying?
We are currently working on a project that utilizes API's
 "API stands for application programming interface. API's are used for software applications to send and receive data. API's can also connect one program to another, to share functionality."


#### What does REST stand for?
* Representational State Transfer

#### REST APIs are designed around *resources*___.

#### What is an identifier of a resource? 
* a URI that uniquely identifies that resource

##### *Give an example.*

*the URI for a particular customer order might be:

https://adventure-works.com/orders/1


#### What are the most common HTTP verbs?
GET, POST, PUT, PATCH, and DELETE.

#### What should the URIs be based on?
"When possible, resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource)."



#### Give an example of a good URI.
"
https://adventure-works.com/orders // Good

https://adventure-works.com/create-order // Avoid"

#### What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
* bad. The more requests, the bigger the load.
* A chatty API exposes a large numer of small sresources, and may require a client application to send multiple requests to find all of the data it requires. 


#### What status code does a successful GET request return?
* the details of that item

#### What status code does an unsuccessful GET request return?
204

#### What status code does a successful POST request return?
201

#### What status code does a successful DELETE request return?
204

### Bookmark and Review

[RegExr](https://regexr.com/) - Pay particular attention to the cheatsheet
[Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)
(*This link appears to have been moved*)
[Regex 101](https://regex101.com/)

As an alternative, I found:
[JavaScript Regex](https://www.programiz.com/javascript/regex#:~:text=In%20JavaScript%2C%20a%20Regular%20Expression,a%20and%20ending%20with%20s%20.)

#### What is Regex?
* "In JavaScript, a Regular Expression (RegEx) is an object that describes a sequence of characters used for defining a search pattern. "

#### Two ways to create a RegEx
1. **Using a regular expression literal**:
The regular expression consists of a pattern enclosed between slashes /. For example,
cost regularExp = /abc/;
Here, /abc/ is a regular expression.

2. **Using the RegExp() constructor function**:
You can also create a regular expression by calling the RegExp() constructor function. For example,
const reguarExp = new RegExp('abc');


#### Things I want to know more about:
[by value, by reference](https://hackernoon.com/grasp-by-value-and-by-reference-in-javascript-7ed75efa1293)
(a good article I wanted to keep notes on)

Most things in JS are objects. The only things that aren't are Primitive Data Types.
##### What are the primitive data types?
*string, number, boolean, null and undefined. These Primitive Data Types also are immutable, which means that once created they cannot be modified.

"One of the differences between the two is that Primitive Data Types are passed By Value and Objects are passed By Reference."

##### What does this mean?
* "**By Value means creating a COPY of the original.** Picture it like twins: they are born exactly the same, but the first twin doesn’t lose a leg when the second twin loses his in the war.

* **By Reference means creating an ALIAS to the original.** When your Mom calls you “Pumpkin Pie” although your name is Margaret, this doesn’t suddenly give birth to a clone of yourself: you are still one, but you can be called by these two very different names."

When working with primitives, the =operator creates a copy of the original variable. That’s what by value means.

When working with objects, the =operator creates an alias to the original object, it doesn’t create a new object. That’s what “by reference” means.


also good:
[React- everything you need to know in 5 minutes](https://hackernoon.com/react-everything-you-need-to-know-in-5-minutes)

And:
[class vs functional components](https://plainenglish.io/blog/which-is-better-class-components-or-functional-component-in-react-a417b4ef6c1a)

**class:** 
class Hello extends React.Component {
  render() {
    return <h1>Hello World!</h1>;
  }
}

const element = <Hello />;
ReactDOM.render(
  element,
  document.getElementById('root')
);

**functional:**
function Hello() {
  return <h1>Hello World!</h1>;
}

const element = <Hello />;
ReactDOM.render(
  element,
  document.getElementById('root')
);

(both do the same thing in react)
