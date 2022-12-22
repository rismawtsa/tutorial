# Array vs ArrayList

The differences between Array and ArrayList:

1. Array is a fixed-size data structure while ArrayList is not, even if we specify some initial capacity, we can add more elements.

```
// === Array ===
// Need to specify the size of array
int a[] = new int[3];
a[0] = 1;
a[1] = 2;
a[2] = 3;
// We can not add more elements to a

// === ArrayList ===
// No need to specify the size
ArrayList<Integer> b = new ArrayList<Integer>();
b.add(1);
b.add(2);
b.add(3);

// Specify the initial capacity
ArrayList<Integer> c = new ArrayList<Integer>(2);
c.add(1);
c.add(2);
c.add(3);

// We can add more elements to b and c
```

2. Array elements are accessed using square brackets `[]`, while ArrayList has a set of methods to access its elements and modify them.

```
// === Array ===
int a[] = new int[2];
a[0] = 1;
a[1] = 2;
System.out.println(a[0]);

// === ArrayList ===
ArrayList<Integer> b = new ArrayList<Integer>();
b.add(1);
b.add(2);

System.out.println(b.get(0));
```

3. Array elements could be primitive data types or objects of a class, while ArrayList only support object entries, not the primitive data types.

   > Note: When we do ArraList.add(1), it converts the primitive `int` data types into an Integer Object.

```
// === Array ===
int a[] = new int[10];
Integer b[] = new Integer[3];

// === ArrayList ===
ArrayList<Integer> c = new ArrayList<Integer>();
ArrayList<String> c = new ArrayList<String>();

// not allowed
ArrayList<char> c = new ArrayList<char>(); // causes compiler error
```

4. Array has length property which provides the length or capacity of the array. It is a total space allocated in memory during the initialization of the array, not the actual numbers of its element. Meanwhile, ArrayList doesn't have length property, but has size() method which provides the total number of objects available in the collection.

```
// ===== Array =======
String string[] = new String[10];
string[0] = "hi";
string[1] = "hello";
System.out.println(string.length) // 10;

// ===== ArrayList ======
ArrayList<String> stringList = new ArrayList<String>();
stringList.add("hi");
stringList.add("hello");
System.out.println(stringList.size())// 2
```
