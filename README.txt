MYLANG v2
____________________________________________________________________________________________________________________________
Language Description: 

> Has comments using a single # symbol at the start of the comment(single lined comments).
> Has integer and floating point variables.
> Variables start with a lower case letter and always followed by exactly 2 decimal numbers. For example a11. The variables are all numeric type variables. If they start with a to n, they are treated as signed integer variables by default. For variables starting from o to z, are by default double precision floating points variables. 
> The language has arithmetic propagation, binary operators( +, -, *, / and also exponential)
> The first 4 are left associative, exponential is right associative a^b^c = a^(b^c)
> precedence: exp, (*,/), (+,-)
> Mixed mode expression will happen as C
> Automatic type conversion to one to which it is assigned. 
> Has if and if else like in C and also has a while loop like in C. 
> All the comparison operators from C are there <,>, ≥ etc.
> Has a print statement called "display" 
> {} Is present in the beginning and end of the entire program. 
> ; is the statement Terminator. 
____________________________________________________________________________________________________________________________

How to run the code: (prerequisites : gcc, flex and bison installed on the target device)

The repository comes with the a.exe file but if you want to build one on your machine you need to follow the given steps (for windows terminal, popwershell, linux and mac will be different):

bison -d mylang.y && flex mylang.l mylang.tab.h && gcc mylangInterpreter.c lex.yy.c mylang.tab.c

The repository also contains 5 sample programs to test the compiler with, use the following commands in the command prompt to run the codes. 

a.exe < printPrimes.txt
a.exe < printEven.txt
a.exe < calculateSI.txt
a.exe < fizzbuzz.txt
a.exe < leapyear.txt
____________________________________________________________________________________________________________________________
Thanks for reading!