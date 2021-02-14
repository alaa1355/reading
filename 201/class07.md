##
# Introduction

Unless you are developing software which _directly_ manipulates a real-world object, such as process control, robotics, avionics or missile guidance systems, then some of the properties and methods which apply to that real-world object may be completely irrelevant in your software representation. If, for example, you are developing an enterprise application such as Sales Order Processing which deals with entities such as Products, Customers and Orders, you are only manipulating the _information_ about those entities and not the actual entities themselves.

##
# Table Object

The Table object represents an HTML \&lt;table\&gt; element.

### Access a Table Object

You can access a \&lt;table\&gt; element by using getElementById():

### Example

var x = document.getElementById(&quot;myTable&quot;);

### Create a Table Object

You can create a \&lt;table\&gt; element by using the document.createElement() method:

### Example

var x = document.createElement(&quot;TABLE&quot;);

##


##


##
# Table Object Methods

| **Method**                                                                     | **Description**                                                     |
|--------------------------------------------------------------------------------|---------------------------------------------------------------------|
| [createCaption()](https://www.w3schools.com/jsref/met_table_createcaption.asp) | Creates an empty \&lt;caption\&gt; element and adds it to the table |
| [createTFoot()](https://www.w3schools.com/jsref/met_table_createtfoot.asp)     | Creates an empty \&lt;tfoot\&gt; element and adds it to the table   |
| [createTHead()](https://www.w3schools.com/jsref/met_table_createthead.asp)     | Creates an empty \&lt;thead\&gt; element and adds it to the table   |
| [deleteCaption()](https://www.w3schools.com/jsref/met_table_deletecaption.asp) | Removes the first \&lt;caption\&gt; element from the table          |
| [deleteRow()](https://www.w3schools.com/jsref/met_table_deleterow.asp)         | Removes a row (\&lt;tr\&gt;) from the table                         |
| [deleteTFoot()](https://www.w3schools.com/jsref/met_table_deletetfoot.asp)     | Removes the \&lt;tfoot\&gt; element from the table                  |
| [deleteTHead()](https://www.w3schools.com/jsref/met_table_deletethead.asp)     | Removes the \&lt;thead\&gt; element from the table                  |
| [insertRow()](https://www.w3schools.com/jsref/met_table_insertrow.asp)         | Creates an empty \&lt;tr\&gt; element and adds it to the table      |