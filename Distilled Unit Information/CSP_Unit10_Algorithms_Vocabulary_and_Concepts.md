# CSP Unit 10 – Algorithms: Vocabulary & Concepts

## How to read this

Each lesson lists only what's new: formal vocabulary and the concepts students should walk away with. Timing, prep, links, teaching tips, and teacher dialogue are cut.

- **Vocabulary** is copied word for word from the lesson's formal vocabulary box. Lessons without a box say "No formal vocabulary" and get concepts only.
- **Good to know** terms are defined in passing in the lesson but aren't in a formal vocabulary box. Their basic definitions are my own wording.
- **Key concepts** are condensed from the lesson's overview, objectives, presenter notes, discussion goals, and Check for Understanding.

Source: Code.org CS Principles (2025–26), Unit 10 lesson plans, licensed CC BY-NC-SA 4.0. Changes made: content condensed, reorganized, and paraphrased; teacher-facing material removed.

## Lesson 1: Algorithms Solve Problems

**Vocabulary**

| Term | Definition |
| --- | --- |
| Algorithm | a finite set of instructions that accomplish a task |
| Iteration | a repetitive portion of an algorithm which repeats a specified number of times or until a given condition is met |
| Problem | a general description of a task that can (or cannot) be solved with an algorithm |
| Selection | deciding which steps to do next |
| Sequencing | putting steps in an order |

**Key concepts**

- Computer scientists think about problems and the algorithms that solve them, not just code.
- Many problems are similar. Solving one may solve another or point to a strategy for it, so always ask "Have I seen this problem before?"
- Problems differ in how much work they need. Some can stop as soon as a match is found, some need to check everyone, and some need all the data recorded and sorted.
- The same problem can be solved by many different algorithms, written as code, AP pseudocode, or flowcharts.
- Deciding whether two algorithms are "the same" is nuanced. For example, turning left three times instead of turning right, or creating extra lists or variables, might matter depending on the context.
- Sequencing, selection, and iteration are the building blocks of algorithms.

## Lesson 2: Algorithm Efficiency

**Vocabulary**

| Term | Definition |
| --- | --- |
| Binary Search | a search algorithm that starts at the middle of a sorted set of numbers and removes half of the data; this process repeats until the desired value is found or all elements have been eliminated |
| Efficiency | a measure of how many steps are needed to complete an algorithm |
| Linear Search | a search algorithm which checks each element of a list, in order, until the desired value is found or all elements in the list have been checked |

**Key concepts**

- There are many ways to reach the same goal, but some algorithms take far fewer steps than others.
- Linear search checks items one by one in order and works on any list.
- Binary search repeatedly checks the middle item and eliminates half of the remaining data. It's much faster, but the list must be sorted first.
- The longer the list, the bigger binary search's advantage over linear search.
- Two algorithms that solve the same problem can have very different efficiencies.
- Students practice tracing the steps of a binary search.

## Lesson 3: Unreasonable Time

**Vocabulary**

| Term | Definition |
| --- | --- |
| Reasonable Time | Algorithms with a polynomial efficiency or lower (constant, linear, square, cube, etc.) are said to run in a reasonable amount of time |
| Unreasonable Time | Algorithms with exponential or factorial efficiencies are examples of algorithms that run in an unreasonable amount of time |

**Key concepts**

- More efficient algorithms matter more as the input size grows, because their amount of work grows more slowly.
- Problems that seem similar can differ hugely in difficulty. A "pair raffle" (checking pairs of tickets) takes many checks, but a "group raffle" (checking groups of any size) takes vastly more.
- Algorithms whose work grows at a polynomial rate or slower are reasonable. Algorithms whose work grows exponentially (or factorially) are unreasonable. Their running time explodes even for fairly small inputs.
- Mathematical reasoning about how the number of steps grows backs up the intuition that one problem is much harder than another.
- An unreasonable-time algorithm (like the group raffle) isn't practical to run for a school of almost any size.

## Lesson 4: The Limits of Algorithms

**Vocabulary**

| Term | Definition |
| --- | --- |
| Decision Problem | a problem with a yes/no answer (e.g., is there a path from A to B?) |
| Heuristic | provides a "good enough" solution to a problem when an actual solution is impractical or impossible |
| Optimization Problem | a problem with the goal of finding the "best" solution among many (e.g., what is the shortest path from A to B?) |
| Undecidable Problem | a problem for which no algorithm can be constructed that is always capable of providing a correct yes-or-no answer |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Factorial (n!) | Multiplying all whole numbers from n down to 1. For example, 4! = 4 × 3 × 2 × 1 = 24. |
| Traveling Salesperson Problem | Finding the shortest route that visits every location, which is a classic optimization problem |

**Key concepts**

- The Traveling Salesperson Problem is an optimization problem, not a decision problem. We know a path exists, and the question is which one is shortest.
- Finding the best path means checking every possible path. The number of paths grows factorially with each added location (node), so solving it exactly takes an unreasonable amount of time for most cases.
- Heuristics trade a guaranteed best answer for a "good enough" one in reasonable time. The Next-Closest heuristic (always go to the nearest unvisited place) usually works well but isn't always optimal.
- Undecidable problems are different from unreasonable-time problems. No algorithm can ever always give a correct yes/no answer to an undecidable problem, while an unreasonable-time problem can be solved, just too slowly to be practical.

## Lesson 5: Parallel and Distributed Algorithms

**Vocabulary**

| Term | Definition |
| --- | --- |
| Distributed Computing | a model in which programs are run by multiple devices |
| Parallel Computing | a model in which programs are broken into small pieces, some of which are run simultaneously |
| Sequential Computing | a model in which programs run in order, one command at a time |
| Speedup | the time used to complete a task sequentially divided by the time to complete a task in parallel |

**Key concepts**

- Besides writing faster algorithms, programs can be sped up by running parts of them on many processors or computers at once.
- Whenever multiple processes happen at the same time, that portion of the algorithm is parallel.
- Parallel algorithms bring challenges: waiting for the slowest process to finish, and splitting work up and recombining it.
- Speedup = sequential time ÷ parallel time.
- Speedup is almost always less than the number of processors (2 people sorting doesn't give a speedup of 2), because some portions stay sequential.
- As more processors are added, the extra benefit shrinks and speedup eventually reaches a limit.
