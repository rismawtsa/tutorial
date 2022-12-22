# Convert String to Integer

To convert String to integer, we can use methods of the Integer class. They are parseInt() and valueOf().

## parseInt(String s)

This method returns an `int`, a primitive data type. The characters in the String should be decimal digits, except the first character may be a minus sign `-` to indicate a negative value or a plus sign `+` to indicate a positive value. If the String does not contain a valid integer then it will throw a `NumberFormatException`.

```
int a = Integer.parseInt("1"); // 1
int b = Integer.parseInt("-1"); // -1
int c = Integer.parseInt("+1"); // 1

int d = Integer.parseInt("1+"); // Exception java.lang.NumberFormatException
```

## valueOf(String s)

This method returns an `Integer` object that represents the value specified by the String. In the [java documentation](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html#valueOf-java.lang.String) state that it is equal to the value of `new Integer(Integer.parseInt(s))`. This method will return a `NumberFormatException` if the String cannot be parsed as an integer.

```
Integer a = Integer.valueOf("1"); // 1
Integer b = Integer.valueOf("-1"); // -1
Integer c = Integer.valueOf("+1"); // 1

Integer d = Integer.valueOf("1+"); // Exception java.lang.NumberFormatException
```
