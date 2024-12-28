# Closure and setTimeout Bug in JavaScript

This repository demonstrates a common issue in JavaScript related to closures and the `setTimeout` function.  The code appears straightforward, but it produces an unexpected result due to how closures capture variables.

The problem is that the `console.log(i)` statement inside `setTimeout` doesn't execute until after the loop has completed. By that time, `i` has already reached its final value of 10, causing every logged output to be 10 instead of the expected sequence of numbers from 0 to 9.