# Ex.No: 6   Logic Programming – Factorial of number   
### DATE: 18-03-24                                                                            
### REGISTER NUMBER : 212221040080
### AIM: 
To  write  a logic program  to solve Towers of Hanoi problem  using SWI-PROLOG. 
### Algorithm:
1. Start the program
2.  Write a rules for finding solution of Towers of Hanoi in SWI-PROLOG.
3.  a )	If only one disk  => Move disk from X to Y.
4.  b)	If Number of disk greater than 0 then
5.        i)	Move  N-1 disks from X to Z.
6.        ii)	Move  Nth disk from X to Y
7.        iii)	Move  N-1 disks from Y to X.
8. Run the program  to find answer of  query.

### Program:
```
hanoi(1, X, Y) :-
    write('Move disk from '),
    write(X),
    write(' to '),
    write(Y),
    nl.
hanoi(N, X, Y) :-
    N > 1,
    N1 is N - 1,
    hanoi(N1, X, Z),
    hanoi(1, X, Y),
    hanoi(N1, Z, Y).
```

### Output:

![Screenshot (204)](https://github.com/KayyuruTharani/AI_Lab_2023-24/assets/142209319/10dc6356-8c61-44a0-b16f-3a1f9bc214b9)



### Result:
Thus the solution of Towers of Hanoi problem was found by logic programming.
