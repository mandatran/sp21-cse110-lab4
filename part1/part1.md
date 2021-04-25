# Part 1. Intro to Javascript

## Part 1a. A Quick Introduction...

1. 20
2. 20
3. 20
4. Error, `result` is defined in the `if` block but is called outside of the `if` block scope in line 13.
5. Error, `result` in line 7 cannot be reassigned because it is a constant variable.
6. Error, `result` in line 7 cannot be reassigned and it is outside of scope it is defined.

## Part 1b. A Little More of a Challenge...

1. logs `3` because i is being incremented 3 times by the for loop and is declared with `var` so it is still in scope.
2. logs `150` because it logs `discountedPrice` which is last updated when `i = 2` in the for loop. So `discountedPrice = 300 * (1 - 0.5) = 150`. Declared with `var` so it is still in scope.
3. logs `150` because it logs `finalPrice` which is last updated when `i = 2` in the for loop. So since `discountedPrice = 150` from question 2, then `finalPrice = Math.round(150 * 100) / 100 = 150`. Declared with `var` so it is in scope.
4. `[ 50, 100, 150 ]`. The function returns an array of discounted prices, each element in the original array was multiplied by `1 - 0.5 = 0.5` in the for loop and in the final price is the same as the discounted price because `Math.round()` rounds each value to the nearest integer, but these are already integers.
5. At line 12 an error occurs because `i` is not defined within the scope when declared with `let`.
6. At line 12 an error occurs because `discountedPrice` is not defined within the scope.
7. logs `150` because of the same reasons described in (3.), the `let` variable declaration is still in scope for `finalPrice`.
8. logs `[ 50, 100, 150 ]` because of the same reasons described in (4.), and is still in scope.
9. Error because `i` is declared with `let` which is not in scope.
10. logs `3`, the length of the array because it is in scope.
11. logs `[ 50, 100, 150 ]` similar to what is described in (4.), and does not throw an error because each time an element is being assigned to `discountedPrice`, it is only being assigned one time.
12. 
    * A. `student.name;`
    * B. `student['Grad Year'];`
    * C. `student.greeting();`
    * D. `student['Favorite Teacher'].name;`
    * E. `student.courseLoad[0];`
13. Arithmetic
    * A. '32'
        * integers map to their exact string representation
    * B. 1
        * strings are converted to numbers when the `-` is applied to non-numbers
    * C. 3
        * `null` converts to `0` numerically
    * D. '3null'
        * `null` converts to the string `'null'`
    * E. 4
        * `true` converts to the numerical value `1` then is added to `3`
    * F. 0
        * `false` is converted to `0` numerically and `null` is converted to `0` as well
    * G. '3undefined'
        * `undefined` is converted to the string `'undefined'`
    * H. NaN
        * `'3'` is converted to the numerical value `3` but the numerical value of `undefined` is `NaN` which is why the difference is `NaN`
14. Comparison
    * A. true
        * the string `'2'` becomes the number `2`
    * B. false
        * strings are compared in lexicographical order, `'1'` comes before `'2'`
    * C. true
        * compares the values of different types and the string `'2'` becomes the number `2`
    * D. false
        * strict equality checks equality without converting the types, and `2` is a number and `'2'` is a string
    * E. false
        * `true` converts to the number `1` which is not equal to `2`
    * F. true
        * `Boolean(2)` is `true` (since `2` is not an empty value) which is equivalent to `true`
15. `==` is regular equality, which converts operands of different types. `===` is strict equality that does not perform any type conversions.
16. see js file
17. result: `[ 2, 4, 6 ]`. The array `[1, 2, 3]` and the function `doSomething` are passed in as parameters to `modifyArray`. In the for loop, the value returned by `doSomething`, which is twice the original value, is pushed to the new array. The new array is then returned.
18. see js file
19. 
```js
1
4
3
2
```
