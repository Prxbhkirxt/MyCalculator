# Simple Calculator App

A clean and functional Android calculator application built using Java and Android Studio for the GDG App Development Round 2 task.

## Overview
This application performs standard mathematical calculations in real time using expression parsing powered by Mozilla Rhino.

## Features
- **Arithmetic Operations:** Addition (+), Subtraction (-), Multiplication (*), Division (/)
- **Expression Evaluation:** Supports compound expressions and bracket grouping `(` `)`
- **Clear & All Clear:**
  - `C`: Clears the last entered character/digit
  - `AC`: Resets both input and result fields
- **Formatting:** Automatically truncates unnecessary `.0` suffixes for whole-number calculations

## Tech Stack
- **Language:** Java
- **UI:** XML Layouts with Google Material 3 Design
- **Engine / Library:** Mozilla Rhino (`org.mozilla:rhino:1.7.14`)
- **IDE:** Android Studio

## How It Works
1. Button inputs are dynamically appended to a calculation string shown in the expression display.
2. The expression is passed to the embedded JavaScript runtime (Rhino Context) to evaluate mathematical precedence accurately.
3. The result is calculated and displayed live in the result TextView.
