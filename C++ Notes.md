## Strings

### String Declaration

Make sure to `#include <string>`

```c++
string myString = "Hello World!";
```

### Methods

1. <b>Size</b>

    `myString.size()`

    Returns the number of characters in string

2. <b>Insert</b>

    `myString.insert(position, string2)`

    Inserts at `position` (index) in `myString` the string in `string2`

3. <b>Replace</b>
    `myString.replace(position, nbrOfCharacters, string2)`

    Replaces the characters of `position`, `position + 1`, ... , `position + n - 1`.

    Can be used to remove characters from a string: `myString.replace(position, nbrOfCharacters, "")` <-- Empty string

4. <b>Find</b>

    `myString.find(substring)`

    Returns the 1st character index of the 1st occurence (from the left)

    IF the substring doesn't appear in `myString`, it returns a predefined value: `string::npos`

5. <b>rFind</b>

    `myString.find(substring)`

    Same as find but returns the 1st character of the last occurence (it starts from the right)

    IF the substring doesn't appear in `myString`, it returns a predefined value: `string::npos`

6. <b>Substr</b>

    `myString.substr(start, length)`

    Returns the substring of length `length` beginning at the position `start`


## Vectors

### Declaration

Make sure to `#include <vector>`

```c++
vector<elementTypes> myVect(nbrOfElements, filledValue);

// Example
vector<int> myVect(4, 100);
// myVect: {100,100,100,100}  
```

### Methods

1. <b>Size</b>

```c++
size_t myVectSize = myVect.size();
```

Returns the vector size (number of elements in the vector). (Return type: size_t)
2. <b>Front</b>

```c++
myVect.front();
```

Same as `myVect[0]`.

3. <b>Back</b>

```c++
myVect.back();
```

Same as `myVect[myVect.size() - 1]`.

4. <b>Empty</b>

```c++
myVect.empty();
```

Returns whether the vector is empty or not. (Return Boolean)

5. <b>clear</b>

```c++
myVect.clear();
```

Removes all elements in a vector, transforming it to an empty vector. (No return)

6. <b>Pop Back</b>

```c++
myVect.pop_back();
```

Delete the last element in the vector. (No return)

7. <b>Push Back</b>

```c++
myVect.push_back(newElem);
```

Adds `newElem` to the end of the vector. (No return)

## Type Aliases

#### Anatomy

```c++
typedef type alias;
```

#### Example

```cpp
typedef vector<double> Vecteur;
typedef vector<Vecteur> Matrice;

Matrice rotation(3, Vecteur(3, 1.0));
```
