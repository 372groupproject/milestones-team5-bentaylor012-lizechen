# Document the code snippets

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
### There are two main control structures for icon. If/then/else statements and While loops
