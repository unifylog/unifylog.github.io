---
layout: post
title: "Fit XT CSV Import"
date: 2015-09-06 15:11:03 -0700
comments: true
categories: 
- Fit XT
- 90Droid
- FAQ
---
We have introduced the ability to import CSV files, here we describe the expected format.

CSV stands for Comma Separated Values. A CSV file is a plain text file that contains columns separated by commas and every new line corresponds to a row. 

Every file defines one and only one Exercise Program.
For every *Program* you must define *Days*, *Exercise Groups* and *Exercises* in that order. 
The number of columns varies depending according to the rules defined below.

## Comments
A line that starts with `#,` is considered a comment and hence ignored. Exaple:

```
#,"This is a comment line, it starts with #, and the rest is ignored"
```

## Exercise Program 
*There can only be one per file* 
### Columns
PROGRAM, Name, Notes
### Example
``` 
"PROGRAM","90 day Classic","Program Notes"
```
## Days
There can be multiple in the file. Order of appearance is important
### Columns
DAY,Exercise Group Name1, Exercise Group Name 2,...
### Example
```
"DAY","Chest","Abs"
```

## Exercise Groups
There can be multiple in the file. Order of appearance is important
### Columns
GROUP, Group Name, Group Notes,Exercise Name1, Exercise Name 2,...

### Examples
```
"GROUP","Chest","Sample Import Group","Push-ups","Pull-ups","Curls"
"GROUP","Abs",,"Uphill Bicycle","Crunches"
```

## Exercises 
There can be multiple in the file. Order of appearance is important
### Columns
EXERCISE, Exercise Name, Exercise Notes,Exercise Type (C=Cardio,R=Reps,RW=Reps and Weight,T=Count down timer,SW=Stop Watch), Duration, Youtube video Id, Youtube video duration, Youtube video start time

### Example
```
"EXERCISE","Push-ups",,"R","0",,"0","0"
"EXERCISE","Pull-ups",,"R","0",,"0","0"
"EXERCISE","Curls",,"RW","0",,"0","0"
"EXERCISE","Uphill Bicycle",,"R","0",,"0","0"
"EXERCISE","Crunches",,"R","0",,"0","0"
```

#Template
[Download](https://drive.google.com/uc?export=download&id=0B2Gx0PNDQPS8Tm1RWGVZc1h5LTQ)

Here is an example by [Vasco B.](https://plus.google.com/107240213889695247387 "Google Plus Profile") 
[Download](https://drive.google.com/uc?export=download&id=0B6mU0S1ofGyNd0FpdHZUalEzWXM)