# 📘 Summary – Module 2: HTML, CSS & JS Parsing

This module explains how browsers parse HTML, CSS, and JavaScript to build structured representations and prepare for rendering.

---

## 📂 Topics Covered:

### 1. HTML Parsing (`html-parsing.md`)
- Converts raw HTML into the DOM Tree.
- Parsing is blocked by synchronous scripts.
- Tokenization and tree construction step-by-step.

### 2. CSS Parsing (`css-parsing.md`)
- CSS is parsed into CSSOM (CSS Object Model).
- CSS is render-blocking and needs to be fully loaded before render.
- Style rules mapped to element selectors.

### 3. JS Parsing & Execution (`js-parsing-and-execution.md`)
- JavaScript is parsed, compiled (into bytecode), and executed.
- Describes the difference between `async`, `defer`, and normal scripts.
- Includes JS engine phases and event loop basics.

### 4. DOM + CSSOM → Render Tree (`dom-cssom.md`)
- DOM and CSSOM combine to create the Render Tree.
- Layout → Paint → Composite steps detailed.
- Diagrams showing data flow from parse to paint.

---

## ✅ Key Takeaways:

- HTML parsing constructs structure (DOM).
- CSS parsing adds styles (CSSOM).
- JavaScript modifies DOM/CSSOM dynamically.
- DOM + CSSOM = Render Tree → Layout & Painting
