# JS Debugging

![javascript debugging](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2019/08/JavaScript-Debugging-and-Testing.png)

When you are writing JavaScript, do not expect to write it perfectly the first time.
Programming is like problem solving: you are given a puzzle and not only do you have to solve
it, but you also need to create the instructions that allow the computer to solve it. too.

The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope.

Functions in JavaScript are said to have lexical scope.
They are linked to the object they were defined within.
So, for each execution context, the scope is the
current execution context's variables object, plus the
variables object for each parent execution context.

If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code.

## ERROR OBJECTS

Error objects can help you find where your mistakes are
and browsers have tools to help you read them.

1. Syntax Error:
SYNTAX IS NOT CORRECT
This is caused by incorrect use of the rules of the
language. It is often the result of a simple typo.

2. Reference Error:
VARIABLE DOES NOT EXIST
This is caused by a variable that is not declared or is
out of scope.

3. Eval Error:
INCORRECT USE OF eval() FUNCTION
The eval() function evaluates text through the
interpreter and runs it as code . It is rare that you would see this type
of error, as browsers often throw other errors when
they are supposed to throw an Eva 1 Error.

4. URI Error:
INCORRECT USE OF URI FUNCTIONS
If these characters are not escaped in URls, they will
cause an error: / ? & I : ;

5. Type Error:
VALUE IS UNEXPECTED DATA TYPE
This is often caused by trying to use an object or
method that does not exist.

6. RangeError:
NUMBER OUTSIDE OF RANGE
If you call a function using numbers outside of its
accepted range.

7. Error:
GENERIC ERROR OBJECT
The generic Error object is the template (or
prototype) from which all other error objects are
created.

8. NaN:
NOT AN ERROR
Note: If you perform a mathematical operation using
a value that is not a number, you end up with the
value of NaN, not a type error.

## HOW TO DEAL WITH ERRORS

1. DEBUG THE SCRIPT TO FIX ERRORS:
If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it.

2. HANDLE ERRORS GRACEFULLY:
You can handle errors gracefully using try, catch,
throw, and f i na 1 ly statements.

## BROWSER DEV TOOLS & JAVASCRIPT CONSOLE

The JavaScript console will tell you when there is a problem with a script,
where to look for the problem, and what kind of issue it seems to be.

You can also just type code into the console
and it will show you a result.

MORE CONSOLE METHODS

1. console. info() can be used for general information
2. console.warn() can be used for warnings
3. console .error () can be used to hold errors.

### BREAKPOINTS

You can pause the execution of a script on any
line using breakpoints. Then you can check the
values stored in variables at that point in time.

![debug](https://cdn-media-1.freecodecamp.org/images/7IKv-WVp8ztTZyyC-zlAnOmOxN5gpi9FGmD4)

CHROME

1. Select the Sources option.
2. Select the script you are
working with from the left-hand
pane. The code will appear to
the right.
3. Find the line number you want
to stop on and click on it.
4 . When you run the script, it
will stop on this line. You can
now hover over any variable to
see its value at that time in the
script's execution.

If you set multiple breakpoints, you can step
through them one-by-one to see where values
change and a problem might occur.

### CONDITIONAL BREAKPOINTS

![conditional breakpoints](https://miro.medium.com/max/1428/1*KYgJT7S4itxXtKRWXqqHRA.png)

You can indicate that a breakpoint should be
triggered only if a condition that you specify is
met. The condition can use existing variables.

### DEBUGGER KEYWORD

You can create a breakpoint
in your code using just the
debugger keyword. When the
developer tools are open, this
will automatically create a
breakpoint.

## HANDLING EXCEPTIONS

If you know your code might fail, use [try, catch, and finally](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/try...catch).

Each one is given its own code block:

The try statement consists of a try-block, which contains one or more statements. {} must always be used, even for single statements. At least one catch-block, or a finally-block, must be present. This gives us three forms for the try statement:

try...catch
try...finally
try...catch...finally
A catch-block contains statements that specify what to do if an exception is thrown in the try-block. If any statement within the try-block (or in a function called from within the try-block) throws an exception, control is immediately shifted to the catch-block. If no exception is thrown in the try-block, the catch-block is skipped.

The finally-block will always execute after the try-block and catch-block(s) have finished executing. It always executes, regardless of whether an exception was thrown or caught.


THROWING ERRORS
If you know something might cause a problem for your script, you can
generate your own errors before the interpreter creates them.

### DEBUGGING TIPS

1. ANOTHER BROWSER:Some problems are browserspecific.
Try the code in another
browser to see which ones are
causing a problem.
2. ADD NUMBERS:Write numbers to the console
so you can see which the items
get logged. It shows how far your
code runs before errors stop
3. SEARCH:Stack Overflow is a Q+A site for
programmers.
Or use a traditional search
engine such as Google, Bing, or
4. VALIDATION TOOLS:There are a number of on line
validation tools that can help you
try to find errors in your code:
5. CODE PLAYGROUNDS:If you want to ask about
problematic code on a forum, in
addition to pasting the code into
a post, you could add it to a code
playground site (such as
JSBin.com, JSFiddle. com, or
Dabbl et. corn) and then post a
link to it from the forum.
6. STRIP IT BACK:Remove parts of code, and strip
it down to the minimum you
need. You can do this either by
removing the code altogether, or
by just commenting it out using
multi-line comments
7. EXPLAINING THE CODE:Programmers often report
finding a solution to a problem
while explaining the code to
someone else.

### Resources used in this reading

1. duckett_html book.
2. <https://www.w3schools.com/js/js_mistakes.asp>
3. <https://developer.mozilla.org/en-US/docs/Web/JavaScript>

