## Strings

### String Declaration

Make sure to `#include <string>`

```c++
string myString = "Hello World!";
```

### Methods

1. Size
    `myString.size()`

    Returns the number of characters in string

2. Insert
    `myString.insert(position, string2)`

    Inserts at `position` (index) in `myString` the string in `string2`

3. Replace
    `myString.replace(position, nbrOfCharacters, string2)`

    Replaces the characters of `position`, `position + 1`, ... , `position + n - 1`.

    Can be used to remove characters from a string: `myString.replace(position, nbrOfCharacters, "")` <-- Empty string

3. Find
    `myString.find(substring)`

    Returns the 1st character index of the 1st occurence (from the left)

    IF the substring doesn't appear in `myString`, it returns a predefined value: `string::npos`

4. rFind
    `myString.find(substring)`

    Same as find but returns the 1st character of the last occurence (it starts from the right)

    IF the substring doesn't appear in `myString`, it returns a predefined value: `string::npos`

5. Substr
    `myString.substr(start, length)`

    Returns the substring of length `length` beginning at the position `start`
