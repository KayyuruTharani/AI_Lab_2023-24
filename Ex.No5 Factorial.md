# Ex.No: 5   Logic Programming – Factorial of number   
### DATE:18-03-2024                                                                            
### REGISTER NUMBER : 212221040080
### AIM: 
To  write  a logic program for finding the factorial of given number using SWI-PROLOG. 
### Algorithm:
1. STEP 1: Start the program
2. STEP 2:  Write a rules for finding factorial of given program in SWI-PROLOG.
3.   a)	factorial of 0 is 1 => written as factorial(0,1).
4.   b)	factorial of number greater than 0 obtained by recursively calling the factorial    function.
5. STEP 3: Run the program  to find answer of  query.
6. STEP 4: Stop the program.

### Program:
```
factorial(0, 1).
factorial(N, Result) :-
    N > 0,
    N1 is N - 1,
    factorial(N1, Result1),
    Result is N * Result1.

```

### Output:

![Screenshot (203)](https://github.com/KayyuruTharani/AI_Lab_2023-24/assets/142209319/6cca7d2e-6545-4fe0-b3e9-dce78ea50553)


### Result:
Thus the factorial of given number was found by logic programming. 
