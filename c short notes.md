# CHAPTER 1
In 1970 a programmer,Dennis Ritchie,created a new language called c.
(a)The name came about because it superseded the old programming language he was using : B.
(b)C was designed with one goal in mind: writing operating systems.
(c)The language was extremely simple and flexible, and soon was used for many different types of programs.
(d)It quickly became one of the most popular programming languages in the world.

STRUCTURE OF C PROGRAM 
(a)C is a case sensitive language.
(b)C Program consist of one or more functions.
(c)One function that must be present in every C program is main(). This is the 1st function called up when program execution begins.

C program basically consists of the following parts:
Preprocessor Commands
Functions
Variables
Statements & Expressions
Comments

let us write a c program to print HELLO WORLD
#include<stdio.h>
int main()
{
printf("hello world")
return 0;
}

VARIABLE 
Variable in C programming is called as container to store the data
there are two types of variable:
(a)local Variables:local variable is variable having local scope.

(b)Global variables:global variable is a Variable that is globally available
RULES FOR VARIABLE NAME
Characters allowed : Underscore(_), Capital Letters ( A - Z ), Small Letters ( a - z ), and Digits ( 0 - 9 ).
Blank spaces and commas are not allowed.
No Special Symbols other than underscore(_) are allowed.
First Character should be alphabet or Underscore.
Variable name Should not be Reserved Keywords.
KEYWORDS
Keywords are reserved words which have standard, predefined meaning in C. They cannot be used as program-defined identifiers

*Generally all keywords are in lower case although uppercase of same names can be used as identifiers.

List of C keywords are as follows :

char int long union continue goto while if double enum const for sizeof do else struct register float signed volatile typedef switch break extern short void auto case static return unsigned default
DATA TYPES
DataTypes are used for declaring variables And functions of different types.
When Program store data in variables, It is necessary that each variable must be assigned a specific data type.

# CHAPTER 2
It is used to execute an instruction or sequence / block of instruction only if condition is fulfilled. if statement, expression is evaluated first and then, depending on whether the value of the expression (relation or condition) is true or false, transfers the control to the particular statement or group of statements.

Different forms of implementation of if-statement are :

Simple if statement
if-else statement
Nested if-else statement
Else if statement

(a)[Simple if statement]

This is used to executed the statements only if the condition is true.

Syntax :

    if(condition)
    {
        block of statement;
    }
(b) [If..else statement] is used when different block of statement is to be executed on condition true and false.

Syntax :


    if(condition)
    {
        block 1 of statement;
    }
    else
    {
        block 2 of statement;
    }
if condition is true then block 1 statement will be executed and if condition is false block 2 statement will execute.
(c) to show a multi-way decision based on several conditions, we use the [else if statement.]

Syntax :

 if(condition_2)
 {
    block 1 statement;
 }
 else if (condition_2)
 {
    block 2 statement;
 }
 else if(condition_n)
 {
    block n statement;
 }
 else
 {
    block x statement;
 }

here, the conditions are evaluated in order from top to bottom. As soon as any condition evaluates to true, then statement associated with the given condition is executed and if all condition are false, then control is transferred to statement_x skipping the rest of the condition.
(d) [nested if else]
 You can combine multiple if / if-else / if-else-if ladders when a series of decisions are involved. So you can make sure that your program executes certain instructions when a series of conditions are met.

Some use case :

1.
    

    if(condition)
    {
        //block of statement

        if(condition)
        {
            //block of statement
        }
    }
    


2.
    

    if(condition)
    {
        //black of statement
    }
    else
    {

        if(condition)
        {
            //block of statement
        }
        else
        {
            //block of statement
        }

    }
    


3.
    

    if(condition)
    {
        //black of statement
    }
    else if(condition)
    {

        if(condition)
        {
            //block of s…

  
# CHAPTER 3
  LOOP 
  (a)[for loop]
  oops are used to repeat a block of code.

Syntax of for Loop :

 for (init; condition; increment)
 {
    // block of statement.
 }
   (c) [while loop]
 while loop statement in C programming language repeatedly executes a target statement as long as a given condition is true.

Syntax :


while( condition )
{
    statement(s);
}
    (c)[do-while loop]
 A do-while loop is similar to a while loop, except that a do-while loop is guaranteed to execute at least one time. The conditional expression appears at the end of the loop, so the statement(s) in the loop execute once before the condition is tested.

Syntax :


do
{
    statement(s);
} while( condition );


# CHAPTER 4
switch statements are also used when we need our program to make a certain decision based on a condition and then execute accordingly.

Syntax :


switch (<variable>)
{
    case a-constant-expression :
        //Code to execute if <variable> == a-constant-expression
        break;

    case b-constant-expression  :
        //Code to execute if <variable> == b-constant-expression
        break;
    .
    .
    .
    case n-constant-expression :
        //Code to execute if <variable> == n-constant-expression
        break;

    default:
        //Code to execute if <variable> does not equal the value following any of the cases
}
    [break keyword]

break statement neglect the statement after it and exit compound statement. in the loop and transfer the control outside the loop

Break it's sole purpose to passes control out of the compound statement i.e. Loop, Condition, Method or Procedures.

Example :


while(a)
{
    while(b)
    {
        if(b == 10)
        {
            break;
        }
    }
    // break will bring us here.
}

continue keyword

Similar,To break statement continue statement also neglect the statement after it in the loop and send control back to starting point of loop for next iteration instead of outside the loop
    
# CHAPTER 5
 FUNCTIONS
    A function is a block of statements, which is used to perform a specific task.
A C program has at least one function named main().

Types of functions :

There are two types of function in C

Library function
User defined function

Library Function :

Library functions are the built-in function in C such as puts(), gets(), printf(), scanf() etc. These are the functions which already have a definition in header files.


User defined function :

C allows programmer to define their own function according to their requirement.


Syntax of function :

return_type function_name (argument list)
{
    Block of code
}
return_type : return types are the type of data that is returned by the function. If nothing is returned then the return type is void.

argument list : argument list contains variables names along with their data types. These arguments are inputs for the function.


Syntax :


#include <stdio.h>

void function_name()
{
    //code
}

int main()
{
    //Calling function
    function_name();
}
    
    
    # POINTER
    Pointer is a variable that points to an address of a value.
     Pointer => address that contains the value


Symbols used in pointer :

& (ampersand sign) : ‘Address of operator’. It determines the address of a variable.

* (asterisk sign) : indirection operator / value at address. Accesses the value at the address.

Example :


int i = 3 ;

This declaration tells the C compiler to :-

Reserve space in memory to hold the integer value.
Associate the name i with this memory location.
Store the value 3 at this location.

We may represent the location of i in the memory by :-
 Syntax :


datatype *variable_name
    WAYS TO DECLARE POINTER:-
 Here, i, ch and f are declared as pointer variables, i.e.variables capable of holding addresses.
Remember that, addresses are always going to be whole numbers, therefore pointers always contain whole numbers.
Now we can put these two facts together and say that the pointers are variables that contain addresses, and since addresses are always whole numbers, pointers would always contain whole numbers.
The declaration float *f does not mean that f is going to contain a floating-point value. What it means is, f is going to contain the address of a floating-point value.
Similarly, char *ch means that ch is going to contain the address of a char value.




