# SE-assignment2
Software Engineering Assignment #2

This repository demonstrates basic version control operations using **Git** and **GitHub** as part of the *CINS 5318 Software Engineering* course.

## Project Description
The project begins with a simple `Hello, World!` program and evolves through branching, feature additions, pull-requests, conflict resolution, and issue tracking.  
It illustrates how multiple contributors can collaborate, merge changes, and maintain clean commit history.


## Installation
Clone this repository and run `hello.py`.

1. Clone the repository:
    ```
    git clone https://github.com/your-username/SE-assignment2.git
    
    cd SE-assignment2
    ```
2. Ensure Python is installed (3.8 or newer).
3. Run the program:
    ```
    python hello.py
    ```

## Usage Example

Running hello.py prints:
    ```
    Hello, World!
    Hi! Paul Okoli
    ```


## Issues and Resolutions

### Issue #1 – Add Personalized Greeting Message to the Hello World Program

**Description:**
Extend the hello.py file to include a personalized greeting after the default message.
Demonstrates feature branching and pull-request workflow.

**Implementation Steps:**
1. Created a new branch feature-1.
2. Updated hello.py to print both the default and personalized greetings.
3. Committed and pushed changes with the message:
   ```
   git commit -m "Added personalized greeting feature, closes #1"
   ```
4. Opened and merged a pull request (feature-1 → main).

**Resolution:**
Successfully merged after code review. Issue automatically closed using commit keyword closes #1.


### Issue #2 – Resolve Merge Conflict between main & feature-2

**Description:**
Simulate and resolve a merge conflict by modifying the same line of code in both main and feature-2 branches.

**Implementation Steps:**
1. Modified hello.py in both main and feature-2 branches with different text.
2. Created a pull request from feature-2 to main, which triggered a merge conflict.
3. Pulled both branches locally and resolved the conflict manually by editing the file:
   ```
   print("Hello, World! from main and feature-2 combined.")
   ```
4. Committed the fix and pushed changes:
   ```
   git commit -m "Resolved merge conflict between the main & feature-2 branch, closes #2"
   ```

**Resolution:**
Conflict resolved locally and verified after merging. Issue automatically closed using commit keyword closes #2.