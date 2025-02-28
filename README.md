# git_assignment_HeroVired

## Overview
This project is part of the **HeroVired Git Assignment**. It is a simple calculator application called **CalculatorPlus** that supports basic arithmetic operations and square root calculations. The project follows a structured Git workflow, including branching, merging, and release management.

## Features Implemented
- Addition
- Subtraction
- Multiplication
- Division (with zero-division handling)
- Square Root Calculation

## Git Workflow Steps

### 1. Repository Setup
- Created a **private GitHub repository**: `git_assignment_HeroVired`
- Cloned the repository locally

### 2. Created the Development Branch
```bash
  git checkout -b dev
```

### 3. Implemented Calculator Features
- Added basic arithmetic operations
- Implemented the square root function
- Fixed the division bug to handle division by zero

### 4. Committing and Pushing Changes
```bash
  git add calculator.py
  git commit -m "Added calculator"
  git push origin dev
```

### 5. Merging Changes into Main
- Merged `dev` into `main` after testing
- Created **Version 1.0 Release**

### 6. Creating Feature Branch for Square Root
```bash
  git checkout -b feature/sqrt
```
- Implemented and tested the square root feature
- Committed and pushed changes

### 7. Fixing the Division Bug in `dev`
```bash
  git checkout dev
  git merge feature/sqrt
  git checkout feature/sqrt
  git merge dev
```

### 8. Merging and Releasing Version 2.0
- Merged `feature/sqrt` into `dev`
- Merged `dev` into `main`
- Created **Version 2.0 Release**

## Screenshots

### Repository Creation
![image](https://github.com/user-attachments/assets/2e6c1dd4-fd00-4edc-b0cf-6907cbb401d3)

### Implementing Calculator Features and fixing the Division Bug
![image](https://github.com/user-attachments/assets/d4abfd35-f4da-43f6-b4bc-e23c5f9a5ff3)

### Output 
![image](https://github.com/user-attachments/assets/c4a2257e-9ce4-4fa6-826a-3268d5c9ba86)




## Conclusion
The **CalculatorPlus** application successfully implements basic arithmetic operations along with the square root feature. The Git workflow includes proper branching, merging, and release management, ensuring a structured development process.


