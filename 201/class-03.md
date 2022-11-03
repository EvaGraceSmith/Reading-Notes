# Readings: HTML Lists, Control Flow with JS, and the CSS Box Model

### Learn HTML- Ordered and Unordered lists

When should you use an unordered list in your HTML document?

* When creating a list of related items, in no particular order

How do you change the bullet style of unordered list items?

* By using the list-style-type property in CSS

When should you use an ordered list vs an unorder list in your HTML document?

* Use an ordered list when the order matters

Describe two ways you can change the numbers on list items provided by an ordered list?

* By using the type attribute

  * type="1" The list items will be numbered with numbers (default)
  * type="A" The list items will be numbered with uppercase letters
  * type="a" The list items will be numbered with lowercase letters
  * type="I" The list items will be numbered with uppercase roman numbers
  * type="i" The list items will be numbered with lowercase roman numbers

    <ol type="1">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>

</ol>

### Learn CSS- The Box Model

Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?
List and describe the four parts of an HTML elements box as referred to by the box model.

* Margin is the moat outside the castle walls
* Border are the castle walls
* Padding is the streets surrounding the castle (Padding=Matting)
* Element is the castle

### Learn JS- Arrays. Operators and Expressions. Conditionals. Loops

What data types can you store inside of an Array?

* primitives=(boolean, number, string, null, undefined) and object (6 total)

Is the people array a valid JavaScript array? *yes*

If so, how can I access the values stored? If not, why?

* console.log(people);

 const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];

List five shorthand operators for assignment in javascript and describe what they do.

* The addition assignment operator (+=) adds the value of the right operand to a variable and assigns the result to the variable. 
* The subtraction assignment operator (-=) subtracts the value of the right operand from a variable and assigns the result to the variable.
* The multiplication assignment operator (*=) multiplies a variable by the value of the right operand and assigns the result to the variable.
* The division assignment operator (/=) divides a variable by the value of the right operand and assigns the result to the variable.
* The remainder assignment operator (%=) divides a variable by the value of the right operand and assigns the remainder to the variable.


Read the code below and evaluate the last expression and explain what the result would be and why.

 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;

Describe a real world example of when a conditional statement should be used in a JavaScript program.
A Shopping Cart

Give an example of when a Loop is useful in JavaScript.
Adding up a total in a Shopping Cart