# ⚙️ How Polyfills Work Internally

Polyfills work by **checking for feature support** and defining a fallback if it's missing.

## 🔍 Pattern:
```js
if (!('featureName' in object)) {
  // Define your fallback
}
```

## 🧠 Browser Workflow:
1. JS engine checks native implementation
2. If missing, uses the polyfilled code
3. Works as if the browser had native support

## 🔐 Caveat:
Polyfills only work if included *before* the feature is used in your code.