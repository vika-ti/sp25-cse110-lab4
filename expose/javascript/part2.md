### Question 1
Line 12 will print 3. An array of three prices was passed into the function. i is defined with var inside a for block. Since it is defined with var, it has function scope and can be accessed by the console log. 

### Question 2
discountedPrice is defined with var, meaning it can be accessed outside the for block. It will print 150. Although discounted price will be used to hold the three passed values with the discount applied, it will hold the last value as it is not reinitialized to 0 anywhere. The last price is 300. With a 0.5 discount, the value is 300*(1-0.5) = 150.

### Question 3
Line 14 prints the value 150. finalPrice has function scope. Although the for loop pushes the finalPrice to the discounted array, the value of finalPrice is not reinitialized and simply holds the last value. The last price passed was 300. The discounted price is 150, while finalPrice multiplies and divides by 100 using math.round, meaning this value is not changed.

### Question 4
This function returns an array of the final discounted prices. These values can be accessed outside of the function only because they are returned.

### Question 5
This will throw a reference error since i will not be defined outside the for block. This is because let has block scope.

### Question 6
Once again, there is a reference error. discountedPrice is defined with let, having block scope, inside of the for loop.

### Question 7
Line 14 prints 150. Although finalPrice is defined with let, it is not in a block like for or if. Therefore, it can be accessed inside the function. The last value that finalPrice was assigned was 150, a 50% discount on 300.

### Question 8
This function returns an array of the discounted prices. This array has three values, [50, 100, 150]. Discounted is defined in the same function using let, and can be accessed.

### Question 9
A reference error is thrown. As explained above, i is declared with let inside a for loop and has block scope. You are accessing it outside of that block.

### Question 10
Prints 3. Length is defined with const, which has block scope. Length is not in a block like the for loop.

### Question 11
The function returns the discounted price array of [50, 100, 150]. Variable discounted has block scope and is defined with const, but there is no reassignment. 

### Question 12
A. student.name
B. student["Grad Year"]
C. student.greeting()
D. student["Favorite Teacher"].name
E. student.courseLoad[0]

### Question 13
A. '3'+2 prints 32
The plus operator triggers string concatenation when used with a string. 
B. '3'-2 prints 1
This cannot be concatenation, so both operands are converted to numbers and subtracted.
C. 3 + null prints 3
In numeric operations, the null is a 0. 
D. '3' + null prints 3null
A string and a plus operators triggers string concatenation again.
E. true + 3 prints 4
True is converted to 1, and 1 + 3 = 4
F. false + null prints 0
False is converted to 0 and null is also 0. 0 + 0 = 0.
G. '3' + undefined prints 3undefined
String concatenation occurs. Undefined is now a string.
H. '3' - undefined prints NaN
Undefined cannot be converted into a number, so it is not a number.

### Question 14
A. '2' > 1 prints true
'2' is converted into a number, and 2 is greater than 1.
B. '2' < '12' prints false
String comparison occurs, and the '1' in '12' comes after '2'.
C. 2 == '2' prints true
'2' is converted into a number with ==, so they are the same.
D. 2 === '2' prints false
This not only checks the value bit also type. Since one is a number and one is a string, it is false.
E. true == 2 prints false
True is converted to 1, and 1 is not equal to 2.
F. true === Boolean(2) prints true
Boolean(2) is true since it is non-zero. It is the same type and both are true.

### Question 15
The '==' operator checks for the same value after type conversion. The '===' operator checks both the value and type. Both must match.

### Question 16
part2-question16.js

### Question 17
This function will return [2,4,6] array. modifyArray is called and simply loops through the passed array. As it loops through the values, it calls the doSomething array, which multiples the value by 2. It is returned back to modifyArray, where it is pushed to the new array. newArr is returned with the new values.

### Question 18
part2-question18.js

### Question 19
The output is
1
4
3
2
1 and 4 are printed immediately, and in order. Although 3 has a 0 second delay, it will not be printed until the function completes. 2 is printed and run after a 1 second delay and is therefore printed last.