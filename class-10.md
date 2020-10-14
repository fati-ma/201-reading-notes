# JS Debugging
#### Read: 10 submission 

#### Hello, This is Fatima. You can view my webpage using the following [link](https://fati-ma.github.io/201-reading-notes/class-10)
#### You can go back to the [home](https://fati-ma.github.io/201-reading-notes/) page.

#### In this blog I will give a summary for chapter 10 of the book: "Javascript and Jquery" :books:

- [x] *Chapter 10: Error Handling & Debugging* ✔️


## Chapter 10: Error Handling & Debugging

The JavaScript interpreter uses the concept of **execution contexts**.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope. 


### EXECUTION CONTEXT

- **GLOBAL CONTEXT**
Code that is in the script, but not in a function.
There is only one global context in any page. 

- **FUNCTION CONTEXT**
Code that is being run within a function.
Each function has its own function context. 

- **EVAL CONTEXT**
Text is executed like code in an internal function
called eval ()

### VARIABLE SCOPE

- **GLOBAL SCOPE**
If a variable is declared outside a function, it can
be used anywhere because it has global scope. 

- **FUNCTION-LEVEL SCOPE**
When a variable is declared within a function,
it can only be used within that function. This is
because it has function-level scope.


### EXECUTION CONTEXT & HOISTING 

Each time a script enters a new execution context, there are two phases
of activity: 

1: **PREPARE**
• The new scope is created
• Variables, functions, and arguments are created
• The value of the this keyword is determined 

2: **EXECUTE**
• Now it can assign values to variables
• Reference functions and run their code
• Execute statements 


### UNDERSTANDING SCOPE 

In the interpreter, each execution context has its own va ri ables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's v a ri ables object. 

Functions in JavaScript are said to have **lexical scope**.
They are linked to the object they were defined within.
So, for each execution context, the scope is the
current execution context's variables object, plus the
variables object for each parent execution context. 

### UNDERSTANDING ERRORS 

If a JavaScript statement generates an error, then it throws an **exception**.
At that point, the interpreter stops and looks for exception-handling code. 

### ERROR OBJECTS

#### Syntax Error
(SYNTAX IS NOT CORRECT)

1. MISMATCHING OR UNCLOSED QUOTES 
2. MISSING CLOSING BRACKET 
3. MISSING COMMA IN ARRAY 
4. MALFORMED PROPERTY NAME 


#### Reference Error
(VARIABLE DOES NOT EXIST)

1. VARIABLE IS UNDECLARED
2. NAMED FUNCTION IS UNDEFINED

#### Eval Error
(INCORRECT USE OF eval() FUNCTION )

#### URI Error
(INCORRECT USE OF URI FUNCTIONS)

#### Type Error
(VALUE IS UNEXPECTED DATA TYPE)

#### RangeError
(NUMBER OUTSIDE OF RANGE)

#### Error
(GENERIC ERROR OBJECT)

#### NaN
(NOT AN ERROR)


### HOW TO DEAL WITH ERRORS

1: **DEBUG THE SCRIPT TO FIX ERRORS**
2: **HANDLE ERRORS GRACEFULLY **


### HANDLING EXCEPTIONS

Using `try`, `catch`, and `finally`.

```
try {

catch (exception) {

finally {

}
```

### THROWING ERRORS 

If you know something might cause a problem for your script, you can
generate your own errors before the interpreter creates them. 

```
throw new Error( 'message') ; 
```

### Key points:

- Debugging is the process of finding errors. It involves a
process of deduction. 

- The console helps narrow down the area in which the
error is located.

- JavaScript has 7 different types of errors. Each creates
its own error object, which can tell its line number
and gives a description of the error. 












