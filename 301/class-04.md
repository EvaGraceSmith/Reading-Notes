
### [React Docs - Forms](https://reactjs.org/docs/forms.html)

#### What is a ‘Controlled Component’?
An input form element whose value is controlled by React by keeping (maintaining) it's own state and only updated with setState. The React component that renders a form also controls what happens in that form on subsequent user input.


#### Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
Update the state as soon as they enter them, because then you can pass that value to other ui elements and reset it if needed. 


#### How do we target what the user is entering if we have an event handler on an input field?
change the react state using
this.setState({value: event.target.value})




### [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

#### Why would we use a ternary operator?
Because we are lazy coders, and less code that does the same thing is awesome. 

#### Rewrite the following statement using a ternary statement:

if(x===y){
  console.log(true);
} else {
  console.log(false);
}

 x===y ? console.log(true) : console.log(false);

### Bookmark and Review


[React Bootstrap - Forms](https://react-bootstrap.github.io/forms/overview/)

[React Docs - conditional rendering](https://reactjs.org/docs/conditional-rendering.html)

## Things I want to know more about