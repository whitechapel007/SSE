---
marp: true
title: "Software Engineering Foundations - Week 2, Session 1 (Extended)"
theme: default
paginate: true
---

# 🧑‍💻 Software Engineering Foundations

### **Week 2 – Session 1: Logic, Conditions & Control Flow (Extended)**

**Instructor:** Ememe Tochukwu Ebuka
**Audience:** Beginners
**Goal:** Understand how computers make decisions and control program flow, with real-world examples and hands-on exercises.

---

# 🎯 Learning Objectives (Extended)

By the end of this session, learners will be able to:

✅ Explain what logic and conditions mean in programming
✅ Understand Boolean concepts clearly
✅ Use **comparison** and **logical** operators confidently
✅ Write programs with `if`, `else`, `else if`, and `switch` statements
✅ Apply nested and compound conditions
✅ Debug logical errors efficiently
✅ Solve small real-world problems using control flow

---

# 🔁 Recap from Week 1

- Variables store information
- Data types: Number, String, Boolean, Array, Object
- Operators: arithmetic, comparison, logical basics
- Input/output using console and prompt

> Now we’ll learn **how to make decisions** based on these values!

---

# 💭 Understanding Logic in Everyday Life

Logic = making decisions based on **conditions**.

**Examples:**

- If it’s raining → take an umbrella
- Else → wear sunglasses
- If you are hungry → eat
- Else → continue studying

**Analogy:** Think of a **flowchart** at a grocery store checkout:

```
[Customer arrives] --> [Has items?] --No--> [Exit]
                     |--Yes--> [Pay] --> [Exit]
```

---

# 🧠 Boolean Concepts (True/False)

- Boolean = **true or false** value
- Computers make decisions using Booleans
- Boolean expressions result from **comparison operators** or **logical operations**

**Examples:**

```js
let isRaining = true;
let hasUmbrella = false;

console.log(isRaining && hasUmbrella); // false
console.log(isRaining || hasUmbrella); // true
console.log(!isRaining); // false
```

---

# 🧮 Comparison Operators (In Depth)

| Operator | Meaning          | Example     | Result |
| -------- | ---------------- | ----------- | ------ |
| `==`     | Equal to         | `5 == 5`    | true   |
| `!=`     | Not equal        | `5 != 3`    | true   |
| `>`      | Greater than     | `7 > 3`     | true   |
| `<`      | Less than        | `2 < 5`     | true   |
| `>=`     | Greater or equal | `6 >= 6`    | true   |
| `<=`     | Less or equal    | `4 <= 9`    | true   |
| `===`    | Strict equal     | `5 === "5"` | false  |
| `!==`    | Strict not equal | `5 !== "5"` | true   |

> **Tip:** Use `===` in JavaScript to avoid type coercion surprises.

---

# 🧩 Logical Operators (Detailed)

| Operator | Meaning | Example                  | Result            |
| -------- | ------- | ------------------------ | ----------------- | --------------- | --- | --------------- | ------------------- |
| `&&`     | AND     | `(age > 18 && age < 60)` | true if both true |
| `        |         | `                        | OR                | `(day === "Sat" |     | day === "Sun")` | true if either true |
| `!`      | NOT     | `!(isRaining)`           | true if false     |

**Example with real-world scenario:**

```js
let hasTicket = true;
let isVIP = false;

if (hasTicket || isVIP) {
  console.log("Entry allowed");
} else {
  console.log("Entry denied");
}
```

---

# ⚙️ Conditional Statements (`if`, `else`, `else if`)

Basic syntax:

```js
if (condition) {
  // code if true
} else {
  // code if false
}
```

Example:

```js
let age = 20;

if (age >= 18) {
  console.log("You can vote!");
} else {
  console.log("You are too young to vote.");
}
```

**Flow Diagram:**

```
[Start] --> [Condition true?] --Yes--> [Execute True Block] --> [End]
                       |No
                       --> [Execute False Block] --> [End]
```

---

# 🔄 Multiple Conditions with `else if`

```js
let score = 75;

if (score >= 90) {
  console.log("A Grade");
} else if (score >= 70) {
  console.log("B Grade");
} else if (score >= 50) {
  console.log("C Grade");
} else {
  console.log("Fail");
}
```

**Tip:** Check conditions **top-down**; the first true condition runs.

---

# 💡 The `switch` Statement (Advanced Beginner)

Use `switch` for multiple discrete options:

```js
let day = "Tuesday";

switch (day) {
  case "Monday":
    console.log("Start of the week");
    break;
  case "Friday":
    console.log("Almost weekend");
    break;
  default:
    console.log("Regular day");
}
```

> **Remember:** Use `break` to avoid fall-through. You can also group cases:

```js
case "Saturday":
case "Sunday":
  console.log("Weekend!");
  break;
```

---

# 🧱 Nested & Compound Conditions

```js
let isLoggedIn = true;
let isAdmin = false;

if (isLoggedIn) {
  if (isAdmin) {
    console.log("Welcome, Admin");
  } else {
    console.log("Welcome, User");
  }
} else {
  console.log("Please log in");
}
```

**Diagram (simplified)**

```
[Start] -> [Logged In?] -> Yes -> [Admin?] -> Yes -> [Admin Welcome]
                                    -> No  -> [User Welcome]
               -> No  -> [Log In Prompt]
```

---

# 🛠️ Real-World Scenario Examples

**1️⃣ Bank App Login**

- If username & password correct → show “Welcome”
- Else → show “Access Denied”

**2️⃣ Traffic Light Simulation**

- If red → stop
- If yellow → slow
- If green → go

**3️⃣ Game Logic (Beginner)**

- If health ≤ 0 → “Game Over”
- If powerUp active → increase score

**Exercise:** Draw a flowchart for your favorite real-world app decision.

---

# 🧠 Debugging Logical Errors

Common mistakes:

- Using `=` instead of `==` or `===`
- Forgetting `{}` for nested blocks
- Overlapping conditions
- Not handling edge cases (e.g., negative numbers)

**Debugging tips:**

1. Use `console.log()` to check variable values
2. Break complex conditions into smaller steps
3. Test each branch separately

---

# ✍️ Practice Exercises

**Exercise 1:** Age Group Categorizer

- Ask user for age
- Print: Child, Teenager, Adult, Senior

**Exercise 2:** Even or Odd Checker

- Ask user for number
- Print: “Even” or “Odd”

**Exercise 3:** Traffic Light Message

- Ask user for light color
- Print: “Stop”, “Slow”, or “Go”

**Exercise 4:** Simple Login

- Hardcode username/password
- Ask for input
- Print “Access Granted” / “Access Denied”

---

# 🏡 Mini Quiz (Interactive)

1. What does `&&` do?
2. Difference between `==` and `===`
3. When to use `switch` over `if-else`?
4. Explain what happens in nested conditions

> Discuss answers live with the student

---

# 🔗 Resources & Further Reading

- MDN if...else: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else
- MDN switch: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch
- JavaScript.info: https://javascript.info/ifelse
- Visualgo (Flow Control Simulator): https://visualgo.net/en

---

# 📝 Tutor Notes (Hidden)

- Pause after every section and ask student for **real-life examples**
- Draw ASCII diagrams on board to explain flow
- Use console.log exercises live to demonstrate branching
- Encourage students to make mistakes and debug

---

# 🎉 Wrap-Up & Next Steps

- Students should now:
  ✅ Understand comparison & logical operators
  ✅ Write if, else, else if, switch statements
  ✅ Handle nested and compound conditions
  ✅ Apply logic to real-world problems

> Next session: **Functions, Loops & Problem Solving** 🚀
