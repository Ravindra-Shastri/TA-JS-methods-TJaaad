Watch this video to understand what to do in this exercise block [link](https://www.youtube.com/watch?v=zGpplZj4zY0&feature=youtu.be)

## Getting To Know Array Methods

Go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) and look for the name of method to learn about it.

**Write in your own way of understanding (don't copy paste)**

Only if you are done with step 1 you should go ahead.

1. Practice it by yourself in console (2-3 times to understand)
2. Data types of parameters
3. Return value type
4. Write three examples
5. In your words what this method does.
6. Does it mutate the original value or not (check https://doesitmutate.xyz)

Example:

1. `concat`

   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: a single Array consisting of by all the values passed as parameters in the same order.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.concat(4); //[1,2,3,4]
     let sentanceArray = 'A quick brown fox jumped over a lazy'.split(' ');
     sentanceArray.concat('dog').join(' '); //"A quick brown fox jumped over a lazy dog"
     let colors = ['red', 'green', 'blue'];
     colors.concat('black', 'red', 21, true); // ['red','green','blue','black', 'red', 21, true]
     ```
   - `concat` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array

2. `join`

- Parameter: separator(Optional) join() methods creates and returs a new string by concatenating all of the elements in an array.
   - Return: A string with all aray elements joined.if arr.length is 0 then return empty string.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.join(); //"1,2,3"
     let sentanceArray = ['A quick brown fox jumped over a lazy dog'];
     sentanceArray.join(); //"A quick brown fox jumped over a lazy dog"
     let colors = ['red', 'green', 'blue'];
     colors.join(); // "red,green,blue"
     ```
   - `join`method creates and returs a new string by concatenating all of the elements in an array.


3. `flat`

- Parameter: (depth)flat specifies the depth level,means how deep a nested array structure should be flattened. 1 is Default. 
   - Return: A new arrey with concatinated elements of sub-arrays.
   - Example:
     ```js
     let numbers = [1, [2, 3,[4,5,[6,7,[8,9]]]]];
     numbers.flat(4); //(9)[1,2,3,4,5,6,7,8,9]
     let sentanceArray = [A quick brown [fox jumped over a lazy]].
     sentanceArray.flat(2); //["A quick brown fox jumped over a lazy dog"]
     let colors = ['red', 'green', 'blue'];
     colors.flat(); // ["red","green","blue"]
     ```
   - `flat` specifies the depth level,means how deep a nested array structure should be flattened. 1 is Default. 

4. `push`
- Parameter:(elementN) The element(s) to add to the end of the array.
   - Return: The new length property of the object upon which the method was called.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.push(4); //[1,2,3,4]
     let sentanceArray = ['A quick brown fox jumped over a lazy']
     sentanceArray.push('dog'); //["A quick brown fox jumped over a lazy", "dog"]
     let colors = ['red', 'green', 'blue'];
     colors.push('black'); // ["red","green","blue","black"]
     ```
   - `push`The push() method adds one or more elements to the end of an array and returns the new length of the array.

5. `indexOf`
- Parameter: (searchElement) to locate index of element in the array.
   - Return:The first index of the element in the array; -1 if not found.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.indexOf(2); // 1
    let sentanceArray = ['A quick brown fox jumped over a lazy dog'];
     sentanceArray.indexOf('dog').// -1
     let colors = ['red', 'green', 'blue'];
     colors.indexof('red'); // 0
     ```
   - `indexof` The indexOf() method returns the last index at which a given element can be found in the array, or -1 if it is not present.

   - No it does not mutate the original array

6. `lastIndexOf`
   - Parameter: (searchElement) to locate index of element in the array.
   - Return:The last index of the element in the array; -1 if not found.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.lastIndexOf(2); // 1
    let sentanceArray = ['A quick brown fox jumped over a lazy dog'];
     sentanceArray.lastIndexOf('dog');// -1
     let colors = ['red', 'green', 'blue'];
     colors.lastIndexOf('green'); // 1
     ```
   - `lastIndexof`The lastIndexOf() method returns the last index at which a given element can be found in the array, or -1 if it is not present.

   - No it does not mutate the original array

7. `includes`
- Parameter: The value to search for.
   - Return: A Boolean which is true if the value searchElement is found within the array .
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.includes(4); //false
     let sentanceArray = 'A quick brown fox jumped over a lazy dog'
     sentanceArray.includes('dog'); //true
     let colors = ['red', 'green', 'blue'];
     colors.includes('black'); // false
     ```
   - `includes` The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.

   - No it does not mutate the original array

8. `reverse`
- Parameter:The first array element becomes the last, and the last array element becomes the first.
   - Return:  reversed array.

   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.reverse(); //(3)[3,2,1]
     let sentanceArray = ['A quick brown fox jumped over a lazy dog','dog'];
     sentanceArray.reverse();//["dog","A quick brown fox jumped over a lazy dog"]
     let colors = ['red', 'green', 'blue'];
     colors.reverse()// (3)["blue","green","red"]
     ```
   - `reverse` The first array element becomes the last, and the last array element becomes the first.
   -  it  mutate the original array.

9. `every`
- Parameter: A function to test for each element, taking three arguments.
   - Return: true if the callbackFn function returns a truthy value for every array element. Otherwise, false.(It returns a Boolean value).
   - Example:

 ```js
     function isBigEnough(element, index, array) {
  return element >= 10;
}

[12, 5, 8, 130, 44].every(isBigEnough);// false

const isBelowThreshold = (currentValue) => currentValue < 40;

const array1 = [1, 30, 39, 29, 10, 13];

console.log(array1.every(isBelowThreshold));
// true
```

- `every` The every() method tests whether all elements in the array pass the test implemented by the provided function. 


   - No it does not mutate the original array

10. `shift`
- Parameter:shift() method removes the first element     from an array and returns that removed element.
   - Return: removed element from the array; undefined if the array is empty.

   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.shift(); // 1
     let sentanceArray = ['dog','A quick brown fox jumped over a lazy'];
     sentanceArray.shift(); //"dog"
     let colors = ['red', 'green', 'blue'];
     colors.shift(); // "red"
     ```
   - `shift` removes the first element from an array and returns that removed element.
   - it mutates the original array.

11. `splice`
- Parameter: splice() method changes the contents of an array by removing or replacing existing elements .
   - Return: An array containing the deleted elements.

   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.splice(2); //[3]
     let sentanceArray = ['A quick brown fox jumped over a lazy dog'];
     sentanceArray.splice(); // []
     let colors = ['red', 'green', 'blue'];
     colors.splice(); // [] 
     ```
   - `splice` splice() method changes the contents of an array by removing or replacing existing elements .
   -  it mutates the original array.

12. `find`
- Parameter: (callbackFn)
Function to execute on each value in the array, taking 3 arguments:
- Return: The value of the first element in the arrathat satisfies the provided testing function.
- Example:
 ```js
  const array1 = [5, 12, 8, 130, 44];

const found = array1.find(element => element > 10);

console.log(found); // 12

const inventory = [
  {name: 'apples', quantity: 2},
  {name: 'bananas', quantity: 0},
  {name: 'cherries', quantity: 5}
];

function isCherries(fruit) {
  return fruit.name === 'cherries';
}

console.log(inventory.find(isCherries));
// { name: 'cherries', quantity: 5 }
```
- `find` Function to execute on each value in tharray, taking 3 arguments.
- No it does not mutate the original array

13. `unshift`
- Parameter: (elementN) The elements to add to the front of the arr.
   - Return:The new length property of the object upon which the method was called.

   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.unshift(0); //[0,1,2,3]
     let sentanceArray = ['A quick brown fox jumped over a lazy dog'];
     sentanceArray.unshift('dog'); //["dog","A quick brown fox jumped over a lazy dog"]
     let colors = ['red', 'green', 'blue'];
     colors.unshift('black','brown'); // (5)["black","brown","red","green","blue"]
     ```
   - `unshift` The unshift() method adds one or more elements to the beginning of an array and returns the new length of the array.
   -it mutates the original array.

14. `findIndex`
- Parameter: callbackFn
A function to execute on each value in the array until the function returns true, indicating that the satisfying element was found.

 - Return: The index of the first element in the array that passes the test. Otherwise, -1.

 - Example:
 ```js
   const array1 = [5, 12, 8, 130, 44];

const isLargeNumber = (element) => element > 13;

console.log(array1.findIndex(isLargeNumber));
// 3

function isPrime(num) {
  for (let i = 2; num > i; i++) {
    if (num % i == 0) {
      return false;
    }
  }
  return num > 1;
}

console.log([4, 6, 8, 9, 12].findIndex(isPrime)); // -1, not found

   ```
 - `findIndex` The findIndex() method returns theindex of the first element in the array thatsatisfies the provided testing function. 
   - No it does not mutate the original array

15. `filter`
- Parameter: (callbackFn) Function is a predicate, to test each element of the array. Return a value that coerces to true to keep the element, or to false otherwise.
   - Return: A new array with the elements that pass the test. If no elements pass the test, an empty array will be returned.

  Example:
```js
     const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

const result = words.filter(word => word.length > 6);

console.log(result);
// Array ["exuberant", "destruction", "present"]

function isBigEnough(value) {
  return value >= 10
}

let filtered = [12, 5, 8, 130, 44].filter(isBigEnough)
// filtered is [12, 130, 44]

```
   - `filter` A new array with the elements that pass the test. If no elements pass the test, an empty array will be returned.

   - No it does not mutate the original array

16. `flat`
- Parameter: The depth level specifying how deep a nested array structure should be flattened. Defaults to 1.
   - Return:A new array with the sub-array elements concatenated into it.
   - Example:
     
```js
     let numbers = [1, 2, [3,4,[5,6,[7,8]]]];
     numbers.flat(4); //(8) [1,2,3,4,5,6,7,8]
     let sentanceArray = ['A quick brown fox jumped over a lazy dog'];
     sentanceArray.flat(); //["A quick brown fox jumped over a lazy dog"]
     let colors = ['red', 'green', 'blue'];
     colors.flat(); // (3)["red","green","blue"]

  ```
   - `flat`  flat() method creates a new array with all sub-array elements concatenated into it recursively up to the specified depth.
   -  it mutates the original array.

17. `forEach`
- Parameter: Function to execute on each element. It accepts between one and three arguments.
   - Return: undefined, because it's not return anything.
   - Example:
 ```js
     const array1 = ['a', 'b', 'c'];

array1.forEach(element => console.log(element));

//  "a"
//  "b"
//  "c"

const arraySparse = [1,3,,7]
let numCallbackRuns = 0

arraySparse.forEach(function(element) {
  console.log(element)
  numCallbackRuns++
})

console.log("numCallbackRuns: ", numCallbackRuns)

// 1
// 3
// 7
```
   - `forEach` The forEach() method executes a provided function once for each array element.
   - No it does not mutate the original array.

18. `map`
- Parameter:Function that is called for every element of arr. Each time callbackFn executes, the returned value is added to newArray.
   - Return:A new array with each element being the result of the callback function.
   - Example:

 ```js
     let numbers = [1, 4, 9]
    let roots = numbers.map(function(num){
        return Math.sqrt(num)
    });// undefined

    const array1 = [1, 4, 9, 16];

// pass a function to map
const map1 = array1.map(x => x * 2);

console.log(map1);
// Array [2, 8, 18, 32]

 ```
   - `map` map() method creates a new array populated with the results of calling a provided function on every element in the calling array.
   - No it does not mutate the original array.

19. `pop`
- Parameter:pop() method removes the last element from an array and returns that element. This method changes the length of the array.
   - Return: The removed element from the array; undefined if the array is empty.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.pop(); // (2)[1,2]
     let sentanceArray = ['A quick brown fox jumped over a lazy dog'];
     sentanceArray.pop(); //"A quick brown fox jumped over a lazy dog"
     let colors = ['red', 'green', 'blue'];
     colors.pop(); // (2) ["red","green"]
     ```
   - `pop` pop() method removes the last element from an array and returns that element. This method changes the length of the array.
   -it mutatets the original array.

20. `reduce`
- Parameter: A function to execute on each element in the array (except for the first, if no initialValue is supplied).
   - Return: The single value that results from the reduction.
   - Example:
 ```js
     const array1 = [1, 2, 3, 4];
const reducer = (accumulator, currentValue) => accumulator + currentValue;

// 1 + 2 + 3 + 4
console.log(array1.reduce(reducer));
// 10

// 5 + 1 + 2 + 3 + 4
console.log(array1.reduce(reducer, 5));
// 15

let sum = [0, 1, 2, 3].reduce(function (accumulator, currentValue) {
  return accumulator + currentValue
}, 0)
// sum is 6

  ```
   - `reduce` reduce() method executes a reducer function (that you provide) on each element of the array, resulting in a single output value.
   - No it does not mutate the original array

21. `slice`
- Parameter: The slice() method returns a shallow copy of a portion of an array into a new array object selected from start to end .
   - Return:A new array containing the extracted elements.

   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.slice(1); // (2)[2,3]
     let sentanceArray = 'A quick brown fox jumped over a lazy dog';
     sentanceArray.slice(2); //"quick brown fox jumped over a lazy dog"
     let colors = ['red', 'green', 'blue'];
     colors.slice(2); // ["blue"]
     ```
   - `slice` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array.

22. `some`
- Parameter: (callback) A function to test for each element, taking three arguments:

- Return: true if the callback function returns a truthy value for at least one element in the array. Otherwise, false.

   - Example:
 ```js
     const array = [1, 2, 3, 4, 5];

// checks whether an element is even
const even = (element) => element % 2 === 0;

console.log(array.some(even));
// expected output: true

function isBiggerThan10(element, index, array) {
  return element > 10;
}

[2, 5, 8, 1, 4].some(isBiggerThan10);  // false
[12, 5, 8, 1, 4].some(isBiggerThan10); // true
Copy to Clipboard

     ``` 
   - `some`The some() method tests whether at least one element in the array passes the test implemented by the provided function.
   - No it does not mutate the original array.

