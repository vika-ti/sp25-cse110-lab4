### Question 1
Line 9 prints the value 20, since you pass two values of 10 and add is true. Since it is true, it enters the if statement and adds 10 with 10. The value is stored in result, and printed.

### Question 2
Line 13 prints 20 as well. The variable result is defined with var inside the function. As a result, you can access this variable from anywhere in the function. 

### Question 3
You should not use var, because it has function scope. If you can access a variable outside a certain block, like the if in this example, then you may accidently overwrite variables, access variables you should not be able to access, or just create unexpected behaviours in general. 

### Question 4
Line 9 prints 20. The keyword 'let' also allows you to declare variables, but their only difference is the scope. The console print statement is inside the if block, meaning it can access the variable result. 

### Question 5
Line 13 will return an error, since result is not a variable that it views is defined. It cannot access the variable since it is defined with 'let', a keyword with block scope rather than function scope. Result will not be defined.

### Question 6
An error will be thrown on line 7, since you are trying to change the value of a constant variable. Nothing will be printed on line 9 as a result.

### Question 7
Line 13 would also print nothing. Aside from the previous error, the keyword 'const' also has block scope rather than function scope. Result will not be defined.