1. line 12 will print "3", which can be shown through tracking the for loop based on our input. Our for loop runs 3 times (we are running it from 0 to (prices.length (which is 3) - 1). i++ makes it so we increment after we go through the loop (the for loop goes through i = 0, i = 1, and then has its final iteration at i = 2). At the end of this i = 2 iteration, we increment i one more time even though we've already broken the for loop, resulting in a value of 3 being produced.
2. line 13 will print "150", because the last element of the array that is passed into prices is 300 and the discount is 0.5, meaning that the final value of discountedPrice will be prices[2] (300) * (1 - discount(0.5)), which comes out to 150
3. line 14 will print "150", because once again we are only dealing with the last element of the passed array (300), and we already determined that the value of discountedPcies will be 150. finalPrice sort of deals with whole number rounding, which since we already have a whole number, it will not really do anything to our value, multiplying it by 100, rounding it, and then dividing it by 100. 
4. This function returns the array of finalPrices stored in discounted ([50, 100, 150]). This is because we are pushing them in the order that they came in, after discounting them individually in our for loop. This is our original array ([100, 200, 300]) with the 50% off discount (everything is half of its original value)
5. Line 12 will result in an error, because i is defined in the for loop block, and we attempt to access it outside of that block, which results in an error.
6. Line 13 will result in an error for the same reason as number 5 (discounted price is defined in the for loop block, but is being accessed outside of that block, which results in an error
7. Line 14 will print "150" because finalPrice is defined in the function block, which is also where we attempt to access it, resulting in a valid use of the let keyword.
8. This function returns the array of finalPrices stored in discounted ([50, 100, 150]). This is because discounted is defined in the function block (contains everything except for the call statement), meaning that it can be accessed at any point inside of the function block (which our call is in). This is a valid use of the let keyword, resulting in no errors being made.
9. Line 11 will result in an error, because i is still initialized with the let keyword, meaning that we cannot access it outside of the for loop (which we attempted to do, which is why we had an error).
10. Line 12 will return "3" because we are just returning the length of prices (3 elements). At no point do we attempt to change the value of the constant, so we have no error in retrieving this value.
11. This returns the discounted array [50, 100, 150] (unrounded now that finalPrice is no longer there, but doesn't matter for our example). This is because even though the array has the const keyword, we can still push elements to it. What we would not be able to do with a const array would be reassignment, which we did not attempt to do, resulting in no errors being made. 
12. <br>
A) student.name; <br>
B) student["Grad Year"]; <br>
C) student.greeting(); <br>
D) student["Favorite Teacher"].name; <br>
E) student.courseLoad[0]; <br>
13. <br>
A) '3' + 2 = '32' because "3" is a string, and it just converts 2 to a string and adds it to the end of 3 <br>
B) '3' - 2 = 1 because javascript actually converts the string 3 to an int this time and subtracts 2 from it to get 1 <br>
C) 3 + null = 3 because null is treated as a 0 when it is an int, and 3 + 0 = 3 <br>
D) '3' + null = '3null' because it is just adding the string null onto the end of the string "3" <br>
E) true + 3 = 4 because true has an integer value of 1 and 1 + 3 = 4 <br>
F) false + null = 0 because false has a value of 0, and 0 + 0 = 0 <br>
G) '3' + undefined = '3undefined' because it is just adding the string 'undefined' to the end of the string '3' <br>
H) '3' - undefined = NaN (Not a number) because 3 is treated as an integer, and you are subtracting undefined from a number, which is undefined <br>
14. <br>
A) '2' > 1 returns true because '2' is converted to an int, and 2 is greater than 1, making this statement true <br>
B) '2' < '12' returns false because it just compares the first character, and '2' is considered greater than '1' <br>
C) 2 == '2' returns true because '2' is converted to an int, and 2 == 2 is true <br>
D) 2 === '2' returns false because === checks both value and type, and since we are comparing a string with an int, this is false <br>
E) true == 2 returns false because true has an integer value of 1, and 1 does not equal 2 <br>
F) true === Boolean(2) returns true, because they are both booleans, and are both true, meaning that they are the same value and the same type <br>
15. == just compares the two through value (ex: 2 == 2, '2' == 2), where === compares the two through value and type ('2' === '2', '2' does not === 2) <br>
17. the result will be newArr ([2, 4, 6]). The for loop runs 3 times, and each time, we run callback on each array slot, which multiplies the number by 2 and then pushes it into the newArr. This results in the three numbers that were inputted ([1,2,3]) being multiplied by 2 (through doSomething), and being put in the new array) <br>
19. The output of this above code is 1, 4, 3, 2. This is because of the delays, the calls to print 1 and 4 are instant, the call to print 3 is delayed by 0 ms (it still comes after the no delay calls), and the call to print 2 is delayed by a whole second (shows up a second after 1, 4, and 3 are printed). 
