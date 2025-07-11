# 🔁 The Event Loop – Managing Async Flow

The event loop enables JavaScript to handle asynchronous tasks like I/O, timers, and events.

## 🎯 Components:
- **Call Stack** – Executes code
- **Web APIs** – Browser-provided async services (e.g., setTimeout)
- **Callback Queue** – Queued async callbacks
- **Event Loop** – Moves tasks from queue to stack when empty

## ⏱️ Visual Flow:
```text
JS Call Stack ← Event Loop ← Callback Queue ← Web APIs
```

## 🧪 Example:
```js
console.log("Start");
setTimeout(() => console.log("Timeout"), 0);
console.log("End");
```

Output:
```
Start
End
Timeout
```

## 💡 Tip:
Use `Performance tab` in DevTools to observe it live.