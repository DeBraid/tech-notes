# Javascript Generators

Run to completion: the `yield` keyword can pause a function, holding it's state in place. It can be paused more than once.

> ES6 generator functions are "cooperative" in their concurrency behavior. Inside the generator function body, you use the new yield keyword to pause the function from inside itself. Nothing can pause a generator from the outside; it pauses itself when it comes across a yield.

In order to restart a paused generator, it must be evoked from OUTSIDE.

> Stopping and starting is not just a control on the execution of the generator function, but it also enables 2-way message passing into and out of the generator, as it progresses.

Send messages out with yield, in with each restart.

## Syntax

* `function *foo () {}` AND `function* foo () {}` are both valid syntax.

* `yield` expression (not `yield` statement)




