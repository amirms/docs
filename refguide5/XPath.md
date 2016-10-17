---
title: "XPath"
category: "refguide5"
space: "Reference Guide 5"
---


Mendix XPath is one of the Mendix query languages designed to retrieve data. XPath uses path expressions to select data of Mendix objects and their attributes or associations. Examples of XPath queries are:

*   `//Sales.Customer`
    Retrieve all customers.
*   `//Sales.Customer[Name='Jansen']`
    Retrieve all customers with name 'Jansen'.
*   `avg(//Sales.Order[IsPaid = true()]/TotalPrice)`
    Retrieve the average of the total prices of all paid orders.

<div class="alert alert-warning">{% markdown %}

In the Modeler you do not write complete queries but only the constraints. The entity is implicitly determined by the context. So, instead of `//Sales.Customer[Name='Jansen']` you only write `[Name='Jansen']` in the context of a customer. In Java you do write whole queries including the double slashes and the entity name.

{% endmarkdown %}</div>

A common Mendix XPath query consists of a several elements.

<table><thead><tr><th class="confluenceTh">A</th><th class="confluenceTh">B</th><th class="confluenceTh">C</th><th class="confluenceTh">D</th></tr></thead><tbody><tr><th class="confluenceTh">Aggregate function (optional)</th><th class="confluenceTh">Entity to retrieve (required)</th><th class="confluenceTh">Constraint (optional)</th><th class="confluenceTh">Attribute to retrieve (optional)</th></tr><tr><td class="confluenceTd">avg</td><td class="confluenceTd">//Sales.Order</td><td class="confluenceTd">[IsPaid = true()]</td><td class="confluenceTd">/TotalPrice</td></tr></tbody></table>

Element B describes the core of each query and consists of a description of the object being retrieved. This segment always starts with two forward slashes '//' and includes the name of the entity you wish to access preceded by the module containing the entity separated by a period. E.g. //Sales.Customer would return all objects of entity 'Customer' in the module 'Sales'.

Element C of a query is optional and contains one or more constraints to restrict the data being retrieved.

Consider the following query:

`//Sales.Customer[Name='Jansen']`

The constraint is clearly visible between brackets and restricts the objects retrieved to those for which the attribute 'Name' equals 'Jansen'. Objects with any other name than Jansen are excluded from the list.
The number of possible constraints on a single query is unlimited. For more information on how to add and manipulate these constraints see [this page](XPath+Constraints).

Element D of a query is optional and specifies an attribute of the retrieved entity. This option is rarely used in the modeler itself as all data is stored in objects, making it cumbersome and needlessly complicated to deal with a list of single attribute. However, various java actions have use of such lists. Also, this functionality can be used in conjunction with Part A to create aggregates of certain variables easily.

Element A of a query is optional and specifies an aggregation. Element A can be one of the following functions: [avg](XPath+avg), [count](XPath+count), [max](XPath+max), [min](XPath+min) and [sum](XPath+sum). With the exception of 'count', each of these functions require that a particular attribute is specified in element D.

The exception to these basic guidelines is the ID query. See [this page](XPath+id) for more information.

## [Tokens](XPath+Tokens)

## [Operators](XPath+Operators)

## Functions

The following XPath functions are available:

[XPath functions](XPath+Query+Functions):

*   [avg](XPath+avg)
*   [count](XPath+count)
*   [max](XPath+max)
*   [min](XPath+min)
*   [sum](XPath+sum)

[Constraint functions](XPath+Constraint+Functions):

*   [contains](XPath+contains)
*   [start-with](XPath+starts+with)
*   [ends-with](XPath+ends+with)
*   [not](XPath+not)
*   [true](XPath+true)
*   [false](XPath+false)