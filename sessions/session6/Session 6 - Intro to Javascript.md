# Session 6 - Javascript

**View this in your browser: http://bit.ly/gswd-6**

In this session we're going to look at the basics of Javascript, a programming language used to add complex functionality and interactivity to almost all modern websites.

## 1. What is Javascript?

Javascript is a programming language that runs in every modern web browser, allowing you to write code to add interactivity to your website. On a basic level this might be coding a button to carry out some action. At a more advanced level it will involve updating multiple elements in response to different user interactions, live updating data from a website, adding comments to images, uploading data, instant messaging (e.g Instagram, Facebook).

Javascript is a massive topic in itself so we will only be covering the basics here, but we'll also give you some useful links if you want to learn more.

## 2. Looking at the blog-writer.html file

To start with, open blog-writer.html in a web browser. Try putting in a title and some text, then clicking the "Update preview" button. You'll see that the title is updated in the preview part of the page, but the text isn't yet (that's because you're going to implement this!).

If you have a look at the code for the blog-writer.html file, you'll see the html structure of the page along with bootstrap css. You should also notice that some of the html elements have an id attribute

- The `input` on line 80 has `id="blogTitle"`
- The `button` on line 86 has `id="updatePreview"`
- The `h5` on line 99 has `id="titlePreview"`

These `id` attributes let you identify specific elements so that you can reference them from your Javascript code.

Now that you've looked at the html, if you scroll down towards the bottom of the file you'll see that theres a `<script>` tag. The contents of this tag look a lot different to the rest of the page because this is no longer html/css, it's javascript. Embedding the code in the page like this is useful for small pages and prototyping. For larger, more complex projects it's also possible to include external javascript files (e.g. this is what we've done on lines 113-121 to load the javascript code required for bootstrap).

Some of the lines start with `//`, these are comments and don't do anything, they just serve as a way for the developer to make helpful comments on the code

There are a few key concepts in the code.

A **function** is piece of code that does something and can be "called" as many times as you like. We use the keyword `function` followed by the name we want to give to the function (e.g. `updateTitle`), followed by parentheses `()`. We then use curly braces to define the start and end of the function `{}`. Everything inside the curly braces is the body of the function and defines what it will do. There are a lot of built in functions too, for example on line 147 we're using the `getElementById` function defined on the built in `document` object. You'll notice that that function takes a parameter, in this case it's the `id` of the element that we want to get.

A **variable** is a placeholder for some data you want to store, it might be a piece of text, a number, or a more complex object. In most cases you can declare a variable using the `let` keyword followed by the name you want to give to the variable (e.g. `titleInput`), followed by an `=` sign, then whatever value you want to store. The value is often something that comes from user input.

The other code will usually be statements to do something, or control flow statements to determine whether or not something should be done, or to do something multiple times.

## 3. Making the elements for the text of the blog identifiable
In order to update the preview so that it also shows the text of the blog post, you'll first need to make the relevant html elements identifiable by giving them an `id` attribute. In this case you need to add an id to the `textarea` element on line 84 and another to the `div` on line 100

The value of the `id` attribute has to be unique on the page, so you can't use the same value as one that's already on the page. It should also only container letters and numbers.

## 4. Write a new function to update the blog text
Now that you can identify the html elements you need in code, you can start writing a function to update the blog text.

To start with, see if you can write a new `function` called `updateBlogText` with an empty body `{}`. You can put this between the `updateTitle` function and the `updatePreview` function.

## 5. Write code to get the html elements
Inside of your empty function you can now write some code to get the elements you added `id` attributes to in step 3. To do this you'll need to define a variable for each of them (using `let`) and using the `document.getElementById` function.

If you get stuck, try looking at the updateTitle function (lines 127 and 129). You'll need to do something similar but you'll want to call your variables something different, and use the value of the id attribute from step 3 as the parameter for the function.

## 6. Write code to get the text from the textarea and store it in a variable
Now that you've got variables that represent the html elements, you need to get the value of the textarea and store it in another variable. This is the blog text that you'll need in the next step to set the text of the preview.

Again, if you get stuck, take a look at how it's being done in the `updateTitle` function on line 133. You'll need to do something similar but using a different name for your variable.

## 7. Set the text in the preview
You now have the new blog text in a variable, so it's time to put that text into the preview part of the page. You already have a variable from step 5 with the blog text preview div, so you just need to set the innerText on this.

If you get stuck, take a look at the `updateTitle` function, line 136. You'll need to use the variable names you chose.

## 8. Calling the new function
If you try to update the preview now, it will still only update the title. That's because you've defined a function, but it's not called from anywhere. There's a function already there called `updatePreview` that currently only calls the `updateTitle` function. Add a line underneath it to call your new function. To call a function you type the name of it followed by parentheses and a semi-colon. For example if I had a function called `doSomething`, I could call it in code as `doSomething();`.

## Useful links
As you learn more about development you'll inevitably get stuck or need some outside help, here are a few really useful resources:

- Mozilla Developer Network - One of the best resources for learning about web development
    - [Getting started with the web](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web)
    - [Learn HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML)
    - [Learn CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS)
    - [Learn Javascript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
- [StackOverflow](https://stackoverflow.com/) - A Q&A site where you can ask for help from the community when you get stuck on a problem
- [Code Pen](https://codepen.io) - A site where you can put html, css and javascript in and see the result right away without having to host it somewhere. Great for trying things out and prototyping