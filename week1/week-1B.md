---
marp: true
title: "Software Engineering Foundations - Week 1"
theme: default
paginate: true
---

# Week 1: Introduction & Foundations

---

## Slide 1: Welcome to Software Engineering

- **Course Roadmap**
  - Week 1—Foundations: computers, software, setup
  - Weeks 2–8: Coding basics, core concepts, projects, career guidance
- **Why learn Software Engineering?**
  - Problem solving using technology
  - High-demand, global career
  - Unlimited learning and growth potential

---

## Slide 2: What is Software Engineering?

- **Definition:**
  The branch of engineering that deals with designing, building, testing, and maintaining software.

- **Misconceptions:**

  - Not just writing code
  - Includes teamwork, design, planning, testing, deployment

- **Roles Explained:**

  - **Frontend Developer:** Makes websites/apps beautiful and interactive
    - Tools: HTML, CSS, JavaScript
    - Example: Building a landing page for an online shop
  - **Backend Developer:** Handles behind-the-scenes logic and data
    - Tools: Python, Java, Node.js, SQL
    - Example: Managing a database for customer orders
  - **Full-stack Developer:** Does both frontend and backend!
  - **DevOps Engineer:** Ensures things run smoothly, deploys updates
  - **QA (Quality Assurance):** Checks for errors, makes sure software works well

- **Teamwork:**

  - Most software is built by teams!
  - Communication and collaboration are just as important as technical skills

- **Career Paths & Industries:**

  - Tech, banking, health, education, gaming, research, retail, etc.
  - Software engineers work in startups, big corporations, freelancing, NGOs

- **Skills Needed:**
  - Analytical thinking
  - Problem solving
  - Creativity
  - Perseverance

---

## Slide 3: How Computers Work (for Beginners)

- **What is a Computer?**

  - A device that processes data, follows instructions, and produces results

- **Core Parts:**

  - **CPU:** The "brain"—processes instructions, makes decisions
  - **RAM (Memory):** Remembers what you’re working on right now
  - **Storage (Hard Drive, SSD):** Remembers everything, even when turned off
  - **Motherboard:** The "nervous system" connecting parts together
  - **Input Devices:** Keyboard, mouse, touchscreen
  - **Output Devices:** Monitor, printer, speakers

- **Software vs Hardware**

  - Hardware: Physical parts you can touch (CPU, keyboard, monitor)
  - Software: The instructions (apps, operating system, games, browsers)

- **How it Works Together:**

  - When you use a program (like Word), the CPU reads the instructions from the software, temporarily stores info in RAM, saves your document in storage, interacts with input/output devices

- **Analogy:**

  - Think of a computer as a kitchen:
    - Hardware: stove, fridge, utensils
    - Software: recipes
    - You (cpu): follow instructions (recipes) using tools

- **Common Mistakes Beginners Make:**
  - Mixing up storage and memory
  - Not understanding why computers slow down (too many programs in memory, low storage)

---

## Slide 4: Operating Systems (OS)

- **Definition:**
  The main software that manages hardware, files, and other software.

- **Popular Operating Systems:**

  - Windows (PC)
  - macOS (Mac)
  - Linux (Free, open source—used in many servers and developer tools)

- **Functions of OS:**

  - Boots up the computer
  - Manages user accounts
  - Handles files, folders, external devices (USB, printer)
  - Launches and closes programs

- **User Interface:**

  - GUI (Graphical User Interface): Icons, windows, menus
  - CLI (Command Line Interface): Text commands

- **Why Learn Navigation?**

  - All coding involves creating, saving, moving files and folders
  - A developer’s computer is always organized!

- **Basic OS Activities (Demo & Practice):**

  1. Create folders: `MyProjects`, `Assignments`, `Resources`
  2. Rename folders
  3. Move files between folders
  4. Delete a folder (and restore it from Trash/Recycle Bin)
  5. Open a file in an editor

- **Extra: Basic Command Line Commands**

  - On Windows:
    - `dir` (list files)
    - `mkdir NewFolder` (create new folder)
    - `cd NewFolder` (change directory)
  - On Mac/Linux:
    - `ls`
    - `mkdir NewFolder`
    - `cd NewFolder`

- **Troubleshooting:**
  - Can’t find created folder? Did you check the right directory?
  - Permission error? Try running your OS as administrator/sudo

---

## Slide 5: What is Programming?

- **Real Definition:**
  Programming is writing a set of instructions (called “code”) that a computer can execute to perform a task.

- **Examples of Programs:**

  - Calculator app
  - Instagram feed algorithm
  - ATM software
  - Website with signup/login

- **Programming Languages:**

  - **Python** (beginner-friendly, powerful)
  - **JavaScript** (for web browsers, interactive sites)
  - **Java, C, C++** (used for apps, games, system programs)

- **How Code Works:**

  1. You write code in a text editor.
  2. The computer reads and translates it (compiler/interpreter).
  3. The computer follows the instructions step by step.

- **Analogy:**

  - Programming is like writing a recipe:
    - Step-by-step instructions for a successful dish
    - Precise order, clear measurements (syntax)
    - Mistakes lead to undesirable results (bugs)

- **Why Python?**

  - Zero experience needed
  - Clear, simple syntax (looks like English)
  - Massive community and learning resources
  - Used in websites, games, data science, automation

- **What you’ll do soon:**
  - Write basic Python scripts
  - Make the computer print your name, do simple math, ask for user input

---

## Slide 6: Essential Tools for Developers

- **Text Editors & IDEs:**
  - **Text Editor:** Write code (Notepad, Sublime, VS Code, Atom)
  - **IDE (Integrated Development Environment):** Extra tools for easier coding (VS Code, PyCharm, WebStorm)
- **Code Editor Features:**

  - Syntax highlighting (colors for keywords)
  - Autocomplete
  - Debugging (see and fix mistakes)
  - Extensions/plugins (add-ons for languages, formatting)

- **Recommended Editor: VS Code**

  - Free, light, easy-to-install
  - Supported on Windows, Mac, Linux
  - Widely used in the industry

- **Installation & First-Time Setup:**

  1. Visit [VS Code Download Page](https://code.visualstudio.com/download)
  2. Choose your OS (Windows/Mac/Linux)
  3. Run the installer
  4. Open VS Code and familiarize yourself

- **Keyboard Shortcuts to Remember:**

  - `Ctrl + S` (Save)
  - `Ctrl + N` (New file)
  - `Ctrl + Z` (Undo)
  - `Ctrl + Shift + P` (Command palette)

- **Organizing Code:**

  - Always create a folder for your projects (“MyProjects”)
  - Practice: Create new files (`hello.txt`, `notes.md`)
  - Explore saved files and folder structure

- **Troubleshooting:**
  - Installation failed? Make sure your OS is supported and you have enough storage.
  - Can’t run VS Code? Try restarting the computer.

---

## Slide 7: Practical Activity: Workspace Setup

- **Objective:**
  Set up your environment for coding, get used to using VS Code and file management.

- **Step-by-Step Instructions:**

  1. **Download & Install VS Code**:
     - Go to: [https://code.visualstudio.com/download](https://code.visualstudio.com/download)
     - Install for your OS
  2. **Create Project Folder**:
     - In Documents/Desktop, make a folder called `MyProjects`
     - Inside `MyProjects`, create subfolders for each week: `Week1`, `Week2`, etc.
  3. **Open VS Code**
     - Use File > Open Folder; select `MyProjects`
     - Create a new file (e.g., `welcome.txt`) in `Week1`
  4. **Initial Exploration**:
     - Save the file
     - Try typing and editing content
     - Move the file, rename it within VS Code and your OS
  5. **Screenshot Your Setup**:
     - Take a screenshot of VS Code open with your folder structure.
     - Save in your `Assignments` folder.

- **Extra Challenge:**

  - Change VS Code’s color theme (View > Command Palette > “Color Theme”)
  - Add a simple extension (e.g., Python extension)

- **Tips:**
  - Don’t worry about mistakes — you can always undo or delete and try again.
  - Stay organized: clean folders = faster progress!

---

## Slide 8: Resource Highlights

- **Videos for Context:**

  - [Crash Course Computer Science (Episodes 1–3)](https://www.youtube.com/playlist?list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo)
  - [VS Code First Steps](https://code.visualstudio.com/docs/getstarted/introvideos)
  - [freeCodeCamp Intro to Python (first 20 mins)](https://www.youtube.com/watch?v=rfscVS0vtbw)

- **Reading:**

  - [VS Code Official Documentation](https://code.visualstudio.com/docs)
  - [How Computers Work (Khan Academy)](https://www.khanacademy.org/computing/computer-science/how-computers-work)
  - [Beginner’s Guide to Command Line](https://tutorial.djangogirls.org/en/intro_to_command_line/)

- **Reference:**

  - [Markdown Guide](https://www.markdownguide.org/cheat-sheet/)
  - [What is an IDE?](https://www.freecodecamp.org/news/what-is-an-ide/)

- **Note:**
  - Bookmark these links in a “Resources” folder in your browser

---

## Slide 9: Q&A + Assignment

- **Live Q&A:**

  - Ask anything: setup problems, confusion about files/folders, terminology
  - Share your experience in setting up VS Code and folders

- **Assignment Checklist:**

  1. Install VS Code and confirm it runs
  2. Create a clear project folder structure (`MyProjects`, `Week1`, etc.)
  3. Create and save at least two files in VS Code (`welcome.txt`, `notes.md`)
  4. Take and submit a screenshot of your editor and folder structure
  5. Watch Crash Course Computer Science (Episodes 1–3)
     - Write 5–10 key things you learned from videos (submit as `video_notes.txt`)
  6. (Optional): Customize VS Code theme, install an extension, try the command line

- **Submission Guidelines:**

  - Submit screenshots and all text files to your tutor via email/drive/cloud folder
  - Write a short reflection:
    - What was easy?
    - What was hard or confusing?
    - What are you most interested in learning next?

- **Support:**
  - Post your questions on the course group/forum for help
  - Troubleshooting tips provided in resource section

---

## Slide 10: Next Steps

- **Preview Week 2:**

  - Dive into your first Python code!
  - Learn about variables, data types, and basic logic

- **Advice:**
  - Be curious — explore menus, settings, try things out
  - Mistakes = progress! Every coder starts as a beginner

---
