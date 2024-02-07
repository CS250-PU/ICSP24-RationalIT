# CS250 Intro to [ICSP24 - Rational]

## Rational Class Design

<b>Problem:</b> A rational number is defined to be any number that
can be expressed in the form p/q where p and q are each integers and q
is not equal to 0. For this problem, we are only going to consider
non-negative rational numbers (i.e. the numberator can be any whole
number and the denominator can be any natural number)

---
<b>Task #1: </b> Design a UML diagram.

Create a class called **Rational** that has two private data members: **mNumerator** (representing p) and **mDenominator** (representing q). Further, create a **constructor** that accepts two ints (p and q) as parameters. Set the default values of these parameters to 0 and 1 for p and q respectively. The class is to have a **write** function that writes a Rational object (e.g. p/q) to the screen or a file and a **read** function that reads a Rational object (e.g. p/q) from the keyboard or a file. Save the file in uml as **Rational.uxf** and then drag the saved file into the **uml** folder.

---
<b>Task #2: </b> Convert the UML diagram.

Create a file called **Rational.h** that will represent the converted UML diagram. The location for Rational.h is to be in the **include** folder.

---
<b>Task #3: </b> Implament the Rational functions.

Create a file called **Rational.cpp** that is the definitions for the functions in Rational.h. The location for Rational.cpp is to be in the "src" folder.

---
<b>Task #4: </b> Modify main.cpp

In main.cpp you are to add a statement **#include "../include/Rational.h"** after all other #include statements. Then create a Rational object and call **write** which should print out the Rational **0/1**


## Commands

1. Execute without debugging

    * Open a Terminal session
    * Make sure you are in the directory where the Makefile is located
    * Type the command <b>make</b>. If all goes well, you will see something similar to 

      ```
        @ryan2135 ➜ /workspaces/AssignmentT (main) $ make
        mkdir -p bin
        clang++ -g -Wall -std=c++17 -o bin/main.exe src/*.cpp -Iinclude
        ryan2135 ➜ /workspaces/AssignmentT (main) $ 
      ```
    * Type bin/main.exe

2. Debug

    * Set a break point in your program
    * In the VS Code Activity Bar, select the Debug option (triangle)
    * Select the RUN AND DEBUG lldb - debug option

3. Print PDF

    * Open task bar with Ctrl+P
    * Type <b>task</b> in the task bar followed by a space
    * Select printToPDF
    * The pdf will be created in the pdfs directory