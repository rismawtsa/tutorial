# Fix NoClassDefFoundError

## Issue

Found the `java.lang.NoClassDefFoundError` error when hit

```
java [filename of class extention]
```

![NoClassDefFoundError](images/java.lang.NoClassDefFoundError.png)

## Fixing

1. Deleted/commented the `package`

   If the file is not depending on other files, I just deleted/commented the `package` at the top of `.java` file

   ![commented the package info](images/comment%20the%20package%20line.png)

   Recompiled the file using command `javac [filename].java`. And boom the issue is solved

2. Compile from the source of directory

   ```
   javac hackerRank/java/outputFormating.java
   ```

   Let's run our application

   ```
   java hackerRank.java.outputFormating
   ```

   <br>

> References:
>
> 1. https://jenkov.com/tutorials/java/packages.html#:~:text=A%20Java%20package%20structure%20is,zip%20file%20(JAR%20files)
> 2. https://www.baeldung.com/java-packages
