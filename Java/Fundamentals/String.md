# String

Object of String are **immutable**.

There are 2 ways to create a string:

1. String literal
   ```
   String s = "hello";
   ```
2. Using _new_ keyword

   ```
   String s = new String("hello");
   ```

> String using double quote, single quote for char

# Methods

## compareTo()

The method compareTo() is used for comparing two strings lexicographically. Each character of both the strings is converted into a Unicode value for comparison.

```
int compareTo(String string);
```

It returns following values:

- if string1 > string2, it returns a positive value.
- if string1 = string2, it returns 0.
- if string1 < string2, it returns a negative value.

### example:

```
String s1 = "halo";
String s2 = "java";
int res = s1.compareTo(s2); // -2

explanation:
h = 104;
j = 106;
res = -2; (106-104)
```

[ASCII Table](https://www.javatpoint.com/java-ascii-table#:~:text=In%20Java%2C%20an%20ASCII%20table,ASCII%20requires%20only%20one%20byte.)

> **ASCII: American Standard Code for Information Interchange**, is a standard data-transmission code that is used by the computer for representing both the textual data and control characters.

## toCharArray()

Converting string into a character array.

```
String s = "hello";
char result[] = s.toCharArra();
```
