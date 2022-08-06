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

The form element (or tag) is used to create a form for the user. You can have different inputs within a form. 

--------------------------------------

###  How would you use CSS variables to make a reusable colour palette?

You can use ‘root’ pseudo-class in your CSS to declare colour variables 

###  How would you use flexbox to make elements sit on a single line?

I would apply these two lines of code to the parent element. 

Display: flex; 
Flxs-direction: row;

### How would you use grid to make a layout that automatically adds columns as the screen gets wider?

Not sure 

###  Why is it important to create a responsive design?

Because as developers we do not know what device the user will open the application/website on. We need the application to be accessible for small mobiles to 4k monitors. 

How would you structure your CSS to make it “mobile-first”?

I would write the CSS for the smallest mobile screen. I would then use media queries and different break points for different devices sizes. 


Why should we avoid using var to define variables?

From ES6 onwards (2015 I think…?) a new way to declare variables was introduced. Why…? I think it’s related to the scope and accessing the variable 


How might you make a long, complex chunk of code easier to read?

I would divide the code up into smaller functions and then call that function as and when needed. 

What is a “callback”?

A callback is a function passed to a different function as an argument. 

How would you use array.map() to create a new array with transformed values?

Array.map() takes a function and creates a new array. I would write the function to transform the values 


How would you use array.filter() to create a new array with certain values removed?

Array.filter() takes a function, and elements in an array passed to that function are returned if the pass a ‘test’ 

The  ‘certain values removed’ would be the test 


How would you use array.find() to get a single value from an array?

Array.find() returns the first element in an array that passes a test. The ‘single value’ would be the value that passes the provided test. 




What is a promise?

A promise is other pending, fulfilled or rejected 	How do promises help manage asynchronous code?

What does a promise’s.then method return?

The then method returns another promise 

How could you chain promises together to avoid “callback hell”?

Keep using the .then 

How would you handle a fetch request that failed to get a response from the server?

I would throw a new error 

How would you handle a fetch request that received a 404r esponse from the server?

404 means the pages does not exist. Throw an error. 

What is an HTTP request?

It’s a method of exchanging data 

What kind of request is sent when you click a link in your browser?

HTTP request 

What kind of request is sent when you submit a form in your browser?

HTTP request 

What is an HTTP response?

What does the status code of an HTTP response tell us?

What are some common status codes?

What are HTTP methods for?

What kind of request should have aGET method?

What kind of request should have a POST method?

What kind of request should have a PUT method?

What kind of request should have a DELETE method?

What is the “body” of an HTTPrequest for?

What is the “body” of an HTTPresponse for?



How would you get a reference to a DOM element in your JS?

By their ID or class name 

Document.getelementbyid()

How would you get references to multiple DOM elements at once in your JS?

I would use: Document .queryselectorAll()

How would you update properties of a DOM element?

What’s the difference between a “property” and an “attribute”?

What are some different ways to add content inside a DOM element?

You can use: Document.createElement()

When might the<template> element be useful?

What are the different ways to add event handlers to elements?

You can use onclick() but I believe this isn’t used anymore. 

Why is addEventListener the safest way to add an event handler?

How can you access submitted form values in your JS?



Why are tests useful?

Tests are useful to make sure the code is operating the way we want it to give the inputs/outputs. 

What is the difference between unit and integration tests?

Unit testing is when you test individual functions. 
Integration testing is testing the entire function 

What kind of code is easier to test?

Why should your tests be isolated from each other?

Because you should not rely on a previous test. Each test should test a section individually. 

What is Test Driven Development (TDD)?

When you write a test before working the function for it. Write the test in it’s most simple form and then make it more complex step by step. 

When might TDD be a useful process to follow?

When working on larger more complex programmes. 


What process would you take to find out why your code isn’t working?

Lots of console.log(). Using the debugger tool. 

What tools do JS/dev tools have to help debug your code?



At what point should you ask for someone else’s help?

I think an appropriate amount of time would be 40 minutes stuck on a problem without moving forward. 
