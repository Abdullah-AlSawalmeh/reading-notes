# Error Handling & Debugging :
JavaScript can be hard to learn and everyone makes mistakes when writing it. We will help you learn how to find the errors in your code. and teach you how to write scripts that deal with potential errors gracefully

# JavaScript Debuggers
Debugging is not easy. But fortunately, all modern browsers have a built-in JavaScript debugger.

Built-in debuggers can be turned on and off, forcing errors to be reported to the user.

With a debugger, you can also set breakpoints (places where code execution can be stopped), and examine variables while the code is executing.

Normally, otherwise follow the steps at the bottom of this page, you activate debugging in your browser with the F12 key, and select "Console" in the debugger menu.

# Setting Breakpoints
In the debugger window, you can set breakpoints in the JavaScript code.

At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values.

After examining values, you can resume the execution of code (typically with a play button).

# The Stack

The JavaScript interpreter processes one line of code at a time .

When a statement has to call some other code in order to do its job the new task goes to the top of the pile of things to do. Once the new task has been performed , the interpter can go back to the task in hand.

Each time a script enters a new execution context, there are two phases of activity:

PREPARE :
The new scope is created
Variables, functions, and arguments are created
The value of the this keyword is determined
EXECUTE :
Now it can assign values to variables
Reference functions and run their code
Execute statements


