Intermediate Code Generation for Control Flow Statements in a Compiler.

Project Overview

This project focuses on generating intermediate code for control flow statements, 
specifically if-else conditions and basic arithmetic operations, as part of a simplified compiler design.
The goal is to translate high-level source code into an intermediate representation,
such as three-address code (TAC), which can later be converted into assembly or machine code.
This process is crucial for building compilers that optimize and manage the flow of execution in programs.

How It Works

Input: The project takes a small piece of source code containing an if-else statement and basic operations as input.
Lexical Analysis: The code is first tokenized into meaningful components such as keywords (if, else), identifiers (e.g., a, b, c), and operators (<, +).
Intermediate Code Generation: The token stream is processed to generate TAC that represents the logical flow and operations in a simplified form.
Output: The final output is a series of TAC instructions, which represent the control flow and assignments in the source code.

Example
Input Source Code:
if (a < b) {
      c = c + 1;
    }
else {
       exit;
      }

Generated Intermediate Code:
IF a < b GOTO L1
GOTO L2
L1:
T1 = c
T1 = T1 + 1
c = T1
GOTO END_IF
L2:
EXIT
END_IF:


Thank you for checking out this project!
