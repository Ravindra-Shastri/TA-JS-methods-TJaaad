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
     <!-- ```js
      let numbers = [1, 2, 3];
     numbers.every(2,2,arr); //[1,2,3,2]
     let sentanceArray = 'A quick brown fox jumped over a lazy';
     sentanceArray.every('dog'); //"A quick brown fox jumped over a lazy dog"
     let colors = ['red', 'green', 'blue'];
     colors.every('black'); // ['red','green','blue','black', 'red', 21, true]
     ``` -->
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
  <!-- ```js
  let numbers = [1, 2, 3];
  numbers.find(); //[1,2,3,4]
  let sentanceArray = ['A quick brown fox jumped ovea lazy'].
  sentanceArray.find(); //"A quicbrown fox jumped over a lazy dog"
  let colors = ['red', 'green', 'blue'];
  colors.find('black'); // 
  ``` -->
- `find` Function to execute on each value in tharray, taking 3 arguments.
- No it does not mutate the original array

13. `unshift`
- Parameter: (elementN) The elements to add to the front of the arr.
   - Return:The new length property of the object upon which the method was called.

   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.concat(4); //[1,2,3,4]
     let sentanceArray = 'A quick brown fox jumped over a lazy'.split(' ');
     sentanceArray.concat('dog').join(' '); //"A quick brown fox jumped over a lazy dog"
     let colors = ['red', 'green', 'blue'];
     colors.concat('black', 'red', 21, true); // ['red','green','blue','black', 'red', 21, true]
     ```
   - `unshift` The unshift() method adds one or more elements to the beginning of an array and returns the new length of the array.
   -it mutates the original array.

14. `findIndex`
- Parameter: callbackFn
A function to execute on each value in the array until the function returns true, indicating that the satisfying element was found.

 - Return: The index of the first element in the array that passes the test. Otherwise, -1.

 - Example:
   <!-- ```js
   let numbers = [1, 2, 3];
   numbers.findIndex(1); //[1,2,3,4]
   let sentanceArray = 'A quick brown fox jumped overa lazy';
   sentanceArray.findIndex('dog'); //"A quickbrown fox jumped over a lazy dog"
   let colors = ['red', 'green', 'blue'];
   colors.findIndex('black'); // ['red''green','blue','black', 'red', 21, true]
   ``` -->
 - `findIndex` The findIndex() method returns theindex of the first element in the array thatsatisfies the provided testing function. 
   - No it does not mutate the original array

15. `filter`
- Parameter: (callbackFn) Function is a predicate, to test each element of the array. Return a value that coerces to true to keep the element, or to false otherwise.
   - Return: A new array with the elements that pass the test. If no elements pass the test, an empty array will be returned.

   <!-- - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.concat(4); //[1,2,3,4]
     let sentanceArray = 'A quick brown fox jumped over a lazy'.split(' ');
     sentanceArray.concat('dog').join(' '); //"A quick brown fox jumped over a lazy dog"
     let colors = ['red', 'green', 'blue'];
     colors.concat('black', 'red', 21, true); // ['red','green','blue','black', 'red', 21, true]
     ``` -->
   - `filter` A new array with the elements that pass the test. If no elements pass the test, an empty array will be returned.

   - No it does not mutate the original array

16. `flat`
- Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: a single Array consisting of by all the values passed as parameters in the same order.
   - Example:
     ```js
     let numbers = [1, 2, [3,4,[5,6,[7,8]]]];
     numbers.flat(4); //(8) [1,2,3,4,5,6,7,8]
     let sentanceArray = ['A quick brown fox jumped over a lazy dog'];
     sentanceArray.flat(1); //"A quick brown fox jumped over a lazy dog"
     let colors = ['red', 'green', 'blue'];
     colors.flat(); // (3)["red","green","blue"]
     ```
   - `flat` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array

17. `forEach`
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
   - `forEach` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array

18. `map`
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
   - `map` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array

19. `pop`
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
   - `pop` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array

20. `reduce`
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
   - `reduce` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array

21. `slice`
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
   - `slice` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array

22. `some`
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
   - `some` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array

