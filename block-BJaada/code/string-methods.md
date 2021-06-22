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
`toUpperCase` accepts a index and return to capitalize the string.

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
`toLowerCase`to convert a capital case into a LowerCase.

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
`trim` Removes whitespace from both ends of string.

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
Removes whitespace from end of string.

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
`trimStart`Removes whitespace from Start of string.

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
A new string containing the combined text of provided string.

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
`endsWith`true if the given characters are found at the end of the string otherwise false.

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
`includes`A string to be search for within string.

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
The index of the first occurrence of search value,or -1 if not found.

11. `lastIndexOf`
- Parameter: (searchValue)The string repersenting the value to search for.if searchValue is an empty string,then formIndex is returned("String" data type)
- Return: The index of the last occurrence of search value,or -1 if not found(string data type)
- Example:
```js
let name = "A quick brown fox jumped over a lazy dog"
name.lastIndexOf("dog"); // 37
let houseName = 'Shastri is a student'
houseName.lastIndexOf("is",2) // -1
let sentence = 'A BOY'
sentence.lastIndexOf("Y",5) // 4
```
The index of the last occurrence of search value,or -1 if not found.

12. `padEnd`
- Parameter: (targetLength)The length of the resulting once the current string has been padded.if the value is lower than str.length,the current will we returned.  ("String" data type)
- Return: A string of the specified targetLength with the padString applied at the end of the current string(string data type)
- Example:
```js
let name = "A quick brown fox jumped over a lazy dog"
name.padEnd("dog"); // "A quick brown fox jumped over a lazy dog"
let houseName = 'student'
houseName.padEnd(10,'t') // "studentttt"
let sentence = 'A BOY'
sentence.padEnd(10,'Y') // "A BOYYYYYY"
```
A string of the specified targetLength with the padString applied at the end of the current string.

13. `padStart`
- Parameter: (targetLength)The length of the resulting once the current string has been padded.if the value is less than str.length,then the string is returned as-is.  ("String" data type)
- Return: A string of the specified targetLength with the padString applied at the start of the current string(string data type)
- Example:
```js
let name = "A quick brown fox jumped over a lazy dog"
name.padStart("dog"); // "A quick brown fox jumped over a lazy dog"
let houseName = 'student'
houseName.padStart(10,'t') // "tttstudent"
let sentence = 'A BOY'
sentence.padStart(10,'Y') // "YYYYYA BOY"
```
A string of the specified targetLength with the padString applied at the start of the current string.

14. `repeat`
- Parameter: (count)An integer between 0 and +Infinity,indicating the number of times to repeat the string("String" data type)
- Return: A new string containing the specified number of copies of the given string(string data type)
- Example:
```js
let name = "A quick brown fox jumped over a lazy dog"
name.repeat("dog"); // ""
let houseName = 's'
houseName.repeat(10) // "ssssssssss"
let sentence = 'BOY'
sentence.repeat(4) // "BOYBOYBOYBOY"
```
A new string containing the specified number of copies of the given string.

15. `replace`
- Parameter: regexp(pattern)A RegExp object or literal.The match or matches are replaced with newSubstr or the value returned by the specified replacerFunction("String" data type)
- Return: A new string,with some some or all matches of a pattern replaced by a replacement(string data type)
- Example:
```js
let name = "A quick brown fox jumped over a lazy dog"
name.replace('dog','boy'); //"A quick brown fox jumped over a lazy boy"
let houseName = 'stadent'
houseName.replace('a','u') // "student"
let sentence = 'This is a Boy'
sentence.replace('is','at') // "That is a Boy"
```
A new string,with some some or all matches of a pattern replaced by a replacement.

16. `slice`
- Parameter: regexp(beginIndex) The zero-based index at which to begin extraction.if negative,it is treated as str.length + beginIndex. if beginIndex is not a number after Number(beginIndex),it is treated as 0. 
("String" data type)
- Return: A new string containig the extracted section of the string(string data type)

- Example:
```js
let name = "A quick brown fox jumped over a lazy dog"
name.slice(0,11); //"A quick bro"
let houseName = 'student'
houseName.slice(0,3) // "stu"
let sentence = 'This is a Boy'
sentence.slice(0,4)//"This"
```
A new string containig the extracted section of the string.

17. `split`
- Parameter: separator(Optional)The pattern describing where each split should occur. The separator can be a simple string or it can be a regular expression.  
("String" data type)
- Return: An Array of strings,split at each point where the separator occurs in the given string(string data type)

- Example:
```js
let name = "A student"
name.split(''); //(9)["A","","s","t","u","d","e","n","t"]
let houseName = 'student'
houseName.split(''); // (7)["s","t","u","d","e","n","t"]
let sentence = 'Boy'
sentence.split(''); // (3) ["B","o","y"]
```
An Array of strings,split at each point where the separator occurs in the given string.

18. `substring`
- Parameter: (indexStart)The index of the first character to include in the returned substring  
("String" data type).
- Return: A new string containing the specified part of the given string(string data type).

- Example:
```js
let name = "A student"
name.substring('0,1'); // "A student"
let houseName = 'student'
houseName.substring('0,1'); // "student"
let sentence = 'Boy'
sentence.substring('0,1'); // "Boy"
```
A new string containing the specified part of the given string(string data type).