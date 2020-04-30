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
#

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
#

## Milestone 3: Data Types

### Totally, there are 12 types.
|Types|   |    |    |
|----|----|----|----|
|null(n)    |     string(s) | co-expression(C) | table(T)|
|integer(i)  |    cset(c)  |  procedure(p)    |  set(S)|
|real(r)    |     file(f)   | list(L)         |  record types(R)|



