## HTML (HYPERTEXT MARKUP LANGUAGE) -
The HyperText Markup Language, or HTML is the standard markup language for documents designed to be displayed in a web browser.

### Headings

- <h1>First Heading</h1>
- <h2>Second headind</h2>
- <h3>Third headind</h3>
- <h4>Fourth headind</h4>
- <h5>Fifth headind</h5>
- <h6>Sixth headind</h6>

I would keep it up to from heading 1 2 and 3 just so whoever your audience is isn't straining their eyesight


## White Space and Line Breaks

### White Space

Inside HTML, it does not care for white space. Whether you have multiple spaces, or even lines or spaces inbetween two words. HTML only counts it as one. This makes it very useful for readability. We can seperate words, code, etc to make it easier to read for us or other coders that read our code. But what if you want to add some white space? What if you want actual space? Well your going to need to have to force it. When I mean force it, I mean adding `&nbsp;`. Each time we add this, it creates one space. If you wanted to force Tab something, your going need to write that out four &nbsp;&nbsp;&nbsp;&nbsp;times, like so.

## CSS

Css  (cascading style sheet) - Brings the color to your page allowing your page to look more lively but not interactive like JS will. More to follow below

### Block and Inline Elements

In block elements, we are looking at the tags that incase a whole, tags like, `<main></main>`, `<body></body>`, and `<p></p>`.

Inline elements are ones that more inside of block elements, and inside sentenses. We think of tags like `<strong></strong>`, `<a href=""></a>`,  and `<em></em>`.

## Linking CSS File

### Applying CSS

There are 3 ways of adding CSS to your file. You can place your CSS inside your element, on your header, or link an external CSS style sheet. Just note, that you can link multiple CSS files to one HTML. Some developers use differnt CSS pages for the font and colors, while the other page could be design the layout.

While placing your CSS in your element seems fairly simple, you can see what CSS is being done to just that section, the down side, if you want to use the same CSS to multiple pages, you have to then copy it over instead of just having it in your external file.

Adding CSS to your header. This makes it simple, head to the top of the page, and see all the CSS that is on that page. With everything in one place, it makes it simple to see everything at once, but with the problem with adding it to your elements, coping it over to multiple pages can be tedious to constantly do.

### Linking your CSS

Linking your CSS page. Why would you want to create a whole new page and have all your CSS there when you place it in your file? One big reason why is with an external CSS, you can create templates. And have CSS effect the same elements on different pages. You would not have to copy over every single CSS you made for that element on each page, and instead you can write one page, link the file, and the file will show the same CSS throughout all of your pages.

Finally, what happens if I wirte my CSS in my page, and the exrnal page. As the page is being read, we add the link to your CSS at the top, it then reads down from there, Only the bottom most CSS of any taged element will display.

An example of linking CSS would be:  
`<link href="css/styles.css" type="text/css" rel="stylesheet" />`  
Href is the path to the CSS file, type is the type of document, and rel is the relationship.

## Elements

As its own box

There are rules in CSS, they contain two parts, a selector and a declaration. inside the declaration there is Property and a Value.

### Selector

A **selector** would be:  
`p {`
    font-family: Arial;}

### Declaration

A **declaration** would be:  
p {
    `font-family: Arial;}`

### Property

Inside the declaration there is a property and a value:
The **property** is:  
p {
    `font-family:` Arial;}

### Value

The **value** is:  
p {
    font-family: `Arial;}`

## Seclectors

There many differnt types of selectors, from:

* `universal: * {}`
  * This targets all elements on the page
* `Type: h1, h2 {}`
  * Targets all the `<h1>`, and `<h2>` elements
* `Class: .note {}`
  * Target all elements with the class attribute
* `ID: #Introduction {}`
  * Same as the class, but targets all the id attributes
* `Child: li>a {}`
  * This targets the child of `<li>` which would be the `<a>` tag elements, but no other `<a>` tags on the page because it targets just the child of `<li>`.
* `Descendant: p a {}`
  * Targets all the `<a>` tags inside the `<p>` tags, even if there are elements nested inbetween them.
* `Adjacement sibling: h1+p {}`
  * This targets the first `<p>` tag after the `<h1>` tag and no other `<p>` tags after.
* `General sibling: h1~p {}`
  * This targets all the `<p>` that are siblings that are below the `<h1>` tag. This is different then the Descendant because it looks for siblings, not every `<p>` tag under.

## CSS Rules Cascade

When applying CSS, know that it read in a cascading order, from top to bottom. For example, if you have two selectors doing the same thing, but different color, which ever is read after, is the one that will be applied. There are things that can change this rule, for example if you have CSS written in the HTML vs a linked CSS page, since HTML reads from top to bottom as well, it will choose the one that it on the HTML page because it is written after. Another way you can bypass this, is applying the !important after the value to signify its importance over the other same selectors that may be read after. When you also have something that is more specific, like targeting a whole page vs one selector, it will choose the more specific one. 

<hr />

## Below We Will Start on JS or JavaScript

## Variables

When making a variable, they all start with a "`var`", this is a **variable keyword**. Comes after it is your **variable name**. Example would be var `quantity;`.  
When naming a variable, it can be anything you want it to be, lets say the above, if we used it for quanitity, but named the variable `var chocolate`, we would think it has something to deal with chocolate specifically. There are some rules for naming a variable. 

1. It must begin with a letter, dollar sign($), or an underscore(_)
2. It can contain letter, dollar sign($), or an underscore(_) but must not use a dash (-) or a period (.) in the name
3. You can not use reserved keywords, they are special words, if you variable isn't working, it could be that it is a reserved keyword. The reserved keywords are special words that tell the code to do something specific. An example would be `var true;`, we know true is a reserved keyword and we can not use it.
4. All variables are case sensitive, if you name something with a capital letter like `Speaker`, the variable `speaker` will be different
5. Use a variable that represents what you are trying to store, like `deliciousFoods` is going to represent some kind of food.
6. use camel casing when using multiple words. Because we dont want to add dashes or periods, we capitalize every new word after the first. Example would be: `var chocolateSwissMerinueButtercream`. 

## Storing Variables

Assigning a variable uses an **assignment operator** `=`. Example of this would be `quantity = 3;`. The `3` would be **variable value**. 

### Changing Stored Variables

Variables can be overwritten as well, this helps when say you want to use on variable, but turn it **off and on** with **true and false**.

### Storing a string as a Variable

Storing a variable is different between numbers and strings. String being one or more letters or words. Numbers `5` are just by themselves, while strings `'words in my string'` use quotes, either single or double. Just make sure that both quotes are the same, wether single or double. If your using quotes inside a string like `'let's'`, make sure to change your outer quotes to oposite of what your using inside, or it will read the string `'let'` then have a `s'` which it has no idea what to do with and thinks you want to apply something else. When having a **quote** inside a string, you put a `\` in front of the quote you want to have the code not read. It is a **character skip**.

## Linking JS

When adding JavaScript to your program, you want to make sure to be able to link your `.js` file to your HTML page. As HTML reads from top to bottom, you want to place your file right above the bottom `</body>` tag, you want to do this because you want the page to be rendered so the viewer can look at the page first, instead of wait for your `.js` file to load and cause a wonderful white screen with nothing loaded to the screen.

## Comments

Comments are very useful to descibe what is happening in the program. Sometimes it can be difficult to see what it happening at a glace, but making a small comment on what is going on makes understanding your code, and makes other people reading your code very easy as well.

One other thing that commenting is very good for is how when making a function or script. Commenting on what is going on, as in writing everything out on a whtie board before tackling the problem can make things very easy, as everything is on paper for you to outline and follow through with.

Every coding language has their own commenting feature. In JS you comment out one line with `//` and if you want to comment out more then just one line it would be `/*` at the start and `*/` at the end.

## Data Types

### Numeric Date Type

Numberic Data Types are very simple, they are numbers, and they signify their number property. `1`, `0.1` are all numbers. If you declare something and somehow it doesnt come out to be a number, it will return `NaN` or `null` depending on the situation. This signifies that whatever you were trying to accomplish, it was not a number that the code recongized and therefore was not able to turn into a numeric data type.

### String Data Type

A string data type consist of letters and other characters. With a string, it can be anything, it can be numbers, letters, symbols. It is used to represent its face value, what you read is waht you see. Examples of strings would be:

`'Words like this'`, `"Or even numbers like this 10"`  
With these two, notice that there are `''` and `""` around the string, it doesn't matter which you use, but make sure that the first and end are the same type. You can not do something like this: `"This does not work'`

### Boolean

Booleans are very simple. They are either **true or false**, **0 or 1**, or simple as a **yes** or **no**. Boolean's are very nice to use if their is only one outcome.

Using booleans inside of a variable is very powerful and reliable. If you wanted to just have a variable run or not run if something happened, placing in a boolean variable would make that be possible.

Example: `booVariable = true;`

Now whenever you called upon `booVariable`, it would be true where ever you placed it. 

## Arrays

Stores not just one variable, but multiple variables. This can consist of strings, booleans, and numbers in any order.

Use an array when working with a list or a set of values that are related to each other, an example of this would be a shopping cart, it consist of many values that are related to each other. Its nice when you dont need to know how many values you can hold.
