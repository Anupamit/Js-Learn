# Table of Contents

- [Js-Output](#js-output)
- [Js-Programs](#js-programs)
- [Js-Statements](#js-statements)
- [Js-Syntax](#js-syntax)
- [Js-Comment](#js-comment)
- [Js-Variable](#js-variable)
- [Js-Let](#js-let)
- [Js-Const](#js-const)
- [Js-Operators](#js-operators)
- [Js-Datatype](#js-datatype)
- [Js-Function](#js-function)


# Js-output
- JavaScript can "display" data in different ways:
 
      Writing into an HTML element, using innerHTML.
      Writing into the HTML output using document.write().
      Writing into an alert box, using window.alert().
      Writing into the browser console, using console.log().
  
  
# Js-programs
  - A computer program is a list of "instructions" to be "executed" by a computer.
  - In a programming language, these programming instructions are called statements.
  - A JavaScript program is a list of programming statements.


# Js-statements
  - JavaScript statements are composed of: Values, Operators, Expressions, Keywords, and Comments.
  - This statement tells the browser to write "Hello World." inside an HTML element with id="demo".
  
### Semicolons
- Semicolons separate JavaScript statements. 
- Add a semicolon at the end of each executable statement.``` Ex:- let anupam = a + b;```

### White Space
- JavaScript ignores multiple spaces. 
- You can add white space to your script to make it more readable.
- A good practice is to put spaces around operators ```Ex:- ( = + - * / ):```

### Js Keyword
      Keyword:-Description
      var:-Declares a variable
      let:-Declares a block variable
      const:-Declares a block constant
      if:-Marks a block of statements to be executed on a condition
      switch:-Marks a block of statements to be executed in different cases
      for:-Marks a block of statements to be executed in a loop
      function:-Declares a function
      return:-Exits a function
      try:-Implements error handling to a block of statements

# Js-syntax
- JavaScript syntax is the set of rules, how JavaScript programs are constructed.
- The JavaScript syntax defines two types of values:
   - Fixed values (Fixed values are called Literals.)
   - Variable values (Variable values are called Variables.)


### Literals
1. Numbers are written with or without decimals.


       Ex:- 12.3 : 1265
 
2. Strings are text, written within double or single quotes.
 
 
       Ex:- "Anupam Rai" & 'Anupam Rai'
 
### Variables
- In a programming language, variables are used to store data values.
- JavaScript uses the keywords var, let and const to declare variables.
- An equal sign is used to assign values to variables.

         let y;
         y = 2;

### Operators
- JavaScript uses arithmetic operators ```( + - * / )``` to compute values. ```Ex:- (2 + 4) * 3;```
- JavaScript uses an assignment operator ( = ) to assign values to variables.

         let x, y;
         x = 2;
         y = 6;


### Expression
- An expression is a combination of values, variables, and operators, which computes to a value.
- The computation is called an evaluation.
- For example, ``` 5 * 10 evaluates to 50 & "John" + " " + "Doe" ```


### Keyword
- JavaScript keywords are used to identify actions to be performed.
- The ```let & var``` keyword tells the browser to create variables.

          let x, y;
          x = 3 + 6;
          y = x * 9;
          
### Comment
- Not all JavaScript statements are "executed".
- Code after double slashes // or between /* and */ is treated as a comment.
- Comments are ignored, and will not be executed.

      
      let x = 5;   // I will be executed

      // x = 6;   I will NOT be executed
    
### Identifiers
- Identifiers are names.
- In JavaScript, identifiers are used to name variables (and keywords, and functions, and labels).
- The rules for legal names are much the same in most programming languages.
- In JavaScript, the first character must be a letter, or an underscore (_), or a dollar sign ($).
- Subsequent characters may be letters, digits, underscores, or dollar signs.
- Numbers are not allowed as the first character.
- This way JavaScript can easily distinguish identifiers from numbers.
- All JavaScript identifiers are case sensitive.

# Js-comment
- JavaScript comments can be used to explain JavaScript code, and to make it more readable.
- JavaScript comments can also be used to prevent execution, when testing alternative code.

### Single Line Comments
- Single line comments start with //.
- Any text between // and the end of the line will be ignored by JavaScript (will not be executed).
- This example uses a single-line comment before each code line.


      //Anupam kumar

### Multi-line Comments
- Multi-line comments start with /* and end with */.
- Any text between /* and */ will be ignored by JavaScript.
- This example uses a multi-line comment (a comment block) to explain the code.


      /*anupam kumar
      kushinagar
      up*/
    
# Js-variable
- There are 3 ways to declare a JavaScript variable:
   - Using var
   - Using let
   - Using const
- Variables are containers for storing data (values).
- JavaScript variables are containers for storing data values.
- In this example, x, y, and z, are variables, declared with the``` var``` keyword.

      var x = 6;
      var y = 3;
      var z = x + y;

### Identifiers
- All JavaScript variables must be identified with unique names.These unique names are called identifiers.
- JavaScript identifiers are case-sensitive.
- Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).

### Assignment Operator
- The "equal to" operator is written like ``` == ``` in JavaScript
- In JavaScript, the equal sign (=) is an "assignment" operator, not an "equal to" operator.

  ```  x = x + 2 ```
  
### Data Type
- JavaScript variables can hold numbers like 100 and text values like "Anupam Rai".
- In programming, text values are called text strings.
- JavaScript can handle many types of data, but for now, just think of numbers and strings.
- Strings are written inside double or single quotes. Numbers are written without quotes.
- If you put a number in quotes, it will be treated as a text string.

      var x = 4.44;
      var person = "Anupam Rai";
      var answer = 'Yes I am!';
      
### Declaring (Creating) Variable
- Creating a variable in JavaScript is called "declaring" a variable.
- You declare a JavaScript variable with the ``` var ``` keyword.

       var personName;
- After the declaration, the variable has no value (value of undefined).To assign a value to the variable, use the equal sign.

      personName = "Anupam";
- You can also assign a value to the variable when you declare it.

      var carName = "Volvo";
* It's a good programming practice to declare all variables at the beginning of a script.

### One Statement, Many Variables
- You can declare many variables in one statement.
- Start the statement with var and separate the variables by comma.

      var person = "Anupam Rai", carName = "Bolero", price = 1200000;
- A declaration can span multiple lines

       var person = "Anupam Rai",
       carName = "Bolero",
       price = 1200000;
### Value = undefined
- In computer programs, variables are often declared without a value. The value can be something that has to be calculated, or something that will be provided later, like user input.
- A variable declared without a value will have the value undefined.
- The variable carName will have the value undefined after the execution of this statement.

      var carName;
  
### Re-Declaring Variables
- If you re-declare a JavaScript variable, it will not lose its value.
- The variable carName will still have the value "Bolero" after the execution of these statements.
  
      var carName = "Volvo";
      var carName;
      
### Arithmetic variables
- As with algebra, you can do arithmetic with JavaScript variables, using operators like = and +.
 
      var x = 5 + 2 + 3;
- You can also add strings, but strings will be concatenated.

      var x = "John" + " " + "Doe";
- If you put a number in quotes, the rest of the numbers will be treated as strings, and concatenated.

      var x = "5" + 2 + 3;
-  JavaScript treats a dollar sign as a letter, identifiers containing $ are valid variable names.

       var $$$ = "Hello World";
       var $ = 2;
       var $myMoney = 5;
- JavaScript treats underscore as a letter, identifiers containing _ are valid variable names:

      var _lastName = "Johnson";
      var _x = 2;
      var _100 = 5;
      
      
 # Js-Let
 - The let keyword was introduced in ES6 (2015).
 - Variables defined with let cannot be Redeclared.
 - Variables defined with let must be Declared before use.
 - Variables defined with let have Block Scope.


 ### Block Scope
 - Before ES6 (2015), JavaScript had only Global Scope and Function Scope.
 - ES6 introduced two important new JavaScript keywords ``` let ``` and ``` const ```.
 - These two keywords provide Block Scope in JavaScript.
 - Variables declared inside a { } block cannot be accessed from outside the block.

       {
         let x = 2;
       }
 - Variables declared with the``` var ``` keyword can NOT have block scope.
 - Variables declared inside a { } block can be accessed from outside the block.

       {
         var x = 2;
       } 
       
### Redeclaring Variables
- Redeclaring a variable using the``` var ``` keyword can impose problems.
- Redeclaring a variable inside a block will also redeclare the variable outside the block.

       var x = 11;
       
       {
         var x = 2;
       } 
       //2
       
- Redeclaring a variable using the ``` let ``` keyword can solve this problem.
- Redeclaring a variable inside a block will not redeclare the variable outside the block.

       let x = 11;
       
       {
         let x = 2;
       } 
       //11
       
- Redeclaring a JavaScript variable with ``` var ``` is allowed anywhere in a program.

      var x = 4;
      var x = 5;
      //3
      
- With ``` let ```, redeclaring a variable in the same block is NOT allowed:

      var x = 2;    // Allowed
      let x = 3;    // Not allowed

      {
      let x = 2;    // Allowed
      let x = 3     // Not allowed
      }

      {
      let x = 2;    // Allowed
      var x = 3     // Not allowed
      }
      
- Redeclaring a variable with ``` let ```, in another block, IS allowed:

      let x = 2;    // Allowed

      {
      let x = 3;    // Allowed
      }

      {
      let x = 4;    // Allowed
      }
      //2
      
### Let Hoisting
- Variables defined with ``` var ``` are hoisted to the top and can be initialized at any time.
- Meaning: You can use the variable before it is declared.

      carName = "Bolero";
      var carName;
      //Bolero
      
- Variables defined with ``` let ``` are also hoisted to the top of the block, but not initialized.
- Meaning: Using a ``` let ``` variable before it is declared will result in a ReferenceError.

      carName = "Saab";
      let carName = "Volvo";
      //ReferenceError
      
# Js-Const
- The ``` const ``` keyword was introduced in ES6 (2015).
- Variables defined with ``` const ``` cannot be Redeclared.
- Variables defined with ``` const ``` cannot be Reassigned.
- Variables defined with ``` const ``` have Block Scope.
- A const variable cannot be reassigned.

      const PI = 3.141592653589793;
      PI = 3.14;    
      PI = PI + 10;
      // This will give an error
      
- JavaScript ``` const ``` variables must be assigned a value when they are declared.

      const PI = 3.14159265359;
      //Correct
      
            const PI;
            PI = 3.14159265359;
            //Incorrect

- As a general rule, always declare a variable with ``` const ``` unless you know that the value will change.
- Use ``` const ``` when you declare:
   - A new Array
   - A new Object
   - A new Function
   - A new RegExp
   
### Constant Objects and  Arrays
- The keyword ``` const ``` is a little misleading. It does not define a constant value. It defines a constant reference to a value.
- Because of this you can NOT:
    - Reassign a constant value
    - Reassign a constant array
    - Reassign a constant object
    
But you CAN:
  - Change the elements of constant array
  - Change the properties of constant object

### Constant Arrays
- We can change the elements of a constant array.

      const cars = ["Saab", "Volvo", "BMW"];
      cars[0] = "Toyota";
      cars.push("Audi");
      // You can add an element:
         Toyota,Volvo,BMW,Audi
         
- But you can NOT reassign the array.

      const cars = ["Saab", "Volvo", "BMW"];
      cars = ["Toyota", "Volvo", "Audi"];    
      // ERROR
      
### Constant Objects
- You can change the properties of a constant object.

      const car = {type:"Fiat", model:"500", color:"white"};
      car.color = "red";
      car.owner = "Johnson";
      // You can add a property:
      
- But you can NOT reassign the object.

      const car = {type:"Fiat", model:"500", color:"white"};
      car = {type:"Volvo", model:"EX60", color:"red"};    
      // ERROR
  
### Block Scope
- Declaring a variable with ``` const ``` is similar to ``` let ``` when it comes to Block Scope.

      const x = 10;
      {
      const x = 2;
      }
      //10
    
### Redeclaring
- Redeclaring a JavaScript ``` var ``` variable is allowed anywhere in a program.

      var x = 2;     
      var x = 3;     
      x = 4;         
      // Allowed
      
- Redeclaring an existing ``` var ``` or ``` let ``` variable to const, in the same scope, is not allowed.

      var x = 2;     // Allowed
      const x = 2;   // Not allowed

      {
      let x = 2;     // Allowed
      const x = 2;   // Not allowed
      }

      {
      const x = 2;   // Allowed
      const x = 2;   // Not allowed
      }
      
- Reassigning an existing ``` const ``` variable, in the same scope, is not allowed.

      const x = 2;     // Allowed
      x = 2;           // Not allowed
      var x = 2;       // Not allowed
      let x = 2;       // Not allowed
      const x = 2;     // Not allowed

      {
        const x = 2;   // Allowed
        x = 2;         // Not allowed
        var x = 2;     // Not allowed
        let x = 2;     // Not allowed
        const x = 2;   // Not allowed
      }
- Redeclaring a variable with ``` const ```, in another scope, or in another block, is allowed:

      const x = 2;       // Allowed

      {
        const x = 3;   // Allowed
      }

      {
        const x = 4;   // Allowed
      }
      
 ### Const Hoisting
- Variables defined with ``` var ``` are hoisted to the top and can be initialized at any time.
- Meaning: You can use the variable before it is declared.

      carName = "Bolero";
      var carName;
      //Bolero
- Variables defined with ``` const ``` are also hoisted to the top, but not initialized.
- Meaning: Using a ``` const ``` variable before it is declared will result in a ReferenceError.

      alert (carName);
      const carName = "Volvo";
      //ReferenceError
# Js-Operators
- The assignment operator (=) assigns a value to a variable.
- The addition operator (+) adds numbers.
- The multiplication operator (*) multiplies numbers.
- The addition assignment operator (+=) adds a value to a variable.
- The + operator can also be used to add (concatenate) strings.

# Js-Datatype
- JavaScript variables can hold different data types: numbers, strings, objects and more.

      let x;                                         // Now x is undefined
      let length = 16;                               // Number
      let lastName = "Johnson";                      // String
      let x = {firstName:"John", lastName:"Doe"};    // Object
      
### Number
- JavaScript has only one type of numbers, Numbers can be written with, or without decimals.

    let x = 16.2;                                         
    let x = 16; 
    
### Boolean
- Booleans can only have two values ``` true ``` or ``` false ```.

      let x = 3;
      let y = 3;
      let z = 5;
      (x == y)       // Returns true
      (x == z)       // Returns false
      
### Arrays
- JavaScript ```arrays``` are written with square brackets.
- ```Array``` items are separated by commas.

      const cars = ["Bolero", "Pickup", "I20"];
      cars[1] //pickup

### Object
- JavaScript ```objects``` are written with curly braces {}.
- ```Object``` properties are written as name:value pairs, separated by commas.

      const person = {firstName:"Anupam", lastName:"Rai", age:25, eyeColor:"black"};
### typeof Operator
- You can use the JavaScript ```typeof``` operator to find the type of a JavaScript variable.
- The ```typeof``` operator returns the type of a variable or an expression.

      typeof ""                 // Returns "string"
      typeof "Anupan"          // Returns "string"
      typeof "Anupam Rai"     // Returns "string"

### Undefined
- In JavaScript, a variable without a value, has the value ```undefined```. The type is also ```undefined```.
- Any variable can be emptied, by setting the value to ```undefined```. The type will also be ```undefined```.
- An empty value has nothing to do with ```undefined```.
- An empty string has both a legal value and a type.

      let car;                 // Value is undefined, type is undefined
      car = undefined;        // Value is undefined, type is undefined
      let car = "";          // The value is "", the typeof is "string"


# Function
- A JavaScript ```function``` is a block of code designed to perform a particular task.
- A JavaScript ```function``` is executed when "something" invokes it (calls it).
- A JavaScript ```function``` is defined with the ```function``` keyword, followed by a name, followed by parentheses ().
- Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).
- The code to be executed, by the ```function```, is placed inside curly brackets: {}
- Function parameters are listed inside the parentheses () in the ```function``` definition.
- Function arguments are the values received by the ```function``` when it is invoked.
- Inside the ```function```, the arguments (the parameters) behave as local variables.

      function number(a1, a2){
      return a1 * a2;
      }                  //function gives the product of two number
   
### Function Invocation
- The code inside the function will execute when "something" ```invokes``` (calls) the function:
    - When an event occurs (when a user clicks a button)
    - When it is invoked (called) from JavaScript code
    - Automatically (self invoked)   

### Function Return
- When JavaScript reaches a ```return``` statement, the function will stop executing.
- If the function was invoked from a statement, JavaScript will ```"return"``` to execute the code after the invoking statement.
- Functions often compute a ```return``` value. The ```return``` value is ```"returned"``` back to the "caller".

      let x = myFunction(2, 4);
      function myFunction(a, b){
      return a * b;
      }
      
### Local Variables
- Variables declared within a JavaScript function, become ```LOCAL``` to the function.
- Local variables can only be accessed from within the function.
- Since local variables are only recognized inside their functions, variables with the same name can be used in different functions.
- Local variables are created when a function starts, and deleted when the function is completed.

# Js-Objects
- In real life, a Bike is an ```object```.
- A Bike has properties like weight and color, and methods like start and stop.
- All Bikes have the same properties, but the property values differ from Bike to Bike.
- All Bikes have the same methods, but the methods are performed at different times.

