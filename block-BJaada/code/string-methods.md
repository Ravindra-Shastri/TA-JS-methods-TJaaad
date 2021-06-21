Watch this video to understand what to do in this exercise block [link](https://www.youtube.com/watch?v=zGpplZj4zY0&feature=youtu.be)

#### Getting To Know String Methods

Go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) and look for the name of method to learn about it.

**Write in your own way of understanding (don't copy paste)**

Only if you are done with step 1 you should go ahead.

1. Practice it by yourself in console (4-5 times to understand)
2. Data types of parameters
3. Return value type
4. Write three examples
5. In your own words and one sentence explain what this method does.

Example:

1. `charAt`

   - Parameter: (index) defaults to 0 - (number data type)
   - Return: character at specific index in the string (string data type)
   - Example:
     ```js
     let name = 'Arya Stark';
     name.charAt(2); //"y"
     let sentence = 'A quick brown fox jumped over a lazy dog';
     sentence(4); // "i"
     let houseName = 'Starks';
     houseName.charAt(0); // "S"
     ```
   - `charAt` accepts a index (number data type) and return the character on that index in the string.

2. `toUpperCase`
- Parameter: Convert to UpperCase("string" data type)
- Return: A new string converted to UpperCase(string data type)
- Example:
```js
let name = 'John Snow'
name.toUpperCase() // "JOHN SNOW"
let houseName = 'Shastri'
houseName.toUpperCase() // "SHASTRI"
let sentence = 'John is a boy'
sentence.toUpperCase() // "JOHN IS A BOY"
```
3. `toLowerCase`
- Parameter: Convert to LowerCase("string" data type)
- Return: A new string converted to LowerCase(string data type)
- Example:
```js
let name = 'JOHN SNOW'
name.toLowerCase() // "john snow"
let houseName = 'SHASTRI'
houseName.toLowerCase() // "shastri"
let sentence = 'JOHN IS A BOY'
sentence.toLowerCase() // "john is a boy"
```
4. `trim`
- Parameter: Removes whitespace from both ends("string" data type)
- Return: A new string stripped of whitespace(string data type)
- Example:
```js
let name = "  John Snow  "
name.trim() // "John Snow"
let houseName = '  Shastri   '
houseName.trim() // "Shastri"
let sentence = '   JOHN IS A BOY  '
sentence.trim() // "JOHN IS A BOY"
```

5. `trimEnd`
- Parameter: Removes whitespace from end("string" data type)
- Return: A new string stripped of whitespace(string data type)
- Example:
```js
let name = "  John Snow  "
name.trimEnd() // "  John Snow"
let houseName = '  Shastri   '
houseName.trimEnd() // "  Shastri"
let sentence = '   JOHN IS A BOY  '
sentence.trimEnd() // "  JOHN IS A BOY"
```
6. `trimStart`
- Parameter: Removes whitespace from Start("string" data type)
- Return: A new string stripped of whitespace(string data type)
- Example:
```js
let name = "  John Snow  "
name.trimStart() // "John Snow   "
let houseName = '  Shastri   '
houseName.trimStart() // "Shastri   "
let sentence = '   JOHN IS A BOY  '
sentence.trimStart() // "JOHN IS A BOY   "
```
7. `concat`
- Parameter: Concatenates the string("string" data type)
- Return: A new string containing the combined text of provided string (string data type)
- Example:
```js
let name = "John"
name.concat("a",name) // "JohnaJohn"
let houseName = 'Shastri'
houseName.concat("and",houseName) // "ShastriaShastri"
let sentence = 'A BOY'
sentence.concat("the",sentence) // "A BOYtheA BOY"
```
8. `endsWith`
- Parameter: Determines whether a string ends with characters of a specified string("String" data type)
- Return: true if the given characters are found at the end of the string otherwise false(Boolean data type)
- Example:
```js
let name = "A quick brown fox jumped over a lazy dog"
console.log(name.endsWith("dog",name.length)); // true
let houseName = 'Shastri is a student'
houseName.endsWith("t",houseName.length) // true
let sentence = 'A BOY'
sentence.endsWith("t",sentence.length) // false
```
9. `includes`
- Parameter: A string to be search for within string("String" data type)
- Return: true if the search string are found anywere within the string otherwise false(Boolean data type)
- Example:
```js
let name = "A quick brown fox jumped over a lazy dog"
name.includes("dog"); // true
let houseName = 'Shastri is a student'
houseName.includes("is",2) // true
let sentence = 'A BOY'
sentence.includes("Y",5) // false
```
10. `indexOf`
- Parameter: (searchValue)The string value to search for.("String" data type)
- Return: The index of the first occurrence of search value,or -1 if not found(string data type)
- Example:
```js
let name = "A quick brown fox jumped over a lazy dog"
name.indexOf("dog"); // 37
let houseName = 'Shastri is a student'
houseName.indexOf("is",2) // 8
let sentence = 'A BOY'
sentence.indexOf("Y",5) // -1
```


11. `lastIndexOf`
- Parameter: (searchValue)The string value to search for.("String" data type)
- Return: The index of the first occurrence of search value,or -1 if not found(string data type)
- Example:
```js
let name = "A quick brown fox jumped over a lazy dog"
name.indexOf("dog"); // 37
let houseName = 'Shastri is a student'
houseName.indexOf("is",2) // 8
let sentence = 'A BOY'
sentence.indexOf("Y",5) // -1
```
12. `padEnd`
13. `padStart`
14. `repeat`
15. `replace`
16. `slice`
17. `split`
18. `substring`
