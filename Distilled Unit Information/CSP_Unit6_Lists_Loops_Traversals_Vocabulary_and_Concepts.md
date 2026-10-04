# CSP Unit 6 – Lists, Loops, and Traversals: Vocabulary & Concepts

## How to read this

Each lesson lists only what's new: formal vocabulary and the concepts students should walk away with. Timing, prep, links, teaching tips, and teacher dialogue are cut.

- **Vocabulary** is copied word for word from the lesson's formal vocabulary box. Lessons without a box say "No formal vocabulary" and get concepts only.
- **Good to know** terms are defined in passing in the lesson but aren't in a formal vocabulary box. Their basic definitions are my own wording.
- **Key concepts** are condensed from the lesson's overview, objectives, presenter notes, discussion goals, and Check for Understanding.

Source: Code.org CS Principles (2025–26), Unit 6 lesson plans, licensed CC BY-NC-SA 4.0. Changes made: content condensed, reorganized, and paraphrased; teacher-facing material removed.

## Lesson 1: Lists Explore

**Vocabulary**

| Term | Definition |
| --- | --- |
| Data Abstraction | manage complexity in programs by giving a collection of data a name without referencing the specific details of the representation |
| Element | an individual value in a list that is assigned a unique index |
| Index | a common method for referencing the elements in a list or string using numbers |
| List | an ordered collection of elements |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Length | The number of elements in a list |

**Key concepts**

- A variable holds one value. Storing lots of information in separate variables gets hard to create and name, and lists solve that.
- In JavaScript, a list is created with square brackets and comma-separated values, then assigned to a variable: `var myNumbers = [25, 20, 10];`
- Indexes count up from 0. A list of 3 elements has indexes 0 to 2.
- Access an element with square brackets: `myNumbers[1]`. List accesses work inside expressions just like variables, and you can assign a new value to an index.
- Evaluate list accesses inside the brackets first, then assign.
- Three commands change a list's length:
    - **appendItem** adds an item at the end, creating a new last index.
    - **insertItem** places an item at a given index and shifts later items right, adding a new index at the end.
    - **removeItem** removes the item at a given index, shifts later items left, and removes the last index.

## Lesson 2: Lists Investigate

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Lists and variables both store information, and both start with `var` in JavaScript. Lists store multiple items of any type, in square brackets.
- Lists manage complexity (data abstraction). You only need a list's name to use it, not how it was created, and separate variables aren't needed for each element.
- `.length` gives the number of elements. Since indexes start at 0, the last index is `.length - 1`.
- Lists can work with UI elements, such as supplying the options for a dropdown.
- In App Lab's Data tab, you import a dataset from the Data Library to view and use it. `getColumn(table, column)` returns a column of data as a list.
- Common list patterns are reviewed in the lesson and appear in the Help & Tips tab.

## Lesson 3: Lists Practice

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students pick an app whose design is complete and use lists and list patterns to make it work, through a progression of about ten levels.
- This is hands-on practice accessing, updating, adding to, and removing from lists, plus debugging list code.

## Lesson 4: Lists Make

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students build a Reminders app from a blank screen. A single list stores all the reminders.
- The app uses the List Scrolling pattern: a variable keeps track of the current index so the user can move through a list's elements one at a time.
- Plan first: what information should be stored in a list, how many lists are needed, and which list patterns apply.

## Lesson 5: Loops Explore

**Vocabulary**

| Term | Definition |
| --- | --- |
| Infinite Loop | occurs when the ending condition will never evaluate to true |
| Iteration | a repetitive portion of an algorithm which repeats a specified number of times or until a given condition is met |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| While Loop | A loop that keeps running its code as long as a Boolean condition is true |
| For Loop | A loop that combines a while loop's three parts (starting value, condition, and update) into one statement |

**Key concepts**

- Loops replace repetitive code. A while loop runs its code over and over until its condition is no longer true. It stops when the Boolean expression evaluates to false.
- If the condition can never become false (for example, the counter is never updated), the loop never ends. That's an infinite loop.
- A while loop has three distinct parts: setting a starting value, checking a condition, and updating the value. A for loop puts all three in one statement.
- Students trace loops by hand with a robot on a game board (`moveForward`, `turnRight`, `turnLeft`, and `canMove(direction)`, which is true or false depending on whether a wall is in the way).
- Both functions and loops handle repetition. Choosing which one fits depends on the situation.

## Lesson 6: Loops Investigate

**Vocabulary:** No formal vocabulary.

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Simulation | A simplified model of the real world used to test ideas, run experiments, or draw conclusions |
| ++ | Shorthand that adds 1 to a variable |

**Key concepts**

- Loops simplify algorithms that repeat steps, like timing a hallway walk 20 times and averaging the results.
- Simulations are abstractions that remove details or simplify functionality. They let you test hypotheses more cheaply, safely, and quickly than doing it for real (for example, flight simulators, or flipping a coin a million times).
- Simulations can contain bias in which real-world elements they include, so watch for it.
- Inside a loop, random numbers can produce a variety of outcomes, like the real world (Coin Flipper app).
- Loops can update a set of screen elements by building IDs from the loop variable: `"text" + i` gives "text0," "text1," and so on (Font Tester app).

## Lesson 7: Loops Practice

**Vocabulary:** No formal vocabulary.

**Key concepts**

- This is hands-on practice writing and debugging programs with loops.
- The trickiest part is usually the iterator variable: its starting value, how it changes each round, and when the condition stops the loop.
- AP-style questions ask students to trace a loop and predict what it displays.

## Lesson 8: Loops Make

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students build a Lock Screen Maker app from a blank screen, combining lists and loops.
- Planning means spotting where an app likely uses a list (icons chosen from a list) and where it likely uses a loop (updating 20 icons with each button press).

## Lesson 9: Traversals Explore

**Vocabulary**

| Term | Definition |
| --- | --- |
| Traversal | the process of accessing each item in a list one at a time |

**Key concepts**

- A for loop is the standard way to traverse a list, because computers are good at checking things one by one:
    - The counter `i` usually starts at 0, the same as a list's first index.
    - The loop continues while `i < list.length`. The length is one more than the last index.
    - `i` increases by 1 after each round, and `list[i]` accesses the current element.
- When the loop ends, `i` equals the list's length.
- JavaScript list indexes start at 0, but AP exam pseudocode starts list indexes at 1.
- Traversals can:
    - search a list for a value and report its index,
    - reduce a list to a single value, like the smallest number,
    - filter some elements into a new list.
- Traversal matters most for long lists (1,000 or 1,000,000 elements) that you can't scan by eye.

## Lesson 10: Traversals Investigate

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students investigate three apps whose functions each traverse a list for a specific purpose.
- Example: an average function sets a total to 0, adds each element of the list to the total as it traverses, then divides the total by the list's length.
- Students modify apps to add new insights by writing their own traversals, such as totaling every element in a list.
- Common traversal patterns (including filter and reduce) are reviewed at the end.

## Lesson 11: Traversals Practice

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Simple traversals: print every element, print every element with its position, and traverse two parallel lists together.
- Filter practice: keep only the elements that meet a condition (for example, names longer than 6 letters, or countries in Central America).
- Reduce practice: boil a list down to one value (for example, the maximum price).
- Traversals often work with data imported from App Lab's data library.
- Debugging traversals uses the same tools as lists, like the Watch panel.

## Lesson 12: Traversals Make

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Students build a Random Forecaster app from a blank screen, using traversals to process lists.
- The key pattern is the List Filter Pattern: Filtering Multiple Lists. One column's list decides which items from another column's list are kept.

## Lesson 13: Project – Hackathon

**Vocabulary:** No formal vocabulary. This is a five-day unit project.

**Key concepts**

- Partners choose a dataset, make a paper prototype, plan element IDs and programming constructs, split into designer and programmer roles, build the app, and individually complete a Create PT-style written response.
- Each app traverses a list from its dataset using one of three patterns:
    - **Filter** (most common): use one column's list to decide what's kept from another column's list.
    - **Map:** add to or change each item in a list.
    - **Reduce:** boil a list down to a single value.
- Students explain how their program would have to be written differently without lists. Usually that would mean a large amount of extra code.
