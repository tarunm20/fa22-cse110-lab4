   1) On line 12 we return the current value of i after the for loop is completed because i was initialized using the var keyword. Using var means that we can access a given variable within the scope of the function. Even if it was initialized within a smaller block but is being accessed outside that scope. In this example i=3 because prices is length 3. Although we count starting at 0, since the for loop incrememnts the variable first then checks the condition, i=3.
   2) We get a similar response to question 1 because discountedPrice was initialized with the var keyword. In this case it returned 150 which was the most recent update to the variable.
   3) Although finalPrice was initialized outside of the scope of the for loop, since it is still within the scope of the function, and was initialized using the var keyword, we can access the variable. In this case the most recent update of finalPrice returns 150.
   4) The function returns all the discounted prices from the prices list we initialized. In this case we get [ 50, 100, 150 ].
   5) We get the error "ReferenceError: i is not defined". This is because we are using the let keyword meaning we can only access the initialized variable within the scope it was defined in. In this case, we can only access i within the for loop but we are trying to print it outside.
   6) Similar to the previous question, we are getting the error "ReferenceError: discountedPrice is not defined". This error is occuring because discountedPrice was initialized with the let keyword and is defined within the for loop but we are trying to print it outside.
   7) Unlike the previous examples, we are not getting any errors in this case. There are no errors occuring because finalPrice, even though it was defined with the let keyword, is being called within the scope of its definition. In this case it was defined within the function's scope, so it can be accessed anywhere within the function.
   8) This function will return the desired output. In this case we get [ 50, 100, 150 ]. This output occurs because all the variables defined with the let keyword are being used within the scope of their definition. Therefore, there are no errors with the usage of the variables.
   9) In this example, we get an error "ReferenceError: i is not defined". This error occurs because we use the let keyword to define the i variable. Since i was defined within the scope of the for loop, we have no access to the variable outside of the loop.
   10) In this case, we do not get any errors and the length variable is printed out. Since we defined length using the const keyword, and we do not attempt to change the variable in the function, we do not get any errors. The value printed is 3.
   11) In this example, the function returns [ 50, 100, 150 ] as expected. We are just taking the discounted prices and appending them to the disconuted list which we are returning. Although we defined discounted as a const, we are not changing what the variable actually is, we are only appending data to what is already there.
   12) 
   A) student.name
   B) student["Grad Year"]
   C) student.greeting()
   D) student["Favorite Teacher"].name
   E) student.coursLoad[0]
   13) 
   A) We get 32. Since + is used for addition and concatenation, if either variable is a string, the other one is converted to a string and the operation is conducted.
   B) We get 1. Since - is used for subtraction. The variable that is not a number will be converted and then the operation occurs.
   C) We get 3. When null is used for arithmetic it is treated as 0.
   D) We get 3null. Since one of the operands is a string, the other is converted and concatenated.
   E) We get 4. When using arithmetic with true(1) and false(0), the values are converted to their number equivalent. 
   F) We get 0. Since false and null are both 0 we get 0.
   G) We get 3undefined. Since we are doing a string operation, undefined is converted to a string.
   H) We get NaN. When undefined is used with a numeric operator, it's converted to NaN.
   14)
   A) We get true. We are doing a numeric comparison so the values are converted to numbers respectively.
   B) We get false. Since we are using strings, they are converted to their lexicographical values and then compared.
   C) We get true. Using the == comparator, we convert the values to numerical values and compare them.
   D) We get false. Using the === comparator, we compare both sides at face value. Since an integer does not equal a string, we return false.
   E) We get false. Since we are trying to compare to a number, true is converted to 1. In this case 1 == 2 is false.
   F) We get true. When we use the Boolean(x) function, we cast the input to either a 0 or 1. In this case, any value that is not 0 returns 1. Therefore, 1 === 1 is true.
   15) The difference between == and === is that == converts either side of the comparison respectively so that we can compare their intended values. On the other hand, === compares both sides based on their face value, or fundamental value. For example, 1==true will return true, but 1===true will return false. Since true can be converted to 1, but fundamentally true is a boolean instead of an integer.
   16) In a seperate file.
   17) The function call returns [ 2, 4, 6 ]. After calling the function in the final line, we are taken to modifyArray where we initialize a new array and create a for loop. In the loop, we take each element in 'array' and call another function 'callback' with the element as the function parameter. In this case 'callback' is the doSomething function. We then execute the doSomething function with the element and return the value back to the modifyArray function which pushes the result into newArr. We repeat this step until we iterate through the whole array and finally return the modified array.
   18) In a different file.
   19) The output is 1 4 3 2.