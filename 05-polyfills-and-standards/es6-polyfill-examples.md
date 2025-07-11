# 📘 ES6+ Polyfill Examples

Let’s look at examples of polyfills for modern ES6+ features:

---

### ✅ `Object.assign`
```js
if (!Object.assign) {
  Object.assign = function(target, ...sources) {
    sources.forEach(source => {
      for (let key in source) {
        if (Object.prototype.hasOwnProperty.call(source, key)) {
          target[key] = source[key];
        }
      }
    });
    return target;
  };
}
```

---

### ✅ `Promise`
Use libraries like `es6-promise`:
```html
<script src="https://cdn.jsdelivr.net/npm/es6-promise@4/dist/es6-promise.auto.min.js"></script>
```

---

### ✅ `Array.from`
```js
if (!Array.from) {
  Array.from = function(obj) {
    return [].slice.call(obj);
  };
}
```