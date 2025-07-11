# ⚡ Async Behavior in JS – Promises, Microtasks, Macrotasks

Modern JavaScript uses Promises and async/await for non-blocking logic.

## 🔄 Microtasks vs Macrotasks:

| Type       | Source               | Runs After |
|------------|----------------------|------------|
| Microtask  | `Promise.then`, `queueMicrotask` | Current task |
| Macrotask  | `setTimeout`, `setInterval`     | Entire script |

## 🧪 Example:
```js
console.log("script");

setTimeout(() => console.log("setTimeout"), 0);

Promise.resolve().then(() => console.log("promise"));

console.log("end");
```

Output:
```
script
end
promise
setTimeout
```

## ⚠️ Tip:
Microtasks run before any rendering – avoid blocking them.