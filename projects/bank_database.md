---
layout: project
type: project
image: img/bank_database_logo_square.png
title: "Bank Interface & Database"
date: 2023-10-31
published: true
labels:
  - C Code
summary: "A usable bank interface that is able to acces and modify all bank customers
information within the banks database within C and then C++ (though not included)."
---
## Why A Bank?
<div class="text-center p-4">

This project was made for my 212 project  to create a bank interface that will allow users to add, remove and modify the account information of bank customers. It keeps a separate list file that saves all records in the database to that file before closing the interface allowing it to be accessed again upon startup. The code for this project was written in C and was run on UHUnix systems.

While working on this project I encountered a few problems. I would have to say that the hardest problem I had with this project was ensuring that the text document with all the account information was read and written to and from the text file correctly. The second problem that I had was with the input. I was not able to have it recognize when the string input was being read and correctly. For the longest time there were excess characters that continued to spill over into the next string inputted section but I eventually learned how to fix this problem by increasing the input size and clearing the characters left over from the input.

This project was also comprised of multiple file including:
<br>![image](https://github.com/DavidRickards/DavidRickards.github.io/assets/113159664/c3de7f39-8cb7-491f-ad53-2261db4ba5ea)

Is is an Example of some of the output from a trial run:
```
-_-_--_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_
To select an option please type out the name of the operation below and hit enter:
add      :  Adds a new record into the database.
printall :  Prints all records in the database.
find     :  Prints all records with specified account number.
delete   :  Deletes exsisting record(s) from the database using specified account number.
quit     :  Quits the program.
Command : d

Enter account number to delete below. 
Enter account number: 0

Invalid input given.  Please enter a positive integer as the account number
Enter account number: f

Invalid input given.  Please enter a positive integer as the account number
Enter account number: -3

Invalid input given.  Please enter a positive integer as the account number
Enter account number: 9

Delete unsuccessful. No record found with that account number in database.

-_-_--_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_
To select an option please type out the name of the operation below and hit enter:
add      :  Adds a new record into the database.
printall :  Prints all records in the database.
find     :  Prints all records with specified account number.
delete   :  Deletes exsisting record(s) from the database using specified account number.
quit     :  Quits the program.
Command : d

Enter account number to delete below. 
Enter account number: 1

Delete Complete! All records with given account number have been removed.
```
</div>

 
