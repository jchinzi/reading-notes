## Domain Modeling

Domain modeling is the process of creating a conceptual model in code for a specific problem.

 - A **model** describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. 
- An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an **object-oriented model**.

*Object Oriented Programming - Step by Step*
1. The new keyword instantiates (i.e. creates) an object.
1. The constructor function initializes properties inside that object using the this variable.
1. The object is stored in a variable for later use.

*Final Take Aways*
- When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
- Model its attributes with a constructor function that defines and initializes properties.
- Model its behaviors with small methods that focus on doing one job well.
- Create instances using the new keyword followed by a call to a constructor function.
- Store the newly created object in a variable so you can access its properties and methods from outside.
- Use the this variable within methods so you can access the object's properties and methods from inside.

---

## HTML Ch. 6 - Tables

HTML tables are written row by row:
> `<table>` element used to create table

> `<tr>` table row: indicates the start of a row

> `<td>` table data  (or `<td>` for a table heading)

**table cell**: individual block in a grid

*colspan*: attribute that can be used on a `<th>` or `<td>` element to indicate how many columns it should run across

*rowspan*: attribute that can be used on a `<th>` or `<td>` element to indicate how many rows it should span down

`<thead> <tbody> <tfoot>` elements can be used between `<table>` and `<tr>` to differentiate portions of the table to help with CSS styling

---

## JavaScript Ch. 3 - Functions, Methods, and Objects

The **new** keyword and the **Object()** constructor create a blank object that you can then add properties and methods to.

You can update the values of a property using dot notation or square brackets

The **delete** keyword will delete a property

**Object Constructors** use a function as a template for creating objects
  
  - the name of a constructor function *usually* begins with a capital letter to help remind developers to use the **new** keyword when they create an object using that function

*Browser Object Model* contains objects that represent the current browser window or tab

- See pg. 124 for examples

*Document Object Model* uses objects to create a representation of the current page

- See pg. 126 for examples

*Global JavaScript Objects* represent things the JS language needs to create a model of

- See pg. 128 & 129 for examples of String Objects
- See pg. 132 for examples of Number Objects
- See pg. 134 for examples of Math Objects
- See pg. 137 for examples of Date (and Time) Objects




---
[Home](https://jchinzi.github.io/reading-notes/)