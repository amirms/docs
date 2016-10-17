---
title: "XPath true"
category: "refguide5"
space: "Reference Guide 5"
---


The function true() returns the boolean value `true`.

To use the values `true` or `false` in XPath queries, it is necessary to either call true()/false() functions or to enclose the values in quotation marks.

<div class="alert alert-info">{% markdown %}

```
//Sales.Customer[IsGoldCustomer = true()]

```

This query returns all customers who are classified as gold customers.

{% endmarkdown %}</div>