# CSS Stylings

## 0. Before you start

To get started:
1. Open up https://jsfiddle.net 
2. Paste the contents of blog_example_with_themes.html into the HTML pane and press run
3. Paste the contents of style.css into the CSS pane and press run again

Hopefully you noticed what a big difference adding the styles made to how the page looked!  Have a look and see if you can spot the various places the colours in the CSS file show up.

Now it's time to modify the contents of the CSS pane yourself to change how the HTML looks.

The format of the CSS file is as following

`thingYouWantToStyle { attribute-name: value; }`

let's take a look at an example in the CSS file

```CSS
h1 { 
   color: blue; 
   background-color: yellow; 
   border: 1px solid black; 
} 
```
`h1` is the tag that the style will be applied to, see if you can find the h1 tag in the HTML pane. `background-color` is the name of the property (or attribute) we want to change and `yellow` is the value we want to set.

Note: Don't forget the `;` it's really important!

Note: Notice that all the attributes we're setting are surrounded by `{` `}`


## 1. Text styles

**color**

keywords (https://developer.mozilla.org/en-US/docs/Web/CSS/color_value#Color_keywords)

`p { color: red }`

hexadecimal values

`p { color: #ff0000 }`

rgb

`p { color: rgb(255,0,0) }`

**font-family**

`p { font-family: arial; }`

The browser will only apply a font if it is available on the computer/phone/tablet the website is being accessed on. 
There are only a certain number of fonts that are generally available across all devices and can therefore be used without much worry. 
These are the so-called web safe fonts. Check here for a list: https://www.cssfontstack.com/

You can use font stacks to specify fallbacks if your font is not available:

`p { font-family: "Trebuchet MS", Verdana, sans-serif; }`

**font-size**

There are a couple of different ways to set the font size but for the moment we're going to just be looking at the simplest one which is pixels.  Since there are multiple ways of setting the font size you have to put `px` after the number e.g. `20px;`

Have a go at setting the font size yourself, if you get stuck then look at hints below.

Hint:

Look at the definition of CSS at the top of the page:
 - The thing you want to style is `p` tags
 - The attribute you want to set is `font-size`
 - The value we're setting is `20px`

If you get stuck then just ask for help! : )

Note: You don't have to include the p { } but every time you can just put the font-size line below something else is another p { } block.

Now try setting the following attributes against the `p` tags and see what they do.  The attribute name is in bold and the possible values are in brackets.  If you get stuck then ask one of the instructors for help!

**font-style** (normal, italic)

**font-weight** (normal, bold)

**text-transform** (none, uppercase, lowercase, capitalize)

**text-decoration** (none, underline, overline, line-through)

**text-shadow** (horizontal offset in size, vertical offset size, blur radius size, base colour)

`h1 { text-shadow: 4px 4px 5px red; }`

**text-align** (left, right, center, justify)

**line-height**

## 2. List styles

These styles apply to the `ul` and `ol` tags, so don't put them in the `p` blocks, ask one of the instructors if you have any problems with this.

**list-style-type**: Sets the type of bullets to use for the list, for example, square or circle bullets for an unordered list, or numbers, letters or roman numerals for an ordered list.

**list-style-position**: Sets whether the bullets appear inside the list items, or outside them before the start of each item.

**list-style-image**: Allows you to use a custom image for the bullet, rather than a simple square or circle.

See here for a list of different list styles to try: https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-type


## 3. Link styles

`<p><a href="#">A simple link</a></p>`

You'll notice a few things as you explore the default styles.

* Links are underlined.
* Unvisited links are blue.
* Visited links are purple.
* Hovering a link makes the mouse pointer change to a little hand icon.
* Focused links have an outline around them — you should be able to focus on the links on this page with the keyboard by pressing the tab key
* Active links are red (Try holding down the mouse button on the link as you click it.)

Try setting the following selectors to change the default styles

``` 
a {

}


a:link {

}

a:visited {

}

a:focus {

}

a:hover {

}

a:active {

}
```

## 4. Selectors

In the these examples you will notice that we used some different selectors. Here are the main types of selector you will use. Try them out in your project:

**Type selectors** 

We have already used these quite a lot e.g.

`p { color: red }`

This selects all p tags.

**Class selectors** 

Uses the class attribute. You can also use multiple classes to combine styles.

```
<ul>
  <li class="first done">Create an HTML document</li>
  <li class="second done">Create a CSS style sheet</li>
  <li class="third">Link them all together</li>
</ul>
```

```
/* The element with the class "first" is bolded */
.first {
  font-weight: bold;
}

/* All the elements with the class "done" are strikethrough */
.done {
  text-decoration: line-through;
}
```
**Attribute selectors** 

Matches elements using their attributes. For example a list like this:

```
Ingredients for my recipe: <i lang="fr-FR">Poulet basquaise</i>
<ul>
  <li data-quantity="1kg" data-vegetable>Tomatoes</li>
  <li data-quantity="3" data-vegetable>Onions</li>
  <li data-quantity="3" data-vegetable>Garlic</li>
  <li data-quantity="700g" data-vegetable="not spicy like chili">Red pepper</li>
  <li data-quantity="2kg" data-meat>Chicken</li>
  <li data-quantity="optional 150g" data-meat>Bacon bits</li>
  <li data-quantity="optional 10ml" data-vegetable="liquid">Olive oil</li>
  <li data-quantity="25cl" data-vegetable="liquid">White wine</li>
</ul>
```

Can be styled with CSS:
```
/* All elements with the attribute "data-vegetable"
   are given green text */
[data-vegetable] {
  color: green;
}

/* All elements with the attribute "data-vegetable"
   with the exact value "liquid" are given a golden
   background color */
[data-vegetable="liquid"] {
  background-color: goldenrod;
}
```

**Pseduo-classes**

A CSS pseudo-class is a keyword added to the end of a selector, preceded by a colon (:). We used these when styling the links above.

**Combinators and multiple selectors**

You can combine selectors to make your style target a very specific element. It can also be useful to apply styles accross lots of different elements in one place to save repeating yourself.

So all headers could have the same font for example:

```
h1, h2, h3 {
  font-family: "Trebuchet MS", Verdana, sans-serif;
}
```

There are also different ways of specifying combinations such as matching elements that are descendants of specific elements. For more examples see here:
https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Combinators_and_multiple_selectors
