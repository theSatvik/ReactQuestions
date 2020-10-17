// Author - Satvik Shrivas

Difference Between var , let and const with examples -

First and foremost all of the above mentioned keywords are nothing but are used
to declare and define JavaScript variables. 

1.var - 

---> "var" is used to clear any type of datatype such as integer , floating point values , boolean , object , array , string ,etc.
--->The scope of a JavaScript variable declared outside the function is global.
---> The scope of javaScript variable declared by the means of "var" is its current execution context or
     on the whole document which means the identifier or keyword used to declare the current variable cannot be again declared .
    
     For example : 
            //Program - 1
            var a=10;
            var b=20;
            var c=a+b;
            //now our program 1 is completed 
             
            // Program - 2 
            var a=40;
            // this will generated an error as a is declared globally
                
2. let : -

--->The let statement declares a local variable in a block scope.
 It is similar to var, in that we can optionally initialize the variable.

--->The let statement allows you to create a variable with the scope limited to the block on which it is used.
--->It is similar to the variable we declare in other languages like Java, .NET, etc.

 For example - 
  let a=10 ;
    {
       let a=35;
       let a=33;
       console.log(a);
    }
  
  console.log(a);

//output
 --> 33
 --> 10

3.const : -
-->const statement values can be assigned once and they cannot be reassigned.
 The scope of const statement works similar to let statements.

for example : 

 const a= 10;
 a=25 ;    //Error Message : Uncaught TypeError: Assignment to constant variable.
   or 
  const a ; //if it is not declared at the time of declaration it will give the same above mentioned error
