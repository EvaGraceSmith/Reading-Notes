## Readings: Object-Oriented Programming, HTML Tables

### Domain Modeling

#### Explain why we need domain modeling.

"When you implement a domain model, you translate the business processes into software. You try to make this translation in a way that results in the software resembling the original processes as much as possible. And to achieve this, you follow certain techniques and adopt paradigms in your design, development, and implementation."  [Functional and reactive domain modeling](https://livebook.manning.com/book/functional-and-reactive-domain-modeling/chapter-1/)

### HTML Table Basics

#### Why should tables not be used for page layouts?
* Layout tables reduce accessibility for visually impaired users
*  table layouts generally involve more complex markup structures than proper layout techniques. This can result in the code being harder to write, maintain, and debug.
* Tables are not automatically responsive

#### List and describe 3 different semantic HTML elements used in an HTML <table>.

**bgcolor**
The background color of the table. It is a 6-digit hexadecimal RGB code, prefixed by a '#'. One of the predefined color keywords can also be used.

To achieve a similar effect, use the CSS background-color property.

**border**
This integer attribute defines, in pixels, the size of the frame surrounding the table. If set to 0, the frame attribute is set to void.

To achieve a similar effect, use the CSS border shorthand property.

**cellpadding**
This attribute defines the space between the content of a cell and its border, displayed or not. If the cellpadding's length is defined in pixels, this pixel-sized space will be applied to all four sides of the cell's content. If the length is defined using a percentage value, the content will be centered and the total vertical space (top and bottom) will represent this value. The same is true for the total horizontal space (left and right).

[Table Elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/table)


### Introducing Constructors

#### What is a constructor and what are some advantages to using it?
A constructor is just a function called using the new keyword. When you call a constructor, it will:

* create a new object
* bind this to the new object, so you can refer to this in your constructor code
* run the code in the constructor
* return the new object.

#### How does the term this differ when used in an object literal versus when used in a constructor?
"Objects created using object literal are singletons, this means when a change is made to the object, it affects the object entire the script. Whereas if an object is created using constructor function and a change is made to it, that change won't affect the object throughout the script."
[object literal v constructor](https://www.tutorialspoint.com/what-is-the-main-difference-between-objects-created-using-object-literal-and-constructor-function#:~:text=Objects%20created%20using%20object%20literal%20are%20singletons%2C%20this%20means%20when,the%20object%20throughout%20the%20script.)

### Object Prototypes Using A Constructor

#### Explain prototypes and inheritance via an analogy from your previous work experience.

[JavaScript Prototypes](https://ui.dev/beginners-guide-to-javascript-prototype)

It's like having two girls. The first girl we had to buy everything new for, new clothes at each age, age appropriate toys. New schooling materials.
For girl number two, we got to reuse the clothes. Saves money, space and time. Rather than "First Daughter's stuff"  and "Second Daughter's stuff" we just have "Daughter's stuff". 

*NOTE: This is a very common front end developer interview question*

### Bookmark and Review

[HTML Table Advanced Features and Accessibility](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Advanced)