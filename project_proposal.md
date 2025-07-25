# Project Proposal: Digital Watch-Clock (Assembly Language)

This proposal outlines the plan to develop a **Digital Clock** using **Assembly Language** and the **Irvine32 library**. The project will create a real-time, text-based console clock that displays the current system time in `HH:MM:SS` format using ASCII-based 7-segment digits.


## Team Members

- **Dania Khan** (23K-0072)  
- **Zoha Ahmed** (23i-2555)  
- **Nimra Haq** (22F-3357)

## Objective

To implement a console-based digital clock in Assembly language that:
- Displays the current time in a digital format
- Updates the display every second
- Uses low-level screen control for visual output
- Demonstrates efficient real-time programming in Assembly


## Motivation

While modern languages simplify time and UI tasks, doing so in **Assembly** requires:
- Direct access to system APIs
- Manual screen rendering using characters
- Careful memory and CPU management

This challenge provides a great opportunity to strengthen our understanding of **hardware-level operations**, **system calls**, and **performance-sensitive design**.


## Problem Statement

Creating a dynamic digital clock in Assembly involves:
- Accessing system time without built-in libraries
- Displaying numbers using custom 7-segment ASCII graphics
- Updating only when a second changes, without flickering or overloading the CPU

## Scope

- The clock will display time in `HH:MM:SS` format
- Each digit will be rendered using a grid of characters to simulate a 7-segment display
- The clock will update once every second using system time from the Windows API
- The screen will refresh with minimal flicker and low CPU usage
- Output will be colorized (light cyan text on black background)


## 🛠 Technologies & Tools

- **Assembly Language (MASM)**  
- **Irvine32 Library** (for console and API support)  
- **Windows API** (`GetLocalTime`)  
- Windows Command Prompt (runtime environment)

## 🗂 Project Methodology

### 1. Planning
- Design 7-segment character representations
- Define layout for digits and colon separators

### 2. Development
- Use `GetLocalTime` to access system time
- Convert time values into digit representations
- Implement digit drawing logic with ASCII characters

### 3. Optimization
- Use `Delay` procedure to reduce CPU consumption
- Refresh only when the second value changes
- Ensure flicker-free screen updates


##  Project Timeline

| Week | Milestone                               |
|------|------------------------------------------|
| 1    | Research system time APIs and digit design |
| 2    | Implement digit rendering and formatting  |
| 3    | Integrate time fetching and display loop  |
| 4    | Optimize performance and refresh control  |
| 5    | Final testing, polish, and documentation  |


## Expected Learning Outcomes

- Master low-level programming and instruction handling in Assembly
- Develop efficient screen drawing techniques using ASCII characters
- Understand real-time system interaction using Windows APIs
- Gain hands-on experience in performance-aware coding
- Improve collaboration and structured development skills


## Success Criteria

- Clock accurately displays real-time system time
- Time updates once per second without skipping or flickering
- Output remains visually clean and color-enhanced
- Code is modular, efficient, and well-commented
- The project runs successfully on a Windows machine using MASM and Irvine32

## Conclusion

This project will showcase how real-time behavior, user output, and efficient design can be achieved in a low-level language like Assembly. It emphasizes learning through challenge and is a great stepping stone toward deeper understanding of embedded systems, OS development, and hardware interaction.

