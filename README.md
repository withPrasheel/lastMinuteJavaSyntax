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

| No. | Methods                                                  | Description                                                                 |
| --- | -------------------------------------------------------- | --------------------------------------------------------------------------- |
| 1   | `var Math.abs(a)`                                        | return the Absolute value of the given value.                               |
| 2   | `var Math.max(a,b)`                                      | returns the Largest of two values.                                          |
| 3   | `long round(float/double x)`                             | round off the decimal numbers to the nearest value.                         |
| 4   | `double sqrt(double x)`                                  | return the square root of a number.                                         |
| 5   | `double cbrt(double x) `                                 | return the cube root of a number.                                           |
| 6   | `double pow(double a, double b) `                        | returns the value of first argument raised to the power to second argument. |
| 7   | `Math.signum(a) => (a>0): 1.0 / (a<0): -1.0 / (a==0): 0` | ab                                                                          |
