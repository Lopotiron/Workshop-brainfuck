# Brainfuck Coding Workshop

## Workshop Outline

1. [Quick Introduction to Brainfuck Basics](#introduction)
2. [Hands-On Coding Exercises with Core Commands](#core-commands)
3. [Building Incrementally Complex Programs](#complex-programs)
4. [Creating a &#34;Hello, World!&#34; Together](#hello-world)
5. [Coding Challenges and Mini-Projects](#challenges)

## 1. Quick Introduction to Brainfuck Basics

- **Memory and Pointer**: Brainfuck operates on a **memory array** with a **pointer**. The pointer starts at the first cell (initially set to 0).
- **Commands Overview**:
  - `>` : Move pointer to the **right**.
  - `<` : Move pointer to the **left**.
  - `+` : **Increment** value at the pointer.
  - `-` : **Decrement** value at the pointer.
  - `.` : **Output** the character corresponding to the cell’s ASCII value.
  - `,` : **Input** one character into the current cell.
  - `[` : Start a **loop** (runs if the current cell is not zero).
  - `]` : End of loop.

## 2. Hands-On Coding Exercises with Core Commands

Each exercise introduces key commands. Participants should try each exercise and discuss solutions.

### Exercise 1: Simple Output

- **Goal**: Output a single character using `.`.
- **Task**: Set the first cell to ASCII 65 (`A`) and print it.
- **Solution**:
  ```brainfuck
  +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++.  # ASCII 65 for 'A'
  ```

### Exercise 2: Multiple Characters

- **Goal**: Output multiple characters in sequence.
- **Task**: Output "HI" by setting two cells to ASCII values for `H` (72) and `I` (73).
- **Solution**:
  ```brainfuck
  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++.
  >+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++.
  ```

### Exercise 3: Basic Input and Output

- **Goal**: Use `,` to accept input and then output it.
- **Task**: Read a character and output it twice.
- **Solution**:
  ```brainfuck
  ,.
  .
  ```

## 3. Building Incrementally Complex Programs

These exercises use combinations of commands to build simple logic.

### Exercise 4: Loop to Set a Value

- **Goal**: Use `[ ]` to create loops.
- **Task**: Set a cell to "2" using a loop.
- **Solution**:
  ```brainfuck
  +++++[>++++++++++<-]>.
  ```

### Exercise 5: Simple Counter

- **Goal**: Create a countdown using a loop.
- **Task**: Set the cell to "5", then decrement and output it until it reaches 0.
- **Solution**:
  ```brainfuck
  +++++[>++++++++++<-]>+++
  <+++++[>.-<-]
  ```

### Exercise 6: Character Printer

- **Goal**: Print a character sequence (e.g., "ABC").
- **Task**: Use loops to print "ABC" by incrementing the values.
- **Solution**:
  ```brainfuck
  ++++++[>++++++++++<-]>+++++
  <++[>+<-]>.
  ```

### Exercise 7: Number Printer

* **Goal:** Make a number printer.
* **Task:** Create a sequence where you can print any number by incrementing from 0 up to 9. Use loops in it
* **Solution:**

  ```
  +++++[>+++++++++<-]>+++.
  ```

## 4. Creating a "Hello, World"

**Goal**: Guide participants in writing a "Hello, World" program.

```brainfuck
>++++++++[<+++++++++>-]<.
---.
+++++++..
+++.
>>>+++++[<++++++>-]<++.
>>>++++++++[<++++++++++>-]<+++++++.
--------.
+++.
------.
--------.
```

- **Breakdown**:
  - Guide through setting ASCII values.
  - Use loops for fast incrementing.
  - Test each part as you go.

## 5. Coding Challenges and Mini-Projects

### Challenge 1: Custom Greeting

- **Goal**: Modify "Hello, World!" to print a custom greeting like "Hello, Brainfuck!".

### Challenge 2: Number Printer

- **Goal**: Write a program that outputs the numbers `1` to `5` in sequence, each on a new line.

### Challenge 3: Simple Addition

- **Goal**: Write a program that takes two single-digit inputs, adds them, and outputs the result.
  - **Hint**: Store the first input, move to a new cell for the second, then add the cells and print the sum.

### Challenge 4: ASCII Art

- **Goal**: Create a simple ASCII art pattern using character output commands.
  - **Example**: Try to make a smiley face using characters like `:-)`.

### Challenge 5: Calculator

* **Goal:** Take 2 basic numbers and addition them, do one for substractions.
  * **Example:** Take 2 and 3 from input and do 2 + 3 then print it
