# What is Hoisting ?
- Hoisting allows functions to be safely used in code before they are declared.
- Variable and class declarations are also hoisted, so they too can be referenced before they are declared. 
## Function hoisting
- One of the advantages of hoisting is that it lets you use a function before you declare it in your code.
    - with hoisting
                        myname('Anupam')
                        function myname(name){
                            console.log("My name is " + name)
                        }
    - without hoisting
                        function myname(name){
                            console.log("My name is " + name)
                        }
                        myname('Anupam')
## Variables Hoisting
- Hoisting works with variables too, so you can use a variable in code before it is declared and/or initialized.
   ### Var Hoisting
   - Here we declare then initialize the value of a var after using it.
   - The default initialization of the `var` is `undefined`
                        console.log(num); // Returns `undefined` from hoisted var declaration (not 6)
                        var num; // Declaration
                        num = 6; // Initialization
                        console.log(num); // Returns 6 after the line with initialization is executed.
   ### Let and Const Hoisting
   - Variables declared with let and const are also hoisted but, unlike var, are not initialized with a default value.
    An exception will be thrown if a variable declared with let or const is read before it is initialized.
   - The default initialization of the `let` and `const` is `ReferenceError`.
                        console.log(num); // Throws ReferenceError exception as the variable value is uninitialized
                        let num = 6; // Initialization
   ### Class Hoisting
   - However the class is not initialized by default, so any code that uses it before the line in which it is initialized is executed will throw a `ReferenceError`.


# What is the purpose of Const ?
- The value of a constant can't be changed through reassignment ,and it can't be redeclared.
                        const age= 22;
                        try {
                        number = 99;
                        } catch (err) {
                        console.log(err);
                        // expected output: TypeError: invalid assignment to const `number'
                        // Note - error messages will vary depending on browser
                        }
                        console.log(number);
                        // expected output: 22

# What is Closures ?
- A closure is the combination of a function bundled together with references to its surrounding state.
- A closure gives you access to an outer function's scope from an inner function.
- In JavaScript, closures are created every time a function is created, at function creation time.
- JavaScript variables can belong to the local or global scope.
- Global variables can be made local (private) with closures.
- A closure is a function having access to the parent scope, even after the parent function has closed.


                    function me() {
                        var name = "Anupam"; // name is a local variable created by init
                        function displayName() { // displayName() is the inner function, a closure
                            console.log(name); // displayName() uses variable declared in the parent function    
                        }
                        displayName();    
                    }
                    me();
- Every closure has three scopes:
    - Local scope (Own scope)
    - Enclosing scope (can be block, function, or module scope)
    - Global scope -: A function can access all variables defined inside the function.
- Variables created without a declaration keyword (var, let, or const) are always global, even if they are created inside a function.
- Global and local variables with the same name are different variables. Modifying one, does not modify the other

# What is Event Loop ?
- JavaScript has a runtime model based on an event loop, which is responsible for executing the code, collecting and processing events, and executing queued sub-tasks.
- If event loop is not happening then the browser can’t do anything else it’s being blocked. This means that the browser can’t render, it can’t run any other code, it’s just stuck. And here comes the problem — your app UI is no longer efficient and pleasing.
- 3 ways to represent the event loop.
   - Stack -: Function calls from a stack of frames
   - Heap -: Objects are allocated in a heap which is just a name to denote a large (mostly unstructured) region of memory.
   - Queue -: A JavaScript runtime uses a message queue, which is a list of messages to be processed. 

                        while (queue.waitForMessage()) {
                        queue.processNextMessage()
                        }
- The event loop got its name because of how it's usually implemented,`queue.waitForMessage()` waits `synchronously` for a message to arrive (if one is not already available and waiting to be handled).
- Each message is processed completely before any other message is processed.
- A very interesting property of the event loop model is that JavaScript, unlike a lot of other languages, never blocks.Handling I/O is typically performed via events and callbacks, so when the application is waiting for an DB query to return or an XHR request to return, it can still process other things like user input.

# What is Single Threaded Language ?
- JavaScript is a single-threaded language because while running code on a single thread, it can be really easy to implement as we don’t have to deal with the complicated scenarios that arise in the multi-threaded environment like deadlock.
- It is synchronous (all the work is done line by line) in nature.
- 
                        console.log('A'); 
                        setTimeout(() => {
                            console.log('B');
                        }, 3000);
                        console.log('C');
                        //output: ACB

# What is Callback function ?
- A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action.
                        function greeting(name) {
                        alert('Hello ' + name);
                        }
                        function processUserInput(callback) {
                        var name = prompt('Please enter your name.');
                        callback(name);
                        }
                        processUserInput(greeting);

# What is Asynchronous JavaScript?
- Functions running in parallel with other functions are called asynchronous.

# What is Promise in js?
- A Promise is a JavaScript object that links producing code and consuming code.
- The Promise object supports two properties: state and result.
    - Pending(undefined)
    - Fulfilled(a result value)
    - Rejected(an error object)

# What is Async/Await?
- async makes a function return a Promise, await makes a function wait for a Promise.
- The keyword await before a function makes the function wait for a promise: The await keyword can 
  only be used inside an async function.
                        async function myFunction() {
                        return "Hello";
                        }
                        async function myDisplay() {
                        let myPromise = new Promise(function(resolve) {
                            resolve("I love You !!");
                        });
                        document.getElementById("demo").innerHTML = await myPromise;
                        }
                        myDisplay();

# What is Currying ?
- Currying is a transformation of functions that translates a function from callable as f(a, b, c) into callable as f(a)(b)(c)
- Currying doesn’t call a function. It just transforms it.
                        function curry(f) { // curry(f) does the currying transform
                        return function(a) {
                            return function(b) {
                            return f(a, b);
                            };
                        };
                        }

