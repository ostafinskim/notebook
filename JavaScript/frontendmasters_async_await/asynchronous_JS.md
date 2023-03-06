# JavaScript - The new hard parts

As soon as we start running our code we create a global execution context.

- Thread of execution ( parsin and executing the code line by line ).
- Live memory of variables with data ( known as Global Variable Environment ).

When we want to execute code inside a function we create local execution context, with local variables environment.

Call stack helps JavaScript to keep track of current execution context.

JavaScript is single threaded (one command executing at a
time) and has a synchronous execution model (each line is
executed in order the code appears).

Some of web browser features (WEB API):

- DOM
- console
- localStorage
- XHR

ref: <https://developer.mozilla.org/en-US/docs/Web/API>
