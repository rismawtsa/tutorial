# Data Types

## Primitive

Java has 8 primitive data types: char, boolean, byte, short, int, long, float and double.

Data types used to hold integers:

- byte: 8-bit signed integer, has a minimum value of -128 and a maximum value of 127 (inclusive)
- short: 16-bit signed integer, has a minimum value of -32.768 and a maximum value of 32.767 (inclusive)
- int: 32-bit signed integer, has a minimum value of -2<sup>31</sup> and a maximum value of 2<sup>31</sup>-1. In Java SE 8 and later, we can use `int` data type to represent an **unsigned 32-bit integer**, which has a minimum value of 0 and maximum value of 2<sup>32</sup>-1.
- long: 64-bit signed integer, has a minimum value of -2<sup>63</sup> and a maximum value of 2<sup>63</sup>-1. In Java SE 8 and later, we can use `long` data type to represent an **unsigned 64-bit integer** which has a minimum value of 0 and a maximum value of 2<sup>64<sup>-1.

> **Unsigned integers** (often called `uints`) are just like integers (whole numbers) but have the property that they don't have a `+` or `-` signed associated with them. Those they are always **non-negative** (zero or positive)

<br/>

refs:

- https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html
- https://www.cs.utah.edu/~germain/PPS/Topics/unsigned_integer.html
