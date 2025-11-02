---
marp: true
title: "Software Engineering Foundations - Week 1"
theme: default
paginate: true
---

# 🧑‍💻 Software Engineering Foundations

### **Week 1 – Introduction to Software Engineering (Expanded)**

**Instructor:** Ememe Tochukwu
**Duration:** 2 Sessions (Session 2 expanded)
**Audience:** Complete Beginners

---

# 🎯 Week 1 Overview (Quick)

**Session 1:** Introduction to Software Engineering (unchanged)
**Session 2:** First Steps with Code (JavaScript) — **Expanded & Deep Dive**

🧠 **Session 2 Goals (expanded)**

- Understand what programming is and why it matters
- Learn JavaScript basics with clear examples
- Practice input/output in browser and Node.js
- Learn variables, data types, operators, and debugging
- Build several small, hands-on exercises
- See visual diagrams and beginner-friendly analogies

---

# 💻 Session 2 — First Steps with Code (JavaScript) (Cover slide)

**Estimated time:** 2.5–3 hours (can split into smaller chunks)
Tip: Pause after each exercise and let the student try it for 10–15 minutes.

---

## 🎯 Learning Objectives (detailed)

By the end of this session the learner will be able to:

- Explain what programming is and how computers execute code
- Write and run simple JavaScript programs in the browser and Node.js
- Use variables and common data types correctly
- Use arithmetic, comparison, and logical operators
- Convert between types (string ⇄ number) safely
- Build small interactive programs with user input
- Use basic debugging techniques to fix errors

---

## 🧠 What Is Programming? (with analogy)

Programming = giving **precise instructions** to a computer.
Analogy: A **recipe** for baking a cake — missing one step can ruin the result.

**Steps matter**, and computers will do **exactly** what you tell them.

**Real-world example:** Turning on a light vs writing code:

- You flip a switch (human-friendly).
- In code: you must call the function `turnOnLight()` and pass the right arguments — computers will not guess.

---

## 🖥️ JavaScript at a Glance (visual cheat-sheet)

- **What:** Language used for web interactivity and general scripting
- **Where it runs:** Browser (client) & Node.js (server/desktop)
- **Why use it:** Ubiquitous on the web, beginner-friendly, immediate feedback

```
Browser         <--- JavaScript --->   Web Page (DOM)
Node.js (local) <--- JavaScript --->   Terminal apps & servers
```

Quick Links:

- MDN JavaScript First Steps — https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps
- JavaScript Info (in-depth) — https://javascript.info/

---

## ✍️ Set up and run your first JavaScript file (step-by-step)

**1. Create file:** `hello.js` inside a folder (e.g., `week1/`)
**2. Add code:**

```js
console.log("Hello, world!");
```

**3. Run in Node.js:** (open terminal in folder)

```bash
node hello.js
```

**4. Run in Browser:** Create `hello.html` and open in browser.

```html
<!DOCTYPE html>
<html>
  <body>
    <script>
      console.log("Hello from the browser!");
      document.body.innerText = "Check the console (F12)";
    </script>
  </body>
</html>
```

**Tip:** Press F12 → Console to see `console.log` output in the browser.

---

## 🧩 Syntax fundamentals (very beginner-friendly)

- **Statements** end with `;` (optional in many cases but good habit)
- **Functions** are lines of reusable code: `console.log()`
- **Blocks** use `{ }` to group code
- **Case-sensitive:** `myVar` ≠ `myvar`

**Example (annotated):**

```js
// Print a message to the console
console.log("Hello, Student!"); // console.log -> function, string -> "Hello, Student!"
```

---

## 💬 Comments — why they help

**Single-line:** `// explain something`
**Multi-line:** `/* longer explanation */`

Use comments to:

- Explain intent (why this code exists)
- Leave TODOs for later
- Help students read code

---

## 📦 Variables — explained with visuals

Variables are **named containers** for data.

```
[ name ] ---> "Ada"
[ age  ] ---> 25
[ todos ] ---> ["buy milk", "study"]
```

Declaration types:

- `let` → variable that can change
- `const` → constant value (can't be reassigned)
- `var` → legacy (avoid for beginners)

```js
let name = "Ada";
const pi = 3.14159;
```

**When to use which:** use `const` whenever possible; use `let` when you expect the value to change.

---

## 🧠 Data Types — visual table & examples

| Type      |         Example | When you use it              |
| --------- | --------------: | ---------------------------- |
| String    |       `"Hello"` | Text like names, messages    |
| Number    |    `42`, `3.14` | Counts, prices, calculations |
| Boolean   | `true`, `false` | Yes/no, on/off conditions    |
| Array     |       `[1,2,3]` | Lists of items               |
| Object    | `{name: "Ada"}` | Structured data (records)    |
| null      |          `null` | Intentionally empty value    |
| undefined |     `undefined` | No value assigned yet        |

**Examples:**

```js
let price = 200; // Number
let product = "Notebook"; // String
let isOpen = false; // Boolean
let items = ["pen", "notebook"]; // Array
let user = { name: "Aisha", age: 28 }; // Object
```

---

## 🧮 Operators — grouped with examples

### Arithmetic

```js
5 + 3; // 8
10 - 2; // 8
4 * 2; // 8
8 / 2; // 4
7 % 3; // 1 (remainder)
```

### Comparison

```js
5 === "5"; // false (strict equality)
5 == "5"; // true (loose equality — avoid)
10 > 3; // true
```

### Logical

```js
true && false; // false
true || false; // true
!true; // false
```

**Visual:**

```
(5 > 2) && (3 < 10)  -> true && true -> true
```

---

## 🔄 Type conversion & `typeof`

JavaScript can change types automatically — but that can cause confusion.

```js
let x = "10"; // string
let y = Number(x); // convert string to number -> 10
console.log(typeof y); // "number"
```

**Useful check:** `typeof value`

```js
console.log(typeof "hello"); // "string"
console.log(typeof 123); // "number"
console.log(typeof true); // "boolean"
```

**Tip:** Prefer explicit conversion: `Number()`, `String()`, `Boolean()`

---

## 🧑‍💻 Input & Output (Beginner-friendly)

**Browser prompt (easy):**

```js
const name = prompt("What's your name?");
alert(`Welcome, ${name}!`);
```

> Note: `prompt`/`alert` are easy for beginners but not used often in production

**Node.js input (more realistic)** using `prompt-sync`:

```bash
npm init -y
npm install prompt-sync
```

```js
// app.js
const prompt = require("prompt-sync")({ sigint: true });
const name = prompt("Enter your name: ");
console.log(`Hello, ${name}!`);
```

**Alternative:** Try Replit (https://replit.com) for instant online runs (no install).

---

## 🧩 Interactive Mini-Project: Greeting + Age Checker (walk-through)

**Goal:** Ask for name and birth year → calculate age → print message and category

1. Ask for name (string)
2. Ask for birth year (string → convert to number)
3. Calculate age = currentYear - birthYear
4. Output: Hello [name], you are [age] years old — Adult/Minor

**Sample solution:**

```js
const prompt = require("prompt-sync")({ sigint: true });
const name = prompt("Name: ");
const birthYear = Number(prompt("Birth year: "));

const currentYear = new Date().getFullYear();
const age = currentYear - birthYear;

console.log(`Hello ${name}, you are ${age} years old.`);
if (age >= 18) {
  console.log("You are an adult.");
} else {
  console.log("You are a minor.");
}
```

---

## ⚡ Practice Challenges (with hints & expected outputs)

### Challenge 1 — Simple Calculator

**Task:** Read two numbers, print sum, product, and difference.
**Hint:** Convert inputs with `Number()`.

**Expected output example:**

```
Sum: 7
Product: 10
Difference: 3
```

### Challenge 2 — Even or Odd

**Task:** Read a number and print "Even" or "Odd".
**Hint:** Use `%` remainder operator.
**Example:** Input: `4` → Output: `Even`

### Challenge 3 — Temperature Converter

**Task:** Convert Celsius to Fahrenheit: `F = (C * 9/5) + 32`
**Example:** Input: `20` → Output: `Fahrenheit: 68`

### Challenge 4 — To-do quick list (array practice)

**Task:** Create an array of 3 tasks, print each with its index.
**Hint:** Use a `for` loop to iterate.

---

## 🧠 Debugging — techniques & examples

**Common errors:**

- SyntaxError: missing `)` or `}`
- ReferenceError: variable not defined
- TypeError: value not a function

**Debugging steps:**

1. Read the error message (it points to the line)
2. Use `console.log()` to check variable values
3. Try small changes and re-run
4. Google the error message (copy & paste)
5. Ask for help with the exact error message

**Example:** Fixing a typo

```js
let username = "Ada";
console.log(usernme); // ReferenceError: usernme is not defined
// Fix: console.log(username);
```

---

## 🖼️ Simple Infographics (ASCII & text diagrams for slides)

### How code runs (very simplified)

```
[Code file: app.js]  --node runtime-->  [JavaScript engine]  --executes--> [Console / Output]
```

### Variable box visual

```
+-----------+
| name: "Ada"|
+-----------+
| age: 25    |
+-----------+
```

### If statement flow

```
[Start] --> [condition?] --yes--> [do A] --> [end]
                         \--no--> [do B] --> [end]
```

---

## 📚 Extra Resources (curated & beginner friendly)

- MDN JavaScript First Steps — https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps
- JavaScript.info — https://javascript.info/ (interactive & deep)
- FreeCodeCamp JS Basics — https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/
- Replit (run code online) — https://replit.com/
- Codecademy JavaScript (interactive course) — https://www.codecademy.com/learn/introduction-to-javascript
- YouTube: "Programming for Beginners" — FreeCodeCamp long-form videos (search on YouTube)

---

## ✅ Assignment #2 (Expanded)

1. Complete the three core challenges (Calculator, Even/Odd, Temp Converter) and save them as separate files (`calculator.js`, `evenodd.js`, `temp.js`).
2. Try the Greeting + Age Checker mini-project.
3. Use `console.log()` statements to show the data types and values (`typeof`) in each program.
4. Push your solutions to a GitHub repo (create one for the course).
5. Optional: Create a short 3–5 minute screencast (phone recording is fine) running your code and explaining what you wrote.

---

## 🧭 Next steps (after this session)

- Week 3: Conditionals, Loops & Functions (practice with arrays & objects)
- Start learning DOM manipulation when comfortable with basics

---

# 🎉 Session 2 — Complete

Great work — you've now got a clear, hands-on path through JavaScript basics with many practical exercises.
