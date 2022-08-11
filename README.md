## Git

### Why do we use Git?

We use git as a version control system. It allows us to track changes to a project. 


### What’s the difference between Git and GitHub?

Git is a version control system that allows you to track changes to a project. 

Github is the website where the changes are stored 

### What happens when you clone a repository?

The command ‘git clone’ allows you to clone a repository to your local drive. 

### What happens when we do git pull origin main ?

The command ‘git pull origin main’ will update your local repository to the newest version 

### How do we create a new branch on our local machine?

Use the command: git checkout -b [new-branch-name]
 
### How do we control which changes will be included in the next commit?

You can use the command git add [name-of-file]
For example, git add index.html 

### When might git add . be inappropriate?

When you want to add ALL the changes you’ve made to the staging area. 

### How do we make sure our local changes don’t conflict with main?

Create a new branch as raise a PR request when working on an issue 

### What does git push origin [branch-name] do?

The command git push origin [branch-name] will push the changes made to that branch. You can the raise a PR to get it merged with the main branch


### Why do we make pull requests instead of just changing main directly?

The ‘main’ is what the output of your project should look like. Your code need to be reviewed / checked before merging with the main. This is why we create branches and PR requests. 

It also helps to avoid conflicts. 

### Why should you review your teammates’ pull requests?

Before merging code to the main, you want to check your teammates’ code is correct. This could cause errors to the main file if not checked. (It’s nice to look at other peoples code, too)

--------------------------------------

## HTML

###  Why is accessibility important?

Because the internet is for everybody.  

### How can you quickly find simple accessibility problems?

We can use the built in checker on the Google Chrome browser, Lighthouse. 

###  What is semantic HTML?

Semantic HTML tags help with accessibility and making the document look neater. It helps screen readers know what to look for and organises your HTML.  

They describe the information within the tag clearly. 

###  Why is it important to use the “correct” semantic element?

They describe the information within the tag clearly and the screen reader will user semantic tags to try and understand the information within the tag. 

### What is the <form> element used for?

The form element (or tag) is used to create a form for the user. You can have different inputs within a form and the user can input information. 

--------------------------------------

## CSS

### How would you use CSS variables to make a reusable colour palette?

You can use ‘root’ pseudo-class in your CSS to declare colour variables. You can then add the variables in your CSS.

### How would you use flexbox to make elements sit on a single line?

I would apply these two lines of code to the parent element. 

display: flex;
flex-direction: row;

The flex direction is set to row by default, so you'll only need to apply 'display: flex' to the parent. 

### How would you use grid to make a layout that automatically adds columns as the screen gets wider?

grid-auto-columns: auto;

###  Why is it important to create a responsive design?

Because as developers we do not know what device the user will open the application/website on. We need the application to be accessible for small mobiles to 4k monitors. 

 ### How would you structure your CSS to make it “mobile-first”?

I would write the CSS for the smallest mobile screen. I would then use media queries and different break points for different devices sizes. 

--------------------------------------

## Javascript 

 ### Why should we avoid using var to define variables?

From ES6 onwards (2015 I think…?) a new way to declare variables was introduced. 

It is related to scope. Function scope and block scope. If you declare a variable using var inside a function, it is accessible outside of that function. 

We should avoid using Var and use let or const instead. 

 ### How might you make a long, complex chunk of code easier to read?

I would divide the code up into smaller functions and then call that function as and when needed. 

###  What is a “callback”?

A callback is a function passed to a different function as an argument. 

--------------------------------------

## Array Methods 

###  How would you use array.map() to create a new array with transformed values?

Array.map() takes an array and creates a new array with the results. 

const array = [1, 2, 3, 4]
const mapMethod = array.map(num => num + 1)

console.log(mapMethod)
//[2,3,4,5]


 ### How would you use array.filter() to create a new array with certain values removed?

Array.filter() takes an array and creates a 'filtered' copy with values that pass a test. 

The  ‘certain values removed’ would fail the test

const numbers = [1, 2, 3, 4]
const result = numbers.filter(num => num > 2)

console.log(result) // [3, 4]


### How would you use array.find() to get a single value from an array?

Array.find() returns the first element in an array that passes a test. The ‘single value’ would be the value that passes the provided test. 

const numbers = [1, 2, 3, 4]
const result = numbers.find(num => num > 2)

console.log(result) // [3]

--------------------------------------
## Promises & fetch

### What is a promise?

A promise is other pending, fulfilled or rejected. It represents executing/not executing an asynchronous operation

### How do promises help manage asynchronous code?

A promise represents the completion of an asynchronous function. It might return a value. 

### What does a promise’s.then method return?

The then() method always returns a promise 

### How could you chain promises together to avoid “callback hell”?

You can chain promise together using the .then() 

### How would you handle a fetch request that failed to get a response from the server?

I would use the response.ok method to check status codes. If it's not ok, I would throw a new error 

### How would you handle a fetch request that received a 404 response from the server?

I would use the response.ok method to check status codes. If it's not ok, I would throw a new error 

--------------------------------------

## HTTP 

### What is an HTTP request?
Hypertext Transfer Protocol (HTTP)
HTTP makes a request to accsess some bit of information. The request is made to the URL.  

You can make HTTP requests using the fetch function. 

### What kind of request is sent when you click a link in your browser?

GET equest 

###  What kind of request is sent when you submit a form in your browser?

POST request 

### What is an HTTP response?

It's the response you get from your request. 

###  What does the status code of an HTTP response tell us?

The HTTP response tells you if a request has been completed / or not

### What are some common status codes?

404 - not found 
200 - okay

Click [here](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status) for more. 

###  What are HTTP methods for?

The HTTP method indicates which action should be used. GET, POST, PUT etc. 

### What kind of request should have a GET method?

Requesting or getting information from an API. 

### What kind of request should have a POST method?

posting or sending information // Forms 

### What kind of request should have a PUT method?

PUT has similar properties to POST, but PUT ..
The HTTP PUT method is used to update or replace an existing resource on the server

### What kind of request should have a DELETE method?

I am not sure what kind of requested should use the DELETE method.

The HTTP DELETE method is used to delete a resource from the server.

### What is the “body” of an HTTPrequest for?

The body is optional -  It's data requested by the client 

### What is the “body” of an HTTPresponse for?

--------------------------------------
## DOM

### How would you get a reference to a DOM element in your JS?

By their ID or class name 
Document.getelementbyid()
Document.querySelectorAll()
Document.querySelector()

### How would you get references to multiple DOM elements at once in your JS?

I would use: Document.queryselectorAll()

### How would you update properties of a DOM element?

If you have a DOM element you want to update, I would use: 

idname.textConent = 'change to this'
idname.innerHTML = 'change to this'

### What’s the difference between a “property” and an “attribute”?

### What are some different ways to add content inside a DOM element?

You can use: Document.createElement(). Create an element in the DOM and add content to it. 

### When might the template element be useful?

The HTML template element does NOT render when the page is loaded. If you have HTML elements that are awating valuse, you can wrap them in template tags.

Maybe creating the same content multiple times. Rather than creating a new element every time. 

### What are the different ways to add event handlers to elements?

You can use onclick() but I believe this isn’t used anymore. (or good practice)

I may use something like element.addEventListener("click", myFunction)

### Why is addEventListener the safest way to add an event handler?

The eventlsitener attaches the event handler to that element. You can also add multiple eventlisteners to the same element. 

###  How can you access submitted form values in your JS?

using the .value property. 

<input type="text" name="name" id="uniqueID" value="value" />
let nameValue = document.getElementById("uniqueID").value;

--------------------------------------
## Tests

### Why are tests useful?

Tests are useful to make sure the code is operating the way we want it to given the inputs/outputs. 

### What is the difference between unit and integration tests?

Unit testing is when you test individual functions to check whether they are acting as expected. 

Integration testing is testing the whether the code integrates with things outside of our control. 

### What kind of code is easier to test?

Code that returns fixed values?? 

### Why should your tests be isolated from each other?

If you have a large programme with many lines of code, you should not rely on that code to run your test. Each test test should be individually/independent. 

You'll return accurate results 

### What is Test Driven Development (TDD)?

When you write a test before working the function for it. Write the test in it’s most simple form and then make it more complex step by step. 

### When might TDD be a useful process to follow?

When working on larger more complex programmes. 

--------------------------------------
## Debugging

### What process would you take to find out why your code isn’t working?

Lots of console.log(). Using the debugger tool. 

### What tools do JS/dev tools have to help debug your code?

console / breakpoints inside Chrome can be used for debugging 

### At what point should you ask for someone else’s help?

I think an appropriate amount of time would be 40 minutes stuck on a problem without moving forward. 
