# Ex.No: 7  Logic Programming –  Logic Circuit Design
### DATE: 1-04-24                                                                         
### REGISTER NUMBER : 212221040080
### AIM: 
To write a logic program to design a circuit like half adder and half subtractor.
###  Algorithm:
1. Start the Program
2. Design a AND gate logic if both inputs are 1 then output is 1.
3. Design a OR gate logic if any one of input is 1 then output is 1.
4. Design a XOR gate logic if both inputs are different then output is 1.
5. Design a NOT gate logic if input is 0 then output is 1.
6. Design a half adder and half subtractor using the rules.
7. Test the logic.
8. Stop the program.

### Program:

# halfadder
```
half_adder(A, B, Sum, Carry) :-
  xor(A, B, Sum),
  and(A, B, Carry).

xor(0, 0, 0).
xor(0, 1, 1).
xor(1, 0, 1).
xor(1, 1, 0).

and(0, 0, 0).
and(0, 1, 0).
and(1, 0, 0).
and(1, 1, 1).
```
# half Subtractor
```
half_sub(A, B, Dif, Brr) :-
  xor(A, B, Dif),
  not(A, X),
  and(X, B, Brr).

xor(0, 0, 0).
xor(0, 1, 1).
xor(1, 0, 1).
xor(1, 1, 0).

and(0, 0, 0).
and(0, 1, 0).
and(1, 0, 0).
and(1, 1, 1).

not(1, 0).
not(0, 1).
```



### Output:

![Screenshot (364)](https://github.com/KayyuruTharani/AI_Lab_2023-24/assets/142209319/c423af01-5094-4cb2-aa8b-9b4668932bab)

![Screenshot (365)](https://github.com/KayyuruTharani/AI_Lab_2023-24/assets/142209319/3a5c5559-73db-443a-90c2-c2c249a9ead7)



### Result:
Thus the truth table of circuit verified sucessfully.
