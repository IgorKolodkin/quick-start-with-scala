# Working with atring in acala #

These are the most important `String` methods:

```scala
val a: String = "Quick start with scala"
val b: String = "scala"
```

Method | Description | Result of example
:------: | ----------- | --------
`a.length` | is the length of the string in characters | 22
`a.substring(i)` | returns the part of the string starting at index `i` | `a.substring(6) - "start with scala"`
`a.substring(i,j)` or `a.slice(i,j)` | returns the part of the string starting at index `i` and going up to index `j-1`. | `a.substring(6, 11) - "start"`
`a.contains(b)` | returns true if `b` is a substring of `a` | `true`
`a.indexOf(b)` | returns the index of the first occurrence of the substring `b` in `a` (or -1) | 17
`a.indexOf(b, i)` | returns the index of the first occurrence after index `i` of the substring `b` in `a` (or -1) | `a.indexOf(b, 1) - 17`
`a.toLowerCase` and `a.toUpperCase` | return a copy of the string with all characters converted to lower or upper case | `a.toUpperCase QUICK START WITH SCALA` 
`a.capitalize` | returns a new string with the first letter only converted to upper case | 
`a.reverse` | returns the string backwards |
`a.isEmpty` | is the same as `a.length == 0` | 
`a.nonEmpty`| is the same as `a.length != 50` | 
`a.startsWith(b)` | returns true if `a` starts with `b` | 
`a.endsWith(b)` | returns true if `a` ends with `b` | 
`a.replace(c1, c2)` | returns a new string with all characters `c1` replaced by `c2` |
`a.replace(b1, b2)` | returns a new string with all occurrences of the substring `b1` replaced by `b2` |
`a.trim` | returns a copy of the string with white space at both ends removed | 
`a.format(arguments)` | returns a string where the percent-placeholders in `a` have been replaced by the arguments |
`a.split(b)`| splits the string into pieces and returns an array with the pieces. `b` is a regular expression | 

bo split around white space, use `a.split("s+")`
