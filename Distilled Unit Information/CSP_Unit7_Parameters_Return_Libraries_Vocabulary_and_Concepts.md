# CSP Unit 7 – Parameters, Return, and Libraries: Vocabulary & Concepts

## How to read this

Each lesson lists only what's new: formal vocabulary and the concepts students should walk away with. Timing, prep, links, teaching tips, and teacher dialogue are cut.

- **Vocabulary** is copied word for word from the lesson's formal vocabulary box. Lessons without a box say "No formal vocabulary" and get concepts only.
- **Good to know** terms are defined in passing in the lesson but aren't in a formal vocabulary box. Their basic definitions are my own wording.
- **Key concepts** are condensed from the lesson's overview, objectives, presenter notes, discussion goals, and Check for Understanding.

Source: Code.org CS Principles (2025–26), Unit 7 lesson plans, licensed CC BY-NC-SA 4.0. Changes made: content condensed, reorganized, and paraphrased; teacher-facing material removed.

## Lesson 1: Parameters and Return Explore

**Vocabulary**

| Term | Definition |
| --- | --- |
| Argument | the value passed to the parameter |
| Parameter | a variable in a function definition. Used as a placeholder for values that will be passed through the function |
| Return | used to return the flow of control to the point where the procedure (also known as a function) was called and to return the value of expression |

**Key concepts**

- A function with parameters is like a general recipe. Its placeholders (tiers, flavor) are replaced by whatever values are passed in, so one function can produce many different results.
- Parameters are placeholders in the function definition. Arguments are the actual values passed in when the function is called (for example, 4 and "chocolate").
- Local variables created inside a function can't be accessed or updated outside it (variable scope).
- A function can make decisions based on the arguments passed to it.
- When a program reaches a `return`, the function stops and sends a value back to where it was called. That value can be stored in a variable: `var cakeCalculator = cakeCost(3, "lemon");`
- Better-organized code helps the people who read it, debug it, and build on it.

## Lesson 2: Parameters and Return Investigate

**Vocabulary**

| Term | Definition |
| --- | --- |
| Procedural Abstraction | a process and allows a procedure to be used only knowing what it does, not how it does it. Procedural abstraction allows a solution to a large problem to be based on the solution of smaller subproblems. This is accomplished by creating procedures to solve each of the subproblems. |

**Key concepts**

- Parameters and return values don't let programs do more than before. They make programs cleaner, better organized, easier to read, and easier to reuse.
- Clean code is mainly for people, but over time it makes it possible to write larger, more complex programs.
- Well-named functions make a program read like a description of what it does.
- Using parameters to generalize lets a single function handle many different tasks.
- Procedural abstraction means you can use a procedure knowing only what it does, not how. Large problems get solved by writing procedures for smaller subproblems.

## Lesson 3: Parameters and Return Practice

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students practice reading, writing, and debugging functions with parameters and return values. These programs work a little differently from earlier ones, so they take practice.
- Parameters and return make code neater and let it work in more situations.
- Return makes partial traversals possible. A function can stop partway through a list (for example, once it finds a specific element) and return right away, instead of always visiting every element.
- AP-style questions ask what a procedure returns for different arguments.

## Lesson 4: Parameters and Return Make

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students build a Rock Paper Scissors app by filling in "blank functions." Most of the program is already written, so this is a different kind of Make project than a blank screen.
- Parameters and return let a program be chunked into pieces with well-defined behavior (procedural abstraction). Each function can be written and tested separately.
- Teammates who agree in advance on what each function does can write them separately and then combine them into one working app.
- Debugging strategies: build and test small parts at a time, run the code slowly, use the watcher, and explain the difference between what you expect and what actually happens.

## Lesson 5: Libraries Explore

**Vocabulary**

| Term | Definition |
| --- | --- |
| API | Application Program Interface specifications for how functions in a library behave and can be used |
| Library | a group of functions (procedures) that may be used in creating new programs |

**Key concepts**

- Libraries let you easily share functions between programs.
- A library needs documentation (its API) for each function: how it works, every parameter (its data type and a short description), and what it returns, if anything.
- Without documentation, a user has to guess what a function does, what types its parameters need, and what it returns.
- Functions that use global variables (accessing or updating variables elsewhere in the program) aren't ready to share. Rework them to use local variables, parameters, and a return.
- Library functions are called with the library name, then the function name, then the arguments. App Lab's built-in Math library (`Math.round`) works this way.

## Lesson 6: Libraries Investigate

**Vocabulary**

| Term | Definition |
| --- | --- |
| Modularity | the subdivision of a computer program into separate subprograms |

**Key concepts**

- Testing library functions (for example, with `console.log`) shows whether a bug is in the library or in your own code.
- Good library functions are self-contained. Watch out for global variables or references to element IDs that might not exist in someone else's project.
- Existing algorithms can be combined to build new ones. Examples include finding a max or min, a sum or average, checking divisibility, and a robot's path through a maze.
- Building on existing algorithms reduces development time and testing, and makes errors easier to find.
- Procedural abstraction gives a process a name and lets it be used knowing only what it does. It encourages code reuse and manages complexity, and libraries are an example.
- Users only need the documentation, so a library's creator can update its functions (for example, to make them faster) without telling users, as long as the functions still behave as documented.

## Lesson 7: Libraries Practice

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Libraries handle detailed or repetitive tasks so you can focus on the big picture. Programs that use them are shorter and read more like what they actually do.
- Because other people rely on a library working exactly as documented, libraries must be carefully tested and debugged before they're shared.
- Libraries are another level of procedural abstraction. The detailed code still runs, but once it's written, you don't have to think about it.

## Lesson 8: Project – Make a Library Part 1

**Vocabulary:** No formal vocabulary.

**Key concepts**

- This is the final programming project before the Create PT. Students build a library of functions that classmates can actually import and use as new building blocks.
- Students brainstorm common problems they've run into while programming and choose a theme for their library.
- Design comes first: write the API for each function, including its name, purpose, parameters (with data types), and what it returns, as comments.
- Students start with one function that includes all four Create PT features: a parameter, a return value, a loop, and a conditional.

## Lesson 9: Project – Make a Library Part 2

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students write tests for their functions to confirm they return the expected values.
- Good tests call the function with many different inputs, including values just below, at, and just above the cutoffs in its conditionals.
- Students trade libraries with a classmate, who imports the library, tries using it, and gives feedback on whether it works and is documented clearly.

## Lesson 10: Project – Make a Library Part 3

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students debug and finish their libraries using their test results and classmate feedback.
- The written responses are taken nearly word for word from the Create PT. Students explain the purpose and functionality of one of their functions and describe two different calls to it with different arguments.
- The project caps the study of procedural abstraction and prepares students for the Create PT in Unit 9.
