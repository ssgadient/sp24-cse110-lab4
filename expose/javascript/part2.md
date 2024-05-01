Question 1: The console outputs 3. The for loop initializes i = 0, and increments until `i = prices.length = 3`. \
Question 2: The console outputs 150. discountedPrice updates for the last time when i = 2, so `discountedPrice = price[2] * (1 - discount) = 300 * 0.5 = 150`. \
Question 3: The console outputs 150. finalPrice updates for the last time when `i = 2`, so `finalPrice = Math.round(discountedPrice * 100) / 100 = 150 * 100 / 100 = 150`. \
Question 4: The function returns the list `[50, 100, 150]`. At the end of each loop, discounted receives rounded discounted price, which is in this case is a list of the original prices with each price cut in half. \
Question 5: Reference error. i is not defined outside the scope of the for loop. \
Question 6: Reference error. Similarly to question 5, discountedPrice is not defined outside the scope of the for loop. \
Question 7: The console outputs 150. Since finalPrice is defined outside of the for loop, its scope includes the entire function including the for loop. Therefore it can be updated by the for loop, as well as accessed in line 14. \
Question 8: The function returns the list `[50, 100, 150]`. Similarly to question 7, discounted is defined outside the for loop, so its scope is the entire function, and can be updated by the for loop and accessed outside the for loop. It therefore returns the same list as shown in question 4. \
Question 9: Reference error. Similarly to question 5, i is not defined outside the scope of the for loop. \
Question 10: The console outputs 3. length is defined outside the for loop as const, and nothing has attempted to change length before it is accessed. \
Question 11: The function returns `[50, 100, 150]`. The reason why it does not throw a type error is because discounted is not be reassigned, its data is being mutated. The discounted variable refers to an object (an array) and we are not creating a new object when we push to an array, we are simply changing the original object's properties. const prevents reassignment, but not modification of the object's internals. \
Question 12: 
- A. `student.name`
- B. `student['Grad Year']`
- C. `student.greeting()`
- D. `student['Favorite Teacher'].name`
- E. `stduent.courseLoad[0]`\
Question 13: 
- A. `'32'`. The addition operator checks if an operand is a string, and if it is, it converts the other operand to a string and concatenates. 
- B. `1`. The subtraction operator converts both others operand to a number and subtracts. 
- C. `3`. Since neither operand is a string, it converts both sides to numbers and adds. `null` is mapped to 0 so the answer is 3. 
- D. `'3null'`. Since one of the operands is a string, it converts `null` to string and concatenates. 
- E. `4`. Since neither operand is a string, it converts both sides to numbers and adds. `true` is mapped to 1 so the answer is 4. 
- F. `0`. Since neither operand is a string, it converts both sides to numbers and adds. `null` is mapped to 0 and `false` is mapped to 0 so the answer is 0. 
- G. `'3undefined'`. Since one of the operands is a string, it converts `undefined` to string and concatenates. 
- H. `NaN`. The subtraction operator converts both `'3'` and `undefined` to numbers, where are `3` and `NaN` respectively. Therefore, we have `3-NaN = NaN` \
Question 14: 
- A. `true`. If the objects are of different types, the comparison operator converts both operands to numbers and compares. `'2'` gets converted to `2` and since `2 > 1` we output `true`. 
- B. `false`. If the objects are both string, the comparison operator uses lexicographical order to compare. Since `'12'` comes before `'2'` lexicographically, then we output `false`. 
- C. `true`. This is a nonstrict equality check, where the type of operands is not considered. Since `'2'` is converted to `2`, the check returns `true`. 
- D. `false`. This is a strict equality check, where the type of operand matters. Since `'2'` is not the same type as `2`, the check returns `false`. 
- E. `false`. The operand `true` is converted to `1` but since 1 does not equal 2, the check returns `false`. 
- F. `true`. The Boolean wrapper converts any "empty" values (such as empty string, 0, null, undefined) to `false` and any "non-empty" values (such as 'hello', 1) to `true`. Since `Boolean(2)` is evaluated as `true`, then we pass the check `true === true` and return `true`. \
Question 15: As stated above, the `==` operator checks if the numerical values are the same but does not consider type, whereas the `===` operator checks for both value and type. \
Question 16: See code \
Question 17: `[2, 4, 6]`. Essentially, every time the for loop increments, the doSomething function is called on the element at the current index. The value returned by the function is then pushed into the newArr. \
Question 18: See code \
Question 19: `1 \n 4 \n 3 \n 2`