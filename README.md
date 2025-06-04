# COMPILER-DESIGN-BASICS

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: RAVI PRABHA

*INTERN ID*: CT04DN1602

*DOMAIN*: C PROGRAMMING

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTHOSH 

## (The lexical analyzer program written in the C programming language is a fundamental example of how compilers begin the process of understanding source code. It focuses on the first stage of compilation known as lexical analysis, where the source code is read character by character and broken into meaningful sequences called tokens. These tokens are then categorized into keywords, identifiers, and operators, which are essential components of any programming language.

The program begins with the inclusion of necessary header files such as <stdio.h>, <string.h>, <ctype.h>, and <stdlib.h>. These libraries support input/output operations, string manipulation, character testing (like checking if a character is a letter or digit), and standard utility functions.

Next, a small set of keywords is declared in a 2D character array. These are reserved words in the C language like int, float, if, else, while, return, and char. The function isKeyword() checks if a given word matches any of these predefined keywords. It uses a simple for loop and the strcmp() function to compare the input word with each keyword.

Similarly, the function isOperator() checks if a character is a valid operator. It returns true if the character is one of the standard arithmetic or relational operators such as +, -, *, /, =, <, or >.

In the main() function, the program opens a file named input.txt which contains the source code to be analyzed. It checks if the file exists and handles the case where it doesn’t by displaying an error message and exiting the program.

The core logic of the lexical analyzer lies in reading the file character by character using fgetc(). A buffer is used to collect sequences of alphanumeric characters which potentially form identifiers or keywords. Whenever the program encounters a non-alphanumeric character such as whitespace or an operator, it terminates the current word in the buffer and checks whether it is a keyword using the isKeyword() function. If not, it assumes it is an identifier (such as a variable name or a numeric constant).

If the current character is an operator, it is printed as an operator immediately. This separation of operators from identifiers is crucial because in real programming code, they often appear adjacent to each other without spaces.

This process continues until the end of the file. At each step, the program prints the type and value of each token it identifies. The output provides a clear understanding of which parts of the code are keywords, which are identifiers, and which are operators.

In essence, this program demonstrates the basics of how source code is scanned and broken into parts during compilation. Though simplified, it reflects how real compilers function internally. It can be further extended to detect numbers, delimiters (like semicolons and brackets), and comments, or even to handle more complex token patterns using regular expressions or finite automata.

Overall, this lexical analyzer serves as an excellent learning tool for beginners in compiler design and helps them visualize how programming languages are interpreted by machines).

#OUTPUT
![Image](https://github.com/user-attachments/assets/0795bc3a-7c9e-48ea-b8dd-7e028a86bb2c)
