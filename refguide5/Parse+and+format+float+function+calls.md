---
title: "Parse and format float function calls"
category: "refguide5"
space: "Reference Guide 5"
---


See [http://docs.oracle.com/javase/7/docs/api/java/text/DecimalFormat.html](http://docs.oracle.com/javase/7/docs/api/java/text/DecimalFormat.html) for all pattern possibilities.

## parseFloat

Parses a String value to a Float value. Takes optional parameters for format and default value.

### Input parameters

*   value to parse
    Type: String
*   pattern to match on (optional)
    Type: String
*   default value (optional)
    Type: Float

### Output

A Float value that matches the input String value. If the value cannot be parsed (i.e. does not match the format parameter or contains illegal characters) the default value will be returned. If no default value was provided, an error occurs.

<div class="alert alert-info">{% markdown %}

```java
parseFloat('3.45')

```

returns:

```java
3.45

```

with default value:

```java
parseFloat('noFloat',5.05)

```

returns:

```java
5.05

```

with format parameter:

```java
parseFloat('$3.33', '$#.##')

```

returns:

```java
3.33

```

{% endmarkdown %}</div>

## formatFloat

Converts a Float value to a String value, according to a specified format.

### Input parameters

*   value to convert
    Type: Float
*   format that the result should be in
    Type: String

### Output

A String representation of the Float value, in the format specified by the 'format' parameter.
Type: String

<div class="alert alert-info">{% markdown %}

```java
formatFloat(1234.56, '#,###.#')

```

returns:

```java
'1,234.5'

```

{% endmarkdown %}</div>