## [HTML Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)
[Your first Web Form](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form) 

[How To Structure A Web Form](https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form).

#### Why are forms so important in web development?
"Web forms are a very powerful tool for interacting with users — most commonly they are used for collecting data from users, or allowing them to control a user interface
Using the correct structure when building an HTML form will help ensure that the form is both usable and accessible."

#### When designing a form, what are some key things to keep in mind when it comes to user experience?
1. Be simple and straightforward
2. Use one column
3. Arrange your form fields from easiest to hardest
4. Use inline form field validation
5. Align text to the left
6. Clearly title your form
7. Don’t ask for phone numbers
8. Use auto-fill browsers
9. Address possible user concerns with summary boxes
10. Design mobile forms differently
11. Use positive error messages
12. Include smart defaults
13. Add progress bars for long forms
14. Use reCAPTCHAs, not CAPTCHAs
15. Enable the ability to tab to next form field

[Form design](https://blog.hubspot.com/marketing/form-design)

From a user experience (UX) point of view, it's important to remember that the bigger your form, the more you risk frustrating people and losing users. Keep it simple and stay focused: ask only for the data you absolutely need.


#### List 5 form elements and explain their importance.

##### The <input> Element
One of the most used form element is the <input> element.
The <input> element can be displayed in several ways, depending on the type attribute.

##### The <label> Element
The <label> element defines a label for several form elements.

The <label> element is useful for screen-reader users, because the screen-reader will read out loud the label when the user focus on the input element.

##### The <select> Element
The <select> element defines a drop-down list

##### The option Element
The <option> elements defines an option that can be selected.

##### The <textarea> Element
The <textarea> element defines a multi-line input field (a text area):

[Form Elements](https://www.w3schools.com/html/html_form_elements.asp)


## [Learn JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
### [Introduction To Events](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events).

#### How would you describe events to a non-technical friend?
"In the case of the Web, events are fired inside the browser window, and tend to be attached to a specific item that resides in it. This might be a single element, a set of elements, the HTML document loaded in the current tab, or the entire browser window. There are many different types of events that can occur.
* The user selects, clicks, or hovers the cursor over a certain element.
* The user chooses a key on the keyboard.
* The user resizes or closes the browser window.
* A web page finishes loading.
* A form is submitted.
* A video is played, paused, or ends.
* An error occurs."


#### When using the addEventListener() method, what 2 arguments will you need to provide?
The name of the event and a function to handle the event.
The method addEventListener() works by adding a function, or an object that implements EventListener, to the list of event listeners for the specified event type on the EventTarget on which it's called.

#### Describe the event object. Why is the target within the event object useful?
Sometimes, inside an event handler function, you'll see a parameter specified with a name such as event, evt, or e. This is called the event object, and it is automatically passed to event handlers to provide extra features and information.

#### What is the difference between event bubbling and event capturing?
Event bubbling describes how the browser handles events targeted at nested elements.

Event Capture is like event bubbling but the order is reversed: so instead of the event firing first on the innermost element targeted, and then on successively less nested elements, the event fires first on the least nested element, and then on successively more nested elements, until the target is reached.

### Bookmark and Review
[HTML5 Input Types](https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types)
This article discusses newer form controls such as:
E-mail address field
Client-side validation
Search field
Phone number field
URL field
Numeric field
Slider controls
Date and time pickers
Color picker control

[Event Reference and listings](https://developer.mozilla.org/en-US/docs/Web/Events)

"This topic provides an index to the main sorts of events you might be interested in (animation, clipboard, workers etc.) along with the main classes that implement those sorts of events. At the end is a flat list of all documented events."