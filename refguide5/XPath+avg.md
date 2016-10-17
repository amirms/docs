---
title: "XPath avg"
category: "refguide5"
space: "Reference Guide 5"
---


The avg()-function returns the average of its argument.
This function requires an XPath query as argument. The query must specify an attribute that has a numeric type.

<div class="alert alert-info">{% markdown %}

```
avg(//Sales.Order/TotalPrice)

```

This query returns the average total price of all placed orders.

```
avg(//Sales.Order[Sales.Customer_Order/Sales.Customer = 'Jansen']/TotalPrice)

```

This query returns the average total price of all orders placed by a customer named Jansen.

{% endmarkdown %}</div>