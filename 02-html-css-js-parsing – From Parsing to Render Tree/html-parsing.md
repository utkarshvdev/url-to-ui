# 🧱 HTML Parsing – From Markup to DOM Tree

## 🔸 What is HTML Parsing?

HTML parsing is the process by which a browser reads HTML text and converts it into a DOM (Document Object Model) – a structured, in-memory representation of the HTML page.

---

## 📥 Step-by-Step Breakdown

1. **Tokenization** – HTML is split into tokens (e.g., <div>, </p>)
2. **Tree Construction** – Tokens are parsed into nodes and assembled into a tree.
3. **DOM Tree** – The final structured representation of the document.

---

## ⏸️ Script Blocking Behavior

- <script> tags block HTML parsing unless marked with async or defer.
- Browser pauses DOM construction to execute scripts.

```html
<script src="main.js"></script> <!-- Blocks parsing -->
<script src="main.js" defer></script> <!-- Runs after DOM -->
```

---

## 🧠 Example: Simple DOM Tree

HTML:
```html
<html>
  <body>
    <h1>Hello</h1>
  </body>
</html>
```

DOM:
```text
Document
 └── html
     └── body
         └── h1
             └── "Hello"
```

---

## ✅ Summary

- HTML is parsed top-down and tokenized.
- DOM construction is incremental.
- Scripts can block parsing unless optimized.