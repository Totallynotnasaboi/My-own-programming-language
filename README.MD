# BASIC ++ (By NASA BOI on YouTube)
This is my very own version of Microsoft BASIC completely rewritten in python.
### Table of contents
* Installation
* Basic usage
* Features and syntax
* File and scripts type

#### Installation
You can install the package via the realeses section (WIP).
There will be packages for debian, arch (also through the AUR) and hopefully Windows!
I will also try to develop a vs-code extension.
If you dont want to wait you can simply run the basic++ python file (you will need python installed)

#### Basic usage
If you installed a package, just run basic++ in the terminal. 
Otherwise just run the python file in the terminal.
You can run your script like this:
```Bash
$ basic++ >> RUN("FILENAME")
```
Otherwise you can write directly on the console, like BASIC.

#### Features
The program has very few features but here's them all:

1. You can add a variable with VAR command. Example:
```Bash
VAR varname = value;
VAR a = 8;
```
2. You can print something with print command:
```Bash
PRINT("Hello World");
```
3. You can add a while loop like this:
```Bash
WHILE True THEN
    PRINT("Infinite Loop");
END
```
4. You can easily add a comment:
```Bash
# This is a comment
```
5. You can add a IF and ELIF statement:
```Bash
IF VAR a = 9 THEN 
    PRINT("A eqauls nine");
ELIF VAR a != 9 THEN
    PRINT("A does not equal nine");
END
```
6. You can add a for loop:
```Bash
FOR i = 0 TO 10 THEN
    PRINT(i);
    i == i + 1
END
```
7. There are many built in functions like:
```
PRINT: prints something
INPUT: takes the user input (works only in empty parenthesis, unlike python)
RUN: runs a file
BREAK: breaks a loop
END: ends the loop/function
CONTINUE: skips a part of the program (like loop through this and this but skip the fourth loop )
RETURN: returns a value
```
Example of return:
```Bash
FUN test()
    VAR num = 5
    RETURN num
END
```
The output will be:
```Bash
test()
$ basic++ >> 5
```

8. You can also create your own functions:
```Bash
FUN test(a, b) -> a + b;
```
the command and output will be:
```Bash
test(3, 6)
$ basic++ >> 9
```

#### Sintax
The sintax is kinda confusing so lets get going.

###### Basic sintax: You need to close lines with a semicolon. if you use the terminal you can terminate lines with the semicolon and a space like this:
```Bash
$ basic++ >> IF i = 9 THEN; PRINT("Test"); PRINT("This is on a new line");
```

We have covered variables and function.

1. Arrays:

You can work with arrays the same you do with other languages. here are some examples:
```Bash
VAR array1 = [1, 2, 3];
VAR primeNums = [1, 2, 3, 5, 7];
```
```Bash
VAR array1 = array1 + 4
```
The output will be:
```Bash
$ basic++ >> [1, 2, 3, 4]
```
If you use multiply...
```Bash
VAR primeNums * [11, 13, 17];
```
...The output will be:
```Bash
$ basic++ >> [1, 2, 3, 5, 7, 11, 13, 17]
```
2. If statements

You can use variables like:
```Bash
IF VAR i = 9 THEN
    PRINT("I is nine");
END
```

1. For loops

In a for loop you can use undefined keywords:
```Bash
FOR i = 0 TO 10 THEN
    # this loops 10 times
    #i is not a variable
    PRINT("loop");
END
```
In a while loop you use variables like this:
```Bash
VAR a = 0;
WHILE VAR a < 10 THEN
    # Loops 10 times
    PRINT(a);
    VAR a == a + 1;
END
```
##### All the expression like loops and ifs finish with a END!

#### File types
Any file extension will work, but the official file extension is .BPP