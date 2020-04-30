# Document the code snippets

## Milestone 1: Introduction

### Variables should be defined before being used in body.
For example,
```
global str, evenList
```
#

### Using write()/read() to output/input string.

#

### Using := to assign a value to a variable.
For example,
```
str := "Welcome to icon language"
```
#

### Using L1 ||| L2 to do list concatenation.
For example,
```
evenList := []
evenList := evenList ||| [1]
```
Then, the value of evenList should be [1]
#

### String scanning uses “move(i)” and “n ? expr”, where i represents the step we move at the string, n represents the string, expr represents the function.
For example,
```
n ? {
        while i := move(1) do
            if (i % 2 == 0) then evenList := evenList ||| [i]
    } 
```
This program is to find even numbers in a string and add them to a list.

## Milestone 2: Control Structures

### Icons control structures are similar to most other languages
Conditional control structures involve switches and if statements
The struction for if statements go "if ... then... (if needed)else...
Example for if/then/else,
```
if n~=3 then write ("same") 
else write ("different")
```
switch cases can be used in times where there maybe a lot of if else statements
```
i=2
case i of{
0       :write("zero")
1       :write("one")
2       :write("two")
}
```
There are 2 main loops in icon the "while" loop and the "until" loop
while loops acts as expected you just need to add "do" at the end of the condition.
Example of a while loop in icon,
```
x=1
while x < 5 do{
        write(x)
        x:=x+1
}
```
until loops are somewhat similar to while loops except that until goes until the expression is met where as a while loop goes until the expression fails.
```
x=10
until x < 5 do {
        write(x)
        x:=x-1
}
```

## Milestone 3: Data Types

### Totally, there are 12 types.
|Types|   |    |    |
| :---: | :---: | :---: | :---: |
|null(n)    |     string(s) | co-expression(C) | table(T)|
|integer(i)  |    cset(c)  |  procedure(p)    |  set(S)|
|real(r)    |     file(f)   | list(L)         |  record types(R)|

The code snippets in M3 show the characters and functions of each type. 

## Milestone 4: Subprogram

### (1) Use $include to link the functions in other icon files

### (2) Use record as the struct in C programming language

In p4_count.ico, we used **procedure** and **record** as subprograms to help the main program to process or store the data.

## Milestone 5: End

### (1) GOAL-DIRECTED EVALUATION'

Usage:
```
if find(target, str) > num then ... else ... 
```
It is used to check if there is a target after num(th) position in str.


### (2) EXCHANGING

Usage:
```
s1 :=: s2
```
It will exchange the value of s1 and s2.

In this case, we don't need to use a new variable to store the temp value.

### (3) TRACE

Usage:
```
&trace := n 
```
where n represents the times you want to trace.

The output is listed below

```
$ make p5_trace
icon p5_trace.ico
p5_trace.ico :    6  | fib(5)
p5_trace.ico :   12  | | fib(4)
p5_trace.ico :   12  | | | fib(3)
p5_trace.ico :   12  | | | | fib(2)
p5_trace.ico :   12  | | | | | fib(1)
p5_trace.ico :   11  | | | | | fib returned 1
p5_trace.ico :   12  | | | | | fib(0)
p5_trace.ico :   11  | | | | | fib returned 0
p5_trace.ico :   12  | | | | fib returned 1
p5_trace.ico :   12  | | | | fib(1)
p5_trace.ico :   11  | | | | fib returned 1
p5_trace.ico :   12  | | | fib returned 2
p5_trace.ico :   12  | | | fib(2)
p5_trace.ico :   12  | | | | fib(1)
p5_trace.ico :   11  | | | | fib returned 1
p5_trace.ico :   12  | | | | fib(0)

... ...
```

#END