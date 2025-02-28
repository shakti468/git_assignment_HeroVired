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
This application successfully implements basic arithmetic operations along with the square root feature. The Git workflow includes proper branching, merging, and release management, ensuring a structured development process.

---


# Git LFS for Large Files (Question 2)

## **Introduction**
Git LFS (Large File Storage) is a Git extension that allows handling large binary files efficiently by storing them outside the main repository.

## **Step 1: Install Git LFS**
Before using Git LFS, ensure it is installed on your system.

**Command:**
```bash
 git lfs install
```

### **Screenshot:** Git LFS Installation Confirmation

## **Step 2: Initialize Git LFS in the Repository**
Run the following command to initialize Git LFS in your repository:
```bash
git lfs install
```

### **Screenshot:** Git LFS Initialization

![image](https://github.com/user-attachments/assets/afc84acf-dfe4-4e61-8d71-44db32873d8e)


## **Step 3: Track Large Files with Git LFS**
To track specific file types (e.g., MP4 videos), run:
```bash
git lfs track "*.mp4"
```

### **Screenshot:** Tracking Large Files with Git LFS

![image](https://github.com/user-attachments/assets/dc137d3a-b678-45ae-88fc-01bec182ea5d)


## **Step 4: Verify .gitattributes File**
Check if `.gitattributes` has the correct entry for the large files:
```bash
cat .gitattributes
```
The output should be:
```
*.mp4 filter=lfs diff=lfs merge=lfs -text
```

### **Screenshot:** .gitattributes File Configuration
![image](https://github.com/user-attachments/assets/33dc4b02-21ee-458c-9e9a-22dcc7d76058)


## **Step 5: Add and Commit Large File**
Now, add and commit the large file:
```bash
git add .gitattributes

git add SampleVideo.mp4

git commit -m "Added large video file using Git LFS"

git push origin lfs
```

### **Screenshot:** Adding and Committing the Large File

![image](https://github.com/user-attachments/assets/35d18314-74a1-4ab0-9005-65fba2c1794f)


## **Step 6: Verify Git LFS Tracking**
To ensure Git LFS is tracking the file correctly, use:
```bash
git lfs ls-files
```
This should list the file being tracked by Git LFS.

### **Screenshot:** Verifying LFS-Tracked Files

![image](https://github.com/user-attachments/assets/28460864-5734-4c96-adc9-704b8b25a17d)


## **Step 7: Clone the Repository on Another Machine**
To verify that Git LFS is correctly handling the file, clone the repository on another machine:
```bash
git clone https://github.com/shakti468/git_assignment_HeroVired.git
cd git_assignment_HeroVired
ls -lh SampleVideo.mp4
```
If the file is downloaded with the correct size, Git LFS is working properly.

## **Step 8: Merge `lfs` Branch into `main`**
After verifying everything, merge the `lfs` branch into `main`:
```bash
git checkout main
git merge lfs
git push origin main
```

### **Screenshot:** Merging LFS Branch into Main

![image](https://github.com/user-attachments/assets/ba463703-6c30-4dd7-9c54-4d804cdabb91)


## **Conclusion**
Git LFS successfully helps manage large files efficiently in Git.

---






