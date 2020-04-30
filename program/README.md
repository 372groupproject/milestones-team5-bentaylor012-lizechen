# Final Project Description

## 1. Getting Started

There are two ways to running icon files.

### 1.1. icon *.ico (Makefile)

Run the project by typing "make" in this directory.

### 1.2. icont *.icn

If we want to use **icont** command, we just need to modify all \*.ico to \*.icn.

Also, remember to modify **$include "\*.ico"** to **$include "\*.icn"** in program.icn

Then run command "icont program.icn", and an executable file will be built.

## 2. Purpose

Our goal is to compute the shortest distance between two cities via Dijkstra's algorithm. 

### 2.1. Input

(1) Input File Format: 

```
name1 name2 distance
```
where **name1** and **name2** are strings and **distance** is a non-negative integer.

e.g. 
```
tucson albuquerque 318
chandler tucson 95
elPaso tucson 262
tucson phoenix 116
phoenix flagstaff 117
yuma elPaso 481
phoenix yuma 159
tucson yuma 220
lasCruces tucson 242
lasCruces elPaso 38
chandler phoenix 21
lasCruces santafe 285
santafe albuquerque 54
```

(2) User Input Format: 

```
name1 name2
```

### 2.2. Output

The minimum distance between these two cities.

## 3. Details

### 3.1. Files

There are three .ico files named **program.ico**, **processData.ico**, **dijkstra.ico**, and one .txt file named **graph.txt**.

### 3.2. Functions

(1) **program.ico**: the main program which inputs and outputs.

(2) **processData.ico**: build the linkedlist based on the inputs.

(3) **dijkstra.ico**: apply the algorithm.

### 3.3. Shining Points

(1) string-scanning: the shortcut to extract the useful elements in a string

(2) avoid memory allocation: more efficient than C programming language








