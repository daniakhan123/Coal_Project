# 🕒 Digital Watch-Clock (Assembly Language Project)

This project demonstrates the implementation of a **Digital Clock** using **Assembly Language** and the **Irvine32** library. The clock displays the current time in `HH:MM:SS` format using 7-segment-style ASCII characters on a console screen. It updates every second and is optimized for low CPU usage.

---

## 👥 Group Members

- **Dania Khan** (23K-0072)  
- **Zoha Ahmed** (23i-2555)  
- **Nimra Haq** (22F-3357)

---

## 🚀 Features

- Displays real-time system clock in 7-segment ASCII format  
- Updates automatically every second  
- Uses `GetLocalTime` from Windows API for accurate timekeeping  
- Clean console display with:
  - Light cyan text  
  - Black background  
- Efficient CPU usage with 50ms refresh delay  

---

## 🛠 Technical Implementation

### 📁 Data Section

- **Time Variables**: Holds hours, minutes, and seconds  
- **Digit Patterns**: 7x8 ASCII representation of digits `0-9`  
- **Display Config**: Defines size and positioning of digits  

### 🧠 Code Structure

#### 1. `main` Procedure
- Retrieves current time via `GetLocalTime`  
- Detects second change to update display  
- Clears screen, sets text color  
- Displays time using custom `DisplayDigit` and `DisplayColon` functions  
- Introduces 50ms delay to reduce CPU load  

#### 2. Display Functions
- `DisplayDigit`: Renders numbers with ASCII 7-segment patterns  
- `DisplayColon`: Renders colon `:` symbol  

#### 3. Helper Procedures
- `Clrscr`: Clears the console screen  
- `SetTextColor`: Sets text color using Windows console attributes  
- `Gotoxy`: Moves the cursor to desired (x,y) position  
- `Delay`: Introduces delay in milliseconds  

---

## 💡 Learning Outcomes

- Hands-on experience with **Assembly language programming**  
- Low-level **screen manipulation** in console applications  
- Using **Windows system API** (`GetLocalTime`) in assembly  
- Efficient use of **CPU resources** with custom delays  
- Understanding of **digit-based pattern printing** in ASCII  

---

## 📦 Requirements

- **MASM** Assembler  
- **Irvine32** Library  
- **Windows OS** (for API support)

---

## ✅ Conclusion

This project effectively demonstrates the power and precision of **Assembly Language** in developing real-time, hardware-near applications. By building a functional digital clock that uses the system’s API and displays time in a visually structured 7-segment ASCII format, we explored critical concepts such as:

- Direct system interaction through API calls  
- Structured and modular low-level code design  
- Efficient console output rendering  
- Performance-optimized delay mechanisms

The clock project not only enhanced our technical understanding of **assembly programming**, but also prepared us for more advanced areas like **embedded systems**, **operating systems**, and **resource-constrained programming**. It stands as a testament to how low-level programming can produce clean, efficient, and interactive user-facing applications.

---

> 🔧 Built with MASM & Irvine32  
> 💻 Developed by Dania, Zoha, and Nimra  
