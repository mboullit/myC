# myC
The purpose of the compilation project is to create a compiler from a mini language called myC to C code with 3 addresses. The proposed source language, a mini C-style language (note, there are some variants compared to the standard C), will therefore have to be compiled into C with 3 addresses. 

## Compilation Project:
This is the depository of the compilation project, welcome !
We managed to do all the 6 tasks :  
    1- un mécanisme de déclarations explicite de variables  
    2- des expresssion arithmétiques arbitraire de type calculatrice  
    3- des lectures ou écritures mémoires via des affectations avec variables utilisateurs ou pointeurs  
    4- des structures de contrôles classiques (conditionelles et boucles)  
    5- un mécanisme de typage simple comprenant notamment des entiers int et des pointeurs int *  
    6- définitions et appels de fonctions récursives  
And we have tried to minimize any memory loss, to the best of our effort, by freeing symbols at the end of every block and freeing their names ...

## Our team 
** Contributors :** Ismail Elomari Alaoui , Boullit Mohamed Fayçal.

## Project description
*This deposit contains 2 folders :*

    - tst : contains test.myc, the file on which we're testing our language analysis, and when compiled, files "tst/test.[ch]".  
    - src : contains source files for our language myc and other C source files.  

*This deposit contains 2 files :*

    - Makefile: used to compile and execute our project (Process is explained in the next section).  
    - compil.sh: It's a bash script, taking for an argument a file to test our language on (tst/test.myc for example), producing files "tst/test.[ch]" and an executable test.  

*The execution :*

    - The command "make" compiles the source files necessary to create a compiler (an executable myc).  
    - The command "make test" uses the file "compil.sh" in order to execute our compiler on the file tst/test.myc. This creates files "tst/test.c" and "tst/test.h" and excutes them.  
    - The command "make clean" cleans the deposit from any executables, and deletes "tst/test.[ch]".
