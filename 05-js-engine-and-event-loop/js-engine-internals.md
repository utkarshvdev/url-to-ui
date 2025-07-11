# 🧠 JavaScript Engine Internals

JavaScript code is executed by the browser's JavaScript engine (e.g., V8 in Chrome).

## 🔍 Key Components:
- **Parser** – Converts code to AST (Abstract Syntax Tree)
- **Interpreter** – Quickly executes unoptimized code
- **Compiler (JIT)** – Optimizes hot code paths
- **Garbage Collector** – Frees unused memory

## ⚙️ Phases of Execution:
1. Parsing
2. Compilation (Baseline → Optimized JIT)
3. Execution

## 🧪 Example:
```js
let sum = a + b;
```
Is parsed into tokens, compiled to bytecode, and then executed.

## 💡 Insight:
Modern engines balance between speed (interpreter) and efficiency (JIT compiled code).