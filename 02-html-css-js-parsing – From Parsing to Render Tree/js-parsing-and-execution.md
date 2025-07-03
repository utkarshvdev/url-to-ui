# ⚙️ JavaScript Parsing and Execution

## 🔸 What Happens When JS Loads?

JS is not just parsed – it is compiled and executed by the browser's JS engine (e.g., V8 in Chrome, SpiderMonkey in Firefox).

---

## 🧩 Steps:

1. **Parsing:** JS code is parsed into an Abstract Syntax Tree (AST)
2. **Compilation:** AST is compiled to bytecode
3. **Execution:** JS engine runs the bytecode

---

## 📦 Script Loading Behavior

- **Normal script:** Blocks parsing
- **Defer:** Executes after DOM is parsed
- **Async:** Executes as soon as it loads (non-blocking)

```html
<script src="main.js"></script>         <!-- Blocking -->
<script src="main.js" defer></script>   <!-- After DOM -->
<script src="main.js" async></script>   <!-- Any time -->
```

---

## 🔁 JS Execution Cycle

1. Call Stack
2. Web APIs
3. Callback Queue
4. Event Loop

---

## ✅ Summary

- JS is parsed, compiled, and executed.
- Use defer/async for non-blocking scripts.
- Understanding the Event Loop is key for async behavior.