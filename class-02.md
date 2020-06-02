## HTML Ch. 2 - Text

**Structural Markup:** Elements that you can use to describe both headings and paragraphs

|Tag|Definition|
|:--|--:|
|`<p>`|Paragraph tag|
|`<b>`|Inline tag to **bold** text|
|`<i>`|Inline tag to *italicize* text|
|`<sup>`|Inline tag to <sup>superscript</sup> text|
|`<sub>`|Inline tag to <sub>subscript</sub> text|
|`<br />`|Inline tag that adds a line break within text.  Does not have a closing tag|
|`<hr />`|Inline tag that adds a horizontal rule to separate sections.  Does not have a closing tag|

---

**Semantic Markup:** Provides extra information

|Tag|Definition|
|:--|--:|
|`<strong>`|Indicates content has strong importance.  By default, will render as **bold**|
|`<em>`|Indicates emphasis that subtly changes the meaning of a sentence.  By default, will render in *italics*|
|`<blockquote>`|Used for longer quotes that will take up a full paragraph.  `<p>` tags can still be used within this element|
|`<q>`|Used for shorter quotes that sit within a paragraph|
|`<abbr>`|Used for abbreviations and acronyms to provide the full alternative text|
|`<cite>`|Used for citations, the text will render as *italicized*|
|`<dfn>`|Indicates the defining instance of a new term|
|`<address>`|Used to contain contact details for the author of a page|
|`<ins>`|Used to show content that has been <ins>inserted</ins>|
|`<del>`|Used to show content that has been <del>deleted</del>.|
|`<s>`|Strikethrough - indicates information that is no longer accurate|

---

**Headings** come in 6 levels: 
<h1>H1</h1> 
<h2>H2</h2> 
<h3>H3</h3> 
<h4>H4</h4> 
<h5>H5</h5> 
<h6>H6</h6>

---
---

## HTML Ch. 10 - Introducing CSS

Introducing CSS to your HTML webpage allows for quite a bit more flexibility when it comes to design.

That's because CSS - or *Cascading Style Sheets* - is a style focused rather than content focused language.  Essentially, CSS asks you to place all of your content within boxes (remember all those tags we used while building with html?) and then provides the tools to reference those boxes in such a way that we can control everything from the color and font of the text to where images are shown and how visitors to our page experience interactive elements like buttons.

The layout of CSS is unique from HTML in that it primarily works with selectors and declarations.

* The **Selector** declares what portion of the code we will be affecting
* The **Declaration** effects a change to that selector by declaring a property and a value for that property.

So, for example, a line of css code that is meant to change the font of content marked as a paragraph would look like this:

> p {
    font-family: Arial;}

In this example, *p* is the selector and the declaration that follows includes the property *font-family* which is set to the value *Arial*.

In addition to using existing tags as selectors, you can also use class or id as a selector. 

>Class Selector is indicated with a . before the attribute name

>ID Selector is indicated with a # before the attribute name

---

#### So, where does this new information go???

Here's where you have a couple options.  You can in fact use some minor CSS elements inline within your HTML.  This might look like using the following code to change the color of the text:

>  `<h3 style="color:blue;">This is a blue heading</h3>` 

When rendered, that code would produce the following: 

<h3 style="color: blue;">This is a blue heading</h3>

However, too much of this can make your code look cluttered.

For a single page website, you may opt for something called internal CSS.  This is not inline like the previous example, but is instead code added within the head tags that will instruct the styling of the rest of the page.  This code will be entered within `<style>` tags and should include a type attribute that indicates what you are using css to style.  This would look like:

> `<head>`

>`<style type="text/css"> CSS CODE HERE </style>`

>`</head>`

This allows you to keep all the CSS formatting up in the head of your code - but even that can end up looking rather cluttered.  That's why many prefer to keep a separate style sheet entirely.  Sometimes even more than one!

But if your CSS code is entirely separate - how, you may ask, can the one influence the other?  Well, this is the perfect time to learn how to link files to your code.

Again, like with internal css, you want to work within the head tags of your code.  However, instead of including the nitty gritty of the css code there, you'll instead include a link using the following format:

> `<link href="FILENAME.css" type="text/css" rel="stylesheet" />`

That line allows your project to pull formatting from the linked css file so that you can keep your workplace tidy without sacrificing your ability to format your page.

---
---

## JavaScript Ch. 2 - Basic JavaScript Introductions

|Term|Definition|
|:--|--:|
|script|Series of instructions that a computer can follow|
|statement|Each individual step in a script, ending in a semicolon|
|code block|one or more statements enclosed within curly braces|
|comment|text that is not read by the computer as code but is useful for people who are working on the code to refer to for clarity|
|variable|a tool to store information, declared using the keyword **var**.  Variable names cannot begin with a number, and names that are more than one word should be written in camelCase.  A variable - once declared - remains undefined until it is assigned a value|
|assignment operator|used to assign a value to a variable (=)|
|array|variable that stores a list of values|
|expression|something that evaluates into a single value, either by assigning a value to a variable or by using multiple values to return a single value|

---
> **Operators**: allow programmers to create a single value from one or more values.

* *Assignment Operators* assign a value to a variable
* *Arithmetic Operators* perform basic math using a variety of symbols (details below)
* *String Operators* combine two strings using the + symbol.  This is also known as *concatenation*
* *Comparison Operators* compare two values and return true or false
* *Logical Operators*  combine expressions and return true or false

|Name|Operator|Purpose|
|:--|:-:|--:|
|Addition| + |Adds one value to another|
|Subtraction| - |Subtracts one value from another|
|Division| / |Divides two values|
|Multiplication| * |Multiplies two values using an asterisk (**not** the letter x)|
|Increment| ++ |Adds one to the current number|
|Decrement| -- |Subtracts one from the current number|
|Modulus| % |Divides two values and returns the remainder|

---

#### There are several unique data types in JavaScript

- **Numeric**: numbers
- **String**: letters and other characters
- **Boolean**: true or false

---
---

## JavaScript Ch. 4 - Decisions and Loops

**Evaluations** analyze values in script to determine whether or not they match expected results

**Decisions** use the results of evaluations to decide which path the script should go down

**Loops** allow one to perform the same set of steps repeatedly

**If Statements** can be used to check a condition - if the condition evaluates as true, the subsequent code block is executed.  If it evaluates as false, the code block will **not** be executed

**If Else Statements** work much like If Statements, except that they provide alternate code to run if the condition evaluates as false.


---

<p style="text-align: center;">Comparison Operators evaluate a situation and return a Boolean: true or false.</p>

|Symbol|Name|Description|
|:-:|:--|--:|
|==|Is Equal To|Compares two values to see if they are the same.|
|!=|Is Not Equal To|Compares two values to see if they are *not* the same.|
|===|Strict Equal To|Compares two values to check that both the data type and value are the same.|
|!==|Strict Not Equal To|Compares two values to check that both the data type and value are *not* the same.|
|>|Greater Than|Checks if the number on the left is *greater than* the number on the right.|
|<|Less Than|Checks if the number on the left is *less than* the number on the right.|
|>=|Greater Than or Equal To|Checks if the number on the left is *greater than or equal to* the number on the right.|
|<=|Less Than or Equal To|Checks if the number on the left is *less than or equal to* the number on the right.

---

<p style="text-align: center;">Logical Operators allow you to compare the results of more than one Comparison Operator.</p>

|Symbol|Name|Description|
|:-:|:--|--:|
|&&|Logical And|Tests more than one condition.  If *all* expressions evaluate to true, then the expression returns true.|
|`||`|Logical Or|Tests at least one condition.  If *any* expression evaluates to true, then the expression returns true.|
|!|Logical Not|Takes a single Boolean value and inverts it.|

---

<p style="text-align: center;">Loops check a condition.  If it returns true, a code block will run.  Then the condition will be checked again and if it still returns true, the code block will run again.  This will continue until the condition returns false.</p>

|Loop Type|Description|
|:--|--:|
|For|Runs code **for** a specific number of times, often by using a counter.|
|While|Code will run for as long as the specified condition is true - useful when you don't know how many times the code will need to run.|
|Do While|Similar to *while* loops, **except that** it will always run the statement inside the curly braces at least once, *even if the condition evaluates to false*.

---
---

## Git Commit Messages

- Be Concise and Consistent
- Good commit messages are less about *what* changed and more about *why* the change was made.

When working with a team, it's important to agree on common conventions for:
  - style
  - content (both what should and should *not* be included)
  - metadata


***The Seven Rules of a great Git commit message***
  1. Separate subject from body with a blank line
  1. Limit the subject line to 50 characters
  1. Capitalize the subject line
  1. Do not end the subject line with a period
  1. Use the imperative mood in the subject line
  1. Wrap the body at 72 characters
  1. Use the body to explain *what* and *why* vs. *how*

If you have trouble writing a concise commit message, you may be making too many changes between commits.

---
[Home](https://jchinzi.github.io/reading-notes/)