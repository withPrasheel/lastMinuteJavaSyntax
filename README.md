# lastMinuteJavaSyntax

## Important Syntax in java

### String Class

Syntax - Taking s1 if one String and (s1,s2) if two strings are required.

| No. | Methods                                                 | Description                                                       |
| --- | ------------------------------------------------------- | ----------------------------------------------------------------- |
| 1   | `char s1.charAt(int index)`                             | returns char value for the particular index                       |
| 2   | `int s1.length()`                                       | returns string length                                             |
| 3   | `String s1.substring(int beginIndex)`                   | returns substring for given begin index.                          |
|     | `String s1.substring(int beginIndex, int endIndex)`     | returns substring for given begin index and end index.            |
| 4   | `boolean s1.contains(CharSequence s)`                   | returns true or false after matching the sequence of char value.  |
| 5   | `boolean s1.equals(Object another)`                     | checks the equality of string with the given object.              |
| 6   | `boolean s1.isEmpty()`                                  | checks if string is empty.                                        |
| 7   | `String s1.concat(String str)`                          | concatenates the specified string.                                |
| 8   | `String s1.replace(char old, char new)`                 | replaces all occurrences of the specified char value.             |
|     | `String s1.replace(CharSequence old, CharSequence new)` | replaces all occurrences of the specified CharSequence.           |
| 9   | `String s1.equalsIgnoreCase(String another)`            | compares another string. It doesn't check case.                   |
| 10  | `String[] s1.split(String regex)`                       | returns a split string matching regex.                            |
|     | `String[] s1.split(String regex, int limit)`            | returns a split string matching regex and limit.                  |
| 11  | `int s1.indexOf(int ch)`                                | returns the specified char value index.                           |
|     | `int s1.indexOf(int ch, int fromIndex)`                 | returns the specified char value index starting with given index. |
|     | `int s1.indexOf(String substring)`                      | returns the specified substring index.                            |
|     | `int s1.indexOf(String substring, int fromIndex)`       | returns the specified substring index starting with given index.  |
| 12  | `String s1.toLowerCase()`                               | returns a string in lowercase.                                    |
| 13  | `String s1.toUpperCase()`                               | returns a string in uppercase.                                    |
| 14  | `String s1.trim()`                                      | removes the beginning and ending spaces of this string.           |
| 15  | `String String.valueOf(int value)`                      | converts the given type into string. It is an overloaded method.  |

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
| 16  | ``                                                              |

### Integer Class

| No. | Methods                                                                       | Description                                                                                                                                                |
| --- | ----------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | `int Integer.compare(int x,int y)`                                            | ?                                                                                                                                                          |
| 2   | `int x.compareTo(int x)`                                                      | ?                                                                                                                                                          |
| 3   | `boolean Integer.equals(Object obj) `                                         | compares the value of the parameter to the value of the current Integer object and returns boolean ( True or False ).                                      |
| 4   | `int object.intValue() `                                                      | returns the value of the specified number as an int.                                                                                                       |
| 5   | `long object.longValue()`                                                     | returns the value of the specified number as an long.                                                                                                      |
| 6   | `int Integer.parseInt (String s) `                                            | parses the String argument as a signed decimal integer object                                                                                              |
|     | `int Integer.parseInt (String s, int radix) `                                 | parses the String argument as a signed decimal integer object in the specified radix by the second argument                                                |
|     | `int Integer.parseInt (CharSequence s,int beginIndex,int endIndex,int radix)` | parses the CharSequence argument as a signed integer in the specified radix argument, beginning at the specified beginIndex and extending to endIndex - 1. |
| 7   | `int Integer.reverse(int i) `                                                 | method returns the numeric value obtained by reversing order of the bits in the specified int value.                                                       |
