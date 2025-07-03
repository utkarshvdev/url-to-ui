# 🎨 CSS Parsing – From Styles to CSSOM

## 🔸 What is CSS Parsing?

CSS parsing is the process of converting CSS code (external or inline) into a CSS Object Model (CSSOM), which maps rules to elements.

---

## 🧩 Steps in CSS Parsing

1. **Tokenization** – Converts styles into tokens (selectors, properties).
2. **Parsing** – Builds the rules tree.
3. **CSSOM** – Maps selectors to style rules.

---

## 🚫 Render Blocking

- CSS is render-blocking. The browser will NOT render any content until the CSSOM is complete.
- This is why CSS files should load fast and early.

---

## 🧠 Example:

CSS:
```css
body {
  font-size: 16px;
  color: blue;
}
```

CSSOM (Conceptual):
```text
Rule: body
 ├─ font-size: 16px
 └─ color: blue
```

---

## ✅ Summary

- CSS is parsed into CSSOM for style computation.
- CSS blocks rendering until fully loaded.