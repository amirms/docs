---
title: "XPath ends-with"
category: "refguide5"
space: "Reference Guide 5"
---


The ends-with() function checks whether a String attribute ends with a specific substring.

<div class="alert alert-info">{% markdown %}

```
//Sales.Customer[ends-with(Name, 'sen')]

```

This query returns all customers whose name ends with the substring 'sen'. Customers with the name 'Jansen' or 'Janssen' will be returned, because both names end with 'sen'.

{% endmarkdown %}</div>