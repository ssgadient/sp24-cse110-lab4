Question 1: 20
Question 2: 20
Question 3: 20
Question 4: Reference error. Since result is only defined inside the block scope, which is the if/else clause, when the function executes line 13, it doesn't know what result is. 
Question 5: Type error. Since result is declared const, it cannot be modified after, but line 4 attempts to change result, causing nodejs to throw an error. 
Question 6: Type error. Same reason as why it failed in line 9. The code never even reaches line 9 or 13. 