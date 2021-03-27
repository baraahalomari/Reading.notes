## Comparision operators:

we can comparing one value to what we expect it might be, and this result called Boolean it will be true or false.
Example of operator
== is equal to : we use this operator to compares two values to see if they are the same.
=== strict equal to : to check that both the data type and value are the same.
!= is not equal to :we use this operator to compares two values to see if they are not the same.
!== strict not equal to : to check that both the data type and value are not the same.
> greater than : to checks if the number on the left is greater than the number on the right.
< less than : to checks if the number on the left is less than the number on the right.
>= greater than or equal to : to checks if the number on the left is greater than or equal to the number on the right.
<= less than or equal to : to checks if the number on the left is less than or equal to the number on the right.

## Logical operators :

the diferant betwen comparision operators and logical operators that logical operators allow you to compare the results of more than one comparision operator>
Example of logical operator:
&& logical and : to test more than one condition.
|| logical or :to test at least one condition.
! logical not : this operator takes a single boolean value and inverts it.

## Loops :
a way to run the code seviral times.

Types of loops:
for loop : to run code a specific number of times.
which uses a counter as a condition 
   for ( var i = 0; i < 5; i++ ) {
           document.write (i);
        }

while loop : if you don't know how many times the code should run 
this loop will continue to run for as long as condition in the parentheses is true.
      while (i < 5) {
      document.write (i) ;
        i++;
       }