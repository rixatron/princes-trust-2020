# Getting started with HTML tags

**View this in your browser: http://bit.ly/gswd-2**

## What is an HTML tag?

HTML tags are just a way of telling the computer to start doing something and stop doing something.  An opening tag (i.e. a tag that tells the computer to start doing something) is a word or character between `<` and `>` characters, sometimes called angle brackets like so:

```HTML
<em>
```

"What the hell does 'em' tell a computer to start doing?" is a legitimate question to ask at this point.  Unfortunately the commands used in HTML are often very short which is great if you're typing them over and over but often useless in helping you understand what they do.  In this case 'em' stands for emphasis and will tell the computer to emphasise all the text that comes after it.

"What the hell does emphasizing the text mean?" Is also a legitimate question to ask and the simplest way to answer is a practical demonstration

*This is emphasized text* this is not.

Assuming you don't want your entire document to be emphasized then you need to have a way of telling the computer to stop emphasizing things.  Thankfully this is fairly simple as you just repeat the opening tag but if with a `/` character just before the closing bracket like so:

```HTML
</em>
``` 

###  Try it out!

1. Visit https://jsfiddle.net in your browser.
2. Paste the contents of first-blog-post.html into the HTML pane
3. Press Run

You should see the text 'ENTER THE TEXT AND HTML FOR YOUR BLOG POST HERE' appear in the results pane.  Find this text in the HTML pane and you will see it sits between `<body>` and `</body>`, all the text you enter in this exercise will go in this section.

Try entering the text below into the HTML pane

```HTML
This text will be normal <em>This text will be emphasized.</em> This text also won't be emphasized.
```

Should look like: This text will be normal <em>This text will be emphasized.</em> This text also won't be emphasized.

Let's try another tag, paste the two snippets below into the HTML pane below the previous example and see how it looks.

```HTML
This text is weak <strong>This text is strong</strong>
```
```HTML
This text is normal <strong>This text is strong,<em>This text is strong and emphasized</em></strong>
```

## Why is all my text stuck together?

You may notice that if you've got more than one piece of text, they're all stuck together.  Let's see if we can fix that. Try removing:

```HTML
This is line 1
This is line 2
```

and replacing it with:

```HTML
<p>This is line 1</p>
<p>This is line 2</p>
```

The `p` in this tag stands for paragraph and provides a way to separate text into nice readable blocks but if you notice the gap between the lines is pretty big, like the gap between two paragraphs.  What happens if you actually just want to put a new line in there? Try this instead:

```HTML
This is line 1<br/>
This is line 2
```

You might notice that this tag looks a little unusual since there's no start and finish.  That's because the line break tag 'br' doesn't need to start and finish since it's just telling the computer to put a new line in here.  This is is called a self closing tag, you don't see them that much but it's worth knowing they exist.

## What else can we do?

Believe it or not you've now actually learned most of the techniques you need to write HTML.  Now all you have to do is learn about more tags and remember what they do.  There's over 100 tags that you can learn but in reality you'll probably only use maybe 20 different ones in this course. Let's try some out!

### Headings

Headings are fairly straight forward, try the code below (As an optional extension: Can you combine the heading tags with the 'em' tag we learned earlier?):

```HTML
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
```

### Lists

Lists come in two flavours ordered and unordered.  Try the following out:

```HTML
<ul>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ul>
```
This is an unordered list, try changing 'ul' to 'ol' in the example above and see what happens, remember to change it in both places!

#### Tags within tags

So you may notice that 'ul' and 'ol' are the first tags we've tried that don't wrap text but instead wrap other elements.  The principle is still the same though the starts just tell the computer 'Start a list' and 'Stop a list' it's just that each item also needs to be wrapped in an item. (Optional Extension: Try the following incorrect samples and see what happens): 

Items without a list
```HTML
<li>First item</li>
<li>Second item</li>
<li>Third item</li>
```

List without items
```HTML
<ul>
First item
Second item
Third item
</ul>
```

List with some items
```HTML
<ul>
<li>First item</li>
Second item
Third item
</ul>
```

## Media

Can you guess what this does? Give it a go!

```HTML
<img src="https://mdn.mozillademos.org/files/6457/mdn_logo_only_color.png"/>
```

The 'img' part is short for image but the rest of this is new to us so let's take a second to look at it more closely. 'src' is short for source and it tells the computer where to find the image to display.  See how all the text is inside the tag rather than outside it? That's what we call an attribute and it's used to provide additional details about how we want the computer to display something.  The format is usually like this

```HTML
<tag attributeName="attribute value"></tag>
```

## Basic elements in an HTML document

Ok so a quick aside but there are some tags that you'll notice in every document.  You need them there for anything to work but you rarely write them yourself and all the templates you use in this course already contain them.

```HTML
<html>
    <body>
    </body>
</html>
```

The 'html' tag is the first tag in a document, it's what tells the computer that we're writing HTML and not just a bunch of text. The 'body' tag basically tells the computer that we're starting the part of the document that contains the text we want to show to the user.  If this doesn't make sense then don't worry it will become much clearer when you encounter the 'head' tag in a future session.

## What now?

If you've got this far then you're doing great! Feel free to browse here https://developer.mozilla.org/en-US/docs/Web/HTML/Element each tag you click shows you a short sample of the HTML for a tag and how it looks in your browser which you can play with yourself!