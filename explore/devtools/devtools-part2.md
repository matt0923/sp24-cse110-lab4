1. The bug was that num1 and num2 were being taken in as strings, meaning that they were just added onto each other and returned as a string (num1 = 1 and num2 = 2 would return "12" instead of 3 like its supposed to).  
2. I would fix the bug by setting num1 and num2 to integers by adding parseInt to both of them, giving me the correct result of the sum of the two numbers. 
