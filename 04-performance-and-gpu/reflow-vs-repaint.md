# 🔁 Reflow vs Repaint – Understanding Performance Costs

Performance bottlenecks often stem from reflows and repaints. Understanding the difference helps in writing optimized UIs.

## 🔄 Reflow (Layout):
Occurs when changes affect layout — size, position, or geometry of elements.

### Examples:
- Changing `width`, `height`, `margin`, `font-size`
- Adding or removing DOM nodes
- Window resize

## 🎨 Repaint:
Occurs when changes affect the appearance but not layout.

### Examples:
- Changing `background-color`, `color`, `visibility`
- Applying `box-shadow` or `border-color`

## ⚠️ Reflow > Repaint:
Reflow is more expensive — it recalculates the layout tree and may trigger subsequent repaints.

## ✅ Tip:
Minimize layout thrashing (e.g., avoid forced synchronous layout reads).