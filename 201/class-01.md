# Reading
Getting Started
Skim [How the Web Works](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works).
Skim [Website Design and Process.](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/What_will_your_website_look_like)
Read the following sections of [JavaScript Basics: Start at “What is JavaScript?”](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics), read through “Comments” section.

## Compose a short poem describing how HTTP sends data between computers. 
 * Client request
 * this is the best
 * Server responds
* this is the bomb

## Describe how HTML, CSS, and JS files are “parsed” in the browser.
They are parsed in this order:
1. HTML
2. CSS
3. JS

## How can you find images to add to a Website?

* Go to Google Images and search.
* When you find the image you want, click on the image to get an enlarged view of it.
* Right-click the image (Ctrl + click on a Mac), choose Save Image As…, and choose a safe place to save your image. Alternatively, copy the image's web address from your browser's address bar for later use.

## How do you create a String vs a Number in JavaScript?
To signify that the value is a string, enclose it in single quote marks.	let myVariable = 'Bob';
Numbers don't have quotes around them. let myVariable = 10;

## What is a Variable and why are they important in JavaScript?
Variables are containers that store values
Variables are necessary to do anything interesting in programming. If values couldn't change, then you couldn't do anything dynamic, like personalize a greeting message or change an image displayed in an image gallery.

# Introduction to HTML
 [Getting Started with HTML.](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started)
[HTML Document Structure.](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure)
 [Metadata in HTML.](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML)

## What is an HTML attribute?
Attributes contain extra information about the element that won't appear in the content.

## Describe the Anatomy of an HTMl element.
* **The opening tag**: This consists of the name of the element  wrapped in opening and closing angle brackets. 
* **The content:** This is the content of the element. 
* **The closing tag:** This is the same as the opening tag, except that it includes a forward slash before the element name. 

## What is the Difference between \<article> and \<section> element tags?
\<article> encloses a block of related content that makes sense on its own without the rest of the page (e.g., a single blog post).
\<section> is similar to \<article>, but it is more for grouping together a single part of the page that constitutes one single piece of functionality 

## What Elements does a “typical” website include?
* <html></html>: The <html> element. This element wraps all the content on the page. It is sometimes known as the root element.
* <head></head>: The <head> element. 
* <meta charset="utf-8">: The <meta> element. This element represents metadata that cannot be represented by other HTML meta-related elements, like <base>, <link>, <script>, <style> or <title>. 
* <title></title>: The <title> element. 
* <body></body>: The <body> element.

##  How does metadata influence Search Engine Optimization?
Specifying a description that includes keywords relating to the content of your page is useful as it has the potential to make your page appear higher in relevant searches performed in search engines 
## How is the <meta> HTML tag used when specifying metadata?
Metadata is data that describes data, and HTML has an "official" way of adding metadata to a document — the <meta> element.

# How to start to design a Website.
[how to design a website.](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Thinking_before_coding)

## What is the first step to designing a Website?
1. Planning- What will it do?
2. Sketch out your design
3. Choosing your assets- what content will appear on your webpage ie
    1. Text
    2. Theme Color
    3. Images
    4. Font

## What is the most important question to answer when designing a Website?
What exactly do I want to accomplish?

[HTML Document Structure](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure)

[Semantics.](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)

## Why should you use an \<h1> element over a \<span> element to display a top level heading?
 the \<h1> element gives the text it wraps around the role of a top level heading on your page.
## What are the benefits of using semantic tags in our HTML?
It gives the piece of code meaning.

[What is JavaScript?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript)

## Describe 2 things that require JavaScript in the Browser?
control multimedia, animate images

## How can you add JavaScript to an HTML document?
JavaScript only needs one friend in the world of HTML — the <script> element
### Internal Directions:
1. First of all, make a local copy of our example file apply-javascript.html. Save it in a directory somewhere sensible.
2. Open the file in your web browser and in your text editor. You'll see that the HTML creates a simple web page containing a clickable button.
3. Next, go to your text editor and add the following in your head — just before your closing </head> tag:
<script>
  // JavaScript goes here
</script>
Copy to Clipboard
4. Now we'll add some JavaScript inside our <script> element to make the page do something more interesting 
5. Save your file and refresh the browser — now you should see that when you click the button, a new paragraph is generated and placed below.

### External Directions:

1. First, create a new file in the same directory as your sample HTML file. Call it script.js — make sure it has that .js filename extension, as that's how it is recognized as JavaScript.
2. Replace your current "<script>" element with the following:
"<script src="script.js" defer></script>"
 Copy to Clipboard
3. Inside script.js, add the following script:
4. Save and refresh your browser, and you should see the same thing


