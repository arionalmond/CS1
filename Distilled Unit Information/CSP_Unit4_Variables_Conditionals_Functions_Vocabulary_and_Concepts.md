# CSP Unit 4 – Variables, Conditionals, and Functions: Vocabulary & Concepts

## How to read this

Each lesson lists only what's new: formal vocabulary and the concepts students should walk away with. Timing, prep, links, teaching tips, and teacher dialogue are cut.

- **Vocabulary** is copied word for word from the lesson's formal vocabulary box. Lessons without a box say "No formal vocabulary" and get concepts only.
- **Good to know** terms are defined in passing in the lesson but aren't in a formal vocabulary box. Their basic definitions are my own wording.
- **Key concepts** are condensed from the lesson's overview, objectives, presenter notes, discussion goals, and Check for Understanding.

Source: Code.org CS Principles (2025–26), Unit 4 lesson plans, licensed CC BY-NC-SA 4.0. Changes made: content condensed, reorganized, and paraphrased; teacher-facing material removed.

## Lesson 1: Variables Explore

**Vocabulary**

| Term | Definition |
| --- | --- |
| Assignment Operator | allows a program to change the value represented by a variable |
| Expression | a combination of operators and values that evaluates to a single value |
| String | an ordered sequence of characters |
| Variable | a named reference to a value that can be used repeatedly throughout a program |

**Introduced code:** `Math.round(x);` · `var x = __;` · `var x;`

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Value | A single piece of information, such as a number or a string |
| Operator | A symbol for an operation: +, −, *, / |
| Evaluate | To work out the single value an expression produces |

**Key concepts**

- Unit 4 lessons follow the EIPM sequence: Explore (hands-on model of a concept), Investigate (read and modify working code), Practice (scaffolded coding), and Make (build an app from a blank screen).
- This unit moves beyond input/output apps to apps that keep track of information and use it to make decisions and do calculations.
- Two types of values so far: numbers (digits, no quotes) and strings (any keyboard characters, inside double quotes). The number 123 and the string "123" are different.
- Expressions follow the order of operations. All four operators work on numbers. With strings, only + works, and it joins them. Combining a number and a string converts the number to a string.
- A variable holds at most one value. Variable names use no quotes or spaces and must start with a letter. `var` creates a variable.
- Assignment is read as "gets" (x ← 3 is "x gets 3"). Assigning a new value erases the old one.
- Always evaluate first, then assign. Assigning one variable from another just copies the value; no lasting connection is made between them.
- `x ← x + 1` uses a variable's current value to "count up by one."
- In JavaScript the assignment operator is =. In programming, = means "put this value in this variable," not "these are equal forever" as in math.

## Lesson 2: Variables Investigate

**Vocabulary:** No formal vocabulary.

**Introduced code:** `Math.round(x);` · `var x = __;` · `var x;`

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Concatenation | Joining strings together (or strings with numbers or variables) into one string |
| Watcher | A debugging tool that shows the value stored in a variable as a program runs |

**Key concepts**

- In JavaScript, `var` declares (creates and names) a variable. Variables can be updated in response to events.
- `Math.round` rounds a value to the nearest integer. `getText` gets the text currently in an element with a given ID.
- **Counter Pattern with Event:** a variable starts at 0, and each time the event fires, it gets its current value plus 1. It's useful for things like a game score.
- **Variables with String Concatenation Pattern:** combine strings, numbers, or variables with + and store the result. For example, "rock" + " and " + "roll" gives "rock and roll".
- Variables can store numbers and strings, including concatenated strings like `temp + " F"`.
- Meaningful variable names matter because code is written for people too. Good names make code easier to read and hint at what's stored.

## Lesson 3: Variables Practice

**Vocabulary:** No formal vocabulary.

**Key concepts**

- This lesson is hands-on practice writing and debugging programs that use variables and expressions.
- The debugging process has four steps: Describe, Hunt, Try, and Document.
- Three debugging skills get the most attention: slowing code with the speed slider, using `console.log` to print output, and using the Watch area to see variables change.
- Practice covers assigning numbers and strings, writing more complex expressions with operators, and using the counter pattern with both numbers and strings.
- `\n` is the new line character. It starts a new line inside a string.

## Lesson 4: Variables Make

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students build the Photo Liker app from a blank screen (the design elements are provided, but there's no code), using variables to store the number of likes and the comments.
- Before building, identify what the app does, its inputs, its outputs, and what information should be stored in variables.
- Breaking a large task like "build an app" into incremental steps is a strategy for future projects, including the unit project and the Create PT.
- Debugging strategies: run the code slowly, add variables to the watcher, use `console.log`, explain the code to a friend, and read the code line by line.
- Comments should explain both the purpose and the function of code segments.

## Lesson 5: Conditionals Explore

**Vocabulary**

| Term | Definition |
| --- | --- |
| Boolean Value | a data type that is either true or false |
| Comparison Operator | <, >, <=, >=, ==, != indicate a Boolean expression |
| Logical Operator | NOT, AND, and OR, which evaluate to a Boolean value |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Boolean Expression | An expression that evaluates to true or false |
| Flowchart | A diagram that shows the steps and decision points used to reach a conclusion |
| Truth Table | A table showing every combination of true and false inputs and what a logical operator produces for each |

**Key concepts**

- Booleans are a third data type, after numbers and strings. They hold true or false and are used to make decisions: if something is true, do this; if false, do that.
- There are six comparison operators. The lesson's speaker notes also call them relational operators. == means "equal to," while a single = means "gets the value" (assignment).
- Reduce both sides of a comparison to a single value first, then compare. Expressions can include variables.
- Flowcharts model how a computer makes a decision: list the variables, evaluate the Boolean expression at each decision point, and follow the true or false path.
- Be precise. "Have 40 dollars" written as `money == 40` means exactly 40, not 40 or more.
- Logical operators combine Boolean expressions:
    - **AND (&&):** true only if both sides are true.
    - **OR (||):** true if either side is true.
    - **NOT (!):** reverses the value.
- Several separate checks can be combined into a single expression with logical operators.

## Lesson 6: Conditionals Investigate

**Vocabulary**

| Term | Definition |
| --- | --- |
| Conditional Statement | affects the sequential flow of control by executing different statements based on the value of a Boolean expression |
| Logical Operator | NOT, AND, and OR, which evaluate to a Boolean value |

**Key concepts**

- Conditionals let programs make decisions by using Boolean expressions to decide whether to run certain code.
- **if:** checks one Boolean expression. If it's true, that code runs. Either way, the program then continues normally.
- **if-else:** adds code that runs when the condition is false.
- **if-else-if:** checks several Boolean expressions in order and runs only the code for the first one that's true.
- In an if-else-if, put the most specific condition first. Otherwise a broader condition can be true first and the specific case never runs.
- Drawing a flowchart for an if-else-if statement helps show how it works.
- Explaining code means describing how it works (for example, "the value in score increases by 1, then `setProperty` shows the new score"), not just repeating the comments.

## Lesson 7: Conditionals Practice

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students pick one of three apps whose design is already complete and use conditional statements to make it work as intended.
- This is practice with Boolean expressions, logical operators, and if / if-else / if-else-if statements, plus debugging (identifying and correcting errors).
- Nested conditionals can check ranges. For example, an `IF (number >= 10)` containing an `IF (number <= 20)` only runs its code for numbers from 10 to 20.
- Swapping AND and OR changes which inputs make a condition true, so it changes the program's outcome.

## Lesson 7 (Alternate): Conditionals Practice

*An alternate to Lesson 7. Only one of the two is taught.*

**Vocabulary:** No formal vocabulary.

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Syntax Error | An error from code that breaks the rules of the programming language |
| Logic Error | An error where the code is valid but works incorrectly |
| Run-time Error | A mistake that shows up while the program is running. These are defined by the programming language. |
| Overflow Error | An error when a computer tries to handle a number outside its defined range of values (also covered in Unit 1) |

**Key concepts**

- Practice starts with Boolean expressions printed with `console.log`, using comparison operators (<, >, <=, >=, ==, !=) and then logical operators (&&, ||, !).
- Syntax errors show up as errors and warnings in the code. Logic errors only show up when you test, so testing your code is essential.
- Use the debugging process throughout.

## Lesson 8: Conditionals Make

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students build a Museum Ticket Generator app from a blank screen, practicing both flowcharts and complex conditional statements.
- Plan before coding: what the app does, its inputs (age and day dropdowns, discount code, generate button), its outputs (the ticket), the variables it needs, and the conditional logic.
- Pricing rules with multiple conditions call for if-else-if statements combined with AND / OR.
- Debugging strategies: run the code slowly, add variables to the watcher, and explain the code to a friend.

## Lesson 9: Functions Explore and Investigate

**Vocabulary**

| Term | Definition |
| --- | --- |
| Function | a named group of programming instructions. Also referred to as a "procedure". |
| Function Call | a command that executes the code within a function |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Function Declaration | The code that defines a function: its name and the commands it contains |

**Key concepts**

- A song written with a repeated chorus "out of order" is shorter to write but sings the same. Functions work the same way: they remove repetition and make the overall structure easier to see.
- A function is declared once to give a group of commands a name, and it can be called as many times as needed.
- When a function is called, the program jumps to the function's code, runs it, and then returns. Running code slowly shows this change in order.
- Functions remove repeated code and make event handlers simpler to read. A change to the function applies everywhere it's called, so code only has to be written and debugged once.
- **updateScreen pattern:** a single function that updates what's displayed on the screen, called whenever the screen needs to change.
- Parameters, arguments, and return values aren't covered in this unit. For now, a function is simply a named collection of commands that can be used in multiple places.

## Lesson 10: Functions Practice

**Vocabulary:** No formal vocabulary.

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Variable Scope | Where in a program a variable can be used. A global variable (created outside any function or event) can be used anywhere. A local variable (created inside a function or event) can only be used there. |

**Key concepts**

- Students practice calling functions that are already declared, then find repeated code and replace it with a function they create.
- Calling a function changes the order in which lines of code run.
- Variable scope (global vs. local) comes back from the variables lessons. Students only need a basic understanding at this point.
- **When to make a function:** beginners usually notice repeated code after writing it twice and then move it into a function. With more experience, programmers spot the need sooner, and eventually they plan their functions before they start coding.

## Lesson 11: Functions Make

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students build a Quote Maker app from a blank screen, using a function to reduce repeated code.
- Practice anticipating functions: decide early that you'll need one instead of writing code twice and fixing it later.
- In this app, a function can update the screen. It contains the conditional that's checked every time the user interacts with the screen.
- Comments should explain both the purpose and the function of each code segment.

## Lesson 12: Project – Decision Maker App

**Vocabulary:** No formal vocabulary. This is a three-day unit project (Practice PT).

**Key concepts**

- Students build an app that helps a user make a decision. It must take in at least one number and one string from the user, use all of that information in the decision, and include at least one function that updates the screen.
- Day 1 is planning, Day 2 is building in App Lab, and Day 3 is peer review, updates, and submission.
- The core structure is an `updateScreen()` function that contains a conditional statement. It's called whenever the user changes an input, after the matching variable is updated.
- Comments explain what a function does (its purpose) and how it does it (its functionality).
- Written responses practice Create PT-style questions about a conditional statement and a procedure in the student's own program.
