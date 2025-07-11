# 📚 Call Stack and Memory Management

JavaScript is single-threaded and uses a call stack to manage function execution.

## 🧱 Call Stack:
- LIFO structure
- Functions pushed/popped as they're called and completed

```js
function greet() {
  console.log("Hi");
}
greet();
```

## 🧠 Memory:
- **Heap:** Stores objects and functions
- **Stack:** Tracks function call context

## 🚮 Garbage Collection:
- Automatic cleanup of unused memory
- Triggered periodically by the engine

## ⚠️ Common Pitfalls:
- Memory leaks (event listeners, closures)
- Stack overflow (deep recursion)