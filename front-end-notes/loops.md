#JavaScript Loops

##JavaScript supports different kinds of loops:

###for - loops through a block of code a number of times

```
for (statement 1; statement 2; statement 3) {
    code block to be executed
}
```
####Statement 1:
  ```
  for (*var i = 0*; statement 2; statement 3) { 
    code block to be executed
  }
  ```

  Normally you will use statement 1 to initiate the variable used in the loop (i = 0).

  This is not always the case, JavaScript doesn't care. Statement 1 is optional.

  You can initiate many values in statement 1 (separated by comma).

  ####Statement 2:
  ```
  for (var i = 0; *i<10*; statement 3) { 
    code block to be executed
  }

  Often statement 2 is used to evaluate the condition of the initial variable.

  This is not always the case, JavaScript doesn't care. Statement 2 is also optional.

  If statement 2 returns true, the loop will start over again, if it returns false, the loop will end.

  If statement 2 is omitted, a break statement must be added or an infinite loop will follow.

####Statement 3:

Often statement 3 increases the initial variable.

This is not always the case, JavaScript doesn't care, and statement 3 is optional.

Statement 3 can do anything like negative increment (i--), positive increment (i = i + 15), or anything else.

Statement 3 can also be omitted (like when you increment your values inside the loop)





###for/in - loops through the properties of an object

```
var wordObj= {
  word1: "Jesus",
  word2: "Loves",
  word3: "You"
}

for (statement 1 in statement 2) {
    code block to be executed
}
```

####Statement 1:

```
var wordObj= {
  word1: "Jesus",
  word2: "Loves",
  word3: "You"
}

for (*myArbitrayWord* in statement 2) {
    code block to be executed
}
```

  Statement 1 is an arbitray word used to represent a value at each key location in the specified object.

####Statement 2: 

```
var wordObj= {
  word1: "Jesus",
  word2: "Loves",
  word3: "You"
}

for (myArbitrayWord in wordObj) {
    code block to be executed
}
```

  Statement 2 is the name of the object you wish to loop over. 




###while and do/while - loops through a block of code while a specified condition is true

```
while(statement 1){
  code to be executed
}
```

####Statement 1:

```
while(*true*){
  code to be executed
  break statement: break;
}
```

Whenever statement one is false the loop will break. The difference between while and do/while is a while loop will excute only when Statement 1 is true, and a do/while will execute atleast once and then continue to execute until Statement 1 is evaluated to false.