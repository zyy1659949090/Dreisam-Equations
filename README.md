# Dreisam-Equations

Dreisam Equations

Description

During excavations in the Dreisamwuste, a desert on some far away and probably uncivilized planet, sheets of paper containing mysterious symbols had been found. After a long investigation, the project scientists have concluded that the symbols might be parts of equations. If this were true, it would be proof that the Dreisamwuste was civilized a long long time ago.
The problem, however, is that the only symbols found on the sheets are digits, parantheses and equality signs. There is strong evidence that the people living in the Dreisamwuste knew only of three arithmetic operations: addition, subtraction, and multiplication. It is also known that the people of the Dreisamwuste did not have prioritization rules for arithmetic operations - they evaluate all terms strictly left to right. For example, for them the term 3 + 3 * 5 would be equal to 30, and not 18.

But currently, the sheets do not contain any arithmetic operators. So if the hypothesis is true, and the numbers on the sheets form equations, then the operators must have faded away over time.

You are the computer expert who is supposed to find out whether the hypothesis is sensible or not. For some given equations (without arithmetic operators) you must find out if there is a possibility to place +, -, and * in the expression, so that it yields a valid equation. For example, on one sheet, the string "18=7 (5 3) 2" has been discovered. Here, one possible solution is "18=7+(5-3)*2". But if there was a sheet containing "5=3 3", then this would mean that the Dreisamwuste people did not mean an equation when writing this.

Input

Each equation to deal with occupies one line in the input. Each line begins with a positive integer (less than 230) followed by an equality sign =. (For your convenience, the Dreisamwuste inhabitants used equations with trivial left sides only.) This is followed by up to 12 positive integers forming the right side of the equation. (The product of these numbers will be less than 230.) There might be some parentheses around groups of one or more numbers. There will be no line containing more than 80 characters. There is no other limit for the amount of the parentheses in the equation. There will always be at least one space or parenthesis between two numbers, otherwise the occurrence of white space is unrestricted.

The line containing only the number 0 terminates the input, it should not be processed.

Output

For each equation, output the line "Equation #n:", where n is the number of the equation. Then, output one line containing a solution to the problem, i. e. the equation with the missing +, -, and * signs inserted. Do not print any white space in the equation.

If there is no way to insert operators to make the equation valid, then output the line "Impossible".

Output one blank line after each test case.

Sample Input

18 = 7 (5 3) 2

30 = 3 3 5

18 = 3 3 5

5 = 3 3

0

Sample Output

Equation #1:

18=7+(5-3)*2

Equation #2:

30=3+3*5

Equation #3:

Impossible

Equation #4:

Impossible

Hint

In case of mutiple answers, output the least one in order (+ < - < *).
