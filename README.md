# tarpit
My take on "[Out of the Tar Pit](https://github.com/papers-we-love/papers-we-love/blob/master/design/out-of-the-tar-pit.pdf)"

# Further Thoughts
I've had the opportunity to use the ideas in the flowchart and have found them really helpful. Tarpit code is really easy to read, test, and re-use. However, I feel like the flowchart is a bit too narrow in focus. The term "logic" is all encompassing; so much so that it interrupts my thought process. So I'm adding the following supplemental definitions.

## Plumbing Code
This is code that is concerned with the setup of data pathways. Wiring up the http server, connecting to the database, listening on a port, etc. This is all about bootstrapping and connecting. This is technically represented in the flow chart in the last decision tree, however, the wording is too general.

## Controlling Code
Think of this as the infrastructure code. Security, caching, logging, routing, validation, etc. This is the code that isn't plumbing and that the business doesn't ask for but definitely needs. Just like Plumbing Code, this is represented in the last decision tree.

## Business Code
This is the actual business code. This is the reason for creating an app in the first place. I think of this as the decision making code. This is the one that is actually in the flow chart but, again, it's called "logic" everywhere.

![tarpit_graph](tarpit.png)
