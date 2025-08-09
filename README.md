# Loops-in-C-plus-plus

## Overview
In C++, loops are used to execute a block of code repeatedly based on a condition.  
They are essential in controlling the flow of programs, especially when performing repetitive tasks such as iterating through arrays, processing input, or executing logic multiple times.

**Common types of loops include:**
- **for loop** – iterates a fixed number of times.
- **while loop** – continues as long as a condition is true.
- **do-while loop** – executes the loop body at least once before checking the condition.

---

## Theory

### 1. For Loop
Used when the number of iterations is known.

### 2. While Loop
Used when the number of iterations is not known and depends on a condition.

### 3. Do-While Loop
Runs at least once regardless of the condition.

---

### Loop Control Statements in C++:
- **break** – Terminates the loop prematurely.
- **continue** – Skips the current iteration and moves to the next.
- **goto** – Jumps to a labeled statement (not recommended for regular loop control).

---

## Program Analysis

### 1. Print 'SIT' 5 times
Demonstrates a simple `for` loop which prints `"SIT"` 5 times, each on a new line.

### 2. Print Even Numbers from 0 to 10
Uses conditional logic and controlled incrementing inside the loop to print even numbers from 0 to 10.

### 3. Validating Password from User by While Loop (A Working Login Page)
Demonstrates user input validation and multiple loop exits by taking input from the user and validating it using an `if` condition.

## Overview
This program simulates a simple login system for **SIT Pune website**.  
It allows a user to:
- Set up a password during account creation.
- Attempt login by entering the correct password.
- Change password if the user remembers the current one.
- Get admin help if the password is forgotten.
- Exit from the login system.

The program demonstrates the use of:
- **Variables** for storing user data.
- **Loops** (`while`) for repeated login attempts.
- **Conditional statements** (`if`, `else if`, `else`) for decision-making.
- **Nested conditions** for verifying password changes.

---

## Theory
The program works on the principle of **authentication and access control**.  
It performs the following:
1. **Registration Phase**  
   - User enters PRN (unique ID).
   - User sets a numeric password.

2. **Login Phase**  
   - User attempts to log in by entering the password.
   - If the password matches, the login is successful.
   - If the password does not match, the user is given multiple options:
     - **Change password** (requires entering current password correctly).
     - **Forgot password** (contact admin).
     - **Exit** from the login process.

3. **Control Flow**  
   - The `while(true)` loop ensures the login process repeats until:
     - The user logs in successfully.
     - Or the user chooses to exit.

This structure is similar to **real-world login mechanisms** where multiple attempts and recovery options are available.

---

## Algorithm
1. Start.
2. Display welcome message for SIT Pune website.
3. Ask the user to enter **PRN**.
4. Ask the user to set a **numeric password**.
5. Start an infinite loop (`while(true)`):
   1. Ask the user to enter the password.
   2. If entered password matches the stored password:
      - Display "Login successful" and set `loggedIn = true`.
      - Exit the loop.
   3. Else:
      - Display "Incorrect password" and options:
        1. Change password:
           - Ask for current password.
           - If correct, ask for new password and update it.
           - Else, display error message.
        2. Forgot password:
           - Display admin contact details.
        3. Exit:
           - Display exit message and break loop.
        4. Any other input:
           - Display "Invalid option".
6. End.

---

### 4. Print Digits in Reverse Order of a Number
Uses a `for` loop with modulus and division to reverse digits and print them one per line.

### 5. Nested For Loop
Shows how nested loop control works: the outer loop runs first for one iteration, then the inner loop executes, and control moves back to the outer loop.
# Nested For Loop in C++

## Overview
In C++, **nested loops** occur when one loop is placed inside another loop.  
The **outer loop** controls how many times the **inner loop** executes.  
This structure is useful for:
- Printing patterns
- Processing 2D arrays
- Generating combinations of data

In this program, the outer loop runs first, and for each iteration of the outer loop, the inner loop runs completely.

---

## Theory
- **Outer Loop**: `for(int i = 1; i <= 2; i++)`
  - Runs **2 times** and controls the main iteration.
- **Inner Loop**: `for(int j = 1; j <= 3; j++)`
  - Runs **3 times** for **each** outer loop iteration.
- **Execution Flow**:
  1. Outer loop starts → prints `Outer` value.
  2. Inner loop runs fully → prints `Inner` values from 1 to 3.
  3. Outer loop increments and repeats.

**Key Points**:
- Total iterations = Outer loop count × Inner loop count.
- Inner loop always completes before outer loop increments.
- Commonly used in matrix operations, tables, and patterns.

---

## Algorithm
1. **Start**
2. Initialize outer loop counter `i = 1`
3. While `i <= 2`:
   - Print `"Outer: i"`
   - Initialize inner loop counter `j = 1`
   - While `j <= 3`:
     - Print `"Inner: j"`
     - Increment `j` by 1
   - Increment `i` by 1
4. **End**

### 6. Printing Star Pattern
Builds a basic triangle shape using stars and prints them left-aligned.

### 7. Printing Reverse Star Pattern
Combines spacing and star printing for alignment, producing a right-aligned pattern.

### 8. Floyd’s Series
Prints numbers in ascending order as per the series, each on a new line, using a nested `for` loop.

## Overview
This C++ program prints a **right-angled triangle** of numbers.  
The numbers start from `1` and increase sequentially in each row.  
The variable `n` defines the number of rows in the triangle.

---

## Theory
- The program uses **nested loops**:
  - **Outer loop** (`i`): Controls the number of rows.
  - **Inner loop** (`j`): Prints numbers in each row.
- The variable `num` stores the current number to be printed and increments after every print.
- Each new row contains one more number than the previous row.

---

## Algorithm
1. **Start** the program.
2. Initialize:
   - `n = 4` (number of rows)
   - `num = 1` (starting number)
3. Loop `i` from `1` to `n`:
   - Loop `j` from `1` to `i`:
     - Print `num` followed by a space.
     - Increment `num` by 1.
   - Print a newline after each row.
4. **End** the program.

### 9. Hourglass Pattern
Prints a symmetric hourglass pattern using two `for` loops — one for the upward triangle and one for the downward triangle.

## Overview
This C++ program prints a **diamond-like pattern** using asterisks (`*`).  
It makes use of **nested loops** to handle both spaces and stars in each row.  
The variable `n` determines the number of rows in each half of the pattern.

---

## Theory
- The program uses **nested loops**:
  - **Outer loop**: Controls the number of rows.
  - **First inner loop**: Prints spaces for alignment.
  - **Second inner loop**: Prints stars with spaces between them.
- The first section creates an **inverted triangle** of stars.
- The second section creates a **normal triangle** of stars.
- By combining both sections, the program produces a diamond-like shape.

---

## Algorithm
1. **Start** the program.
2. Initialize variables `i`, `j`, `k` and set `n = 5`.
3. **Upper Half (Inverted Triangle)**:
   - Loop `i` from `n` down to `1`:
     - Loop `j` from `1` to `n - i` → print spaces.
     - Loop `k` from `1` to `i` → print stars followed by a space.
     - Print a newline.
4. **Lower Half (Normal Triangle)**:
   - Loop `i` from `2` to `n`:
     - Loop `j` from `1` to `n - i` → print spaces.
     - Loop `k` from `1` to `i` → print stars followed by a space.
     - Print a newline.
5. **End** the program.

---

---

## Conclusion
Loops in C++ are powerful tools that simplify repetitive tasks, enhance logic control, and improve code readability.  
Mastering loops (along with control statements like `break` and `continue`) is essential for writing efficient and dynamic C++ programs.  
Whether you’re iterating through data, checking conditions, or building algorithms — **loops are at the heart of C++ programming**.

   
