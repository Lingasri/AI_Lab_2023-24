# Ex.No: 7  Logic Programming –  Logic Circuit Design
### DATE: 16/03/2024                                                                           
### REGISTER NUMBER : 212221040089
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
```
xor(0,1,1).
xor(0,0,0).
xor(1,0,1).
xor(1,1,0).
and(1,1,1).
and(0,0,0).
and(0,1,0).
and(1,0,0).
not(0,1).
not(1,0).
or(0,1,1).
or(1,0,1).
or(0,0,0).
or(1,1,1).
halfadder(A,B,Sum,Carry):-
    xor(A,B,Sum),
    and(A,B,Carry).
halfsubtractor(A,B,Diff,Carry):-
    xor(A,B,Diff),
    not(A,C),
    and(C,B,Carry).
fulladder(A,B,Cin,S,Cout):-
    xor(A,B,X),
    xor(X,Cin,S),
    and(X,Cin,Y),
    and(A,B,Z),
    or(Y,Z,Cout).
```











### Output:

![WhatsApp Image 2024-03-23 at 11 44 51_ed227d0e](https://github.com/Lingasri/AI_Lab_2023-24/assets/143391929/91266c9b-a2fd-4f63-8fdf-f959b8590142)

![WhatsApp Image 2024-03-23 at 11 45 58_7f7d431f](https://github.com/Lingasri/AI_Lab_2023-24/assets/143391929/3f32e468-8167-4e48-95ef-a9c4bf479e50)

![WhatsApp Image 2024-03-23 at 11 46 24_d2775813](https://github.com/Lingasri/AI_Lab_2023-24/assets/143391929/f30855ce-4a62-486c-bc06-69d583eb8ad8)








### Result:
Thus the truth table of circuit verified sucessfully.
