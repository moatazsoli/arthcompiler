// Moataz Soliman

This compiler is written in SCHEME , 
See running instructions at the bottom .

**Scheme is a functional programming language and one of the two main types of the programming language Lisp.

This is a compiler written in SCHEME , for arithmetic expressions of the form:
<op operand1 operand2>
where op is either +, -, *, or / and the operands are either numbers or nested expressions. 


It is assumed that the target machine has instructions:
(move value register)
(add register-1 register-2)
(subtract register-1 register-2)
(times register-1 register-2)
(divide register-1 register-2)

All arithmetic operations will leave the result in the 1st register argument.

An example of a legal expression
is (* (+ 3 6) (- 7 9)). and the result is :

move 3 register-1
move 6 register-2
add register-1 register-2
move 7 register-3
move 9 register-4
subtract register-3 register-4
times register-1 register-3
----------------------------------------------------
****************** Running instrustions ******************

Step 1: install DrRacket.
Step 2: Choose the language "pretty big" under the Language menu item.
Step 3: open the .rkt file of the arithmatic compiler.
Step 4: Run the definition window using the run button at the top right.
Step 5: Enter the operation for compiling.
**THE RUN BUTTON HAS TO BE PRESSED EVERYTIME A COMPILATION IS NEEDED