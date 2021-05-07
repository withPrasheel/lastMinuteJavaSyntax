# lastMinuteJavaSyntax

## Important Syntax in java
Most of the sites these days allow 10^8 operations per second

### String Class

Syntax - Taking s1 if one String and (s1,s2) if two strings are required.

| No. | Methods                                                 | Description                                                                  |
| --- | ------------------------------------------------------- | ---------------------------------------------------------------------------- |
| 1   | `char s1.charAt(int index)`                             | returns char value for the particular index                                  |
| 2   | `int s1.length()`                                       | O(1) - returns string length                                                        |
| 3   | `String s1.substring(int beginIndex)`                   | returns substring for given begin index.                                     |
|     | `String s1.substring(int beginIndex, int endIndex)`     | returns substring for given begin index(inclusive) and end index(exclusive). |
| 4   | `boolean s1.contains(CharSequence s)`                   | returns true or false after matching the sequence of char value.             |
| 5   | `boolean s1.equals(Object another)`                     | checks the equality of string with the given object.                         |
| 6   | `boolean s1.isEmpty()`                                  | checks if string is empty.                                                   |
| 7   | `String s1.concat(String str)`                          | concatenates the specified string.                                           |
| 8   | `String s1.replace(char old, char new)`                 | replaces all occurrences of the specified char value.                        |
|     | `String s1.replace(CharSequence old, CharSequence new)` | replaces all occurrences of the specified CharSequence.                      |
| 9   | `String s1.equalsIgnoreCase(String another)`            | compares another string. It doesn't check case.                              |
| 10  | `String[] s1.split(String regex)`                       | returns a split string matching regex.                                       |
|     | `String[] s1.split(String regex, int limit)`            | returns a split string matching regex and limit.                             |
| 11  | `int s1.indexOf(int ch)`                                | returns the specified char value index.                                      |
|     | `int s1.indexOf(int ch, int fromIndex)`                 | returns the specified char value index starting with given index.            |
|     | `int s1.indexOf(String substring)`                      | returns the specified substring index.                                       |
|     | `int s1.indexOf(String substring, int fromIndex)`       | returns the specified substring index starting with given index.             |
| 12  | `String s1.toLowerCase()`                               | returns a string in lowercase.                                               |
| 13  | `String s1.toUpperCase()`                               | returns a string in uppercase.                                               |
| 14  | `String s1.trim()`                                      | removes the beginning and ending spaces of this string.                      |
| 15  | `String String.valueOf(int value)`                      | converts the given type into string. It is an overloaded method.             |

### Math Class

If the return type is of the type same as an argument then we are using _var_

| No. | Methods                                                         | Description                                                                                                    |
| --- | --------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| 1   | `var Math.abs(a)`                                               | return the Absolute value of the given value.                                                                  |
| 2   | `var Math.max(a,b)`                                             | returns the Largest of two values.                                                                             |
| 3   | `long Math.round(float/double x)`                               | round off the decimal numbers to the nearest value.                                                            |
| 4   | `double Math.sqrt(double x)`                                    | return the square root of a number.                                                                            |
| 5   | `double Math.cbrt(double x) `                                   | return the cube root of a number.                                                                              |
| 6   | `double Math.pow(double a, double b) `                          | returns the value of first argument raised to the power to second argument.                                    |
| 7   | `double Math.signum(a) => (a>0): 1.0 / (a<0): -1.0 / (a==0): 0` | used to find the sign of a given value.                                                                        |
| 8   | `double Math.ceil(double x)`                                    | used to find the smallest integer value that is greater than or equal to the argument or mathematical integer. |
| 9   | `double Math.floor(double a)`                                   | used to find the largest integer value which is less than or equal to the argument                             |
| 10  | `double Math.random()`                                          | returns a double value with a positive sign, greater than or equal to 0.0 and less than 1.0.                   |
| 11  | `double Math.log(double x)`                                     | returns the natural logarithm.                                                                                 |
| 12  | `double Math.log10(double x)`                                   | return the base 10 logarithm of a double value.                                                                |
| 13  | `double Math.exp(double x) `                                    | returns E raised to the power of a double value                                                                |
| 14  | `double Math.sin/cos/tan/asin/acos/atan(double a)`              | return the trigonometric value.                                                                                |
| 15  | `double sinh/tanh/cosh(double x) `                              | return the trigonometric Hyperbolic value.                                                                     |

### Integer Class

| No. | Methods                                                                       | Description                                                                                                                                                |
| --- | ----------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | `int Integer.compare(int x,int y)`                                            | compare two int x>y => 1 \ x=y => 0 \ x<y => -1                                                                                                            |
| 2   | `int x.compareTo(int x)`                                                      | compare two int x>y => 1 \ x=y => 0 \ x<y => -1                                                                                                            |
| 3   | `boolean Integer.equals(Object obj) `                                         | compares the value of the parameter to the value of the current Integer object and returns boolean ( True or False ).                                      |
| 4   | `int object.intValue() `                                                      | returns the value of the specified number as an int.                                                                                                       |
| 5   | `long object.longValue()`                                                     | returns the value of the specified number as an long.                                                                                                      |
| 6   | `int Integer.parseInt (String s) `                                            | parses the String argument as a signed decimal integer object                                                                                              |
|     | `int Integer.parseInt (String s, int radix) `                                 | parses the String argument as a signed decimal integer object in the specified radix by the second argument                                                |
|     | `int Integer.parseInt (CharSequence s,int beginIndex,int endIndex,int radix)` | parses the CharSequence argument as a signed integer in the specified radix argument, beginning at the specified beginIndex and extending to endIndex - 1. |
| 7   | `int Integer.reverse(int i) `                                                 | method returns the numeric value obtained by reversing order of the bits in the specified int value.                                                       |
| 8   | `int Integer.rotateLeft(int i, int distance)`                                 | returns the value obtained by rotating the two's complement binary representation of the specified int value left by the specified number of bits.         |
|     | ` int Integer.rotateRight(int i, int distance)`                               | returns the value obtained by rotating the two's complement binary representation of the specified int value right by the specified number of bits.        |
| 9   | `int Integer.signum(int i)`                                                   | (a>0): 1.0 / (a<0): -1.0 / (a==0): 0                                                                                                                       |
| 10  | `String Integer.toBinaryString (int i)`                                       | returns a string representation of the integer argument as an unsigned integer in binary base 2.                                                           |
|     | `String Integer.toHexString (int i) `                                         | returns a string representation of the integer argument as an unsigned integer in binary base 16.                                                          |
|     | `String Integer.toOctalString (int i)`                                        | returns a string representation of the integer argument as an unsigned integer in binary base 8.                                                           |
| 11  | `String a.toString()`                                                         | returns a String object representing the value of the Number Object.(int/float/double/boolean etc)                                                         |
|     | `String Integer.toString(int i) `                                             | returns a string representation of the int type argument in base 10.                                                                                       |
|     | `String Integer.toString(int i, int radix)`                                   | returns a string representation of the int type argument in the specified radix.(First int to radix conversion)                                            |
| 12  | `Integer Integer.valueOf(int i)`                                              | returns the relevant Integer Object holding the value of the argument passed.                                                                              |
|     | `Integer Integer.valueOf(String s)`                                           | returns the relevant Integer Object holding the value of the argument passed.                                                                              |
|     | `Integer Integer.valueOf(String s, int radix)`                                | convert to int and chnages be base from radix to 10.                                                                                                       |

\*valueOf is present in both Integer and String, Integer.valueOf() give Integer and String.valueOf() gives String

### Collections

![Alt text](./Java-Collections-Hierarchy.png "Title")

```java
Collection<E> P = new "some type"<E>();
Collection<E> Q = new "some type"<E>();
```

| No. | Methods                              | Description                                                                                                                                                                                                              |
| --- | ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1   | `boolean P.add(E element)`           | This method is used to add an object to the collection.                                                                                                                                                                  |
| 2   | `boolean P.addAll(Q);`               | This method adds all the elements in the given collection to this collection.                                                                                                                                            |
| 3   | `P.clear()`                          | used to clear the Collection upon                                                                                                                                                                                        |
| 4   | `boolean P.contains(Object element)` | returns true if the collection contains the specified element.                                                                                                                                                           |
| 5   | `boolean P.containsAll(Q)`           | returns true if the collection contains all of the elements in the given collection.                                                                                                                                     |
| 6   | `boolean P.equals(Q)`                | This method compares the specified object with this collection for equality.                                                                                                                                             |
| 7   | `int P.hashCode()`                   | return the hash code value for this collection.                                                                                                                                                                          |
| 8   | `boolean P.isEmpty()`                | This method returns true if this collection contains no elements.                                                                                                                                                        |
| 9   | `Collections.max(P)`                 | used to return the maximum element of the given collection, according to the natural ordering of its elements. All elements in the collection must implement the Comparable interface.                                   |
| 10  | `E P.remove(Object o)`               | This method is used to remove the given object from the collection. If there are duplicate values, then this method removes the first occurrence of the object.                                                          |
| 11  | `E P.removeAll(Q)`                   | This method is used to remove all the objects mentioned in the given collection from the collection.                                                                                                                     |
| 12  | `int P.size()`                       | This method is used to return the number of elements in the collection.                                                                                                                                                  |
| 13  | `Object[] objects = P.toArray();`    | This method is used to return an array containing all of the elements in this collection. toArray() method returns an array of type Object(Object[]). We need to typecast it to Integer before using as Integer objects. |

### Iterator

Syntax :

```java
Iterator i = Collection.iterator();
```

| No. | Methods               | Description                                                                       |
| --- | --------------------- | --------------------------------------------------------------------------------- |
| 1   | `boolean i.hasNext()` | returns true if Iterator has more element to iterate.                             |
| 2   | `Object i.next()`     | returns the next element in the collection until the hasNext()method return true. |
| 3   | `void i.remove()`     | removes the current element in the collection.                                    |

### ListItrator

‘ListIterator’ in Java is an Iterator which allows users to traverse Collection in both direction.

Syntax:

```java
ListIterator li = list.listIterator();
```

| No. | Methods                      | Description                                                                                |
| --- | ---------------------------- | ------------------------------------------------------------------------------------------ |
| 1   | `void li.add(Object object)` | It inserts object immediately before the element that is returned by the next( ) function. |
| 2   | `boolean li.hasNext( )`      | returns true if the list has a next element.                                               |
| 3   | `boolean li.hasPrevious( ):` | returns true if the list has a previous element.                                           |
| 4   | `Object li.next( )`          | returns the next element of the list.                                                      |
| 5   | `Object li.previous( )`      | returns the previous element of the list.                                                  |
| 6   | `void li.remove( )`          | removes the current element from the list.                                                 |

### ArrayList

Syntax:

```java
ArrayList <E> x = new ArrayList<E>();
```

| No. | Methods                                          | Description                                                                                                                                                         |
| --- | ------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | `int x.size()`                                   | returns length of an ArrayList                                                                                                                                      |
| 2   | `void x.add(int index, E element)`               | used to insert the specified element at the specified position in a list.                                                                                           |
| 3   | `boolean x.add(E e)`                             | used to append the specified element at the end of a list.                                                                                                          |
| 4   | `boolean x.addAll(Collection c) `                | used to append all of the elements in the specified collection to the end of this list, in the order that they are returned by the specified collection's iterator. |
| 5   | `boolean x.addAll(int index, Collection c)`      | used to append all the elements in the specified collection, starting at the specified position of the list.                                                        |
| 6   | `void x.clear()`                                 | used to remove all of the elements from this list.                                                                                                                  |
| 7   | `E x.get(int index)`                             | used to fetch the element from the particular position of the list.                                                                                                 |
| 8   | `boolean x.isEmpty()`                            | returns true if the list is empty, otherwise false.                                                                                                                 |
| 9   | `Object[] x.toArray()`                           | used to return an array containing all of the elements in this list in the correct order.                                                                           |
| 10  | `Object x.clone()`                               | used to return a shallow copy of an ArrayList.                                                                                                                      |
| 11  | `boolean x.contains(Object o)`                   | returns true if the list contains the specified element                                                                                                             |
| 12  | `int x.indexOf(Object o)`                        | used to return the index in this list of the first occurrence of the specified element, or -1 if the List does not contain this element.                            |
| 13  | `E x.remove(int index)`                          | to remove the element present at the specified position in the list.                                                                                                |
| 14  | `boolean x.remove(Object o)`                     | used to remove the first occurrence of the specified element.                                                                                                       |
|     | `boolean x.removeAll(Collection c)`              | used to remove all the elements from the list.                                                                                                                      |
| 15  | `void x.removeRange(int fromIndex, int toIndex)` | to remove all the elements lies within the given range.                                                                                                             |
| 16  | `E x.set(int index, E element)`                  | used to replace the specified element in the list, present at the specified position.                                                                               |
| 17  | `void x.sort(Comparator<? super E> c)`           | used to sort the elements of the list on the basis of specified comparator.                                                                                         |
| 18  | `List<E> subList(int fromIndex, int toIndex)`    | used to fetch all the elements lies within the given range.                                                                                                         |

### LinkedList

Syntax:

```java
LinkedList<E> x =new LinkedList<E>();
```

E: data type

| No. | Methods                                        | Description                                                                                                                                                         |
| --- | ---------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | `boolean x.add(E e)`                           | to append the specified element to the end of a list.                                                                                                               |
| 2   | `void x.add(int index, E element)`             | to insert the specified element at the specified position index in a list.                                                                                          |
| 3   | `boolean x.addAll(Collection <E> c)`           | used to append all of the elements in the specified collection to the end of this list, in the order that they are returned by the specified collection's iterator. |
|     | `boolean x.addAll(int index, Collection<E> c)` | used to append all the elements in the specified collection, starting at the specified position of the list.                                                        |
| 4   | `void x.addFirst(E e)`                         | used to insert the given element at the beginning of a list.                                                                                                        |
|     | `void x.addLast(E e)`                          | used to append the given element to the end of a list.                                                                                                              |
| 5   | `void x.clear()`                               | used to remove all the elements from a list.                                                                                                                        |
| 6   | `Object x.clone()`                             | used to return a shallow copy of an ArrayList.                                                                                                                      |
| 7   | `boolean x.contains(Object o)`                 | used to return true if a list contains a specified element.                                                                                                         |
| 8   | `E x.element()`                                | used to retrieve the first element of a list.                                                                                                                       |
| 9   | `E x.get(int index)`                           | used to return the element at the specified position in a list.                                                                                                     |
| 10  | `int x.indexOf(Object o)`                      | used to return the index in a list of the first occurrence of the specified element, or -1 if the list does not contain any element.                                |
| 11  | `boolean x.offer(E e)`                         | adds the specified element as the last element of a list.                                                                                                           |
| 12  | `E x.peek()`                                   | retrieves the first element of a list                                                                                                                               |
|     | `E x.poll()`                                   | It retrieves and removes the first element of a list.                                                                                                               |
| 13  | `int x.size()`                                 | used to return the number of elements in a list.                                                                                                                    |
| 14  | `E x.set(int index, E element)`                | It replaces the element at the specified position in a list with the specified element.                                                                             |
| 15  | `E x.remove(int index)`                        | used to remove the element at the specified position in a list.                                                                                                     |

### Map

![Alt text](./java-map-hierarchy.png "Title")

```java
Map<K,V> m=new HashMap<K,V>();
```


| No. | Methods                                      | Description                                                                                           |
| --- | -------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| 1   | `void m.put(Object key, Object value)`       | used to insert an entry in the map.                                                                   |
| 2   | `void m.putAll(Map map)`                     | used to insert the specified map in the map.                                                          |
| 3   | `void m.putIfAbsent(K key, V value)`         | It inserts the specified value with the specified key in the map only if it is not already specified. |
| 4   | `void m.remove(Object key)`                  | used to delete an entry for the specified key.                                                        |
| 5   | `boolean m.remove(Object key, Object value)` | It removes the specified values with the associated specified keys from the map.                      |
| 6   | `void m.clear()`                             | used to reset the map.                                                                                |
| 7   | `boolean m.containsValue(Object value)`      | This method returns true if some value equal to the value exists within the map, else return false.   |
|     | `boolean containsKey(Object key)`            | This method returns true if some key equal to the key exists within the map, else return false.       |
| 8   | `boolean equals(Object o)`                   | used to compare the specified Object with the Map.                                                    |
| 9   | `V m.get(Object key)`                        | This method returns the object that contains the value associated with the key else returns null      |
| 10  | `boolean m.isEmpty()`                        | This method returns true if the map is empty; returns false if it contains at least one key.          |
| 11  | `int m.size()`                               | This method returns the number of entries in the map.                                                 |

Map.Entry
```java
for(Map.Entry<Integer, Integer> map : counts.entrySet()) { 
    entry.getValue(); 
    entry.getKey();
}
```
<keyset missing>

  

### [Queue](https://www.geeksforgeeks.org/queue-interface-java/)

Since Queue is an interface, objects cannot be created of the type queue. We always need a class which extends this list in order to create an object.

Syntax:

```java
Normal queue:    Queue<E> lQueue = new LinkedList<E>();

Priority Queue:  Queue<E> pQueue = new PriorityQueue<E>();
                 Queue<E> pbq = new PriorityBlockingQueue<E>();
```
To declare a [Priority queue](http://www.learn4master.com/algorithms/java-priorityqueue-example) which returns maximum value using MaxHeap
```java
Queue<E> queue = new PriorityQueue(int initialCapacity, Comparator<? super E> comparator);
PriorityQueue<Integer> queue = new PriorityQueue<>(size, Collections.reverseOrder());
```

| No. | Methods                   | TC(Q) | TC(PQ) | Description                                                                                                                                                                                                        |
| --- | ------------------------- | --- | --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1   | `boolean q.add(object) ` | O(n) | O(log n) | This method is used to add elements at the tail of queue. More specifically, at the last of linked-list if it is used, or according to the priority in case of priority queue implementation.                      |
|     | `boolean q.offer(object)` | O(n) | O(log n) | This method is used to insert an element in the queue. This method is preferable to add() method since this method does not throws an exception when the capacity of the container is full since it returns false. |
| 2   | `Object q.peek()`         | O(n) | This method is used to view the head(first in) of queue without removing it. It returns Null if the queue is empty.                                                                                                |
|     | `Object q.element()`      | O(n) | This method is similar to peek(). It throws NoSuchElementException when the queue is empty.                                                                                                                        |
| 3   | `Object q.remove()`        | O(n) | This method removes and returns the head of the queue. It throws NoSuchElementException when the queue is empty.                                                                                                   |
|     | `Object q.poll()`          | O(n) | This method removes and returns the head of the queue. It returns null if the queue is empty.                                                                                                                      |
