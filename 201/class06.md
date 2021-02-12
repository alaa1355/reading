#
# **Understanding The Problem Domain Is The Hardest Part Of Programming**

What is the hardest thing about writing code?

There are many common answers to this question:

- Learning a new technology
- Naming things
- Testing your code
- Debugging
- Fixing bugs
- Making software maintainable
- learning the problem domain

**Protein Tracker**

The idea behind the Protein Tracker application is that it allows a user to set a goal for the amount of protein to consume in a day.  The user can add protein amounts which are added to a total protein count that is tracked for that user.

![](201/pic/1a.png)

## Programming is easy if you understand the problem domain

A long time ago, I worked for Hewlett Packard writing software for multi-function printers.

Most of the work at the time was basic waterfall development.  There wasn&#39;t much Agile happening there—at least at the time I was there.

What can you do about it?

If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

1. Make the problem domain easier
2. Get better at understanding the problem domain

**what is an object**

Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.

- If a function is part of an object, it is called a method. Methods represent tasks that are associated with the object.
- If a variable is part of an object, it is called a property. Properties tell us about the object, such as the name of a hotel or the number of rooms it has.
- This object represents a hotel. It has five properties and one method. The object is in curly braces. It is stored in a variable called hotel . 
![](201/pic/2a.png)

![](201/pic/22a.png)

**THE &quot;DOM TREE&quot; IS A MODEL** of a web page As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers&#39; memory. It consists of four main types of nodes.

each node is an object with methods and properties. scripts access and update this dom tree (not the source html file). any changes made to the **dom** tree are reflected in the browser.

**WORKING WITH THE DOM TREE** Accessing and updating the DOM tree involves two steps: 1: Locate the node that represents the element you want to work with. 2: Use its text content, child elements, and attributes.

**ACCESSING ELEMENTS DOM** queries may return one element, or they may return a Nodelist, which is a collection of nodes.

![](201/pic/3a.png)