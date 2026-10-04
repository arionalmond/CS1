# CSP Unit 1 – Digital Information: Vocabulary & Concepts

## How to read this

Each lesson lists only what's new: formal vocabulary and the concepts students should walk away with. Timing, prep, links, teaching tips, and teacher dialogue are cut.

- **Vocabulary** is copied word for word from the lesson's formal vocabulary box. Lessons without a box say "No formal vocabulary" and get concepts only.
- **Key concepts** are condensed from the lesson's overview, objectives, presenter notes, discussion goals, and Check for Understanding.

Source: Code.org CS Principles (2025–26), Unit 1 lesson plans, licensed CC BY-NC-SA 4.0. Changes made: content condensed, reorganized, and paraphrased; teacher-facing material removed.

## Lesson 1: Welcome to CSP

**Vocabulary:** No formal vocabulary.

**Key concepts**

- A technological (computing) innovation starts by spotting a problem or something that needs improving, then building a tool to address it.
- A prototype is a quick, simple sketch or model of an idea, made before anything real is built.
- Computing innovations have both positive and negative effects, and they touch almost every area of life and interest.

## Lesson 2: Representing Information

**Vocabulary:** No formal vocabulary.

**Key concepts**

- Computer science is more about information than about computers. A working definition: information is the answer to a question.
- The same information can be represented in many different ways.
- A device with only two options can send more than two messages by using those options in sequences. Two options repeated twice give 4 messages, three times give 8, and four times give 16.
- Reusing two options in sequence scales better than inventing a new signal for every new message. This is the foundation for how computers represent complex information with bits.

## Lesson 3: Circle Square Patterns

**Vocabulary:** No formal vocabulary.

**Key concepts**

- A numeral like "7" is just one agreed-upon symbol for a number. The same number can be written with words, pictures, math expressions, or other symbols.
- With two symbols (circle and square), 3 place values make 8 possible patterns and 4 place values make 16.
- A number system needs clear, shared ordering rules so that everyone lists the patterns in the same order and the same pattern always means the same number.
- Rules that work for 3 place values usually need to be changed or extended to work for 4. This sets up binary in the next lesson.

## Lesson 4: Binary Numbers

**Vocabulary**

| Term | Definition |
| --- | --- |
| Binary | A way of representing information using only two options |
| Bit | A contraction of "Binary Digit"; the single unit of information in a computer, typically represented as a 0 or 1 |
| Byte | 8 bits |
| Decimal | A way of representing information using ten options |

**Key concepts**

- Decimal is base 10 (symbols 0–9) and binary is base 2 (symbols 0 and 1). Both use place value.
- Decimal place values are powers of 10. Binary place values are powers of 2 (1, 2, 4, 8, 16, …), increasing from right to left.
- When a place reaches its last symbol, it rolls over to 0 and adds 1 to the next place on the left (9 → 10 in decimal, 1 → 10 in binary).
- To convert decimal to binary, put a 1 in the largest place value that fits, subtract it, and repeat. Example: 10 = 8 + 2 = 1010.
- Each added bit doubles the number of values. n bits give 2ⁿ values, from 0 up to 2ⁿ − 1 (4 bits: 16 values, 0–15).
- Odd binary numbers end in 1 and even ones end in 0. Numbers with exactly one 1 are powers of 2.
- Adding 0s to the left of a binary number doesn't change its value. Adding a 0 to the right doubles it.
- Computers use binary because electrical signals have two states, on (1) and off (0).

## Lesson 5: Overflow and Rounding

**Vocabulary**

| Term | Definition |
| --- | --- |
| Overflow Error | Error from attempting to represent a number that is too large |
| Round-off Error | Error from attempting to represent a number that is too precise. The value is rounded. |

**Key concepts**

- A number system is infinite, but any physical representation has a fixed number of place values. Bits can only represent a limited amount of information.
- Overflow happens when a value needs more place values than are available. The digits roll over to 0 but there's no place left for the carried 1, so the stored value is wrong (like an odometer rolling past its maximum).
- An 8-bit Flippy Do overflows at 256. Adding a 9th bit moves the overflow point to 512. Adding bits pushes the limit higher, but any fixed number of bits will eventually overflow.
- Round-off happens when a value is more precise than the available place values can show. Some fractions can't be represented exactly, so the value has to be rounded.
- Rounding choices have real consequences (for example, whether the shop or the customer absorbs the difference), and systems depend on consistent precision.
- Students don't need to convert fractional decimals to binary.

## Lesson 6: Representing Text

**Vocabulary:** No formal vocabulary.

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| ASCII | American Standard Code for Information Interchange; a standard that assigns a number to each letter, digit, and symbol so computers can store and share text |
| Abstraction | Simplifying something complex by hiding its details so you can focus on the bigger picture |

**Key concepts**

- Numbers can represent any kind of information, including text. Each character is assigned a number.
- Systems for representing text are somewhat arbitrary. They work because many people agree to use the same one, not because there's one right answer.
- More characters (spaces, punctuation, capitals, digits) need more numbers, and therefore more bits per character. With a fixed number of bits per character, you can run out, which ties back to overflow.
- ASCII (American Standard Code for Information Interchange) is a standard that assigns a number to the characters on an American keyboard. Students should know it exists but don't need to memorize the table.
- Abstraction means creating a simplified representation of something more complex so you can hide details and focus on the problem at a higher level. Text is an abstraction built on numbers, which are built on bits.
- The same bit pattern can mean different things depending on context. For example, 01000001 is 65 as a number but "A" in ASCII.

## Lesson 7: Black and White Images

**Vocabulary**

| Term | Definition |
| --- | --- |
| Analog Data | Data with values that change continuously, or smoothly, over time. Some examples of analog data include music, colors of a painting, or position of a sprinter during a race. |
| Digital Data | Data that changes discretely through a finite set of possible values |
| Sampling | A process for creating a digital representation of analog data by measuring the analog data at regular intervals called samples. |

**Key concepts**

- A black and white image can be stored as a grid of pixels, one bit per pixel. In the Pixelation Widget, 0 is black and 1 is white.
- An analog image (like a pencil drawing) changes smoothly. To make it digital, you sample it: divide it into squares of equal size and record one value per square.
- Smaller samples (more pixels) give a closer approximation but need more bits and more work. Larger samples need fewer bits but look blockier and less accurate.
- Even with frequent sampling, a digital image is only an approximation of the analog original. Squares that are part black and part white still force a choice.
- How often to sample depends on the situation. The trade-off is accuracy versus the number of bits.
- Bits have now represented numbers, text, and images. The same bit sequence can mean different things depending on context.

## Lesson 8: Color Images

**Vocabulary:** No formal vocabulary.

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| RGB | Red, Green, Blue; the three colors of light mixed in each pixel to make the colors on a screen |
| Metadata | Data that describes other data, such as an image's width, height, and bits per pixel |

**Key concepts**

- Each color pixel is made of red, green, and blue (RGB) light. Bits control how much of each light is on.
- More bits per pixel means more possible colors: 3 bits give 8 colors, 6 bits give 4 shades of each of red, green, and blue, and 9 bits give 8 shades of each.
- Metadata is data that explains other data. In the widget, it's the image's width, height, and bits per pixel.
- Analog color changes smoothly and continuously. A digital image can only show a finite number of colors, changing in discrete steps across equal-sized pixels. A digital image is always an approximation.
- A digital color image is built from layers that work together: sampling decides the pixels, RGB sets each pixel's color, and binary stores the values. Not having to think about every layer at once is an example of abstraction.

## Lesson 9: Lossless Compression

**Vocabulary**

| Term | Definition |
| --- | --- |
| Lossless Compression | A process for reducing the number of bits needed to represent something without losing any information. This process is reversible. |

**Key concepts**

- Compression represents the same information with less data, saving time and space (like abbreviations in a text message).
- In dictionary-based compression, repeated patterns are replaced with symbols. The compressed text and the dictionary (key) must both be sent, or the receiver can't rebuild the message.
- Lossless compression is reversible. The original can always be recreated exactly, with no information lost.
- Compression percentage compares the bytes in the original with the bytes in the compressed version.
- Data with lots of repetition compresses well. Data with little repetition doesn't, and some strategies can even make the result bigger.
- There's no single best strategy. Results depend on the method chosen and the patterns in the data.

## Lesson 10: Lossy Compression

**Vocabulary**

| Term | Definition |
| --- | --- |
| Lossy Compression | A process for reducing the number of bits needed to represent something in which some information is lost or thrown away. This process is not reversible. |

**Key concepts**

- Lossy compression permanently throws away some information, so the original can't be recreated exactly. Removing vowels from text is an example, and the result can become ambiguous.
- For images, a larger sample size gives a smaller file but a worse-looking image. A smaller sample size gives a better image but a larger file.
- The goal is a balance: compress as much as possible while the result is still good enough for its purpose.
- Use lossless compression when exact accuracy matters most (bank records, text files, some images).
- Use lossy compression when file size or speed matters more than perfect quality, especially for multimedia and streaming (images, video, audio).
- The right choice depends on the situation. Usually there's no single correct answer, just trade-offs to weigh.

## Lesson 11: Intellectual Property

**Vocabulary**

| Term | Definition |
| --- | --- |
| Creative Commons | A collection of public copyright licenses that enable the free distribution of an otherwise copyrighted work, used when an author wants to give people the right to share, use, and build upon a work that they have created |
| Intellectual Property | A work or invention that is the result of creativity, such as a piece of writing or a design, to which one has rights and for which one may apply for a patent, copyright, trademark, etc. |

**Key concepts**

- Work you create on a computer is your intellectual property. Using someone else's work as your own without permission is plagiarism and can have legal consequences.
- Ownership gets complicated when analog works become digital. A digital image is ultimately just a binary number, and it can be copied and spread easily.
- Copyright gives creators control over how their work is used. Creative Commons licenses let creators grant others permission to share, use, and build on their work.
- Other licenses that open up access: Open Source (programs made freely available that may be redistributed and modified) and Open Access (online research free of restrictions on access and use).
- When you use others' materials, cite your sources with as much information as possible.
- Digitizing a work can benefit some people and harm others, and these impacts can be intended or unintended. Students argue whether current copyright policy helps or hurts society, using evidence from a text.

## Lesson 12: Project – Digital Information Dilemmas

**Vocabulary:** No formal vocabulary. This is a two-day project that applies the unit's concepts.

**Key concepts**

- Central question: Is the world better or worse because of digital representation?
- Analyzing a case of digitization means identifying four things: what was digitized and how it's represented (image or text, compressed or not, lossy or lossless), the goal of digitizing it, who benefits and who is harmed, and whether those impacts were intended or unintended.
- Digitizing analog content usually involves trade-offs. Students make an overall claim and support it with evidence from an article.
- The project pairs with the Unit 1 Assessment and closes with the Unit 1 vocabulary review.
