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

### 1. Repository Creation
_(Add Screenshot Here)_

### 2. Creating and Switching to `dev` Branch
_(Add Screenshot Here)_

### 3. Implementing Calculator Features
_(Add Screenshot Here)_

### 4. Committing and Pushing Changes
_(Add Screenshot Here)_

### 5. Merging `dev` into `main` (Version 1.0 Release)
_(Add Screenshot Here)_

### 6. Creating Feature Branch `feature/sqrt`
_(Add Screenshot Here)_

### 7. Fixing the Division Bug in `dev`
_(Add Screenshot Here)_

### 8. Merging `feature/sqrt` into `dev` and Creating Version 2.0
_(Add Screenshot Here)_

## Conclusion
The **CalculatorPlus** application successfully implements basic arithmetic operations along with the square root feature. The Git workflow includes proper branching, merging, and release management, ensuring a structured development process.

---
**Repository Link:** _(Add Link Here)_

