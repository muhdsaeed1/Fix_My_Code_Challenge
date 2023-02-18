
## Fix my code challenge 

How to Solve Coding Problems with a Simple Four Step Method

There are four steps to the problem-solving method:

Understand the problem.
Devise a plan.
Carry out the plan.
Look back.

Step 1: Understand the problem.
When given a coding problem in an interview, it’s tempting to rush into coding. This is hard to avoid, especially if you have a time limit.

However, try to resist this urge. Make sure you actually understand the problem before you get started with solving it.

Read through the problem. If you’re in an interview, you could read through the problem out loud if that helps you slow down.

As you read through the problem, clarify any part of it you do not understand. If you’re in an interview, you can do this by asking your interviewer questions about the problem description. If you’re on your own, think through and/or Google parts of the question you might not understand.

This first step is vital as we often don’t take the time to fully understand the problem. When you don’t fully understand the problem, you’ll have a much harder time solving it.

To help you better understand the problem, ask yourself:

What are the inputs?
What kinds of inputs will go into this problem? In this example, the inputs are the arguments that our function will take.

Just from reading the problem description so far, we know that the inputs will be numbers. But to be more specific about what the inputs will be, we can ask:

Will the inputs always be just two numbers? What should happen if our function receives as input three numbers?

Here we could ask the interviewer for clarification, or look at the problem description further.

The coding problem might have a note saying, “You should only ever expect two inputs into the function.” If so, you know how to proceed. You can get more specific, as you’ll likely realize that you need to ask more questions on what kinds of inputs you might be receiving.

Will the inputs always be numbers? What should our function do if we receive the inputs “a” and “b”? Clarify whether or not our function will always take in numbers.

Optionally, you could write down possible inputs in a code comment to get a sense of what they’ll look like:

//inputs: 2, 4

Next, ask:

What are the outputs?
What will this function return? In this case, the output will be one number that is the result of the two number inputs. Make sure you understand what your outputs will be.

Create some examples.
Once you have a grasp of the problem and know the possible inputs and outputs, you can start working on some concrete examples.

Examples can also be used as sanity checks to test your eventual problem. Most code challenge editors that you’ll work in (whether it’s in an interview or just using a site like Codewars or HackerRank) have examples or test cases already written for you. Even so, writing out your own examples can help you cement your understanding of the problem.

Start with a simple example or two of possible inputs and outputs. Let's return to our addition function.

Let’s call our function “add.”

What’s an example input? Example input might be:

// add(2, 3)

What is the output to this? To write the example output, we can write:

// add(2, 3) ---> 5

This indicates that our function will take in an input of 2 and 3 and return 5 as its output.

Create complex examples.
By walking through more complex examples, you can take the time to look for edge cases you might need to account for.

For example, what should we do if our inputs are strings instead of numbers? What if we have as input two strings, for example, add('a', 'b')?

Your interviewer might possibly tell you to return an error message if there are any inputs that are not numbers. If so, you can add a code comment to handle this case if it helps you remember you need to do this.

// return error if inputs are not numbers.
Your interviewer might also tell you to assume that your inputs will always be numbers, in which case you don’t need to write any extra code to handle this particular input edge case.

If you don’t have an interviewer and you’re just solving this problem, the problem might say what happens when you enter invalid inputs.

For example, some problems will say, “If there are zero inputs, return undefined.” For cases like this, you can optionally write a comment.

// check if there are no inputs.

// If no inputs, return undefined.

For our purposes, we’ll assume that our inputs will always be numbers. But generally, it’s good to think about edge cases.

Computer science professor Evans says to write what developers call defensive code. Think about what could go wrong and how your code could defend against possible errors.  

Before we move on to step 2, let’s summarize step 1, understand the problem:

-Read through the problem.

-What are the inputs?

-What are the outputs?

Create simple examples, then create more complex ones.

2. Devise a plan for solving the problem.
Next, devise a plan for how you’ll solve the problem. As you devise a plan, write it out in pseudocode.

Pseudocode is a plain language description of the steps in an algorithm. In other words, your pseudocode is your step-by-step plan for how to solve the problem.

Write out the steps you need to take to solve the problem. For a more complicated problem, you’d have more steps. For this problem, you could write:

// Create a sum variable.

Add the first input to the second input using the addition operator.

// Store value of both inputs into sum variable.

// Return as output the sum variable.

Now you have your step-by-step plan to solve the problem.

For more complex problems, professor Evans notes, “Consider systematically how a human solves the problem.” That is, forget about how your code might solve the problem for a moment, and think about how you would solve it as a human. This can help you see the steps more clearly.

3. Carry out the plan (Solve the problem!)
The next step in the problem-solving strategy is to solve the problem. Using your pseudocode as your guide, write out your actual code.

Professor Evans suggests focusing on a simple, mechanical solution. The easier and simpler your solution is, the more likely you can program it correctly.

Taking our pseudocode, we could now write this:

function add(a, b) {
 const sum = a + b;
 return sum;
}
Professor Evans adds, remember not to prematurely optimize. That is, you might be tempted to start saying, “Wait, I’m doing this and it’s going to be inefficient code!”

First, just get out your simple, mechanical solution.

What if you can’t solve the entire problem? What if there's a part of it you still don't know how to solve?

Colt Steele gives great advice here: If you can’t solve part of the problem, ignore that hard part that’s tripping you up. Instead, focus on everything else that you can start writing.

Temporarily ignore that difficult part of the problem you don’t quite understand and write out the other parts. Once this is done, come back to the harder part.

This allows you to get at least some of the problem finished. And often, you’ll realize how to tackle that harder part of the problem once you come back to it.

Step 4: Look back over what you've done.
Once your solution is working, take the time to reflect on it and figure out how to make improvements. This might be the time you refactor your solution into a more efficient one.

As you look at your work, here are some questions Colt Steele suggests you ask yourself to figure out how you can improve your solution:

Can you derive the result differently? What other approaches are there that are viable?
Can you understand it at a glance? Does it make sense?
Can you use the result or method for some other problem?
Can you improve the performance of your solution?
Can you think of other ways to refactor?
How have other people solved this problem?
One way we might refactor our problem to make our code more concise: removing our variable and using an implicit return:

function add(a, b) {
 return a + b;
}
With step 4, your problem might never feel finished. Even great developers still write code that they later look at and want to change. These are guiding questions that can help you.


