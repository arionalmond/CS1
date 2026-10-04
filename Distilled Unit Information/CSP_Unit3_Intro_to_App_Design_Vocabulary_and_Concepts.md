# CSP Unit 3 – Intro to App Design: Vocabulary & Concepts

## How to read this

Each lesson lists only what's new: formal vocabulary and the concepts students should walk away with. Timing, prep, links, teaching tips, and teacher dialogue are cut.

- **Vocabulary** is copied word for word from the lesson's formal vocabulary box. Lessons without a box say "No formal vocabulary" and get concepts only.
- **Good to know** terms are defined in passing in the lesson but aren't in a formal vocabulary box. Their basic definitions are my own wording.
- **Key concepts** are condensed from the lesson's overview, objectives, presenter notes, discussion goals, and Check for Understanding.

Source: Code.org CS Principles (2025–26), Unit 3 lesson plans, licensed CC BY-NC-SA 4.0. Changes made: content condensed, reorganized, and paraphrased; teacher-facing material removed.

## Lesson 1: Introduction to Apps

**Vocabulary**

| Term | Definition |
| --- | --- |
| Input | data that are sent to a computer for processing by a program. Can come in a variety of forms, such as tactile interaction, audio, visuals, or text. |
| Output | any data that are sent from a program to a device. Can come in a variety of forms, such as tactile interaction, audio, visuals, or text. |
| User Interface | the inputs and outputs that allow a user to interact with a piece of software. User interfaces can include a variety of forms such as buttons, menus, images, text, and graphics. |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Target Audience | The group of people an app is designed for |

**Key concepts**

- Apps are computing innovations designed to solve a problem or provide a service, such as entertainment, social connection, shopping, or finding information.
- Every app has a purpose (what it's meant to do) and a target audience (who it's for). Knowing the purpose helps a developer design with specific goals in mind.
- Computers take input, store and process it, and produce output.
- Apps collect input from users or other programs (button clicks, screen taps, typed text) and produce output (images, text, sounds, video). Output is usually based on input or on how the program was set up.
- Users interact with an app through its user interface.

## Lesson 2: Introduction to Design Mode

**Vocabulary:** No formal vocabulary.

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Design Mode | The part of App Lab used to lay out an app's screens and elements without writing code |
| Element | A single piece of a user interface, such as a button, label, text input, image, or dropdown |
| Element ID | The name given to an element so the program can refer to it |

**Key concepts**

- Design Mode in App Lab is used to build an app's user interface: screens, buttons, text, and images.
- Each element has properties that depend on its type. A label has text alignment and font, and an image has fit settings. Themes set an app's overall look, but any element's design can be overridden.
- Elements that collect input include buttons, text inputs, checkboxes, radio buttons, and dropdowns. Elements that display output include images and text. Most elements can do both, since they can all be clicked and change their content.
- Element IDs should have meaningful names so that it's clear which element is which when you write code.

## Lesson 3: Project – Designing an App Part 1

**Vocabulary:** No formal vocabulary.

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Prototype | A sketch or simple model of an app used to plan its look and features before programming it |
| Bias | An unfair assumption or preference, often based on one person's own experiences, that can show up in an app's content or design |

**Key concepts**

- User interfaces should be designed around the end user's needs. Designs that misjudge users (too much or too little guidance, the wrong device, wrong assumptions about interests) don't work well for them.
- This two-day project starts students' own educational app, built with a partner. Day 1 is brainstorming, choosing a topic, surveying classmates about their needs, and sketching screens. Day 2 is building those screens in Design Mode only, with no code yet.
- Collaboration improves apps. Team members with different experiences can catch bias in each other's content and design choices.
- A development process (formal vocabulary in Lesson 7) breaks app building into small steps. Most combine investigating and reflecting, designing, prototyping, and testing. Some are ordered and some are more exploratory.
- Planning saves time and lets developers test ideas with users before building. Designs often get simpler when they move from paper to screen, and that's fine.

## Lesson 4: The Need for Programming Languages

**Vocabulary:** No formal vocabulary.

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Natural Language | Everyday human language, like English or Spanish |
| Programming Language | A structured, precise language for giving a computer instructions, where each command has one exact meaning |

**Key concepts**

- Writing clear instructions is hard. Even careful instructions turn out to be vague when someone else tries to follow them.
- The core problem is that natural language is ambiguous. Words can have several meanings, so instructions can be interpreted in more than one way.
- Programming languages exist to fix this. They're more structured and precise so instructions can be followed correctly every time, with no room for interpretation.
- A program is a set of instructions for a computer. Programming languages may look like English but differ from it because they must be precise and unambiguous.

## Lesson 5: Intro to Programming

**Vocabulary**

| Term | Definition |
| --- | --- |
| Event Driven Programming | some program statements run when triggered by an event, like a mouse click or a key press |
| Program | a collection of program statements. Programs run (or "execute") one command at a time. |
| Program Statement | a command or instruction. Sometimes also referred to as a code statement. |
| Sequential Programming | program statements run in order, from top to bottom |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| String | Text data, written inside quotation marks. Numbers don't need quotes. |

**Key concepts**

- Code runs one line at a time. In App Lab, yellow highlighting shows which line is running, and the speed slider slows execution down so you can watch it.
- Key commands introduced:
    - `console.log` prints text in the Debug Console and takes one input.
    - `setProperty` changes an element's properties (the same ones from Design Mode) and takes three inputs.
    - `onEvent` runs the code inside it only when a chosen event (click, mouseover, and others) happens on an element.
    - `setScreen` switches screens and is used inside `onEvent` to let users navigate.
    - `playSound` plays a sound from the Sound Library.
    - `randomNumber` picks a new random number between a low and high value each time it runs.
- Code outside an `onEvent` runs right away, even if it comes after an `onEvent` in the program. Code inside an `onEvent` waits for the event.
- Sequential programs run top to bottom all at once. Event-driven programs respond to user actions.
- Lines starting with // are comments (formal vocabulary in Lesson 6). They explain the code but don't run.
- Programming languages are more precise than natural language and have strict rules. Programs need to work for a variety of inputs.
- Describing a program's behavior means explaining both what it does and how its statements accomplish it.

## Lesson 6: Debugging

**Vocabulary**

| Term | Definition |
| --- | --- |
| Comment | form of program documentation written into the program to be read by people and which do not affect how a program runs |
| Debugging | Finding and fixing problems in an algorithm or program |
| Documentation | a written description of how a command or piece of code works or was developed |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Bug | An error or problem in a program that keeps it from working as intended |
| Breakpoint | A marker that pauses a program at a specific line so you can check what's happening |

**Key concepts**

- Debugging is a normal, expected part of programming. Code often doesn't work the first time, and debugging is a skill that improves with practice.
- Debugging follows a process made of many small steps, including documenting what you learned and which strategies worked.
- Tools that help: yellow warnings in the code, the speed slider, breakpoints, and documentation.
- Common bugs: strings missing quotes, values outside the intended range (found by testing with different values), a missing event handler, and an `onEvent` placed inside another `onEvent` (event handlers should never be nested).
- Code can run with no warnings and still be wrong. Testing the app is the only way to catch that kind of bug.
- Comments and documentation are written for people, not the computer, so others can understand your code. Write them as you go, not just at the end. If an environment doesn't support comments, keep documentation in a separate file.
- Working with classmates and searching for bugs more effectively are also debugging skills.

## Lesson 7: Project – Designing an App Part 2

**Vocabulary**

| Term | Definition |
| --- | --- |
| Development Process | the steps or phases used to create a piece of software. Typical phases include investigating, designing, prototyping, and testing. |
| Pair Programming | a collaborative programming style in which two programmers switch between the roles of writing code and tracking or planning high level progress |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Driver / Navigator | The two pair programming roles. The driver writes the code, and the navigator tracks progress and plans ahead. |
| Program Specification | A plan describing what an app should do and how it should behave, used to guide building and testing it |
| Event Handler | Code that runs in response to an event, such as an `onEvent` block |

**Key concepts**

- These final three days of the unit project add code to students' apps, gather feedback, and finish the apps.
- In pair programming, partners switch between driver and navigator every few minutes. It helps because talking through code clarifies thinking, a partner can help when you're stuck, two people catch more bugs, and different perspectives improve the project.
- An app's program specification guides which event handlers it needs. It's also what testers use to check whether features work as described.
- Good feedback is specific and explains why something needs work. Unhelpful feedback is vague or only negative.
- Testing with other users catches bugs you overlooked and shows what isn't obvious to them. Feedback is valuable even before an app is finished.
- Feedback and testing make apps work as designed and drive gradual improvement, which is iterative development.
