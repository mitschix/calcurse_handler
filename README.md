# Script to handle calcurse TODOs

## Description
Little script to handle TODOs in calcurse via the command line. It is possible to query TODOs by a given priority or containing a given string. It is also possible to add a TODO to calcurse with priority, category and description and a note. Furthermore it is possible to add a file containing multiple TODOs.

Priority goes from 1 to 9 highest to lowest - 0 is no priority

## TODOs
1. add ids to todos to mark per script

## Requirements
+ calcurse
+ todohandler in $PATH

## Usage
+ add a TODO with priority **1** with category **linux** with description **learn how to use calcurse**
```bash
todohandler -A 1 linux learn how to use calcurse
```
+ search for all TODOs with priority 1
```bash
todohandler -s 1
```
+ search for all TODOs containing string **linux**
```bash
todohandler -S linux
```
+ add a file with multiple TODOs
```bash
cat todos
1 test this is a test
5 test this is another test
0 test another test it is
```

```bash
todohandler -f todos
```
