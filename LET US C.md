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





