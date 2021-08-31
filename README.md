# Table of Contents

- [Js-Output](#js-output)
- [Js-Programs](#js-programs)
- [Js-Statements](#js-statements)
- [Js-syntax](#js-syntax)



# Js-output
- JavaScript can "display" data in different ways:
 ```
      Writing into an HTML element, using innerHTML.
      Writing into the HTML output using document.write().
      Writing into an alert box, using window.alert().
      Writing into the browser console, using console.log().
  ```
  
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
 ```Ex:- "Anupam Rai" & 'Anupam Rai'
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

   ``` var personName; ```
- After the declaration, the variable has no value (value of undefined).To assign a value to the variable, use the equal sign.

   ``` personName = "Anupam"; ```
- You can also assign a value to the variable when you declare it.

  ``` var carName = "Volvo"; ```
* It's a good programming practice to declare all variables at the beginning of a script.

### One Statement, Many Variables
- You can declare many variables in one statement.
- Start the statement with var and separate the variables by comma.

   ``` var person = "Anupam Rai", carName = "Bolero", price = 1200000; ```
- A declaration can span multiple lines

       var person = "Anupam Rai",
       carName = "Bolero",
       price = 1200000;
### Value = undefined
- In computer programs, variables are often declared without a value. The value can be something that has to be calculated, or something that will be provided later, like user input.
- A variable declared without a value will have the value undefined.
- The variable carName will have the value undefined after the execution of this statement.

  ``` var carName; ```
