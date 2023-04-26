1. On line 12, console.log(i) will output "3" to the console. This is because the var i traverses through the amount of elements in the prices list, which in this case is [100, 200, 300], which is 3 elements.
2. Line 13 will output 150. This is because the for loop traverses through the elements in the prices array, and the discounted price acts as the price in prices multiplied by 1 minus the discount. Therefore, as the for loop ends, discountedPrice has the discounted price of the final item in the array.
3. Line 14 will also just output 150. The 300 multiplied by 0.5 results in 150, which is already a rounded number. The finalPrice variable attempts to round any decimals past the cents, so nothing happens to 150.
4. This function will return an array of such: [50, 100, 150]. This is because the for loop basically traverses through the values in the prices array and applies the discount to each value. The discounted variable then stores all these final prices into an array. 
5. The code causes an error. This is because the i variable is only defined in the for loop since it is using "let i". This has scope only in the for loop, so it is undefined outside, and therefore line 12 throws an error.
6. Similar to number 5, line 13 also throws an error. discountedPrice is initialized with "let" inside of the for loop, meaning that its scoep is inside the for loop. Trying to call the variable outside of the loop on line 13 throws an error.
7. Line 14 outputs 150. finalPrice is initialized on line 4, which is only inside the function. Therefore, the block scope includes the entire function, and it is safe to output the variable. 
8. The function returns the discounted variable, which is an array as such: [ 50, 100, 150 ]. This basically works the same as the code for question 1 in part 2, except using "let" to initialize the variables. This doesn't run into any problems and keeps it the same. The for loop goes through all the prices and scales them by the discount, and outputs the discounted prices in the array "discounted".
9. Line 11 throws an error. On line 6, "let i" is used. Therefore, the scope of the variable i is only in that for loop block. Accessing it outside of the for loop on line 11 throws an error.
10. Line 12 outputs "3". On line 4, length is set to prices.length, which is 3 since there are 3 elements in the prices array: [100, 200, 300]. 
11. This function will return [ 50, 100, 150 ] using the variable discounted. Even though the variable discounted is of type const, it can still be manipulated using .push. It is never reassigned, so the action is fine. Other than that, the function is essentially the same as previously. The length is just store earlier and used to iterate in the for loop. The loop basically declares a variable discountedPrice to store the discounted price and push to the return array for all values in the price array. The const variable "discountedPrice" is redeclared every iteration, which is fine for changing values since it is a global variable that can be redeclared.
12. Notations:
A. student.name
B. student['Grade Year']
C. student.greeting();
D. student['Favorite Teacher'].name
E. student.courseload[0]
13. Arithmetic
A. ‘3’ + 2
Output: '32' because the integers map to their exact string representation.
B. ‘3’ - 2
Output: 1 because the string is converted to a number
C. 3 + null
Output: 3 because the null is converted to 0
D. ‘3’ + null
Output: '3null' because null maps to the string 'null'
E. true + 3
Output: 4 because true becomes 1
F. false + null
Output: 0 becuase false converts to 0 and null converts to 0
G. '3' + undefined
Output: '3undefined' because undefined becomes the string 'undefined'
H. '3' - undefined
Output: NaN becuase undefined has a numeric conversion to NaN
14. Comparison
A. ‘2’ > 1
Output: true because '2' becomes the number 2 
B. ‘2’ < ‘12’
Output: false because it converts to numbers, but only looks at the '1' first in the right side, so 2 < 1 is false
C. 2 == ‘2’
Output: true because it converts '2' to 2, and 2 == 2
D. 2 === ‘2’
Output: false because it is a strict equality and returns false since different types
E. true == 2
Output: false because true equates to 1
F. true === Boolean(2)
Output: true because the object Boolean(2) whose falue is false evaluates to true when passed to a conditional statement
15. The difference between the == and === operators is that the strict equality (===) does not perform the type conversion before checking the equality. Therefore, 2 == '2' would be true, but 2 === '2' would be false since the strict equality sees different types and just returns false
16. look in part2-question16.js
17. The result should be that newArr be [ 2, 4, 6 ]. The doSomething function basically returns the given number times 2. Therefore, when the function is used in the modifyArray function, basically the function first creates a new array to return, then iterates through the "array," and for every element in it it calls doSomething on that value and adds that value to newArr. Therefore, newAr contains all values in the given array multiplied by 2.
18. look in part2-question18.js
19. Output:
    1
    4
    3
    2