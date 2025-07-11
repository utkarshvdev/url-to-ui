# 🧠 What is a Polyfill?

A **polyfill** is a piece of code (usually JavaScript) that implements a modern browser feature on older browsers that do not support it natively.

## 💡 Why Use Polyfills?
- Ensure compatibility for older browsers
- Adopt modern syntax (ES6+) while supporting legacy users
- Bridge the gap during slow standard adoption

## 🧪 Example:
Older browsers didn’t support `Array.prototype.includes`:

```js
if (!Array.prototype.includes) {
  Array.prototype.includes = function(search, start) {
    return this.indexOf(search, start) !== -1;
  };
}
```

This is a **polyfill**.