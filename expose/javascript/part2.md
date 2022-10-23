# Part2
## Question 1.
It will output 3. The `i` is declared by `var` function, so it can be accessed anywhere inside of the functions `discoutPrices` scope. Also, `i` will increasese to 3 since `prices.length` is 3.
## Question 2.
It will output 150 since `discountedPrice` can be accessed anywhere inside of the function `discountPrices`. `i` = 2 , `discount` = 0.5, and `prices[i]` = 300 at the last iteration of `for` loop, so `prices[i] * (1 - discount);` is 150.
## Question 3.
`finalPrice` can be accessed in anywhere of function `discountPrices` and because of line #8, `finalPrice` has values 150 at the last interation of the `for` loop. Hence, #14 outputs 150.
## Question 4.
The function will return an array `[50, 100, 150]`. A reason that the function `discountPrices` returns an array is because it declars an arrya `discounted` and returns it. Each element represents discounted value of 100, 200 and 300 respectively.

## Question 5.
Erros occurs. A variable `i` is declared by function `let` and it can be access only in the `for` loop. Also, line #12 is not in the `for` scope.

## Question 6.
Erros occurs. `discountedPrice` is declared inside of `for` loop by `let`. So, it cannot be accessed on line #13.

## Question 7.
It outputs a value 150. Since `finalPrice` is declared on `discountPrices`, it can be accessed on line #14 although it is declared by `let`.

## Question 8.
It outputs [ 50, 100, 150 ]. `for` loop can access variables `discounted` and `finalPrice` since they are declared on `discountPrices` scope, and it returns array because type of `discounted` is array.

## Question 9.
Error occurs. Since `i` declared by `let` function in `for` scope, it cannot be accessed out side of `for` scope.

## Question 10.
Line 12 outputs 3 without any problem. `length` declared on `discountPrices` scope by `const`, and the function does not reassigne `length` after the first declaration of `length`. So, line 12 can successfully access `length`.

## Question 11.
The function will return an array [ 50, 100, 150 ]. There is no syntax error, and each discounted value of a input array will be stored into `discounted` and be returned.

## Question 12.
### A. 
`student.name`
### B. 
`student['Grad Year']`
### C.
`student.greeting()`
### D.
`student['Favorite Teacher'].name`
#### E.
`student.courseLoad[0]`

## Question 13.
### A. '32'
32 since `2` maps to its string representation.
### B. 1
1 since `'3'` maps to integer 3.
### C. 3
3 since `null` maps to integer 0.
### D. '3null'
3null since `null` maps to its string representation.
### E. 4
since `true` maps to 1.
### F. 0
since `false` maps to 0, and `null` maps to 0.
### G. '3undefined'
since `undefined` maps to its string representation.
### H. NaN
since an error occurs while converting `undefined` to an interger.

## Question 14.
### A. True
since `'2'` becomes an integer 2.
### B. False
since `'2'` is greater than `'1'`. Javascript compares letter by letter while it is comparing strings.
### C. True
since `'2'` becomes an integer 2.
### D. False
since they have the different types.
### E. False
since `true` becomes 1.
### F. true 
since `Boolean(2)' is just true.

## Question 15.
`===` does not do type conversion when it compares unlike `==`.

## Question 16.
[javascript-file](part2-question16.js)

## Question 17.
The parameters `[1,2,3]` and `doSomethign` are stored into variables `array` and `callback` respectively. Then `modifyArray` declares new empty array `newArr`. During the `for` loop, each element in `[1,2,3]` is sent to `doSomething(num)` as a parameter sicne `callback(array[i])` is actually just `doSomething(array[i])`. And then push all the values that returned by `doSomething` into the `newArr`. Finally, return `newArr`. Therefore, the result going to be `[ 2, 4, 6 ]`.

## Question 18.
[Javascript-file](part2-question18.js)

## Question 19.
1 </br>4 </br>3 </br>2</br>Since 1 and 4 have no `setTimeout`, they will printed out immediately. 3 has delay 0 to print, so it will be printed out after 1 and 4. Lastly, 2 is delaied for 1 sec to print, so it will be printed out at the end.
